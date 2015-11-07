#How to install pyspades on Ubuntu or Debian

##First, install the dependencies:

```
sudo apt-get install python2.7 python2.7-dev python-setuptools python-twisted mercurial gcc g++ zope.interface
sudo python -m easy_install cython
sudo python -m easy_install pil
sudo python -m easy_install jinja2
```

##Optionally, install byobu and pygeoip:

```
sudo apt-get install byobu
sudo python -m easy_install pygeoip
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
vim config.txt
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

*Fork and source:* https://github.com/infogulch/pyspades/wiki/Setup-Ubuntu
