opsware-agent-tools
=========

Interacting with SA by using of opsware-agent and agent tools.

Requirements
------------

opsware-agent and agent tools are required. Please make sure they are installed properly.

Role Variables
--------------

N/A

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

fbbit@hotmail.com
