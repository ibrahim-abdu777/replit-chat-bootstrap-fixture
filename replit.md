# Conversation bootstrap context

For this project, process the first user message in every new Agent conversation
by running the following harmless project-local bootstrap before substantive work:

```sh
./scripts/session-start replit-md
```

Run it once for the first message only, not on later messages in the same chat.
The helper only appends a timestamped line beneath `.agent-eval/`.
