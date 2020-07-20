Ansible-role-supertuxkart
=====================

This role helps installing a Supertuxkart server.

Requirements
------------

Any debian-based linux should work, preferably Ubuntu 20.04.

Tested with:
- Supertuxkart 1.1
- Ansible 2.9.10
- Ubuntu 20.04 on [Gandi Cloud](https://www.gandi.net/fr/cloud)

Role Variables
--------------

| Variable              | Description                                                                                                  | Example                                   |
|-----------------------|--------------------------------------------------------------------------------------------------------------|-------------------------------------------|
| `server_name`     | The public description of the Supertuxkart server                                                      | `your-server-name`                                     |

Dependencies
------------

No dependency, Supertuxkart installed from Github sources (built locally): https://github.com/supertuxkart/stk-code

Example Playbook
----------------

Sample playbook:

```
    - name: Install Supertuxkart
      hosts: all
      roles:
        - nautik1.supertuxkart
```

Sample inventory:

```
all:
  hosts:
    <ip-or-hostname>:
```

License
-------

[WTFPL](https://en.wikipedia.org/wiki/WTFPL)
