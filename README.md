3DS Portlibs
============

Here is a Makefile for building various portlibs for 3DS. 
It is basically libs compiled with the compiler equivalent to the processor
of the 3DS.

The processor of the 3DS use the armv6k instructions.

You need to first build zlib and install it. Then you can 
build the other portlibs.

    $ make zlib
    $ make install-zlib
    $ make <targets>
    $ make install

This will install the portlibs to `$DEVKITPRO/portlibs/armv6k`. If this is a
privileged location, you will need to `sudo make install-zlib` and `sudo make
install` in order for the portlibs to be installed.

Prerequisite
------------

You need to have installed the following packages :
- autoconf
- cmake
- make
- pkg-config
- libtool

On Debian system, use this set of command to install it

```
sudo apt-get install autoconf cmake make pkg-config libtool
```

You need also to have devkitPro and devkitARM installed on your machine.
For more information, see : https://devkitpro.org/wiki/Getting_Started/devkitARM

List of portlibs supported
--------------------------

* bzip2
* expat
* freetype (requires zlib)
* giflib
* jansson
* libarchive
* libconfig
* libexif
* libfaad2
* libfmt
* libjpeg-turbo
* libmad
* libogg
* libpng (requires zlib)
* libvorbis
* libxml2
* libxmp-lite
* nettle
* minixml
* mbedtls (requires zlib) (without net component)
* sqlite
* tinyxml2
* tremor (requires libogg)
* wslay
* xz
* zlib


Download links:

* [bzip2-1.0.6] (http://www.bzip.org/1.0.6/bzip2-1.0.6.tar.gz)
* [expat-2.1.0] (http://sourceforge.net/projects/expat/files/expat/2.1.0/expat-2.1.0.tar.gz)
* [freetype-2.6.2.tar.bz2] (http://download.savannah.gnu.org/releases/freetype/freetype-2.6.2.tar.bz2)
* [giflib-5.1.1] (http://sourceforge.net/projects/giflib/files/giflib-5.1.1.tar.bz2)
* [jansson-v2.7.tar.gz] (https://github.com/akheron/jansson/archive/v2.7.tar.gz)
* [libarchive-3.1.2] (https://github.com/libarchive/libarchive/archive/v3.1.2.tar.gz)
* [libconfig-1.5] (http://www.hyperrealm.com/libconfig/libconfig-1.5.tar.gz)
* [libexif-0.6.21.tar.bz2] (http://sourceforge.net/projects/libexif/files/libexif/0.6.21/libexif-0.6.21.tar.bz2/download)
* [libfaad2-2.7] (http://downloads.sourceforge.net/faac/faad2-2.7.tar.gz)
* [libfmt-3.0.1] (https://github.com/fmtlib/fmt/archive/3.0.1.tar.gz)
* [libjpeg-turbo-1.4.2.tar.gz] (http://sourceforge.net/projects/libjpeg-turbo/files/1.4.2/libjpeg-turbo-1.4.2.tar.gz/download)
* [libmad-0.15.1b] (http://sourceforge.net/projects/mad/files/libmad/0.15.1b/libmad-0.15.1b.tar.gz)
* [libogg-1.3.2] (http://downloads.xiph.org/releases/ogg/libogg-1.3.2.tar.xz)
* [libpng-1.6.21.tar.xz] (http://prdownloads.sourceforge.net/libpng/libpng-1.6.21.tar.xz?download)
* [libvorbis-1.3.5] (http://downloads.xiph.org/releases/vorbis/libvorbis-1.3.5.tar.xz)
* [libxml2-2.9.3] (http://xmlsoft.org/sources/libxml2-2.9.3.tar.gz)
* [libxmp-lite-4.3.10.tar.gz](http://sourceforge.net/projects/xmp/files/libxmp/4.3.10/libxmp-lite-4.3.10.tar.gz/download)
* [nettle-3.3] (https://ftp.gnu.org/gnu/nettle/nettle-3.3.tar.gz)
* [minixml-2.9] (https://github.com/michaelrsweet/mxml/releases/download/release-2.9/mxml-2.9.tar.gz)
* [mbedtls-2.2.1] (https://tls.mbed.org/download/mbedtls-2.2.1-gpl.tgz)
* [sqlite-autoconf-3100200.tar.gz] (https://www.sqlite.org/2016/sqlite-autoconf-3100200.tar.gz)
* [tinyxml2-3.0.0.tar.gz] (https://github.com/leethomason/tinyxml2/archive/3.0.0.tar.gz)
* [tremor-2a1a8f6] (https://git.xiph.org/?p=tremor.git;a=snapshot;h=2a1a8f621e500fdf0749f115e2206f82919560a3;sf=tgz)
* [wslay-1.0.0] (https://github.com/tatsuhiro-t/wslay/archive/release-1.0.0.tar.gz)
* [xz-5.2.2] (http://tukaani.org/xz/xz-5.2.2.tar.xz)
* [zlib-1.2.8.tar.gz] (http://prdownloads.sourceforge.net/libpng/zlib-1.2.8.tar.gz?download)

Thanks
============

Thanks to :
- The original 3DS portlibs git and all the developers behind it
- Cruel, with his fork of portlibs containing various libs which can be useful
