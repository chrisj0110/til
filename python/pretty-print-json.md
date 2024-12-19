# Pretty print json using python

The python stdlib comes with a json formatter:

```bash
echo '{"foo": "bar", "baz": [1, 2, 3]}' | python -m json.tool
```

```
{
    "foo": "bar",
    "baz": [
        1,
        2,
        3
    ]
}
```
