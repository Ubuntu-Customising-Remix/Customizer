### NAME

Customizer (formerly known as U-Customizer)

	
### SYNOPSIS

    /opt/Customizer/CLI.sh [OPTION] [ARGUMENT]


### DESCRIPTION

Customizer is an advanced LiveCD customization and remastering tool. With it, you can build own Ubuntu-based remix
using Ubuntu Mini Remix, Ubuntu or its derivatives ISO image with a few mouse clicks.


### OPTIONS

    -e,   --extract   Exctract ISO image
    -c,   --chroot    Chroot into the filesystem
    -x,   --xnest     Execute nested X-session
    -p,   --pkgm      Execute package manager
    -d,   --deb       Install Debian package
    -k,   --hook      Execute hook
    -g,   --gui       Install GUI (DE/WM)
    -r,   --rebuild   Rebuild the ISO image
    -q,   --qemu      Test the builded image with QEMU
    -t,   --clean     Clean all temporary files and folders
    -h,   --help      Display this message
    -v,   --version   Show the current version and more


### ENVIRONMENT

    /opt/Customizer                -  Customizer's location
    /opt/Customizer/settings.conf  -  configuration file


### REQUIREMENTS

Core dependencies are:

    coreutils
    sed
    grep
    rsync
    squashfs-tools (>=4.2)
    genisoimage

GUI dependencies are:

    dbus
    xephyr
    qemu
    imagemagick
    gambas2-gb-gui | gambas3-gb-gui
    gambas2-gb-gtk | gambas3-gb-gtk
    gambas2-gb-form | gambas3-gb-form
    gambas2-gb-settings | gambas3-gb-settings
    gambas2-gb-image | gambas3-gb-image
    gambas2-runtime | gambas3-runtime


### INSTALL AND RUN

This is how you can download and install using script from Terminal.

    wget https://github.com/downloads/fluxer/Customizer/install.sh
    chmod +x install.sh
    sudo ./install.sh -i

This is how you can run Customizer from program launcher or Terminal

    sudo /opt/Customizer/GUI.gambas

For alternative methods or more details, refer to the official user guides at https://github.com/fluxer/Customizer/wiki

    
### AUTHORS

Ivailo Monev 'SmiL3y' (code developer) `xakepa10@gmail.com`

Michal Glowienka 'eloaders' (PPA maintainer) `eloaders@yahoo.com`

Mubiin Kimura 'clearkimura' (documentation) `clearkimura@gmail.com`


### BUGS REPORT

Create and submit your issue at https://github.com/fluxer/Customizer/issues

**IMPORTANT** You should include the following details: what version of system host, 
what version of customizer, what ISO image, description of problem, full output log that is 
not just the part of what you consider relevant, and if possible, relevant screenshots.

Example of issue submission details:

    Ubuntu 12.04, Customizer 3.2.1, ubuntu-mini-remix-12.04-amd64. Using GUI, after select 'Build',
    cannot create ISO image file, Terminal shows Error 119: No kernel found when compiling image.

The developers will look into submitted issues from time to time, usually a day or two.
Only issues found in latest versions of Customizer are concerned. Issues in older versions will
be ignored.

To check latest releases, visit https://github.com/fluxer/Customizer/wiki/Changes-log


### COPYRIGHT
    
Copyright (C) 2010-2012  Ivailo Monev

License: GPLv2


### HISTORY

In late 2010, this project was registered on Sourceforge.net. Since November 2011,
documentation is contributed. As December 2011, Customizer development has moved to
GitHub and has been tested thoroughly on Ubuntu 10.04(Lucid Lynx). One year later, 
as December 2012, Customizer stable release has hit 3.2.3.

Presently maintained for compatibility fixes and documentation.


### SEE ALSO

PPA stable  https://launchpad.net/~customizer-dev-team/+archive/stable

PPA devel  https://launchpad.net/~customizer-dev-team/+archive/devel

You can find more information about Customizer at https://github.com/fluxer/Customizer/wiki