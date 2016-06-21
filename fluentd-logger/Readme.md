# fluentd-logger

Receive local logs and forward to another fluentd server, so that the log streams can be transferred in a secure way.

## run

Default settings: receive local from localhost, and write to `` inside container

    # docker run --publish 127.0.0.1:24224:24224 --publish 127.0.0.1:5140:5140 --publish 127.0.0.1:9880:9880 --restart=always {TODO:IMAGE}

- port 24224: fluentd format, used by libraries including docker's [fluentd log driver]()
- port 5140: syslog format
- port 9880: http format
- always restart



Receive more logs:

Forward  (to a remote fluentd server, with ssl)

