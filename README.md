Persepolis Download Manager (PDM)
=============
+ version : 1.18.1
+ Persepolis Download Manager is a download manager which is written in bash language and it is based on aria2 and improves aria2.

![ScreenShot](http://s6.picofile.com/file/8202702626/pdmt.jpg)

![ScreenShot](http://s3.picofile.com/file/8205810476/Screenshot_2015_08_12_09_46_26.jpg)

### Before running install file make sure that all dependencies are installed on your system!
You must install `aria2` , `pm-utils`, `wget` , `bc` , `vorbis-tools` , `xclip` , `xterm` , `zenity` , `libnotify-bin` , `youtube-dl`

## Dependencies for Ubuntu

    $ sudo apt-get install aria2 pm-utils wget vorbis-tools xdg-utils xclip  libnotify-bin xterm zenity youtube-dl
    
## Dependencies for Fedora

    $ sudo yum install aria2 pm-utils wget vorbis-tools xdg-utils xclip  libnotify xterm zenity youtube-dl

## Dependencies for Archlinux

    $ sudo pacman -S aria2 pm-utils wget vorbis-tools xdg-utils xclip  libnotify xterm zenity youtube-dl
    
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

+ Downloading from youtube & aparat & ...

+ If download failed by aria2,PDM retries to download failed links

+ Compatible with Firefox flashgot

and ...

## Options

 -l
      Your Download link.(Use "" for links)

	$ pdmt -l "https://www.google.com/images/srpr/logo11w.png"

 -c
      Configure PDMT!change download folder and ...

	$ pdmt -c

 -i
	If you use proxy , Set Proxy IP.for example 127.0.0.1


 -p
	If you use proxy , Set Proxy  Port.for example 8580

	$ pdmt -l "https://www.google.com/images/srpr/logo11w.png" -i 127.0.0.1  -p 8580

 -u
	If you use proxy and your proxy requires username,enter
        Proxy Username.

 -a
	If you use proxy and your proxy requires password,enter
        Proxy Password.

	$ pdmt -l "https://www.google.com/images/srpr/logo11w.png" -i 127.0.0.1 -p 8580 -u hasan -a kamran
        
 -j
      Set HTTP user.


 -k
      Set HTTP password.

	$ pdmt -l "https://www.google.com/images/srpr/logo11w.png" -j alireza -k salam

 -s
	If you want your download to start at specific time ,
        Set Start time for download in form hh:mm (24 hour format).
        for example 13:24
        Download will be Started at start time.

	$ pdmt -l "https://www.google.com/images/srpr/logo11w.png" -s 13:24

 -e
	If you want your download to pause at specific time ,
        Set End time for download in form hh:mm (24 hour format).
        for example 2:25
	Download will be Paused at end time.

	$ pdmt -l "https://www.google.com/images/srpr/logo11w.png" -e 2:25

example for start at 2:00 and end at 7:00

	$ pdmt -l "https://www.google.com/images/srpr/logo11w.png" -s 2:00 -e 7:00

 -m
	PDMT selects maximum possible 
        number of connections automatically.but you can choose maximum number
        yourself(1-16).default is 16.

	$ pdmt -l "https://www.google.com/images/srpr/logo11w.png" -m 3

 -o
	Aria2 options
        you can write aria2 options after o,for example:

	$ pdmt -l "https://www.google.com/images/srpr/logo11w.png" -o --max-download-limit=10k
        
        
 -d
	After download PDMT can shutdown , hibernate , suspend computer.
        (options are shutdown , hibernate , suspend )



 -w
      Root Password.if you choose one of the after download options,you must 
        enter root password.if you don't enter password after -w or if you enter
        wrong password,PDMT will ask you for root password before start downloading.

	$ pdmt -l "https://www.google.com/images/srpr/logo11w.png" -d shutdown -w salam

 -f
      Download queue.if you have many links and you want to download them in
        queue(one by one),you can use this option.links must enterd in a file
        in seperate lines.every line for one link with no space between lines.
        after that you must enter the file's address that you save links in it.
        for example :
	$ pdmt -f /home/alireza/links.txt

-y      Downloading from Youtube and ...
	enter your youtube link after l and use y switch

        $ pdmt -l "https://www.youtube.com/watch?v=MMwXF9Kveus" -y
	
	you can use queu too.

	$ pdmt -f /home/alireza/links.txt -y

	you can find supported video site here:
	
	https://github.com/rg3/youtube-dl/blob/master/docs/supportedsites.md


 -h
      See help of pdmt

	$ pdmt -h

 -v
      Version of PDMT

	$ pdmt -v

more examples:

	$ pdmt -l "http://www.example.com/2.iso"

or

	$ pdmt -f /home/alireza/links.txt

or (with proxy and start time and end time and shutdown after end time)

	$ pdmt -l "http://www.example.com/2.iso"  -i 127.0.0.1 -p 8580 -s 2:30 -e 7:00 -d shutdown -w mypass

or for download queue

	$ pdmt -f /home/alireza/links.txt  -i 127.0.0.1 -p 8580 -s 2:30 -e 7:00 -d shutdown -w mypass

When download completes you can find your file in :
	
	$ ~/Downloads/Persepolis

before download completes you can find your file in :

	$ ~/.persepolis 

if your download canceled or failed you can get link to PDMT again .PDMT will resume download.

you can find summary of your downloads(link , ...) in a text file :

	$ ~/Downloads/Persepolis/report

![ScreenShot](http://s6.picofile.com/file/8205821142/report.jpg)
##PersepolisDM GUI
you can use PersepolisDM simple GUI for Downloading too.

After installation you can find PersepolisDM in your menu

![ScreenShot](http://s3.picofile.com/file/8204789868/2.jpg)

Click on icon
select your Download type (Download single file or queue)

![ScreenShot](http://s6.picofile.com/file/8213595650/1.jpg)

select Download type (Download single file or queue or Yotube)

after that PersepolisDM will guide you :)

##Configuring PersepolisDM to use with FlashGot
open firefox
open menu
click add-ons
click on get add-ons
in the search box search the flashgot
then click on install and install it
restart the firefox (close and open it again)

![ScreenShot](http://s6.picofile.com/file/8204848942/20.jpg)

then after opening firefox go to Extensions and find flashgot
then click on preferences and click add
write pdmt and select this file for executble path

	$ ~/.persepolis_download_manager_terminal/pdmt_flashgot_gtk

or if you want to FlashGot use GUI use this address

	$ ~/.persepolis_download_manager_terminal/pdm_flashgot_gtk

then in the white field copy/paste the following codes

	$  [-l URL][-g FNAME][-b REFERER][-c COOKIE][-u UA][-h HEADERS]

![ScreenShot](http://s3.picofile.com/file/8210020868/Screenshot_2015_09_03_16_22_31.jpg)

then at the end click on the advance tab and uncheck automatic download manager detection

![ScreenShot](http://s3.picofile.com/file/8204846676/16.jpg)

and on media tab select pdmt

![ScreenShot](http://s3.picofile.com/file/8204846634/15.jpg)

then Click OK!

you can use flashgot for download from youtube , ...

![ScreenShot](http://s4.picofile.com/file/8179632850/11.jpg)

![ScreenShot](http://s6.picofile.com/file/8179631500/10.jpg)

![ScreenShot](http://s3.picofile.com/file/8204847092/17.jpg)



if you use flashgot for youtube or downloading or ... ,a window apears and ask you options

![ScreenShot](http://s3.picofile.com/file/8205813268/form.jpg)

enter your options or if you don't need an option , so leave the field empty!

after that click ok and enjoy!
## Contact me
Me on twiter:
https://twitter.com/AR_AmirSamimi

My weblog:
http://amirsamimi.mihanblog.com

My email adress:
alireza.amirsamimi@ubuntu.ir

PersepolisDM Telegram Channel:
https://telegram.me/persepolisdm

## Read more about PERSEPOLIS
https://en.wikipedia.org/wiki/Persepolis
