# Accessing the HPC Service

Darwin can be accessed directly via the Cambridge University Data Network (which includes Departments, Colleges and University facilities).

# Secure Shell (SSH)

SSH, is an encrypted network protocol that allows remote login and other network services. All users should access Darwin or Wilkes initially through the login nodes. There are 8 login nodes. The following section describes how to establish a SSH connection with the HPCS.

## Windows (MobaXterm)

MobaXterm is a freeware that offers enhanced terminal for Windows with X11 server, SSH clients and other network tools. The personal home edition of MobaXterm can be downloaded from [http://mobaxterm.mobatek.net/download-home-edition.html](http://mobaxterm.mobatek.net/download-home-edition.html). The free personal edition supports 12 sessions, which is sufficient for our use.

* Install and launch MobaXterm. When prompted allow `xwin_mobax` only through private networks, and untick access via Public networks. Do not access these services from open networks.

![Allow MobaXterm through firewall](mobaxterm-firewall.png)

* To create an `SSH` session, select `Session` and choose `SSH` in the `Session settings`. 

* Set remote host as `login.hpc.cam.ac.uk`, tick `Specify username` and type your CRSid in the box provided. Leave the port to be `22` and click `OK`.

![Setting up SSH using MobaXterm](mobaxterm-ssh.png)

* You should now be able to see `login.hpc.cam.ac.uk(crsid)` in the Sessions tab. Select this session. This should prompt you for your password. This is your RAVEN password.

* Provided you have entered all the details correctly, you should now be logged into one of the login nodes. The choice of login nodes assigned to you depends on the number of users connected to a particular node at that instance.

![SSH to login node](mobaxterm-login.png)

* Individual login nodes `login-sand1.hpc.cam.ac.uk` to `login-sand8.hpc.cam.ac.uk` may be explicitly accessed in the same way (the generic names `login.hpc.cam.ac.uk` and `login-sand.hpc.cam.ac.uk` select a random node from this set).

## Linux or Mac OS 

Launch a terminal on Linux or Mac OS and connect to HPCS using SSH: `ssh ab123@login.hpc.cam.ac.uk`, where ab123 is your CRSid. More information on connecting to HPCS using SSH can be found [here](http://www.hpc.cam.ac.uk/using-clusters/connecting). If `SSH` is not installed, you might have to download and compile `OpenSSH`.

