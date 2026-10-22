# deploy-workflows

Reusable GitHub Actions workflows for deploying my apps to Cloud Run (project `meros-apps`).
This repo is public because a public app repo cannot call a reusable workflow from a private one.
It holds no secrets: login uses Workload Identity Federation, and only repos under `meros` are accepted.

See `.github/workflows/deploy-cloud-run.yml` for the inputs. The services, deploy accounts and trust are defined in the private `meros/hosting` repo.
