# null and coalesce

If I have a field named `required` and another named `optional`, and I want to set a `key` to the value of `optional` if it's not null, else the value of `required`, then I can:

```
eval key = if(isnotnull(optional), optional, required)
```

or the reverse using `isnull`:

```
eval key = if(isnull(optional), required, optional)
```

or I can use `coalesce` to use the first non-null value it finds from a list:

```
eval key = coalesce(optional, required)
```

