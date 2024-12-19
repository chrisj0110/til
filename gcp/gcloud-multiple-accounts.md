# gcloud multiple accounts

List credentialed accounts: `gcloud auth list`

List configurations: `gcloud config configurations list`

Create new configuration:

```bash
gcloud config configurations create <configuration-name>
gcloud config set core/account <email>
gcloud config set core/project <project>
gcloud config set compute/region <region>
gcloud config set compute/zone <zone>
gcloud config set functions/region <region>
```

Activate configuration: `gcloud config configurations activate <configuration-name>`

