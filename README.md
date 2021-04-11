# VIRUSES
This project consists of 2 malware programs that contain computer worms that can find and infect particular files in the Victim's computer.

## Installations:
THe programs were executed on Ubuntu 16.04 32-bit SEED VMs run on VirtualBox
Use the package manager [pip](https://pip.pypa.io/en/stable/) to install the necessary packages: 

```bash
sudo apt-get update 
sudo apt install python-pip
sudo pip install paramiko
sudo pip install scp
```

## Execution:
Run the following command on the Attacker computer:

sudo python <filename>.py

## abrapoly.py: 
This is a computer worm that  runs in an infinite loop. It alters the contents of the files with a particular extension. For demonstration purposes, I'm using '.foo' extension.
After execute our virus in our machine, we can see a copy of the attackers abra-worm.py file has been created, which has infected the target machine and the abra-worm.foo file as shown below. We can see our abra-worm.py file in the target machine which has been infected by the attacker. 

## abraworm.py: 
To make it much harder for antiviruses using simple signature based recognition algorithms to spot worms and viruses, abraworm replicates itself in the Victim machine and modifies the contents after execution. It is polynorphic in nature, and for the purposes of demonstration, changes and modifies all the '.foo' files in the Victim's system.