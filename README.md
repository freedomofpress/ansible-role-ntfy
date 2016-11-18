ntfy Ansible role
=================

Configures the [ntfy] pip module for sending alerts.
Many backends are supported: Pushover, Slack, Pushjet.
See the [ntfy] docs for full information.

Requirements
------------

Requires `python-pip`. You'll also need to configure your
API tokens ahead of time, ideally in an encrypted vars file.

Role Variables
--------------

```yaml
# See the ntfy docs for how the config file should be structured:
# https://github.com/dschep/ntfy
ntfy_config: {}
```

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
    - role: ntfy
      tags: ntfy
```

License
-------

MIT


[ntfy]: https://github.com/dschep/ntfy
