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

Put `config.sh` like

```bash
SERVER=mstdn.jp
USER_TOKEN=fd00000000000000000000000000000000000000000000000000000000000000
SLACK_CHANNEL="#timeline"
SLACK_WEB_HOOK=https://hooks.slack.com/services/T22222222/BDDDDDDDD/XYZZZZZZZZZZZZZZZZZZZZZZ
```

`USER_TOKEN` is the mastodon auth token,
which is in the response of `/oauth/token` (as `.access_token`) (e.g. https://github.com/cympfh/mastodon-cli/blob/master/mast#L164 ).

## usage

```bash
bash ./m2s
```

