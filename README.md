#How to install pyspades on Ubuntu or Debian

* Description: Easy-to-deploy pyspades dedictated linux server
* Tested Linux distro's: `Ubuntu 14.04.3` and `Debian 8.2`

##First, install the dependencies:

```
sudo apt-get install python2.7 python2.7-dev python-setuptools python-twisted mercurial gcc g++ zope.interface cython
sudo easy_install cython
```

##Optionally, install byobu:

```
sudo apt-get install byobu
```

##Then clone the repository:

```
git clone https://github.com/kinvaris/pyspades.git
cd pyspades
sh build.sh
```

##Edit the configuration:

```
cd feature_server
vim config.txt.default
```

##Then, to run the server, either:

```
sh run_server.sh
```

##or if you installed byobu:

```
byobu
sh run_server.sh
```

##How to connect to the server:

* If connected to master-server, you can connect like this: `aos://514818670:32887`
* If you want to connect directly to the dedicted server *(make sure the port is open on the firewall or port-forwarded)*: `aos://192.168.1.2`

*Fork & source:* https://github.com/infogulch/pyspades/wiki/Setup-Ubuntu
