ansible-role-contrast
=========

An ansible role to download an agent from Contrast Security TeamServer.

Requirements
------------

The instance running this role will need network access to the Contrast TeamServer

Role Variables
--------------

```
contrast_api_key: apikey
contrast_service_key: servicekey
contrast_username: email@awesome.com
contrast_teamserver_url: https://app.contrastsecurity.com
contrast_teamserver_organization: blarg-foo-random-things
contrast_agent_type: java?jvm=1_6
contrast_agent_path_group: vagrant
contrast_agent_path_owner: vagrant
contrast_agent_path: "/opt"
```

Dependencies
------------

You will need credentials and network access to a Contrast Security TeamServer to download the agent.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: contrast }

License
-------

BSD

Author Information
------------------

David Hafley
