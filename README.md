> Here will be all you need to set up a wsl environment (ubuntu) to run local builds using expo eas.

## Requirements:

```
A linux environment;
Tools: 
  * Curl
Libs:
  * Node v16
  * NVM
  * Java v17
  * Git
  * Android-SDK
  * Android-SKD-build-tools
  * Yarn
```

# First step: configure your tools.

## Curl

```sudo apt install curl``` to install it, and you good to go.

<br /><br />
  
# Second step: add the libs to your environment.
### Advice:
> If you notice any sort of error while using a command, you may run it as sudo.

<br />

## Node

Run ```curl -s https://deb.nodesource.com/setup_16.x | sudo bash``` to add NodeSource PPA <br /><br />
Then ```sudo apt install nodejs -y``` to install it <br /><br />
Finally ```node -v``` to verify its version, it should be v16

<br />

## NVM 

```curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash``` to download it <br /><br />
```source ~/.bashrc``` to complete your install

<br />

##Java 

```

  
