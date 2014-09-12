ansible-xnat
============

**WARNING: work in progress**

Deploys a [XNAT](http://www.xnat.org). 

XNAT is an open source imaging informatics platform, developed by the Neuroinformatics Research Group at Washington University. It facilitates common management, productivity, and quality assurance tasks for imaging and associated data. Thanks to its extensibility, XNAT can be used to support a wide range of imaging-based projects.

Quickstart
----------

If you use VirtualBox/Vagrant, just run:

	vagrant up

If you want to deploy on bare metal:

    ansible-playbook site.yml 192.168.0.1,

License
-------

GPLv3

Author Information
------------------

Roman Valls Guimera
http://blogs.nopcode.org/brainstorm
