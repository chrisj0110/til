# Timeit to measure performance

To quickly measure performance of different approaches:

```bash
$ python -m timeit '"x" in ["a", "b"]'
10000000 loops, best of 5: 27.7 nsec per loop

$ python -m timeit '"x" in {"a", "b"}'
20000000 loops, best of 5: 13.1 nsec per loop
```
