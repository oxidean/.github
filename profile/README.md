<p align="center">
  <img src="oxidean-mark.png" alt="Oxidean" width="120" height="120" />
</p>

<h1 align="center">Oxidean</h1>

<p align="center">
  A self-hostable forge for social coding: git hosting, issues, organizations,<br/>
  releases, and package registries. One codebase powers Oxidean Cloud and
  deployments on your own machines.
</p>

<p align="center">
  <a href="https://app.oxidean.dev">app.oxidean.dev</a> ·
  <a href="https://oxidean.dev">oxidean.dev</a> ·
  <a href="/oxidean/oxidean">oxidean/oxidean</a>
</p>

## What it is

Oxidean is a forge you can run yourself or use hosted. Oxidean Cloud at
[app.oxidean.dev](https://app.oxidean.dev) and self-hosted Oxidean ship from the
same codebase and the same images — self-host with Docker Compose today, or use
the hosted instance.

**Shipped on mainline**

- Git hosting over HTTPS (Smart HTTP + PATs) and SSH
- Organizations, collaborators, repository visibility / ACL
- Issues with comments, labels, and assignees
- Git LFS, releases with assets, repository rename / transfer
- Package registries: OCI, npm, generic
- Postgres, MySQL, or SQLite

Still coming: pull-request review and merge, branch protection, search,
notifications, webhooks, and Actions.

## Repositories

| Repo | Purpose |
|------|---------|
| [`oxidean/oxidean`](/oxidean/oxidean) | The forge — web UI, API, and services (Bun + Rust monorepo) |
| [`oxidean/.github`](/oxidean/.github) | This profile and the org-wide default community files |

## Self-host quick start

Clone [`oxidean/oxidean`](/oxidean/oxidean), then:

```bash
cp .env.example .env
make up && make smoke
```

Open http://localhost to finish setup. Full walkthrough:
[docs/GETTING-STARTED.md](/oxidean/oxidean/blob/main/docs/GETTING-STARTED.md).

## Contributing

Start with the main repo's
[CONTRIBUTING.md](/oxidean/oxidean/blob/main/CONTRIBUTING.md);
the files in this repo are the defaults for everything else in the org.
Coding agents should read
[AGENTS.md](/oxidean/oxidean/blob/main/AGENTS.md) first — the
web UI is Octane, not React.
