# MastodonStream2Slack

## がいねんず

```
Stream: Mastodon -> Slack
```

## requirements

- Bash (zsh)
- curl
- jq

## config

Put `config.json` like

```json
{
    "server": "kirakiratter.com",
    "slack": {
        "channel": "#timeline",
        "webhook": "https://hooks.slack.com/services/0008G(slack-webhook-url)Z000400000080000w000"
    },
    "auth":
        {"access_token":"ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff",
        "token_type":"bearer","scope":"read write follow","created_at":1506900000}
}
```

`.auth` is the response of `/oauth/token` (only `.access_token` required) (e.g. https://github.com/cympfh/mastodon-cli/blob/master/mast#L164 ).

## usage

```bash
bash ./m2s
```

