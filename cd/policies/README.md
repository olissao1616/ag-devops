# CD policy bundle

This folder is the single source of truth for policy/config files consumed by CI validators:

- Conftest (OPA/Rego): `*.rego`
- Polaris: `polaris.yaml`
- kube-linter: `kube-linter.yaml`
- Datree (Helm plugin): `datree-policies.yaml`

Consumers should download these files from a pinned ref (release tag or commit SHA) and run validators against the downloaded copy (e.g., `/tmp/policies`).
