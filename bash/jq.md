# jq

to pretty print json:

```bash
cat file.json | jq
```

to get a field from the root:
```bash
cat file.json | jq '.fieldname'
```

to get all values of `fieldname` anywhere in the doc:

```bash
jq '.. | .fieldname? // empty' file.json
```

to get all values of `fieldname` that happens in a list from the root:

```bash
jq '.[].fieldname' file.json
```

