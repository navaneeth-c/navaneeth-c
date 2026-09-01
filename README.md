### Navaneeth Chandrasekaran

Platform engineer at Confluent, working on Kubernetes fleet infrastructure: runtime
security, observability, cost, and multi-tenancy.

- **Runtime security.** Rolled out Falco across 100k+ nodes on 5k+ production clusters,
  moving the fleet from kernel modules to eBPF along the way
  ([a bug report from that rollout](https://github.com/falcosecurity/falco/issues/2956)).
- **Observability.** Built the OpenTelemetry pipeline that replaced vendor scrapers across
  200+ cloud regions, cutting ~$1.3M/year
  ([upstream issue](https://github.com/open-telemetry/opentelemetry-collector-contrib/issues/35711),
  [another](https://github.com/open-telemetry/opentelemetry-collector-contrib/issues/35859)).
- **FinOps.** Deployed OpenCost across 6,000+ clusters, mapping infrastructure spend to the
  teams that caused it.
- **Multi-tenancy.** Designed the pod lifecycle for a platform that runs untrusted customer
  binaries under Kata Container VM isolation.

Most of my work lives in private infrastructure repos at Confluent; what's public here is
what I can share:

- [k8s-slo-lab](https://github.com/navaneeth-c/k8s-slo-lab) — an SLO, an error budget, and
  multi-window burn-rate alerts running end to end on a local kind cluster, with a
  one-command way to break the service and watch the alert fire.
- [PAM web access for Infisical](https://github.com/Infisical/infisical/pull/7380) — a
  ~900-line feature PR against their codebase (closed in favor of their roadmap; notes in
  the PR).

[LinkedIn](https://linkedin.com/in/navaneeth-c)
