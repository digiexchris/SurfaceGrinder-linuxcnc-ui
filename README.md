
# SG CNC for linuxcnc

#### Surface Grinder CNC
Semi-automatic surface grinder interface similar to hydraulic grinders, but with extra functionality

The left/right traverse allows for all 3 dimensions, so it's possible to traverse at a 3d angle instead of just horizontally!

Infeed also takes a 3d vector, so you can do in/out stepover like usual, but can also plunge or do an angle instead.

TODO:

Make a calculator that sets the stepover vector according to angles

A fork of https://github.com/turboss/sg_cnc.git


## Quick install

install linuxcnc 2.9pre using the debian 11

http://www.linuxcnc.org/

install qtpyvcp from packages (pypi's version is too old for python3)

qtpyvcp packages can be found here 
https://repository.qtpyvcp.com/apt/pool/main/stable/


https://www.qtpyvcp.com/install/prerequisites.html

### Dependencies

```
$ sudo apt install python3-pyqt5 python3-pyqt5.qtquick python3-dbus.mainloop.pyqt5 python3-pyqt5.qtopengl python3-pyqt5.qsci python3-pyqt5.qtmultimedia qml-module-qtquick-controls gstreamer1.0-plugins-bad libqt5multimedia5-plugins pyqt5-dev-tools python3-dev python3-setuptools python3-pip git
```

### installation

```
$ git clone https://github.com/digiexchris/SurfaceGrinder-linuxcnc-ui
$ cd semiauto_sg
$ pip install -e .
```

## Customize

install qtpyvcp
https://www.qtpyvcp.com/install/apt_install.html
https://repository.qtpyvcp.com/apt/pool/main/stable/

```
$ cd semiauto_sg/ui
$ editvcp config.yml
```

## Resources

* [Development](https://github.com/digiexchris/SurfaceGrinder-linuxcnc-ui)
* [Documentation](https://qtpyvcp.com)


## Dependancies

* [LinuxCNC](https://linuxcnc.org) 2.9pre
* Python 3.9
* PyQt5 or PySide2
* [QtPyVCP](https://qtpyvcp.com/)

semiauto_sg is developed and tested using the LinuxCNC Debian 12, It should run on any system that can have PyQt5 installed, but Debian 12 is the only OS
that is officially supported.


## DISCLAIMER

THE AUTHORS OF THIS SOFTWARE ACCEPT ABSOLUTELY NO LIABILITY FOR
ANY HARM OR LOSS RESULTING FROM ITS USE.  IT IS _EXTREMELY_ UNWISE
TO RELY ON SOFTWARE ALONE FOR SAFETY.  Any machinery capable of
harming persons must have provisions for completely removing power
from all motors, etc, before persons enter any danger area.  All
machinery must be designed to comply with local and national safety
codes, and the authors of this software can not, and do not, take
any responsibility for such compliance.


Copyright (c) 2020 All rights reserved.
