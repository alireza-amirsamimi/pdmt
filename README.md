PDMT(Persian Download Manager Terminal)
=============
+ version : 1.03
+ PDMT is a download manager which is written in bash language and it is based on aria2 and improves aria2.

### Before running install file make sure that all dependencies are installed on your system!

## Dependencies for Ubuntu
You must install `aria2` , `pm-utils`, `wget` .

    $ sudo apt-get install aria2 pm-utils wget

After installing dependencies, change your directory with cd command and run install file

    $ sh install

for uninstall PersianDM,

    $ sh unistall

### or...

    $ cd
    $ cd /tmp
    $ wget -O pdmt.tar.gz https://github.com/alireza-amirsamimi/pdmt/archive/master.tar.gz
    $ tar  --overwrite --overwrite-dir -xf pdmt.tar.gz
    $ cd pdmt-master
    $ sh install

## Some features:

+ PDMT configures aria2 automatically for best speed according to your file size

+ you can adjust start time and end time for downloads

+ download queue

+ PDMT can shutdown or suspend or hibernate system  after download 

and ...

+ Tested on Ubuntu 14.04 , Kubuntu 14.04 , Xubuntu 14.04
+ You can see the Screenshots of PersianDM at http://amirsamimi.mihanblog.com/post/17

## Contact me
Me on twiter:
https://twitter.com/AR_AmirSamimi

My weblog:
http://amirsamimi.mihanblog.com

My email adress:
alireza.amirsamimi@ubuntu.ir
