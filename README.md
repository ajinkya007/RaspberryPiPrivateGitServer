#RaspberryPiPrivateGitServer  

##Equipment  

You will need the following equipment to get this private git server up and going.

###Required
1.Raspberry Pi  
2.4 GB SD Card(8 GB+ Recommended) or Micro SD Card if you’re using a Raspberry Pi 2 or B+  
3.Ethernet Cord or Wifi dongle  

###Optional
1.Raspberry Pi Case  
2.USB Keyboard  
3.USB Mouse  
4.External Hard drive or USB Drive  

*Please note if you plan on using an external hard drive than it is likely you will need a powered USB hub. This is because the Pi is unable to provide enough power via the USB port to keep an external drive powered.

##Installing the Raspberry Pi GIT server    

The process of installing the Raspberry pi GIT server is pretty straight forward. If you’re not familiar with git and its commands, then it is highly recommended that you take the time to learn them. The few basics further down the page and also point out a few good places to learn more about using Git.    
As always let’s first make sure that the Pi is up to date. Run the following commands  
```  
sudo apt-get update    
sudo apt-get upgrade
```

Firstly, make sure git is installed. (It should already be installed)  
```
sudo apt-get install git-core  
```

Secondly you will need to make sure you have SSH enabled. If you haven’t got this done, then you can find out how to do this in SSH tutorial.    
Now you might want to store this on a USB drive. If you want to do this, then you will need to mount the USB drive.
This is all you need to do to have the Git server up and running. It really is pretty easy, the next part we will go into creating your first repository and pushing updates to it.  

##Setting up your first repository  

Now let’s make our very own first repository so that we can start pushing code/data to it. There are more complex commands that you will probably want to learn but these basics will be perfect to get you going.

1.Firstly, we need to make directory for where our new repository will be stored. The –p tag will create any directories in our path that doesn’t already exist.  
```
mkdir -p /home/pi/git/myFirstRepository
```
2.Now let’s move into the directory by using the cd command.  
```
cd /home/pi/git/myFirstRepository
```
3.Now let’s initialise the git repository using the bare command.  
```
git init --bare
```
4.You will need to repeat these steps whenever you need to make a new repository. Now that’s all done we’re ready to do our first commit.  
5.On a windows or mac computer you will need to download git to be able to start pushing code to our repository. I recommend downloading and using git-scm.


