Persepolis Download Manager (PDM)
=============
+ version : 1.16.1
+ Persepolis Download Manager is a download manager which is written in bash language and it is based on aria2 and improves aria2.

![ScreenShot](http://s6.picofile.com/file/8202702626/pdmt.jpg)

![ScreenShot](http://s3.picofile.com/file/8205810476/Screenshot_2015_08_12_09_46_26.jpg)

### Before running install file make sure that all dependencies are installed on your system!
You must install `aria2` , `pm-utils`, `wget` , `bc` , `vorbis-tools` , `xclip` , `xterm` , `zenity` , `libnotify-bin`

## Dependencies for Ubuntu

    $ sudo apt-get install aria2 pm-utils wget bc vorbis-tools xdg-utils xclip  libnotify-bin xterm zenity
    
## Dependencies for Fedora

    $ sudo yum install aria2 pm-utils wget bc vorbis-tools xdg-utils xclip  libnotify-bin xterm zenity

## Dependencies for Archlinux

    $ sudo pacman -S aria2 pm-utils wget bc vorbis-tools xdg-utils xclip  libnotify-bin xterm zenity
    
After installing dependencies, change your directory with cd command and run install file

    $ sh install

for uninstall PDM,

    $ sh unistall

### or...

    $ cd
    $ cd /tmp
    $ wget -O pdmt.tar.gz https://github.com/alireza-amirsamimi/pdmt/archive/master.tar.gz
    $ tar  --overwrite --overwrite-dir -xf pdmt.tar.gz
    $ cd pdmt-master
    $ sh install

## Some features:

+ PDM configures aria2 automatically for best speed according to your file size

+ you can adjust start time and end time for downloads

+ download queue

+ PDM can shutdown or suspend or hibernate system  after download 

+ If download failed by aria2,PDM retries to download failed links

+ Compatible with Firefox flashgot

and ...


## Contact me
Me on twiter:
https://twitter.com/AR_AmirSamimi

My weblog:
http://amirsamimi.mihanblog.com

My email adress:
alireza.amirsamimi@ubuntu.ir

## Read more about PERSEPOLIS
https://en.wikipedia.org/wiki/Persepolis
