Heatmap

```Python
sns.heatmap(data=billionaires_df.select_dtypes(include=np.number).corr(), cmap="crest")
```

