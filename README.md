# Ansible role for Memcached

This is a simple Ansible role for installing Memcached via ansible-galaxy.

The role should work on all Debian based distributions.

## Installation

Add this to your `requirements.yml`:

```yml
- src: https://github.com/xcdr/ansible-memcached
  name: xcdr.memcached
```

## Example playbook

```yaml
---

- hosts: myhost
  roles: xcdr.memcached

  vars:
    memcached_params:
    - key: "-l"
      value: "0.0.0.0"
```

## License

MIT
