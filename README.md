sonic-db-sql
-------------

sonic-db-sql is rapper to db-sql api used for VM target.



Description
-----------
VM presents an abstraction of the hardware (thermal sensors, fans, LEDs,
optics,interfaces, etc.) in a VM environment. SDI-VM's sole client is PAS, similarly SAI-Vm client is NAS and it queries
the devices using the API defined in sdi-api and functionality in sai-api.

Building
--------
Please see the instructions in the sonic-nas-manifest repo for more details on the common build tools.  [Sonic-nas-manifest](https://stash.force10networks.com/projects/SONIC/repos/sonic-nas-manifest/browse)

Development Dependencies:

 - sonic-logging
 - sonic-common-utils
 - libsqlite3-dev

Dependent Packages:

 - libsonic-logging1 libsonic-logging-dev libsonic-common1 libsonic-common-dev

BUILD CMD: sonic_build --dpkg libsonic-logging1 libsonic-logging-dev libsonic-common1 libsonic-common-dev -- clean binary

(c) Dell 2016
