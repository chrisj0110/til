# gcloud compute instances list example

An example which gets all compute instances which have a label `asset` which contains "abc", sorted by name:

```bash
gcloud compute instances list --project my-project-1234 --filter="labels.asset ~ abc" --sort-by=name --format="table(labels[vm-type], INTERNAL_IP, NAME, creationTimestamp, labels[image_name], ZONE, MACHINE_TYPE, STATUS)"
```
