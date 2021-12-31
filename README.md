# Anbernic RG552 - Pegasus metadata pack

Disclaimer: I'm not responsible if you damage your RG552 in any way, this a guide that exists to make it as easy as possible to use your RG552 with the Pegasus Frontend, in my opinion one of the best Frontend Emulators out there but you always need to be careful.

The bad thing about Pegasus is that you need to make a lot of configuration, I'm trying to make this pack as plug & play as possible so you don't have to tinker with config files.

This pack contains metadata configuration for the following systems and emulators.

| System                    | Emulator                             |
| ------------------------- | ------------------------------------ |
| Atari 2600                | Retroarch 1.9 stella core            |
| Doom                      | Retroarch 1.9 PrBoom core            |
| GameBoy                   | Retroarch 1.9 Gambatte core          |
| GameBoy Color             | Retroarch 1.9 Gambatte core          |
| GameBoy Advance           | Retroarch 1.5 mGBA core              |
| GameGear                  | Retroarch 1.9 Genesis Plus GX core   |
| Dreamcast                 | Reddream                             |
| Dos                       | Retroarch 1.9 DOSBox core            |
| Final Burn Alpha          | Retroarch 1.9 fba 2020 core          |
| Final Burn Neo            | Retroarch 1.9 fbn core               |
| Mame 2010 ( 0.139 )       | Retroarch 1.9 Mame 2010 core         |
| Master System             | Retroarch 1.9 Genesis Plus GX core   |
| Neo Geo                   | Retroarch 1.9 fba 2020 Neo Geo core  |
| Neo Geo CD                | Retroarch 1.9 fbn core               |
| Neo Geo Pocket & Color    | Retroarch 1.9 Beetle NeoPop          |
| Nintendo DS               | Drastic                              |
| Nintendo NES              | Retroarch 1.9 Nestopia core          |
| Nintendo 64               | Mupen64plus FZ                       |
| PC engine                 | Retroarch 1.9 mednafen pce fast core |
| Playstation               | Retroarch 1.9 PCSX Rearmed core      |
| Pokemon Mini              | Retroarch 1.9 PokeMini core          |
| PSP                       | PPSSPP                               |
| ScummVM                   | Retroarch 1.9 scummvm core           |
| Sega 32X                  | Retroarch 1.9 Genesis Plus GX core   |
| Sega CD                   | Retroarch 1.9 Genesis Plus GX core   |
| Sega Game Gear            | Retroarch 1.9 Genesis Plus GX core   |
| Sega Genesis / Mega Drive | Retroarch 1.9 Genesis Plus GX core   |
| Super Nintendo            | Retroarch 1.9 Snes9x Current core    |
| Wonderswan & Color        | Retroarch 1.9 Beetle Cygne core      |

**Pegasus & gameOS theme for Pegasus disclaimer**

I'm providing both Pegasus installer and gameOS theme so it's easier for you to setup everything.

You can check Pegasus website in [here] https://pegasus-frontend.org/#downloads

You can check gameOS website in [here] https://github.com/PlayingKarrde/gameOS/

# Guide for newbies

## TLDR version.

- Download the contents on the Main Branch and copy everything to your SD CARD.
- Install Pegasus from the apk in the SD card
- Copy the contents of \-internal to your Android Internal Storage so both Pegasus and Retroarch are autoconfigured
- Scrap your roms
- Enjoy

## Step by step version.

### 1 Enable APK installation

First you'll need to enable installing APK packages, which can be done in your RG552 on Settings → Security → Unknown Sources, turned on.

### 2 Download my latest [Pegasus Frontend metadata Pack](https://github.com/dragoonDorise/pegasus-rg552-metadata/archive/main.zip)

Unzip it in your computer. This folder should look like this:

```
  -internal
  atari2600
  doom
  dos
  dreamcast
  fba
  fbn
  gameboy
  gamegear
  gba
  gbc
  genesis
  mame
  mastersystem
  n64
  nds
  neogeo
  neogeocd
  neogeopocket
  nes
  pcengine
  psx
  pokemini
  psp
  scumm
  sega32x
  segacd
  snes
  wonderswan
  pegasus-fe_alpha15-85-gfff1a5b2_android.apk
```

Insert your SD Card in your computer and copy the folders there.

If your RG552 came with roms just merge the folders in the 64GB sd card, that way you can keep your current roms and just add the new configuration files.

### 3 Transfering Games

If your RG552 came with games you can skip this step and go right to the next.

Now that you have the Metadata pack in your RG552 lets copy some games, just drag and drop the rom files in every system folder ( we recommend using no intro roms found on archive.org )

Example: I want to transfer **Legend of Zelda, The - A Link to the Past (USA).zip** for Super Nes, just drag and drop the file to sdcard/snes/, repeat the process with the rest of the systems you want to play.

When you are good to go, insert the SD Card on your RG552 and go to the next step.

### 4 Configuring Pegasus & Retroarch

Use the RG552 file browser app and navigate to your SD card and open **pegasus-fe_alpha15-85-gfff1a5b2_android.apk** file , install Pegasus but **don't open it yet**

Copy the contents of your **-internal** folder in the SD ard to your Android internal storage, on the root folder where you should have a RetroArch and pegasus-frontend folders already, make sure you merge your folders so we add these files to the ones that are already on your RG552.

### 5 Making it pretty

### Option 1 - Pre Scraped Assets

I've added some pre scrapped assets, if your romset comes from a no intro set then you are good to go, no need for scrapping ;)

You can start playing your games!

### Option 2 - Scraping your own assets

If the built in assets doesn't meet your needs, you need to scrap your own, for that we are going to be using [Skraper](http://skraper.net), for that you need to register yourself in [Screen Scrapper](https://www.screenscraper.fr/membreinscription.php)

**Note to Mac users**

Skraper is not available for Mac as of yet, I promise I will try to update this guide ASAP with alternatives for you guys.

I assume you have installed the application with no problem, after several minutes a wizard will appear:

In there complete your screen scrapper login data, click in VALIDATE and click NEXT.

![Screenshot](https://raw.githubusercontent.com/dragoonDorise/pegasus-rp2-metadata/master/guide/13.png)

In the next screen choose "Generic Emulation" and click NEXT

Insert your RG522 SD card onto your computer, now chose the path to your sd card with all the systems in it.

You should see a screen like this:

![Screenshot](https://raw.githubusercontent.com/dragoonDorise/pegasus-rp2-metadata/master/guide/14.png)

Click NEXT until you see this screen:

![Screenshot](https://raw.githubusercontent.com/dragoonDorise/pegasus-rp2-metadata/master/guide/15.png)

Go to the Media tab, we're going to tell Skrapper what images we need. Hit the - button until there is nothing selected

![Screenshot](https://raw.githubusercontent.com/dragoonDorise/pegasus-rp2-metadata/master/guide/16.png)

Click on the + button, then in media type click the left arrow until we get "Image - Screenshot"

Then mark "Resize width", put _960px_ in the input box an also check "mantain aspect ratio"

![Screenshot](https://raw.githubusercontent.com/dragoonDorise/pegasus-rp2-metadata/master/guide/17.png)

Click once more in the + button and repeat but now we need media type : "Image - Logo" depending of your computer language this could be called "Image - Wheel", then again mark "Resize width", put _960px_ in the input box an also check "mantain aspect ratio". Do the same with "Image - Box 2D"

![Screenshot](https://raw.githubusercontent.com/dragoonDorise/pegasus-rp2-metadata/master/guide/18.png)

Hit the play button and wait, depending of the number of roms this could take from minutes from hours.

**If you are using a MAME full romset pack, I recommend using this [trick](https://www.youtube.com/watch?v=GZfoOTckURA) to thin the ROMs you will transfer**

When it's finished you will have a media folder inside of every of your rom systems. Just put your SD card back and you are good to go.

Example: The path the media folder in your RP2 for Super Nintendo should be:

roms/snes/media
