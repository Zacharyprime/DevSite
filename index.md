---
layout: default
---

# KIPR Wombat Images
#### Stable:
<a href="https://www.dropbox.com/s/xmg0iyrar9tj626/Wombat-25.6.img?dl=0"><button>Download 25.6</button></a>

#### In Testing:
<a href="https://www.dropbox.com/s/gdd12xgpzzbuiv9/Wombat-26.1.img?dl=0"><button>Download 26.1</button></a>

#### Experimental:
<a href="https://www.raspberrypi.com/software/operating-systems"><button>Bare pi OS Download</button></a>
<a href="https://gist.github.com/Zacharyprime/c9d7918eccbbffd7f710ea69f464dd4d"><button>Build Instructions</button></a>


# KIPR Wallaby Images
#### Stable:
<a href="https://www.dropbox.com/s/s6cnurla9fl9g29/Wallaby.img?dl=0"><button>Download Wallaby Image (v24)</button></a>


# Install Instructions:
Note: this requires an SD card reader
#### Windows:
1) Download and install Balena Etcher

<a href="https://www.balena.io/etcher/"><button>Balena Etcher Download</button></a>

2) Download a .img file from above.

3) Open balena etcher and follow the prompts to write the image to your SD card. Be sure to select your SD card and not another drive.

4) Unscrew the back panel from the Wombat and replace the SD card.



#### Linux/Mac/Unix:
Note: Balena Etcher will also work with Linux/Mac/Unix.

1) Download an image file from above


2) Find which drive is the SD card (you may need to unplug and plug the SD card to see the difference)
```sh
sudo fdisk -l
```
3) Use dd to write the image to the SD card (make sure the drive letter is correct, sdc is an example)
```sh
sudo dd if="Wombat.img" of="/dev/sdc" bs=4M status=progress
```
Parameters:
<br>

if -> input file

of -> output file
  
bs -> block size *optional
  
status -> Adds a status indicator *optional 
  
4) Unscrew the back panel of the Wombat and replace the SD card with the newly written one.
Note: You can write to the SD card that was already in the Wombat, no need to buy a second SD card.

## Other Resources:
<a href="https://www.kipr.org/"><button> KIPR Website </button></a>
<a href="https://github.com/kipr"><button> KIPR Github Organization </button></a>
<a href="https://github.com/kipr/Simulator"><button> KIPR Robotics Simulator </button></a> <br>
<a href="https://github.com/kipr/KIPR-Development-Toolkit"><button> KIPR Development Toolkit </button></a>
<a href="https://github.com/orgs/kipr/projects/3"><button> Software Version Schedule </button></a>
<a href="https://github.com/kipr/KIPR-Development-Toolkit/blob/master/Docs/WombatDevManual.pdf"><button> Wombat Developer Manual </button></a>

