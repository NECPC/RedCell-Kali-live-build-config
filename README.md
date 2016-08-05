#This code is intended for RedCell-Kali ISO maintainers.

If you just use the ISO I make, you don't need to worry about this repo. 

If you want to build your own ISO the same way I do, this code is for you =)


# First Time Setup
apt-get install curl git live-build cdebootstrap

git clone https://github.com/NECPC/RedCell-Kali-live-build-config.git

Now you can simply build an updated Kali ISO by entering the “live-build-config” directory and running our build.sh wrapper script, as follows:


cd live-build-config

./build.sh --distribution kali-rolling --verbose


\#The “build.sh” script will take a while to complete, as it downloads all of the required packages needed to create your ISO. Good time for a coffee.


Some Debian bugs filed for issues encountered in Kali:

\#684865: live-build: lb_binary_syslinux fails to include flavour in menu entry

\#684891: live-build: add a config parameter to define the project name

\#684893: live-build: fails to find bootloaders files when running from git checkout

\#684896: live-build: loading of build.sh does not work as expected in various scripts
