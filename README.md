# sre-checklist

Reliability reviews need concrete questions about ownership, incident response, and production changes. Use this SRE checklist to identify gaps in your team's practices, or as a starting point for a Kubernetes reliability checklist.

**These checklists are opinionated.** Adapt each item to your responsibilities and environment; an unchecked box is a discussion point, not an automatic failure.

## Features

- Define team responsibilities for infrastructure, monitoring, incident management, and reliability automation.
- Review skills such as coding, CI/CD, infrastructure as code, and configuration management.
- Clarify incident reporting, alert ownership, coverage requirements, and manual response steps.
- Organize production reviews around provisioning, deployment, configuration, and resiliency.
- Identify technology-specific review areas for Git, cloud infrastructure, Kubernetes, GitOps, and Terraform.

## Installation

The supplied project material describes a Markdown checklist. Although the repository metadata lists Go, it does not document a Go executable, command-line interface, or release archive.

Read the checklist directly in the repository. No Go installation is required for that workflow.

If a Go implementation is added, the usual local build commands would be:

```sh
go version
go build -o sre-checklist .
```

These commands require a Go module with a main package; that structure has not been established here. The following release-download template uses the requested tag. Replace `OWNER` with the standalone project's GitHub owner, and confirm the release and asset exist before use:

```sh
curl -fL -o sre-checklist-v0.1.0.tar.gz https://github.com/OWNER/sre-checklist/releases/download/v0.1.0/sre-checklist-v0.1.0.tar.gz
```

## Usage

Copy the relevant checklist into a team document or review issue. Record an owner and follow-up action beside each unresolved item.

For example:

```markdown
### Incident management

- [ ] Document where incidents are reported.
- [ ] Assign responsibility for monitoring alerts during each coverage period.
- [ ] Decide whether round-the-clock coverage is required.
- [ ] Record which response steps still require manual tickets.
```

A possible future CLI invocation would look like this:

```sh
./sre-checklist --section team --format markdown
```

**This invocation is illustrative, not an implemented interface.** The donor material does not establish executable behavior or supported flags.

## License

Apache-2.0. This project is based on [bregman-arie/sre-checklist](https://github.com/bregman-arie/sre-checklist).

When redistributing adapted material, retain applicable copyright and attribution notices, include the license, and identify modified files. Preserve any applicable NOTICE content supplied upstream.

## Related projects

The supplied related-project list contains repositories under different GitHub owners; common authorship and their functionality are not established by the provided material.

- [RedZinXL/warc-gpt](https://github.com/RedZinXL/warc-gpt): Consult its README for its purpose and supported workflows.
- [boostlyapi/autonomous-agentic-rag](https://github.com/boostlyapi/autonomous-agentic-rag): Consult its README for its purpose and supported workflows.
- [Akshay-G-Dev/skooner](https://github.com/Akshay-G-Dev/skooner): Consult its README for its purpose and supported workflows.

