# check-consul
## Description
Checks for Consul.

## Usage
```
check-consul [subcommand] [options]...
```

### check-consul leader-lost [-h host] [-p port] [-w] [-c]
    Description:
        alert when consul leader lost.

    Options:
        -h  consul agent host (default: 127.0.0.1)
        -p  consul agent port (default: 8500)
        -w  set alert level WARNING. exit status 1. (default: not selected)
        -c  set alert level CRITICAL. exit status 2. (default: selected)

### check-consul server-nodes-changed [-h host] [-p port] [-t temp_file] [-w] [-c]
    Description:
        alert when consul server nodes list changed.

    Options:
        -h consul agent host (default: 127.0.0.1)
        -p consul agent port (default: 8500)
        -t save previous server nodes list. (default: /var/tmp/mackerel-agent/consul-server-nodes-changed)
        -w set alert level WARNING (exit status 1). (default: selected)
        -c set alert level CRITICAL (exit status 2). (default: not selected)

### check-consul version
    Description:
        show version.

## License
Copyright 2017 KAYAC Inc.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
