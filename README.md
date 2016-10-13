Simple ansible plays to install iperf3 and mtr on some number of servers
and run the tests.


## Usage:

Configure a hosts.ini with your IPs. See 'hosts.example.ini'. You need
an even number of hosts so that iperf can pair servers and clients together.

## Installation:

```
 $ ansible-playbook -i ./hosts.ini install.yml
```

## Execution:

```
 $ ansible-playbook -i ./hosts.ini perf.yml
```

The results after the execution go into a _results_ directory.
