# gsutil to get URLs from large folder

If your folder contains a lot of files, then GCP Console might struggle to filter to the file(s) you're looking for.

An alternative is to find the file(s) using `gsutil` and then modify the output to give URL(s) for the file(s):

```bash
gsutil ls gs://bucket-name/folder-name/file-name*.* | sed -e "s%gs://%https://console.cloud.google.com/storage/browser/_details/%"
```

If you want to sort the results by timestamp ascending (gsutil appears to sort alphabetically on file name), you can do:

```bash
gsutil ls -l gs://bucket-name/folder-name/file-name*.* | sort -k2 | sed -e "s%gs://%https://console.cloud.google.com/storage/browser/_details/%"
```

This will include the timestamp which you can use `sort` on, like [this](../bash/sorting-output.md).
