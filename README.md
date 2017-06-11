# slack2bq

## Prepare

```shellsession
$ echo "export SLACK_TOKEN='YOUR_SLACK_TOKEN'" > secret.sh
```

## Execute

```shellsession
$ bundle
$ . ./secret.sh
$ bundle exec fluentd --config etc/fluentd/slack-logs.conf --use-v1-config -vv
```
