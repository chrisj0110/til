# gcloud to publish cloud function

From the directory with the source code:

```bash
export FUNCTION_NAME=""  # fill this in
gcloud functions deploy $FUNCTION_NAME --gen2 --runtime=python39 --entry-point=main --memory=256MB --trigger-http --allow-unauthenticated
gcloud functions set-max-instances $FUNCTION_NAME 2
```

