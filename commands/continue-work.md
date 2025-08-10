# Continue work command

This command continues the ongoing work described in the `context.md` context file, the `tasks.md` tasks file, and the `bugs.md` bugs file.

## Usage

```
/continue-work
```

## Implementation

1. **Execute Priority Work**: Proceed with top priorities / next steps as determined from your review of `context.md`
2. **Address Bug Fixes**: Address any problems in `bugs.md`

Any errors that you encounter and fix in your workflow should be concisely described, with the correct way of doing it (e.g. things like formatting command line args, sourcing the environment, etc.), in workflow-wisdom.md. If not already created, create workflow-wisdom.md. It should be a quick reference for future instances.
Never modify tasks.md - it's the reference checklist for the current tasks.
Never modify context.md - this is outside of the scope of this command.

## Output

The command provides a comprehensive summary including:
- Work accomplished during this session
- Next actions and priorities for future sessions
- Any blockers or issues discovered

