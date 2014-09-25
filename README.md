ansible-xnat
============

**WARNING: work in progress**

Deploys a [XNAT](http://www.xnat.org). 

XNAT is an open source imaging informatics platform, developed by the Neuroinformatics Research Group at Washington University. It facilitates common management, productivity, and quality assurance tasks for imaging and associated data. Thanks to its extensibility, XNAT can be used to support a wide range of imaging-based projects.

Quickstart
----------

This playbook assumes that you have installed `ansible` beforehand, if not:

    pip install ansible

If you use [VirtualBox](https://www.virtualbox.org/wiki/Downloads) and [Vagrant](http://www.vagrantup.com/downloads.html), just run:

	vagrant up

If you want to deploy on bare metal:

    ansible-playbook site.yml 192.168.0.1,

or... maybe you prefer [puppet for XNAT deployment](https://bitbucket.org/bigr_erasmusmc/puppet-xnat)?


License
-------

GPLv3

Author Information
------------------

Roman Valls Guimera,
http://blogs.nopcode.org/brainstorm
