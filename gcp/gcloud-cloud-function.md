# gcloud to publish cloud function

From the directory with the source code:

```bash
export FUNCTION_NAME=""  # fill this in
gcloud functions deploy $FUNCTION_NAME --gen2 --runtime=python39 --entry-point=main --memory=256MB --trigger-http --allow-unauthenticated
```

I also have in my .bashrc so I can do `gcp-deploy-cloud-function FUNCTION_NAME PROJECT_ID` (after switching to correct GCP project).

NOTE: you need to be in the directory that contains the source code!

