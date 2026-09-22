---
status: generated
version: "0.1"
---

# Security

Orbi's delivery pipeline is built around two guarantees: your code and keys stay where you put them, and a human is always the last gate before anything ships.

<!-- widget:accordion -->

### Self-hosted: nothing leaves your machine

Running Orbi yourself, your repository, keys and test suite stay on your machine — nothing is uploaded to Orbi.

### Managed Cloud: scoped, temporary access

On Managed Cloud, the runner clones the repository you authorize onto machines Orbi operates, only for the duration of a delivery.

### Bring your own model

Orbi drives the coding agent through your own credentials — any OpenAI-compatible API or a local model. Model spend goes to your provider, not to Orbi.

### Human approval stays the last gate

Work always lands as a normal GitHub pull request, so your branch protection rules, required status checks and human approvals apply exactly as they do for any other PR.

<!-- /widget -->

<!-- widget:callout type=note -->

This MVP keeps state only in GitHub rather than a database or queue, runs one Issue per tick rather than as a daemon, and does not discover repositories or push to protected branches on its own.

<!-- /widget -->

<!-- widget:cards plain cols=2 -->

## Next steps

- [How it works](/concepts) — The full delivery chain these boundaries sit around. {git-branch}
- [FAQ](/faq) — More on Managed Cloud and licensing. {help-circle}

<!-- /widget -->
