# Audit Context Command

This command audits the `context.md` context and `bugs.md` bugs files, and updates them     
accordingly.

## Usage

```
/audit-context
```

## Implementation Steps

1. **Verify Context Claims**: Using extended reasoning mode, verify all claims in `context.md` by reading all *.md and docs/* documentation as necessary, as well as any source files. Do any tests you need to complete this task in full.
2. **Update Context**: Update `context.md` according to your thorough assessment so that the next instance knows exactly what needs to be done next. Make sure to include all outstanding bugs in `bugs.md` first. Make no other changes.
3. **Update Bug Tracking**: Update `bugs.md` to move verified fixed bugs to the "VERIFIED FIXED" section. Create that section if it doesn't exist.

Never modify tasks.md - it's the reference checklist for the current tasks

## Output

The command provides a comprehensive context audit summary including:
- The result of (1) above
- A summary of changes to `context.md` from (2) above
- A summary of changes to `bugs.md` from (3) above
- Next actions and priorities

