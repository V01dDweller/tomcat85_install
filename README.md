# Tomcat 8.5.23 Binary Install #

This is a set  of ansible playbooks and roles that downloads the Tomcat 8.5.23 tar file from Apache and installs it as a systemd service on CentOS7/RHEL7.

Usage:

```
ansible-playbook -i myhosts.ini [-e 'proxy=proxy.domain.com:8080'] tomcat85_install.yml
```

```
Files:
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

