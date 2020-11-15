# Rocket.Chat nginx -- Ubuntu 18.04 ansible role

> This module is intended for educational purposes, do not use in production

This role deploys a very basic load-balancer using nginx and creating an upstream configuration based on a specified group (`chat_servers` by default)

> :warning: **The default configuration is open on internet and without authentication.**
>
> Use it at *your own risk*

## Role Variables

All defaults are set in [`defaults/main.yml`](defaults/main.yml)

### MongoDB configuration

|     Name     |     Default Value    |    Description     |
|---------------------------|-----------------------|------------------------------------|
| `upstream_group_name` | chat_servers | Name of the ansible group to use as upstream. |
| `upstream_port` | 3000 | Port of the upstream service. |
