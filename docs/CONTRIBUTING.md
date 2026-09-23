# Contributing to SEOShark

Thanks for your interest in SEOShark. This repository is a white-label fork of the open-source [OpenSEO](https://github.com/every-app/open-seo) codebase (MIT): branding, deployment and database configuration are ours, and the SEO engine tracks upstream so improvements can be merged in.

## Where a change belongs

- **Branding, deployment, hosting, docs for this fork:** open an issue or pull request here, on `bizztor/seoshark`.
- **The SEO engine itself** (crawler, audit rules, MCP tools, data providers): these files are merged from upstream regularly. A fix that would help every OpenSEO fork is best sent upstream as well, so it does not have to be re-applied after each merge. Open the issue here first if you are unsure; we will say where it should go.

## Issues: the best way to contribute

A succinct, clearly written issue describing the problem you are facing and the behavior you want is the most useful thing you can send. It is much faster to review than a pull request, and small, well-scoped issues often get built the same week.

### /simple-issue-description

To keep issues in one voice and format, refine yours with the `/simple-issue-description` skill before filing it. Install it with:

```sh
npx skills add bizztor/seoshark --skill simple-issue-description
```

See [Set up SEOShark Agent Skills](https://seoshark.example/docs/skills/setup) for other install options.

What a good issue contains:

- Enough detail to reproduce or understand the problem: what you did, what happened, what you expected.
- For a feature request, the full user experience you are proposing, not just the mechanism.
- Plain, short sentences. Trim default coding-agent output before posting it.

## Pull requests

Pull requests are welcome, with a few expectations:

- Keep each PR to one change. Large mixed PRs are hard to review and slow everything down.
- Run `pnpm run ci:check` and `pnpm test` before opening the PR, and describe how you verified the change in the description.
- A short screen recording helps a lot for UI changes, and is a good sign the change was actually exercised.
- Changes to the review control plane (`.github/**`, `.greptile/**`, `AGENTS.md`, `CLAUDE.md`, `.agents/skills/**`) need explicit maintainer review; see `CLAUDE.md`.

Generated or agent-written code is fine as long as you have read, run and understood it. Review time is the scarce resource, so a smaller PR you can vouch for beats a larger one you cannot.

## Security

If you find a security issue, do not open a public issue. Email [support@seoshark.example](mailto:support@seoshark.example) instead.
