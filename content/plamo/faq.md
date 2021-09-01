---
title: Frequently Asked Questions
layout: page
menu:
  main:
    parent: project
    weight: 5
    name: FAQ
---

Why is Plasma Mobile not using Mer/Nemomobile?
----------------------------------------------

Plasma Mobile is a software platform for mobile devices. It is not an
operating system in itself, it consists of Qt5, the KDE Frameworks,
Plasma and various software that's part of the application set. Plasma
Mobile can work on top of the Mer distribution, but due to a lack of
time and resources, we're currently focusing on KDE Neon on PinePhone as a base for
testing and development.

Can Android apps work on Plasma Mobile?
---------------------------------------

There are projects like [Anbox](https://anbox.io/) which is Android running inside Linux container, and use Linux kernel to execute applications to achieve near-native performance. This could be leveraged in the future to have Android apps running on top of a GNU/Linux system with the Plasma Mobile platform,
but it's a complicated task, and as of *today*(September 6th, 2020) some distributions already support Anbox and you can run Plasma Mobile on top of those distributions.

Can I run Plasma Mobile on my mobile device?
--------------------------------------------

Currently, Plasma Mobile runs on the following device types:

* **(Recommended) PinePhone:** We offer official images built for the PinePhone
   on top of KDE Neon. You can find more information on the Plasma Mobile [documentation](https://docs.plasma-mobile.org).

*  **x86-based:** If you want to try out Plasma Mobile on an Intel
   tablet, desktop/laptop, or virtual machine, the x86_64 Neon-based
   Plasma Mobile [image](https://www.plasma-mobile.org/get/) is for
   you. Information on how to permanently
   install it can be found on the Plasma Mobile  [documentation](https://docs.plasma-mobile.org).

*  **postmarketOS devices:** postmarketOS is a distribution based on
   Alpine Linux that can be installed on Android smartphones and other
   mobile devices. This project offers support for a fairly wide range
   of devices, and it offers Plasma Mobile as an available interface.
   Please find your device from the [list of supported devices](
   https://wiki.postmarketos.org/wiki/Devices) and see what's working,
   then you can follow the [pmOS installation guide](
   https://wiki.postmarketos.org/wiki/Installation_guide) to
   install it on your device. Your mileage may vary depending on the
   device in use and when you use a device in the testing category it
   is **not** necessarily representative of the current state of Plasma Mobile.

*  **Other:** Unfortunately support for Halium based devices had to
   be dropped recently (see [technical debt](/2020/12/14/plasma-mobile-technical-debt/)).
   This includes the previous reference device Nexus 5x.

I've installed Plasma Mobile, what is the login password?
---------------------------------------------------------

If you've installed Neon onto your PinePhone via the installation script,
the password should be "1234", and you can then change it afterwards by
running "passwd" in Konsole. For Manjaro it is 123456. When changing it,
please keep in mind that you can currently only enter numbers on the
lock screen.

If you're using the x86 image, no password is set by
default, and you'll have to set it by running "passwd" in Konsole before
you can authenticate for anything.

What's the state of the project?
--------------------------------

Plasma Mobile is currently under heavy development and is not intended
to be used as a daily driver. If you are interested in contributing, [join](/findyourway) the game.
