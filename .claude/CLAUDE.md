# Claude MM Tool - Project Instructions

## Git Commit Guidelines

**IMPORTANT: Do NOT include "Co-Authored-By" lines in commit messages.**

When creating commits, write clear, concise commit messages that focus on what changed and why, without attribution lines.

## Push Workflow

When the user says "push", follow this workflow in order:

1. **Auto-fix lint**: Run `./run lint fix` to auto-fix any linting issues
2. **Manually fix remaining lint errors**: If `./run lint fix` couldn't fix all errors, manually fix them
3. **Verify lint**: Run `./run lint` to confirm all linting errors are resolved
4. **Fix test failures**: Run `./run test` and fix any failing tests
5. **Push**: Run `git push` to push commits to remote

**Important:**
- Always run `./run lint fix` first before manual fixes
- Do not push if linting errors remain
- Do not push if tests fail
