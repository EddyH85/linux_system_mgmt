Linux System Management (In Development)
=========

This is unified Ansible Role to centrally manage some Linux system settings, for open(SUSE), Red Hat/ CentOS and Debian based Distris on Bare-Metal, Vmware vSphere, IBM PowerVM or Cloud Managed Installation.

This role is suitable for system rollout, manage existing systems with ansible to verify some Settings and/or to change them.

The following settings are managed with it:
- Subscription Management (Linux Distribution specific)
- local Users, Pre-Shared-keys and entries in to sudoers
- Set Plattform specific settings and install latest Hypervisor Tools (vSphere, PowerVM, Cloud, Bare-Metal etc.)
    - for Example: I/O Scheduler, Kernel oder mutipath Settings
- Import custom certificates (PKI)
- NTP Client (chronyd)
- DNS Servers settings
- Manage the /etc/hosts entries for the local host with the entries from the DNS server
- Manage other Services, for example Postfix etc.
- Install Monitoring, Performance or Dokumentations Tools (for Example Check_mk and LPAR2RRD)

Requirements
------------

Basic installed Linux System with Ansible Package, existing ansible User and exchanged PSK for the ansible User.

Installation
------------

ansible-galaxy install EddyH85.linux_system_mgmt

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
