# Resynthesizer without Python (for Gimp version 2)

resynthesizer-scm is a gimp plugin that rewrites the python2 code of bootchk/resynthesizer using script-fu(tinyscheme). Like bootchk/resynthesizer, scm version provides functions such as 'heal selection'. [see wiki/README](https://github.com/itr-tert/gimp-resynthesizer-scm/wiki/README)

## Installation

### Linux
[Download: .deb for amd64-CPU Debian・Ubuntu, GNU/Linux](https://github.com/itr-tert/gimp-resynthesizer-scm-download/raw/main/gimp-resynthesizer-scm.deb)  
```
# install depends
sudo apt install libx11-6 libxau6 libxcomposite1 libatk1.0-0 libbabl-0.1-0 libblkid1 libbrotli1 libbsd0 libc6 libcairo2 libdatrie1 libexiv2-27 libexpat1 libffi8 libfontconfig1 libfreetype6 libfribidi0 libgcc-s1 libgdk-pixbuf-2.0-0 libgegl-0.4-0 libgexiv2-2 libgimp2.0 libglib2.0-0 libgraphite2-3 libgtk2.0-0 libgtk3-nocsd0 libharfbuzz0b libjpeg-turbo8 liblcms2-2 libmd0 libmount1 libpango-1.0-0 libpangocairo-1.0-0 libpangoft2-1.0-0 libpcre2-8-0 libpcre3 libpixman-1-0 libpng16-16 libselinux1 libthai0 libuuid1 libxcb-render0 libxcb-shm0 libxcb1 libxcursor1 libxdamage1 libxdmcp6 libxext6 libxfixes3 libxi6 libxinerama1 libxrandr2 libxrender1 zlib1g
# download
wget https://github.com/itr-tert/gimp-resynthesizer-scm-download/raw/main/gimp-resynthesizer-scm.deb
# install
sudo dpkg -i gimp-resynthesizer-scm.deb
```

### Build from source
```
git clone https://github.com/itr-tert/gimp-resynthesizer-scm.git --depth 1
cd gimp-resynthesizer-scm
./autogen.sh --prefix=/usr/local && make && sudo make install
```

### Windows
[Download: .zip file for Windows](https://github.com/itr-tert/gimp-resynthesizer-scm-download/raw/main/gimp-resynthesizer-scm-win.zip)

[Wiki: Download and Install for Windows: Gimp resynthesizer scm](https://github.com/itr-tert/gimp-resynthesizer-scm/wiki/Download-and-Install:-GIMP-resynthesizer-scm)


## Gimp 3
resynthesizer-scm does not work with Gimp 3.  
(2023-10-01): If you want Resynthesizer for Gimp 3, see the working branch of bootchk/resynthesizer repository.  
[https://github.com/bootchk/resynthesizer/tree/resynthesizer3](https://github.com/bootchk/resynthesizer/tree/resynthesizer3)  

----

# GIMP Resynthesizer Plugin Suite

A set of plugins for the GIMP image editing app.

  Copyright 2000 2008  Paul Francis Harrison  
  Copyright 2002  Laurent Despeyroux  
  Copyright 2002  David Rodríguez García  
  Copyright 2010-2021  Lloyd Konneker 

[![Build Status](https://travis-ci.org/bootchk/resynthesizer.svg?branch=master)](https://travis-ci.org/bootchk/resynthesizer)

A library implementing the "resynthesizer" algorithm for texture transfer among images.

And a suite of plugins, that use the algorithm, for the GIMP image processing application.
The plugins do _not_ come with GIMP, they are "third-party" plugins.

## Resources

[Quick user's guide to the Resynthesizer plugins for GIMP](https://github.com/bootchk/resynthesizer/wiki/Quick-user's-guide-to-the-Resynthesizer-plugins-for-GIMP)

[Developer's guide](https://github.com/bootchk/resynthesizer/wiki/Developer's-guide-to-the-Resynthesizer-code-and-dependencies)

[Resynthesizer and GIMP version 3](https://github.com/bootchk/resynthesizer/wiki/Resynthesizer-and-GIMP-version-3)

More topics are in the [Resynthesizer wiki](https://github.com/bootchk/resynthesizer/wiki)

## Installation(python2 version)

[install flatpaked Resynthesizer for Linux](https://github.com/bootchk/resynthesizer/wiki/Install-Resynthesizer#flatpak)

[install Resynthesizer for Windows](https://github.com/bootchk/resynthesizer/wiki/Install-Resynthesizer#windows)

[install Resynthesizer for MacOS](https://github.com/bootchk/resynthesizer/wiki/Install-Resynthesizer#mac-osx)

[build from source](https://github.com/bootchk/resynthesizer/wiki/Build-Resynthesizer-from-source)

## Acknowledgements

Paul Harrison had the original idea and implementation.  He did the hard work, took the leap of faith and experimented with a new algorithm.  His [website](http://www.logarithmic.net/pfh/) has many examples of using the Resynthesizer, links to an explanation of the algorithm, and other cool ideas.

I fixed a few bugs (due to changes in GIMP), rewrote the Scheme plugins into Python, wrote a few plugins, made it better deal with alpha (transparency), threaded it, and made it into a reentrant library in C.

Rob Antonishen contributed the basis for one plugin.  Several people have helped with the build process and with translations.

## License

GNU General Public License v3.0

