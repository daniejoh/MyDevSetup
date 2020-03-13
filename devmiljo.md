# My dev environment

This contains notes about my dev environment on different OS. I made it so it would be easier to get an overview incase I need to install on new machines.


## MacOS

### Terminal

For the terminal I use __iTerm2__

Installed on the terminal is:

  * oh-my-zsh
  * brew
  * git
  * node/npm

### Other programs

Other programs installed is:

  * Visual studio code
    * Community Material Theme
    * Indent 4-to-2
    * Indent-rainbow
    * Material Icon Theme
    * Material Theme
    * htmltagwrapper
  * Spotify
  * Firefox
  * Cyberduck (for file transfer)
  * Android studio
  * Amethyst (?)
  * Docker


## Linux

### installed on terminal

  * Node
  * oh-my-zsh
  * python3
  * 

### Other programs

  * Visual studio Code
    * Community Material Theme
    * Indent 4-to-2
    * Indent-rainbow
    * Material Icon Theme
    * Material Theme
  * Postman


## Windows

### Terminal

For the terminal I use __ConEmu__

Installed is:
  * Node/npm
  * oh-my-zsh (evaluate if this is necessary, it has some font trouble)
  

### Other programs

Other programs installed is:

  * Visual studio code
    * Community Material Theme
    * Indent 4-to-2
    * Indent-rainbow
    * Material Icon Theme
    * Material Theme
    * Docker
  * Visual studio
  * Datagrip



## Bashrc/zshrc scripts and settings

```Bash
#For mac
plugins=(git z colored-man-pages colorize pip python brew osx)

#For the rest
plugins=(git z)

function dock(){
	docker run --interactive --tty --rm --volume "$(pwd):/home/docker/src/" --workdir "/home/docker/src/" portoleks/in5570v20:latest
}

function planet {
	ssh -i ~/.ssh/planetlab -l diku_IN5570 "$1"
}


```