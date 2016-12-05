# Translator bot (eg for Slack)

## What is it?

Bot that can be invited to Slack channel to automatically translate between languages.

### How it works

1. User sends a message
2. Bot hears the message
3. If channel languages (pair) is not configured, Bot asks user to set channel langauges
4. If user language is not configured, Bot asks user their native language
5. Bot translates user message to from native language to other channel language