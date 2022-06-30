---
layout: default
title: Configuration
nav_order: 5
---

# Configuration

## Configure Splunk

- Configure a new index (e.g. pinsafe) for the new logs
- Configure inputs

### Receiving syslogs on Splunk

NOTE: Its recommended to use a separate and dedicated syslog solution (e.g. rsyslog, syslog-ng, etc).

- Configure new TCP port (e.g. 514) pointing to the new index using the "pinsafe" sourcetype

```
[udp://<ip_address>:<port>]
connection_host = ip
index = pinsafe
sourcetype = pinsafe
disabled = 0

```


### Monitoring log files
- Configure a new file monitor input pointing to the new index using the "pinsafe" sourcetype