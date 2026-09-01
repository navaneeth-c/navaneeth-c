### Navaneeth Chandrasekaran

Platform engineer, ~10 years, working at the layer where hardware meets software —
Linux internals, container isolation, and Kubernetes scheduling.

Most of what I do is infrastructure at a scale where the interesting problems stop
being "does it work" and start being "what happens on the 100,000th node":

- **Runtime security** — rolled out Falco across 100k+ nodes on 5k+ production
  clusters, pivoting from kernel modules to **eBPF** to work around host OS
  incompatibilities.
- **Observability** — built a custom OpenTelemetry pipeline replacing vendor
  scrapers across 200+ cloud regions, cutting ~$1.3M/year.
- **FinOps** — deployed OpenCost across 6,000+ clusters, mapping spend back to the
  teams that caused it and turning a 3-day cost feedback loop into a live one.
- **Multi-tenancy** — designed the pod lifecycle for a platform running untrusted
  customer binaries under Kata Container VM isolation.

Lately I've been following the overlap between Kubernetes multi-tenancy and
GPU/AI infrastructure — the scheduling and isolation problems turn out to be
substantially the same ones.

**[k8s-slo-lab](https://github.com/navaneeth-c/k8s-slo-lab)** — run an SLO, an
error budget, and multi-window burn-rate alerts end-to-end on a local cluster,
including a one-command way to break the service and watch the alert fire.

[LinkedIn](https://linkedin.com/in/navaneeth-c)
