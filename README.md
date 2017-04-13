Ansible Role: jq
=========

Install [jq](https://stedolan.github.io/jq/), a lightweight and flexible command-line JSON processor, on any Linux system.

Requirements
------------

None.

Role Variables
--------------

`jq_version`: The version of jq. Avaiable values: 1.5, 1.4, 1.3. (default: 1.5)

Dependencies
------------

None

Installing
----------

This role is only avaiable on github. You can install it by create a `roles.yml` file and install it by `ansible-galaxy install -r roles.yml`

The jq role section of the content of the roles.yml

```yaml
# jq
- src: https://github.com/djx339/ansible-role-jq
  name: jq
```


Example Playbook
----------------

Using default version:

    - hosts: servers
      roles:
        - { role: jq }


Specify version:

    - hosts: servers
      roles:
         - { role: jq, jq_version: 1.5 }

License
-------

BSD

Author Information
------------------

This role was created by [Daniel D](https://github.com/djx339).
