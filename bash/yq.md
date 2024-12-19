# yq

yq is like jq but can be used for xml. For example:

```bash
yq -p=xml '.testsuites.testsuite[].["+@timestamp"]' input.xml
```

