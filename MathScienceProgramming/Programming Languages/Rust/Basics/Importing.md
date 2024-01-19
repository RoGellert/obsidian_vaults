
At the imported file 

```rust
pub fn print_something() {
    println!("Something");
}
```

At the file to which you import

```rust
use project_name::print_something;

fn main() {
	print_something()
}
```
