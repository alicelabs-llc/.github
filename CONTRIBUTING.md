# Contributing to AliceLabs LLC

Thank you for your interest in contributing to our open-source projects.

## Which repo to contribute to?

| You want to... | Go to |
|----------------|-------|
| Fix a bug in the SAM.gov SDK | [`samgov-sdk`](https://github.com/alicelabs-llc/samgov-sdk) |
| Improve the scoring engine | [`govcon-scoring`](https://github.com/alicelabs-llc/govcon-scoring) |
| Fix a legal article or add a new code | [`ecuadorian-legal-codes`](https://github.com/alicelabs-llc/ecuadorian-legal-codes) |
| Add a Burp Suite template | [`burp-quicknotes`](https://github.com/alicelabs-llc/burp-quicknotes) |
| Add a Supabase RLS policy | [`supabase-rls-templates`](https://github.com/alicelabs-llc/supabase-rls-templates) |

## General guidelines

### Commit conventions

We use [Conventional Commits](https://www.conventionalcommits.org/) across all repos:

```
feat: add deadlineFrom filter to search()
fix: correct NAICS scoring when profile has no codes
docs: add Python usage example to ecuadorian-legal-codes
test: add edge case for null responseDeadline
chore: bump vitest to 2.x
```

### PR process

1. Fork the target repo
2. Create a descriptive branch: `feat/add-pagination-cursor` or `fix/null-deadline-crash`
3. Follow the repo-specific `CONTRIBUTING.md`
4. Ensure CI passes before requesting review
5. Fill out the PR template completely

### Code standards

- TypeScript repos: strict mode, no `any`, tests required for new logic
- SQL repos: comments on every policy explaining the business rule
- Data repos: cite sources for all data changes

## Reporting bugs

Use the [bug report template](https://github.com/alicelabs-llc/.github/blob/main/.github/ISSUE_TEMPLATE/bug_report.md) in the relevant repo.

## Security vulnerabilities

**Do not open a public issue for security vulnerabilities.**  
Email [security@alicelabs.site](mailto:security@alicelabs.site) — see [SECURITY.md](SECURITY.md).

## Questions

[contacto@alicelabs.site](mailto:contacto@alicelabs.site)
