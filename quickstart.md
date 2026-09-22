---
status: generated
version: "0.1"
---

# Quickstart

Orbi needs Git, a POSIX shell, and API access to a model you already pay for — no GPU required, and it runs on Linux or macOS.

<!-- widget:stepper -->

### Install Orbi

One-line installer:

```bash
curl -fsSL https://aiready.sh | sh
```

This needs Python 3.14, git, gh and systemd; `orbi doctor` names whatever is missing.

Or the four manual steps:

```bash
git clone https://github.com/orbi-build/orbi.git && cd orbi
uv tool install --force --reinstall --editable --python /usr/bin/python3 .
cp .orbi.example.toml orbi.toml
orbi setup --config orbi.toml
```

### Bring your model

Orbi drives the agent through your own credentials — any OpenAI-compatible API or a locally hosted model. Model spend goes to your provider at your rate; the self-hosted core has no platform fee.

### Label an Issue `ai-ready`

Orbi claims an `ai-ready` Issue from your repository, develops it in an isolated worktree, and runs your real test suite.

### Let review run

A second Orbi session — optionally on a different model — reviews the PR independently and can fix findings in-session before rerunning tests. Only the reviewed commit merges, as a normal GitHub pull request under your branch protection and required checks.

<!-- /widget -->

<!-- widget:cards plain cols=2 -->

## Next steps

- [How it works](/concepts) — The full Issue-to-release chain. {git-branch}
- [Security](/security) — What Orbi can and cannot do to your repository. {shield}

<!-- /widget -->
