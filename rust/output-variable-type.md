# output variable type

```rust
    fn print_type_of<T>(_: &T) {
        use std::any::type_name;
        tracing::info!("{}", type_name::<T>());
    }
    print_type_of(&my_var);

```
