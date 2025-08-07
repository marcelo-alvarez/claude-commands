# Continue work command

This command continues the ongoing work described in the `context.md` context file, the `tasks.md` tasks file, and the `bugs.md` bugs file.

## Usage

```
/continue-work
```

## Implementation

1. **Address Bug Fixes**: Address any problems in `bugs.md`
2. **Execute Priority Work**: Proceed with top priorities / next steps as determined from your review of `context.md`
3. **Execute Task Work**: If there is significant context left, tackle the first incomplete tasks in `tasks.md`. Be sure the amount of work started is not so much that the context will have had to be auto-compacted before completion.

Never modify tasks.md - it's the reference checklist for the current tasks.
Never modify context.md - this is outside of the scope of this command.

## Output

The command provides a comprehensive summary including:
- Work accomplished during this session
- Next actions and priorities for future sessions
- Any blockers or issues discovered

