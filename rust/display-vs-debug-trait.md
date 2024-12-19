# display vs debug trait for output

`{:?}`: This format specifier in Rust uses the Display trait to format the value in a human-readable way. This often works well for smaller values, but it can truncate long strings or complex structures.

`{:#?}`: This format specifier uses the Debug trait to format the value. It gives a more thorough representation, including all fields and information about the data, even for large and complex structures. It might not be as easy to read for humans, but it ensures you see the entire content.

or just `{var_name}` will work if it implements `Display` (otherwise use the above if it implements `Debug`).

