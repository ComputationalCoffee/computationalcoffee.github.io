---
title: "Must Have Programs for Linux"
date: 2021-12-07T17:39:23+01:00
draft: false
---

## Pre-preamble

This is a *series* of articles. I will update this article with the link to the **second part** when I will release it.

In *this part* I will cover the following:

1. **Office Suites**
2. **PDF viewers**
3. **PDF editors**
4. **Media/Content Viewers**

*Stay tuned for part 2!*

## Preamble

With the new _"LTT Challenge"_ videos (you can watch the first one [here](https://www.youtube.com/watch?v=0506yDSgU7M)), Linux-based distributions are now seeing a new
media coverage as never before, and, of course, I'm feeling happy about this.
On the other hand, **new Linux users** means more inexperienced people that might be discouraged by *"something different from Windows/MacOS"*. So, here's my **two tips** for
new Linux users that are coming from proprietary operative systems:

1. **Don't be scared to try and fail**: Linux distributions are diverse, but you can do **absolutely everything** on all of them, with or without a little tinkering!
2. **Start unbiased**: be like when you where a kid approaching Windows/MacOS, don't search functions and tools you can already find on common operative systems,
   things will be partially different, if not different at all! Internet is your friend, but patience will be your best friend!

That taken care of, let's kick things in with my list of **Must have programs for Linux-based distributions!**

**NOTE**: *I will prefer Free and Open Source alternatives to common programs, because this is how we do things on Linux!*

## Office-like suites

### Libreoffice

![The Libreoffice logo](http://www.ocsmag.com/wp-content/uploads/2017/06/libreoffice-logo.png)

A full-featured Office suite for casuals and professionals: documents, drawings, presentations, math and many many more.
It is fully compatible with OpenOffice standards and Microsoft document formats standards.
Looks modern, feels powerful. It's divided in its **different parts** that can be expanded with useful extensions:

* **Libreoffice base**: a cool *dashboard* to see recent documents, and open each one with the appropriate application
* **Libreoffice writer**: the Word processor
* **Libreoffice calc**: the Excel of the bunch
* **Libreoffice impress**: the presentation program
* **Libreoffice draw**: a very cool and useful draw utility
* **Libreoffice math**: a fantastic math tool that supports MathML and Latex

#### How to install Libreoffice

* On **Ubuntu/Debian-based** distributions: you can use your *software center/app store* to search for **Libreoffice** and install it quickly!
  if you need more help, [here](https://linuxconfig.org/how-to-install-libreoffice-ubuntu-20-04-focal-fossa-desktop)'s a guide for you to read.
* On **Arch-based** distributions: you can use pamac/octopi (the equivalent of the Software Center, but for Arch Linux) to search for Libreoffice and 
  the software will do the rest! Alternatively, you can do it in the command line --> `sudo pacman -S libreoffice-fresh`.

### Onlyoffice

![Onlyoffice](https://www.itechcode.com/wp-content/uploads/2021/03/ONLYOFFICE-featured-image.jpg)

A Microsoft-word/excel/powerpoint clone made to be as close as it gets with Windows compatibilty. It was made to be run online, but you can
use it everywhere. It is way simpler than Libreoffice and more easy to use for sure, but it has less features.

#### How to install Onlyoffice

* On **Ubuntu/Debian-based** distributions: same as before (it has both snap and flatpak versions).
* On **Arch-based** distributions: same as before. On the terminal you can install it using an **AUR-helper** (like *paru* or *yay*) with `paru -S onlyoffice-bin`

## PDF readers

### Okular

![Okular view](https://www.tecmint.com/wp-content/uploads/2016/03/Okular-Linux-PDF-Reader.png)

The most popular document viewer you can find on Linux: **pdfs, epubs, xps(s)** and many more! It is the default PDF reader on **KDE** Desktop environment,
but I personally suggest to install it everywhere. It can not only read PDFs but also **modify** and **sign** them!

#### How to install Okular

* On **Ubuntu/Debian-based** distributions: same as before (it has both snap and flatpak versions).
* On **Arch-based** distributions: same as before. On the terminal you can install it with `pacman -S okular`.

### Evince

![Evince view](https://wiki.gnome.org/Apps/Evince?action=AttachFile&do=get&target=evince-1.png)

The default Gnome PDF reader: it is basic, fast and looks really good with a (also good) GTK theme!
You can do basic things like **searching**, **indexing**, **viewing encrypted documents** and more.
I personally recommend this piece of software if you want a basic PDF reader for everyday use.

#### How to install Evince

* On **Ubuntu/Debian-based** distributions: same as before (it has both snap and flatpak versions).
* On **Arch-based** distributions: same as before. On the terminal you can install it with `pacman -S evince`.

### Zathura (only for experienced users!)

![Zathura view](https://i.imgur.com/FbxIk6i.png)

**KISS: keep it simple stupid**. A Vim-like experience, but for PDFs. If you feel like it could not get more minimalistic, this tool will surprise you.
It's a **mouse-free** PDF(and more!) navigation experience with **automatic document reloading**, *easily* customizable and **VERY FAST**. Like, *faf*.

#### How to install Zathura

* On **Ubuntu/Debian-based** distributions: same as before.
* On **Arch-based** distributions: same as before. On the terminal you can install it with `pacman -S zathura`.

## PDF editors

While you can still use **Libreoffice Draw** and **Okular** as basic PDF editors, if you are searching for more (merging, compressing, converting) I got you covered:

### PDFsam (basic)

![PDFsam view](https://i2.wp.com/itsfoss.com/wp-content/uploads/2020/06/pdfsam-basic.png)

The **basic** version of PDFsam, lets you **split, merge, rotate, extract pages** from a PDF.
If you want to support the developer, you can upgrade to the non-FOSS PDFsam paid edition, but I would not recommend that.

*The installation is the same as before.*

### ilovepdf.com (non-FOSS)

![ilovepdf](https://i.imgur.com/n1nSSVn.png)

A good online tool for modifying PDFs and converting them to other formats. There is no app for Linux, but the site is still fine.
It is non-FOSS, website only, so **I would not upload private content there**, but still, have a look at it.

### Sejda PDF Desktop (non-FOSS)

![SejdaPDF view](https://i.imgur.com/ZouXL3j.png)

The ultimate tool to manage PDFs. You can do everything: **Compressing, merging, organizing, splitting, converting, protecting and watermarking** them!
The drawbacks?

* It's non-FOSS, so the thing I said before applies here
* The free version is limited to 3 tasks per day, docs up to 50Mb and 200 pages and more... (it's VERY limiting)
* The paid version costs **a lot**: 59 euro(s) a year, with no option for a perpetual license

### The FOSS alternatives?

These are **the best FOSS PDF editors** that you can find for Linux, ordered by personal preference:

1. Libreoffice Draw
2. Inkscape
3. Scribus
4. Okular
5. Qoppa PDF Studio

Go and try them now online!


## Media Viewer (Video/Audio)

### VLC

![VLC logo](http://productkeyz.com/wp-content/uploads/2019/11/vlc-new-version.jpg)

Everybody knows what VLC is. It's the **best media viewer** you can find on every operative system. It's stable, it has lots of features
and it is easy to use. It has a good and usable graphical user interface, and can even [play videos from YouTube!](https://www.makeuseof.com/tag/7-top-secret-features-free-vlc-media-player-si/)

Here's a list of **what VLC can do**:

* Play videos (every format!)
* Play audio/music (every format!)
* Play files from internet, videos from internet, music from internet
* Have a fast hardware decoding (built-in)
* And many more!

### MPV

![MPV view](https://4.bp.blogspot.com/-85dPrhkj2oo/V8g3z4gHWuI/AAAAAAAALbU/jy_HgnZIsF8VmhDGDRNa9PJf9tdpNpw-gCLcB/s1600/mpv.png)

The fastest media player software you can find on Linux. It is based on MPlayer, mplayer2 and FFMpeg.

Here's a list of **what MPV can do**:

* All the things mentioned above, plus...
* Scripting and plugins
* Very active development, frequent security fixes and updates
* The best GPU video decoding you can find, even better than VLC! It is perfect to play your favorite 4K content.

## Conclusion

**For now, that's all!**
Thanks for reading and I will see you in the second part of the article.

*Author: Federico Torrielli*
