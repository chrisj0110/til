# Watch command

To run `ls` every 60 seconds:

```bash
watch -n 60 ls
```

If you don't have the `watch` command (like in git bash), then:

```bash
while true; do ls; sleep 10; done
```
