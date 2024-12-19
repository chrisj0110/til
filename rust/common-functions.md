# common functions

- `and_then` - handle happy path while None otherwise. example: `arr_2d.get(0).and_then(|row| row.get(0))` returns `Some(value)` else `None` if out of bounds
- `as_str` - convert String to &str
- `collect` - to convert an iter to a vec, String, etc. example: `.collect::<String>()`
- `concat` - concat two Vecs together, for example: `[vec1, vec2].concat()`
- `expect` - convert a Result<T, E> to T. example: `env::var("something").expect("Failed to get something environment variable")`
- `filter` - example: `filter(|d| d.contains("whatever".to_string())`
- `filter_map` - convert iterator of Result<T, E> to iterator of T. example: `for entry in glob(&pattern).unwrap().filter_map(Result::ok) {`
- `find_map` - return the first non-None value, else None. example: `tags.iter().find_map(|tag| Language::try_from(tag.as_str()).ok())`
- `get` - get the nth item from a Vec. example `utterances.get(1).unwrap()`
- `inspect` - can println each item in an iterator chain. example: `nums.iter().inspect(|x| println!("Inspecting: {}", x))`
- `map` - example: `map(|k| k.as_str())`. Can transform an `Option` by mapping the `Some` value, or returns `None` if `None`.
- `map_or` - get 2nd item from a tuple in one line, for example. example: `let result = line.split_once(": ").map_or(Default::default(), |(_, line_num)| line_num)`
- `nth` - get the nth item from an iterator
- `ok` - takes an `Result` value and converts it to an `Option`. example: `let opt_value = res_value.ok()`
- `ok_or_else` - takes an `Option` value and converts it to a `Result` with either `Ok(value)` or `Err(e)`. example: `opt_value.ok_or_else(|| "error string")`
- `parse` - convert a String to another type, for example: `my_string.parse().unwrap()`
- `split_once` - split a string on the first instance of a character. example: `my_str.split_once(" ")`
- `to_string` - convert &str to String
- `unwrap_or_else` - unwraps the `Some(value)` from a `Option`, or else executes the closure. example: let x = result.unwrap_or_else(|| { println!("could not get value"); return })`
- `unwrap_or_else` - unwraps the `Ok(value)` from a `Result`, or else executes the closure. example: let x = result.unwrap_or_else(|e| { println!("{}", e); return })`

