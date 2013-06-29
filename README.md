rpm-zeromq
==========

An RPM spec file for ØMQ. This RPM is for 2.1.7 to be compatible with Storm.


To Build:

`sudo yum -y install rpmdevtools && rpmdev-setuptree`

`sudo yum -y install glib2-devel libuuid-devel e2fsprogs-devel`

`wget https://raw.github.com/nmilford/rpm-zeromq/master/zeromq.spec -O ~/rpmbuild/SPECS/zeromq.spec`

`wget http://download.zeromq.org/zeromq-2.1.7.zip -O ~/rpmbuild/SOURCES/zeromq-2.1.7.zip`

`rpmbuild -bb ~/rpmbuild/SPECS/zeromq.spec`