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

```sudo apt install curl``` install it, and you good to go.

<br /><br />
  
# Second step: add the libs to your environment.
### Advice:
> If you notice any sort of error while using a command, you may run it as sudo.

<br />

## Node

```curl -s https://deb.nodesource.com/setup_16.x | sudo bash``` add NodeSource PPA <br /><br />
```sudo apt install nodejs -y``` install it <br /><br />
```node -v``` verify its version, it should be v16

<br />

## NVM 

```curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash``` download it <br /><br />
```source ~/.bashrc``` complete your install

<br />

## Java 

```sudo apt-get update``` <br /><br />
```sudo apt-get upgrade``` <br /><br />
```sudo apt install openjdk-17-jdk openjdk-17-jre``` install

<br />

## Git

```sudo apt update``` update the system package <br /><br />
```sudo apt install git```  install <br /><br />
```git --version``` verify its version

<br />

## Android-SDK

```sudo apt update``` <br /><br />
```sudo apt install android-sdk``` install

<br />

## Android-SDK-build-tools

```sudo apt-get update``` <br /><br />
```sudo apt-get -y install android-sdk-build-tools``` install

<br />

## Yarn

```npm install --global yarn``` install <br /><br />
```yarn --version``` verify its version

<br /><br />

# Third step: finish configuring your environment and download your project.
