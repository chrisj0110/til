# gcloud compute instances list example

An example which gets the first 5 most recent compute instances which have a label `asset` which contains "abc":

```bash
gcloud compute instances list --project my-project-1234 --filter="labels.asset ~ abc" --sort-by=~creationTimestamp --limit=5 --format="table(labels[vm-type], INTERNAL_IP, NAME, creationTimestamp, labels[image_name], ZONE, MACHINE_TYPE, STATUS)"
```
