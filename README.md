# Grafana Dashboards for Icinga

Assumptions:
* Uses "default" Grafana data source
* Default dashboard is "template"
* Tested with Grafana v9.3.1 and Grafana Module v1.4.2

## InfluxQL

| Dashboard | Check Plugin       | Plugin Type                                                                                  | Repeatable | Panels |
|-----------|-------------------------------------------------------------------------------------------------------------------|------------|--------|
| cpu       | check_cpu_usage    | [Contributed](https://github.com/iamcheko/check_cpu_usage)                                   | Yes        | 1      |
| disk      | check_disk         | Default                                                                                      | Yes        | 1      |
| hostalive | check_ping         | Default                                                                                      | No         | 1      |
| icinga    | icinga             | [Built-in](https://icinga.com/docs/icinga-2/latest/doc/10-icinga-template-library/#icinga)   | No         | 3,4,9  |
| icingadb  | icingadb           | [Built-in](https://icinga.com/docs/icinga-2/latest/doc/10-icinga-template-library/#icingadb) | No         | 4      |
| ido       | ido                | [Built-in](https://icinga.com/docs/icinga-2/latest/doc/10-icinga-template-library/#ido)      | No         | 1,2    |
| load      | check_load         | Default                                                                                      | Yes        | 1      |
| memory    | check_linux_memory | [Contributed](https://github.com/hugme/Nag_checks)                                           | Yes        | 4,1    |
|           | check_mem.pl       | [Contributed](https://github.com/justintime/nagios-plugins)                                  | Yes        | 2,4    |
| procs     | check_procs        | Default                                                                                      | No         | 1      |
| ssh       | check_ssh          | Default                                                                                      | No         | 1      |
| swap      | check_swap         | Default                                                                                      | No         | 1      |
| template  | Generic            | Generic                                                                                      | No         | 1      |
| time      | check_ntp_time     | Default                                                                                      | No         | 1      |
| uptime    | check_uptime       | Default                                                                                      | No         | 1      |
