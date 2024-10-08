## How to Download Affinity Wine

Head to the github and Download the newest release [Here](https://github.com/Twig6943/ElementalWarrior-wine-binaries/releases) 

## Downloading Affinity 

[Affinity Designer](https://store.serif.com/update/windows/designer/2/)

[Affinity Photo](https://store.serif.com/update/windows/photo/2/)

[Affinity Publisher](https://store.serif.com/update/windows/publisher/2/)

From the Drop down Choose the exe

## Required dependencies

## Ubuntu/Debian

```
sudo apt install gcc-mingw-w64 gcc-multilib libasound2-dev libcups2-dev libdbus-1-dev libfontconfig-dev libfreetype-dev libgl-dev libgnutls28-dev libgphoto2-dev libgstreamer-plugins-base1.0-dev libgstreamer1.0-dev libosmesa6-dev libpcap-dev libpulse-dev libsane-dev libsdl2-dev libudev-dev libunwind-dev libusb-1.0-0-dev libvulkan-dev libx11-dev libxcomposite-dev libxcursor-dev libxext-dev libxfixes-dev libxi-dev libxrandr-dev libxrender-dev ocl-icd-opencl-dev samba-dev git p7zip
```
## Arch Linux/CachyOS

```
sudo pacman -Syu alsa-lib alsa-plugins cups desktop-file-utils dosbox ffmpeg fontconfig freetype2 gcc-libs gettext giflib gnutls gst-plugins-base-libs gtk3 libgphoto2 libpcap libpulse libva libxcomposite libxcursor libxi libxinerama libxrandr mingw-w64-gcc opencl-headers opencl-icd-loader samba sane sdl2 v4l-utils vulkan-icd-loader wine-mono winetricks git p7zip
```

## Fedora/Nobara
```
sudo dnf install alsa-lib-devel cups-devel dbus-libs fontconfig-devel freetype-devel glibc-devel.i686 gnutls-devel gstreamer1-devel gstreamer1-plugins-base-devel libgphoto2-devel libunwind-devel libusbx-devel libX11-devel libXcomposite-devel libXcursor-devel libXext-devel libXfixes-devel libXi-devel libXrandr-devel libXrender-devel mesa-libGL-devel mesa-libOSMesa-devel mingw32-gcc mingw64-gcc ocl-icd-devel samba-devel sane-backends-devel SDL2-devel vulkan-headers vulkan-loader vulkan-loader-devel winetricks git p7zip p7zip-plugins
```
## Opensuse/Others
```
sudo zypper install alsa-lib-devel cups-devel dbus-1-devel flex fontconfig-devel freetype-devel glibc-devel-32bit gnutls-devel gstreamer-devel gstreamer-plugins-base-devel libgphoto2-devel libOSMesa-devel libunwind-devel libusb-1_0-devel libusb-compat-devel libX11-devel libXcomposite-devel libXcursor-devel libXext-devel libXfixes-devel libXi-devel libXrandr-devel libXrender-devel Mesa-libGL-devel mingw32-cross-gcc mingw32-cross-wine mingw32-gcc mingw64-cross-gcc mingw64-cross-wine mingw64-gcc ocl-icd-devel samba-devel sane-backends-devel SDL2-devel vulkan-devel vulkan-headers vulkan-tools
```

## Acquiring Pre-built Wine binaries

As affinity is a bit of a complex program, it requires that you run it with a fork of WINE tailor-made for it.

Here are the currently available options:

[ElementalWarriorWine](https://gitlab.winehq.org/ElementalWarrior/wine)

(This fork's repo doesnt contain binaries and as such, pre-built binaries can be found [here](https://github.com/Twig6943/ElementalWarrior-Wine-binaries/releases/tag/binary-release-1.0)


## Installing Heroic Game Launcher flathub

```
flatpak install flathub com.heroicgameslauncher.hgl
```
## Fedora 

```
sudo dnf in lutris
```
## Arch Linux

```
sudo pacman -S lutris
```
## Ubuntu/Debian

```
sudo apt install lutris
```
## Installing Affinity Linux's Prebuilt Wine

Extract the Elemental Warrior's Pre-built wine binaries to Heroic's tools directory

```
/home/USER/.config/heroic/tools/wine
```

## Flatpak's Wine location

```
/home/USER/.var/app/com.heroicgameslauncher.hgl/config/heroic/tools/wine
```
## Settings Up Heroic For Affinity

Open up Heroic and then click on 

```
add game
``` 

Or for Lutris the 

```
+ Button
``` 
and at the bottom 

```
Add Locally Install Game
```

Name it According to the Affinity app you are using

```
Affinity Photo
```

```
Affinity Designer
```
```
Affinity Publisher
```
## Setting the Wine Version

Set the wine version to ElementalWarriorWine

## Selecting the Programs .exe According to what you Want to Install

Select the setup .exe you've downloaded from affinity's website as the executable

Click 
```
Finish
```
## Initialize the prefix

In order to initialize the prefix run the setup file from heroic. (It'll probably crash wait for it to crash if it somehow opens up close it yourself)

## Setting Up Affinity Wine Settings and Winetricks

* Right click on affinity on heroic and open up its settings

* Scroll down until you see winetricks & then click on it

* Search & install these dependencies;
```
dotnet48
```
```
corefonts
``````
```
vcrun2015
```

(Wait while its installing the dependencies. Its %90 not stuck but rather taking its time!!!)

Click on 
```
OPEN WINETRICKS GUI
```
Select 
```
Select the default wineprefix
```
Select 
```
Change settings
```
Toggle 
```
win11
```
Toggle 

```
renderer=vulkan
```
and click OK

Keep pressing "Cancel" till the winetricks window closes

Close heroic games launcher's settings window

## Placing WinMetadata

Unzip [WinMetadata.zip](https://archive.org/download/win-metadata/WinMetadata.zip)

to $HOME/.Affinitywine/drive_c/windows/system32

## Running Affinity Setup and Installing Photo/Designer/Publisher

Press launch and the setup should work

Once its done installing right click to affinity on heroic and go to the details tab

Click on the 3 dots (located on the right top corner)

Edit 

```
App/Game
```

Next Change the executable to 

```
drive_c/Program Files/Affinity/Photo 2/Photo.exe
```
```
drive_c/Program Files/Affinity/Designer 2/Designer.exe
```

```
drive_c/Program Files/Affinity/Publisher 2/Publisher.exe
```

Click finish & launch it.

## Troubleshooting

(Change the settings in the wine tab if it doesn't work or if you have gpu glitches (it should work fine tho) )

# Optional wine dark theme 🍷
1. Download this file https://raw.githubusercontent.com/Twig6943/AffinityOnLinux/main/wine-dark-theme.reg

2. Right click on your affinity app and go to `Settings`

3. Click `winetricks`

4. Click `OPEN WINETRICKS GUI`

5. Select the default prefix

6. Run `regedit`

7. Go to `Registry`, then click `Import registry file`

8. Pick the file you've downloaded earlier (wine-dark-theme.reg)

9. Now you've got a dark theme!
