# Tomcat 8.5.23 Binary Install #

This an ansible playbook and role that downloads the Tomcat 8.5.23 tar.gz file from Apache then installs it as a systemd service on CentOS7/RHEL7. It uses the [oracle_jdk8_install](https://github.com/V01dDweller/oracle_jdk8_install) role which can be skippped if OpenJDK 8 or Oracle JDK 8 is already installed. An uninstall playbook/role is also included.

Tested successfully on CentOS 7 with ansible 2.4.

Usage:

```
ansible-playbook -i myhosts.ini [-e 'proxy=proxy.domain.com:8080'] tomcat85_install.yml
```

```
tomcat85_install
├── README.md
├── roles
│   ├── tomcat85_install
│   │   ├── files
│   │   │   └── tomcat.service
│   │   └── tasks
│   │       └── main.yml
│   └── tomcat85_uninstall
│       └── tasks
│           └── main.yml
├── tomcat85_install.yml
└── tomcat85_uninstall.yml
```
