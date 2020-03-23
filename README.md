Network LDP Configuration
=========

This role will configure ldp parameters for various network vendors (still in development)

Requirements
------------
ncclient


Role Variables
--------------
* logical_interfaces
  * mpls
    * state
    * protocol
  * name
  * unit

Dependencies
------------
Need to configure router id, probably set if you are using IGP role as well

Example Playbook
----------------

    - hosts: vmx1
      roles:
         - { role: network_ldp_configuration }

License
-------

BSD

Author Information
------------------

Marc Colburn
