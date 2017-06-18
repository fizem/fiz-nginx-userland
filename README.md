# fiz-nginx-userland
Objective is to build an nginx rpm package based on user webadm01 and install in a custom rpm database.

How to build the package : 
* Download the nginx.1.13.0.tar.gz tarball from www.nginx.org
* Create a user webadm01 with home directory /home/webadm01 
* Create the following struture : mkdir -p rpmbuild/{SOURCES,SRPMS,RPMS,BUILD,BUILDROOT,SPECS}
* Upload the tarball in ~webadm01/rpmbuild/SOURCES
* To be completed later

How to initialize the rpm database
rpm --initdb --dbpath /home/webadm01/.rpm/rpmdb

How to install the rpm package
rpm -ivh --dbpath /home/webadm01/.rpm/rpmdb --nodeps nginx-1.13-0.i686.rpm



