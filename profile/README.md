# LoKO — Your Local Kubernetes Oasis

**LoKO** is an opinionated CLI tool that spins up a full local Kubernetes environment on your machine with a single command — TLS, DNS, ingress, a local registry, and a ready-to-use catalog of services, all preconfigured.

```bash
brew install getloko/tap/loko
loko config generate   # generate default config
vi loko.yaml           # optionally furthermodify and save the config file
loko create            # create a complete environment
```

→ [getloko.github.io](https://getloko.github.io) · [docs](https://getloko.github.io/user-guide/) · [catalog](https://getloko.github.io/catalog)

---

## What's included

- **A full KinD-based Kubernetes environment** with Traefik ingress, wildcard TLS (mkcert), and local DNS (dnsmasq)
- **Service catalog** — MySQL, PostgreSQL, MongoDB, RabbitMQ, NATS, Valkey, Garage, Redpanda, Forgejo, and more
- **TCP tunneling** via HAProxy so database clients connect directly using your local domain
- **Public sharing** via ngrok for webhook testing and demos
- **GitOps** with Flux CD or ArgoCD and Forgejo for a fully local CD pipeline

## Repositories

| Repo | Description |
|------|-------------|
| [loko](https://github.com/getloko/loko) | LoKO - Your Local Kubernetes Oasis |
| [catalog](https://github.com/getloko/catalog) | LoKO Catalog - Components, Workloads & More |
| [getloko.github.io](https://github.com/getloko/getloko.github.io) | LoKO Documentation |
| [homebrew-tap](https://github.com/getloko/homebrew-tap) | LoKO Homebrew Tap |
| [container-images](https://github.com/getloko/container-images) | LoKO-related container images |
| [dns-operator](https://github.com/getloko/dns-operator) | LoKO DNS Operator |
| [examples](https://github.com/getloko/examples) | LoKO Configuration Examples |
