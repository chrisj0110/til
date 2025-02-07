# time commands in zsh

```sh
zmodload zsh/datetime
export START=$EPOCHREALTIME

# do some command here
echo "$(($EPOCHREALTIME-$START)) for some command"
```

