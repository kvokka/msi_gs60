## Ubuntu 18.04 config extras for MSI GS60 6QE

#### Desclamer

This is not universal solution! This is config for my laptop, which
I found useful to share.

#### Laptop specs: 

MSI GS60 6QE ghost pro

6700HQ/16Gb/256Gb Samsung951 + 1Tb 7200rpm/970M 6Gb/killer 1535 wifi+bt/4k

#### Get +20% of speed back with disabling security patch

https://askubuntu.com/questions/991874/how-to-disable-page-table-isolation-to-regain-performance-lost-due-to-intel-cpu

### Features:

* `fan/` Silent work (idle power consumtion < 10W) with wifi & bt on.  
* `disable_nvidia/` Nvidia card disabled!
* `wifi/` last drivers pack. Required for Debian 9.5, not mandatory for Ubuntu.
* `init_install` my tools bundle.

Hints:

* The minimal fan speed is 3000 rpm and it is impossible to change. So you will hear fans 
from time to time.
