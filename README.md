opsware-agent-tools
=========

Interacting with SA by using of opsware-tools.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

To get CA value form SA, the return value is ca_value which is a list.

    - hosts: servers
      roles:
        - role: opsware-agent-tools
          invoke: get_cust_attr
          ca_name: 
            - example_ca_1
            - example_ca_2

To get customer form SA, the return value is customer_value which is a string.

    - hosts: servers
      roles:
        - role: opsware-agent-tools
          invoke: get_customer

License
-------

BSD

Author Information
------------------

snzh@nnit.com
