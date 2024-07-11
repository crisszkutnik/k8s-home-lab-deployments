<div align="center">
  <img src="https://avatars.githubusercontent.com/u/61287648" align="center" width="180px" height="180px" alt="Kubernetes logo"/>
  <div>
      <i>Managed with Flux and Renovate. Scanned with Trufflehog via GitHub Actions</i>
  </div>
</div>

![GitHub last commit](https://img.shields.io/github/last-commit/crisszkutnik/k8s-home-lab-deployments)
![Renovate enabled](https://img.shields.io/badge/Renovate-Enabled-brightgreen)

---
## :book:&nbsp; Overview

This is the repository for my on-premise Kubernetes cluster that runs in my house. It uses GitOps techniques in order to keep the content of this repository in-sync with the cluster. Basic stuff is:

- [Flux](https://github.com/fluxcd/flux2) for GitOps and keeping the cluster in sync with the repo Also
- [Renovate](https://github.com/renovatebot/renovate) to update dependencies
- [Trufflehog](https://github.com/trufflesecurity/trufflehog) and [GitHub Actions](https://github.com/features/actions) for credential scanning and avoid leaking private credentials

In case you want to check the full index of my on-premise stuff, check [crisszkutnik/kubernetes-home-lab](https://github.com/crisszkutnik/kubernetes-home-lab)

## 💻 Setup, deployments and details

The cluster runs a variety of applications for setup and management such as:

- [Grafana](https://grafana.com/) for charts and observability
- [Loki](https://grafana.com/oss/loki/) and [Promtail](https://grafana.com/docs/loki/latest/send-data/promtail/) for log collection
- [MetalLB](https://metallb.universe.tf/) as load balancer via L2 advertisement
- [NGINX ingress controller](https://docs.nginx.com/nginx-ingress-controller/) is used as an ingress controller

It also runs a bunch of other applications that were developed for personal use
