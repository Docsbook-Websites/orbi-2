---
status: generated
version: "0.1"
---

# How it works

Orbi does not manage GitHub Issues in isolation — Epics and milestones hold scope, dependencies order the work, and review and repair converge each pull request before a release freezes the result.

<!-- widget:accordion -->

### Coordinate: Epic + Milestone + Scope

Epics and milestones group outcomes and define the release boundary, without letting the runner mistake coordination for execution.

### Order: Issue blockedBy Ready

Orbi uses GitHub's own dependency graph. A task enters production only once the Issues that block it are closed.

### Deliver: worktree, agent, tests, review + fix, exact-head merge

An isolated worktree implements the Issue and runs the real test suite. A second session may patch the branch to fix findings; only its reviewed head is allowed to land.

### Release: freeze SHA, full gate, tag + release

A Release Issue validates scope and the repository, then publishes an immutable version — without an agent improvising the release.

### Recovery

Because the Issue, the pull request, the labels and the run ID all live in GitHub rather than in a process, a killed process or a failed test doesn't invent a second story. The next tick reconstructs the same run, branch, worktree and PR.

<!-- /widget -->

<!-- widget:cards plain cols=2 -->

## Next steps

- [Security](/security) — The boundaries this pipeline runs inside. {shield}
- [Quickstart](/quickstart) — Deliver your first Issue. {rocket}

<!-- /widget -->
