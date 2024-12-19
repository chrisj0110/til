# Sorting output

If you have output that looks like the following:

```
81540  2023-08-10T19:14:43Z  https://console.cloud.google.com/storage/browser/_details/bucket-name/folder-name/filename3.png
81540  2023-08-10T19:14:32Z  https://console.cloud.google.com/storage/browser/_details/bucket-name/folder-name/filename2.png
81540  2023-08-10T19:14:20Z  https://console.cloud.google.com/storage/browser/_details/bucket-name/folder-name/filename1.png
```

If you want to sort it by timestamp, you can use `sort`:

```bash
| sort -k2
```

This will sort by the second field.

It can also take a range of fields, so this is equivalent:

```bash
| sort -k2,2
```

You can change the field separator using `-t`:

```bash
| sort -t, -k2
```

You can use general numeric sort using `-g`.

You can reverse it using `-r`.

