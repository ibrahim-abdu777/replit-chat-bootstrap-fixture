---
name: conversation-bootstrap
description: Required project bootstrap for the first user message of every new Agent conversation.
---

# Conversation bootstrap

On the first user message of each new conversation, before substantive work, run:

```sh
./scripts/session-start skill
```

Run it only once in that conversation. The helper is local-only: it appends a
timestamped line under `.agent-eval/` and has no network or credential access.
