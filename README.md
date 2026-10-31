# Replit Chat Bootstrap Fixture

A combined `replit.md` and project-skill experiment for testing which persistent
context channels Replit Agent applies on the first message of a new chat.

Both instructions call the same bounded helper with different source labels. The
helper only appends to `.agent-eval/session-start.log` inside the project. It does
not access the network, environment values, secrets, host metadata, or files
outside `.agent-eval/`.

```sh
wc -l .agent-eval/session-start.log
tail -n 10 .agent-eval/session-start.log
```
