---
title: Compiling Okular from source on Linux
menu:
  main:
   parent: about
   weight: 2
   name: Build It
---

<span style="background-color:#e8f4fa">If you are looking for the pre-compiled packages, visit the [download page](/download/). You can check the packaging status [here](https://repology.org/project/okular/versions)</span>

If you want to compile Okular, you need to have a compilation environment set up, which, in general, should be provided by your distribution. In case you want to compile the development version of Okular, please refer to Build from source at KDE's Community Wiki.

You can download and compile Okular this way:

1. `git clone https://invent.kde.org/graphics/okular.git`
2. `cd okular`
3. `mkdir build`
4. `cd build`
5. `cmake -DCMAKE_INSTALL_PREFIX=/path/to/your/install/dir ..`
6. `make`
7. `make install`

If you install Okular in a different path than your system install directory it is possible that you need to run `source build/prefix.sh; okular` so that the correct Okular instance and libraries are picked up.

## Optional packages

There are some optional packages you could install in order to have some more functionalities in Okular. Some might already be packaged for your distro, but other may not. If you want to avoid any issues, stick to the packages supported by your distribution

* Poppler (PDF backend): To compile the PDF backend, you need [the Poppler library](http://poppler.freedesktop.org), for which the minimum version required is 0.24
* Libspectre: In order to compile and use this PostScipt (PS) backend, you need libspectre >= 0.2. If your distro does not package it, or the packaged version is not enough, you can download it [here](http://libspectre.freedesktop.org)
* DjVuLibre: To compile the DjVu backend, you need DjVuLibre >= 3.5.17. As with Libspectre, you can get it from your distro or [here](http://djvulibre.djvuzone.org).
* libTIFF: This is required for TIFF/fax support. Currently there is no minimum required version, so any quite recent version of the library available from your distro should work. In case of trouble, do not hesitate to contact the Okular developers.
* libCHM: This is needed to compile the CHM backend. As with libTIFF, there is no minimum version requirement
* Libepub: If you need EPub support, you can install this library from your distro or from [sourceforge](http://sourceforge.net/projects/ebook-tools).

