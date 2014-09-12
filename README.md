Role Name
=========

Deploys a [XNAT][1] instance to analyze and store and manipulate [fnmri][2] datasets together with accompanying [DICOM][3] metadata.

Quickstart
----------

If you want to deploy on bare metal:

    ansible-playbook site.yml 192.168.0.1,

If you use VirtualBox/Vagrant, just run:

	vagrant up

License
-------

GPLv3

Author Information
------------------

Roman Valls Guimera
http://blogs.nopcode.org/brainstorm

 [1] http://www.xnat.org/
 [2] http://en.wikipedia.org/wiki/Functional_magnetic_resonance_imaging
 [3] http://en.wikipedia.org/wiki/DICOM
