---
status: generated
version: "0.1"
---

# FAQ

<!-- widget:accordion -->

### What does Orbi actually need to run?

Git, a POSIX shell, and API access to a model you already pay for. Orbi runs on Linux and macOS, on your own machine or your own server — no GPU required, since the model does the thinking and can be a hosted API.

### Which AI models can I use with Orbi?

Bring your own. Orbi drives the agent through your credentials, using any OpenAI-compatible API or a locally hosted model. Model spend goes to your provider at your rate; the self-hosted core has no platform fee.

### How is Orbi different from GitHub Copilot or Cursor?

Those are editors that make you faster while you're typing. Orbi works when nobody is typing: it takes an Issue from your backlog, works in an isolated worktree, and returns a merged pull request after a second session has reviewed and, if needed, repaired it.

### Who reviews the AI's code?

Another Orbi session, running independently of the one that wrote the code — it can change the branch, not just comment, and reruns tests against its own repairs. You stay the last gate: the work lands as a normal GitHub pull request, so your branch protection, required checks and human approvals still apply.

### What happens when a run crashes halfway?

The next tick returns to the same scene. Because the Issue, the pull request, the labels and the run ID live in GitHub rather than in a process, restarts reconstruct the same run, branch, worktree and PR.

### Is Orbi free, and what is Managed Cloud?

The self-hosted core is free forever under the Sustainable Use License (fair-code) — running it on your own repositories costs nothing, for yourself or inside a company of any size. A commercial license is needed only to sell Orbi itself, such as hosting it as a service for your customers. Managed Cloud is Orbi's hosted control plane: sign in with GitHub, install the app, and subscribe.

<!-- /widget -->
