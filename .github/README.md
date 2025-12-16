# PR Title Check

All Pull Request titles must follow this format to link changes to JIRA tickets:

```
[PROJECTKEY-123]: Description
```

## Format Rules

- JIRA key in square brackets: `[PROJECTKEY-123]`
- Project key: uppercase letters (e.g., `DO`, `FE`, `FIN`)
- Ticket number: numeric (e.g., `123`, `256`)
- Colon separator: `:` (space after colon is optional)
- Description: clear, concise text

## Valid Examples

* `[DO-256]: Create DB user`
* `[FE-101]: Add login API`
* `[FIN-202]: Update payment flow`
* `[OPS-45]: Fix deployment issue`

## Invalid Examples

* `DO-256: Create DB user` - Missing brackets
* `[do-256]: Fix issue` - Lowercase project key
* `[DO256]: Fix issue` - Missing hyphen
* `Fix login issue` - Missing JIRA key

## Merge Requirements

PR can be merged only when:
1. ✅ PR title matches format `[PROJECTKEY-123]: Description`
2. ✅ PR Title Check GitHub Action passes
3. ✅ Code Owner approval received (if configured)

**No valid JIRA key = No merge.**