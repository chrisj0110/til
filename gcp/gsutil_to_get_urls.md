# gsutil to get URLs from large folder

If your folder contains a lot of files, then GCP Console might struggle to filter to the file(s) you're looking for.

An alternative is to find the file(s) using `gsutil` and then modify the output to give URL(s) for the file(s):

```bash
gsutil ls gs://bucket-name/folder-name/file-name*.* | sed -e "s%gs://%https://console.cloud.google.com/storage/browser/_details/%"
```
