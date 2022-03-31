# KIPR Wombat Images
## Stable:
<button href="https://www.dropbox.com/s/xmg0iyrar9tj626/Wombat-25.6.img?dl=0">Download 25.6</button>

## In Testing
<button href="https://www.dropbox.com/s/gdd12xgpzzbuiv9/Wombat-26.1.img?dl=0">Download 26.1</button>

## Experimental:
<button href="https://www.raspberrypi.com/software/operating-systems">Bare pi OS Download</button>
<button href="https://gist.github.com/Zacharyprime/c9d7918eccbbffd7f710ea69f464dd4d">Build Instructions</button>

<hr>

# Install Instructions:
Note: this requires an SD card reader
#### Windows:
1. Download and install Balena Etcher

<button href="https://www.balena.io/etcher/">Balena Etcher Download</button>
1. Download a .img file from above.
2. Open balena etcher and follow the prompts to write the image to your SD card. Be sure to select your SD card and not another drive.
3. Unscrew the back panel from the Wombat and replace the SD card.

#### Linux/Mac/Unix:
Note: Balena Etcher will also work with Linux/Mac/Unix.
1. Download an image file from above
2. Find which drive is the SD card (you may need to unplug and plug the SD card to see the difference)
```sh
sudo fdisk -l
```
3. Use dd to write the image to the SD card
```sh
sudo dd if="Wombat.img" of="/dev/sda" bs=4M status=progress
```
Parameters:
if=<input file>

of=<output file>
  
bs=<block size> *optional
  
staus=progress *optional //Adds a status indicator
  
4. Unscrew the back panel of the Wombat and replace the SD card with the newly written one.
Note: You can write to the SD card that was already in the Wombat, no need to buy a second SD card.
