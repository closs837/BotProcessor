# BotProcessor

A small discord.py self-bot: a command processor with cogs for the things I kept needing —
meta commands such as `close` and `uptime`, a REPL for evaluating snippets from chat,
regional-indicator text and a handful of slash-command experiments.

The `bot` package is the whole thing: `bot/__init__.py` sets up the client and logging,
`bot/cogs/` holds the command groups, and `bot/__main__.py` is the entry point.

```
pipenv install
python -m bot
```

`Pipfile` pins discord.py's `rewrite` branch along with `aiohttp` and `websockets`; the
token is read from `TOKEN_DISCORD` in the environment.
