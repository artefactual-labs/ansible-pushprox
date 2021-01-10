# Ansible Role: pushprox

## Description

Deploy [PushProx](https://github.com/prometheus-community/PushProx) proxy and client using ansible.

## Requirements

- Ansible >= 2.7 (It might work on previous versions, but we cannot guarantee it)

## Role Variables

All variables which can be overridden are stored in [defaults/main.yml](defaults/main.yml) file as well as in table below.

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| `pushprox_proxy_web_listen_address` | "0.0.0.0:8080" | Address on which pushprox-proxy will listen |

## Example

### Playbook

Use it in a playbook as follows:
```yaml
- hosts: all
  roles:
    - artefactual.pushprox
```
