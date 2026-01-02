# Claude Code Configuration

This directory contains Claude Code configuration files.

## Contents

### commands/
Custom slash commands for Claude Code. Add markdown files here to create new commands.

Example: `.claude/commands/test.md` creates a `/test` command.

### hooks/
Scripts that run during Claude Code sessions:

- `session-start.sh` - Runs when a session starts
- `tool-call.sh` - Runs when tools are called
- `user-prompt-submit.sh` - Runs when user submits a prompt

### rules/
Project rules, guidelines, and accumulated knowledge for Claude Code:

- `README.md` - Overview of the rules system
- `document-update-workflow.md` - Workflow for updating documentation
- `coding-standards.md` - Coding standards and best practices
- `troubleshooting.md` - Known issues and solutions
- `patterns.md` - Implementation patterns and design decisions
- `project-memory.md` - Project-specific knowledge and context

**Important:** Claude Code should read these files at the start of each session to understand project conventions and accumulated knowledge.

## Documentation

For more information about Claude Code configuration, visit:
https://github.com/anthropics/claude-code
