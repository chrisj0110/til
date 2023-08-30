# Using sets for in checks

I usually do checks like:

```python
answer = my_str in ["a", "b"]
```

Since sets have faster lookup times, this is a bit faster:

```python
answer = my_str in {"a", "b"}
```

```bash
$ python -m timeit '"x" in ["a", "b"]'
10000000 loops, best of 5: 27.7 nsec per loop

$ python -m timeit '"x" in {"a", "b"}'
20000000 loops, best of 5: 13.1 nsec per loop
```
