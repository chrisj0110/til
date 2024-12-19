# deleting old app engine versions

if you want to delete all but the last 10 app engine versions:

```bash
gcloud app versions list --format="value(version.id)" --sort-by="~version.createTime" | tail -n +10 | xargs -r gcloud app versions delete --quiet
```

from [SO](https://stackoverflow.com/a/66911696/59867).

