# tee

To copy output to a file:

```bash
echo "hi" 2>&1 | tee out.txt
```

Or to append to a file, use `tee -a`

