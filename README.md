ansible-xnat
============

Deploys a [XNAT](http://www.xnat.org) instance to analyze and store and manipulate [fnmri](http://en.wikipedia.org/wiki/Functional_magnetic_resonance_imaging) datasets together with accompanying metadata ([DICOM](http://en.wikipedia.org/wiki/DICOM) among others).

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
