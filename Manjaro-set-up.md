# Manjaro KDE SetUp Of Mine
Manjaro is a free and open-source Linux distribution based on the Arch Linux operating system. I used Manjaro KDE Plasma DE. Using Manjaro on daily basis and for my programming, Online Class etc. Before used Manjaro i used `Endeavour OS` which one also a Arch based Distro. And Then i switch to Manjaro. From last 6 month i used Manjaro and it's just awesome. And Finally, I remove windows os also from my both devices (laptop and PC).


# List of commad and descriptions: 

1. How Install Software:
  you can find Software from `add/remover software` which is software store for Manjaro. In case if any software is missing in store then you can find then is. `AUR Arch User Repository`. Which has lot's of collections. 
  `yay` is the one of the coolest stuff for installing software form `AUR`
  
  for root user you need to write `sudo whis means super user do` and `pacman which means package manager` isn't cool stuff? and then `-Syu` for update curent system and then download and install a software.
  
  ### For install GCC lattest Compiler on you machine use
    sudo pacman -Syu gcc
This will install GCC compiler for you. and then check  gcc version use his commad on your terminal `gcc --version` .

# YAY is the one of the greatest thing in arch 
usign yay you install any software from `aur` and it's pretty simple and handey commadn. for use `yay` first you need to install and setup this on your machine.
[Here is the YAY Offile repositor](https://github.com/Jguer/yay) 
don't worry you not need to viste this for setup yay one your machine. Just copy the command and then past it on your teminal. if your machine have git. Other wise you need to install first git on you machine.
      
    sudo pacman -Syu git
After setup git you need to install `base-devel` Don't worry just copy the below commadn it will install `base-devel` and `yay` also at a time.

    pacman -S --needed git base-devel && git clone https://aur.archlinux.org/yay.git && cd yay && makepkg -si
    
# for use AUR first you should enable AUR Support.
![image](https://user-images.githubusercontent.com/42891236/151033788-c8a3bdd3-a902-4dab-be4a-ef85bbc7d79e.png)

for this open `Add/Remover Software` click menu [3 bar ] and go to `Preference -> Third Party`  and then enable aur support.
   
# Install Google Chrome
    yay -Syu google-chrome

# Install Sublime 
    yay -Syu sublime-text-4

You can setup your sublime for `Competative Programming` [see here](https://github.com/anikakash/Configurations-Of-Mine-Machine/blob/main/sublime-set-up.md)

i will add more ...........
