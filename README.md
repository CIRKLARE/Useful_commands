# Useful commands
Useful commands for Linux





sudo apt-get install icoutils

wrestool -x -t 14 source.exe > output.ico




#!/bin/bash
airmon-ng stop wlan0
systemctl restart NetworkManager



#!/bin/bash
airmon-ng check kill
airmon-ng start wlan0


find . type f -ls | grep "NOV"

find . type f -ls | grep "png"



To convert text file to pdf use

Pandoc file.txt -o output.pdf

Or

sudo apt install enscript

enscript -p output.ps file.txt

(ps is post script format)

Then use ps2pdf

ps2pdf output.ps final.pdf

/////////
To reverse it use 
$ pdftotext file.pdf output.txt
////////

To convert image to pdf

img2pdf file.png -o output.pdf

////////
Reverse it

pdftoppm file.pdf output.png -png
//////





@@@@@@@@@@@@@@@@@@@
sudo apt install kali-community-wallpapers
sudo apt install kali-legacy-wallpapers
sudo apt install kali-wallpapers-2019.4
sudo apt install kali-wallpapers-2020.4
sudo apt install kali-wallpapers-2021.4
sudo apt install kali-wallpapers-2022
sudo apt install kali-wallpapers-all


sudo apt install kali-community-wallpapers && sudo apt install kali-legacy-wallpapers && sudo apt install kali-wallpapers-2019.4 && sudo apt install kali-wallpapers-2020.4 && sudo apt install kali-wallpapers-2021.4 && sudo apt install kali-wallpapers-2022 && sudo apt install kali-wallpapers-all
@@@@@@@@@@@@@@@@@@@




1-video to frames
ffmpeg -i input.mp4 -r 2 frames/out-%03d.jpg


2-frames to video
ffmpeg -framerate 30 -pattern_type glob -i "frames/*.jpg" -c:v libx264 -pix_fmt yuv420p out.mp4
ffmpeg -framerate 30 -pattern_type glob -i "*.jpg" -c:v libx264 -pix_fmt yuv420p out.mp4


3-compress video
ffmpeg -i input.mp4 -vcodec libx264 -crf 24 output.mp4

4-mp4 to mp3
ffmpeg -i "input.mp4" -c:a libmp3lame "output.mp3"

####

mkdir outputs
for f in *.mp4; do ffmpeg -i "$f" -c:a libmp3lame "outputs/${f%.mp4}.mp3"; done

merge PDFs
pdfunite 1.pdf 2.pdf out.pdf



sudo apt install boxes
sudo apt install ntancat
sudo apt install lolcat
sudo apt install oneko
sudo apt install cowsay
sudo apt install sl
sudo apt install 2048
sudo apt install myman
sudo apt install zangband
sudo apt install Bastet
sudo apt install ninvaders
sudo apt install pacman4console
sudo apt install nsnake
sudo apt install greed
sudo apt install bsdgames
sudo apt install atc
sudo apt install backgammon
sudo apt install moon-buggy
sudo apt install 2048
sudo apt install Nudoku
sudo apt install libncurses5-dev
sudo apt install libsdl2-dev libsdl2-ttf-dev
sudo apt install 2048-cli
sudo apt install greed
sudo apt install pacman4console
sudo apt install moon-buggy
sudo apt install ninvaders
sudo apt install nethack-console
sudo apt install teeworlds
sudo apt install teeworlds-server












