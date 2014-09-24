# Ansible Role: Tomcat (6/7)

[![Build Status](https://travis-ci.org/geerlingguy/ansible-role-tomcat6.svg?branch=master)](https://travis-ci.org/geerlingguy/ansible-role-tomcat6)

An Ansible Role that installs Tomcat 6 (or 7) on RedHat/CentOS 6.x and Debian/Ubuntu Linux servers.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `vars/main.yml`):

    tomcat_enabled: true

Whether Tomcat should be started at boot (as well as at the time this playbook is run). Set to false if you would like to leave Tomcat installed but not running, or want to control it on your own.

    tomcat.server_port: 8005

The port on which the Tomcat server itself will run (not the difference between this and the `tomcat.catalina_port`).

    tomcat.hostname: localhost

The hostname for this server. `localhost` works fine for many Tomcat web applications which are not dependent on a particular hostname being set (e.g. Apache Solr).

    tomcat.catalina_port: 8983

The port on which Catalina will listen for requests. (This is the port through which webapps will be accessible).

    tomcat.catalina_redirect_port: 8443

This is the port to which requests will be redirected if they come in on a non-SSL port, but are required to be secure via a security constraint.

## Dependencies

  - geerlingguy.java (Installs Java for CentOS 6.x).

## Example Playbook

    - hosts: webservers
      vars_files:
        - vars/main.yml
      roles:
        - { role: geerlingguy.tomcat6 }

*Inside `vars/main.yml`*:

    tomcat.hostname: example.com
    tomcat.catalina_port: 8080

## License

MIT / BSD

## Author Information

This role was created in 2014 by [Jeff Geerling](http://jeffgeerling.com/), author of [Ansible for DevOps](http://ansiblefordevops.com/).
Shortly after generalized for Tomcat7 by [Roman Valls Guimera](http://blogs.nopcode.org/brainstorm)
