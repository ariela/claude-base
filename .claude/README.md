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

## Documentation

For more information about Claude Code configuration, visit:
https://github.com/anthropics/claude-code
