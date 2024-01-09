
-------------------------------------------------------------------------------
```python
import pandas
```

Import csv

```python
df = pd.read_csv()
```

Take top n entries

```python
df.head(n)
```

Summary (mean, median, quantiles)

```python
df.describe()
```

Get info (row_num, etc)

```python
df.info()
```

Drop columns

```python
df.drop(columns = ['A', 'B'])
```

Count null

```python
df.isna().sum()
```

Pandas count aggregation #Pandas-aggretation

```python
df = df[['STNAME','CTYNAME']].groupby(['STNAME'])['CTYNAME'] \
                             .count() \
                             .reset_index(name='count') \
                             .sort_values(['count'], ascending=False) \
                             .head(5)
```