### My home Kubernetes cluster
#### _Managed with Flux and Renovate. Scanned with Trufflehog_

---
## :book:&nbsp; Overview

This is the repository for my on-premise Kubernetes cluster that runs is in my house. Has a bunch of applications, from custom stuff I developed for personal stuff to well-known apps such as Grafana, Nginx, Loki, etc.

- It uses [Flux](https://github.com/fluxcd/flux2) to apply GitOps techniques and keep the cluster state in sync with what is in this repository
- [Renovate](https://github.com/renovatebot/renovate) is set up to keep versions up to date
- [Trufflehog](https://github.com/trufflesecurity/trufflehog) is used for credential scanning and prevent leaking private credentiale
