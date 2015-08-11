PDMT(Persepolis Download Manager Terminal)
=============
+ version : 1.15.2
+ PDMT is a download manager which is written in bash language and it is based on aria2 and improves aria2.

![ScreenShot](http://s6.picofile.com/file/8202702626/pdmt.jpg)

### Before running install file make sure that all dependencies are installed on your system!
You must install `aria2` , `pm-utils`, `wget` , `bc` , `vorbis-tools` , `xclip`
For using flashgot plugin on firefox , you must install `xterm` , `zenity`

## Dependencies for Ubuntu

    $ sudo apt-get install aria2 pm-utils wget bc vorbis-tools xdg-utils xclip
    $ sudo apt-get install xterm zenity
    
## Dependencies for Fedora

    $ sudo yum install aria2 pm-utils wget bc vorbis-tools xdg-utils xclip
    $ sudo yum install xterm zenity

## Dependencies for Archlinux

    $ sudo pacman -S aria2 pm-utils wget bc vorbis-tools xdg-utils xclip
    $ sudo pacman -S xterm zenity
    
After installing dependencies, change your directory with cd command and run install file

    $ sh install

for uninstall PDMT,

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

+ If download failed by aria2,PDMT retries to download failed links

+ Compatible with Firefox flashgot

and ...

+ Tested on Ubuntu 14.04 , Fedora 21 , Archlinux 
+ You can see the Screenshots of PDMT at http://amirsamimi.mihanblog.com/post/25

## Contact me
Me on twiter:
https://twitter.com/AR_AmirSamimi

My weblog:
http://amirsamimi.mihanblog.com

My email adress:
alireza.amirsamimi@ubuntu.ir

## Read more about PERSEPOLIS
https://en.wikipedia.org/wiki/Persepolis
