# promtail_logparser
---
..*For testing, the binary and the configurations are made available in the /opt/promtail
..*The standard installation procedure with service file configuration has to be made for production

###test command to debug the log parsing

`cat lokiregexsample.log | /opt/promtail/promtail-linux-amd64 -config.file=/opt/promtail/config-promtail.yml --stdin --dry-run --inspect --client.url http://127.0.0.1:3100/loki/api/v1/push`
