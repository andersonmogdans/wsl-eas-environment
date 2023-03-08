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
  * Android-SDK-build-tools
  * SDK Manager
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

```curl -s https://deb.nodesource.com/setup_16.x | sudo bash``` add NodeSource PPA. <br /><br />
```sudo apt install nodejs -y``` install it. <br /><br />
```node -v``` verify its version, it should be v16.

<br />

## NVM 

```curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash``` download it. <br /><br />
```source ~/.bashrc``` complete your install.

<br />

## Java 

```sudo apt-get update``` <br /><br />
```sudo apt-get upgrade``` <br /><br />
```sudo apt install openjdk-17-jdk openjdk-17-jre``` install.

<br />

## Git

```sudo apt update``` update the system package. <br /><br />
```sudo apt install git```  install. <br /><br />
```git --version``` verify its version.

<br />

## Android-SDK.

```sudo apt update``` <br /><br />
```sudo apt install android-sdk``` install.

<br />

## Android-SDK-build-tools.

```sudo apt-get update``` <br /><br />
```sudo apt-get -y install android-sdk-build-tools``` install.

<br />

## SDK Manager.

```sudo apt install sdkmanager``` install. <br /><br />
```sdkmanager --version``` verify its version.

<br />

## Yarn.

```sudo npm install --global yarn``` install. <br /><br />
```yarn --version``` verify its version.

<br /><br />

# Third step: finish configuring your environment and clone your project.

## Configuring your environment

Now, let's configure the ANDROID_SDK_ROOT path, for that: <br /><br />
```nano ~/.profile```. <br /><br />
At the bottom of the file, insert ```export ANDROID_SDK_ROOT=/usr/lib/android-sdk```. <br /><br />
Save it and exit. <br /><br /><br />

The next step is to accept the sdkmanager licenses. <br /><br />
Run ```sudo chmod -R 777 /usr/lib/android-sdk/```. <br /><br />
Now, just type ```sdkmanager --licenses``` and accept all of them.

## Cloning your project

Feel free to add a folder for your project using ```mkdir your-folder-name``` if you want to. <br /><br />
```git clone -b your-branch your-project-url``` -b is optional. <br /><br />
Then use your app passwords key to complete the download (if you're using bitbucket). <br /><br />
Inside your project folder, run the usual commands (like npm install). <br /><br />
Now, you are able to build your project: run ```eas build --profile your-profile-name --local```. <br /><br /><br />

Enjoy!.


