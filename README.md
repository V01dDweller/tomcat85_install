tomcat85\_install
=================

Installs Tomcat 8.5.23 from binary tar ball on EL 7 Linux.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

See role defaults.

```yaml
# file: defaults/main.yml
---
tomcat_user: tomcat
tomcat_group: tomcat
tomcat_dir: '/opt/apache-tomcat'
tomcat_version: 8.5.23
...
```

Dependencies
------------

Requires JDK with JAVA\_HOME set. 

Example Playbook
----------------

```yaml
---
- name: Install Tomcat 8.5
  hosts: all
  become: yes
  roles:
    - V01dDweller.tomcat85_install
...
```

License
-------

BSD

Author Information
------------------

By V01dDweller, 2019.
