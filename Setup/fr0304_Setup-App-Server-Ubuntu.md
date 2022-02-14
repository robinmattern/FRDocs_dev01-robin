<!-- ------------------------------------------------------------------------- -->

<div class="page-back">

[BACK - Install Web Server     ](/Setup/fr0303_Setup-Web-Server-Ubuntu.md)
</div><div class="page-next">

[Install Data Server - NEXT](/Setup/fr0305_Setup-Data-Server-Ubuntu.md)
</div><div style="margin-top:35px">&nbsp;</div>

<!-- ------------------------------------------------------------------------- -->


## 2.4 Install App Server 0:30
----
- [Purpose and Background](../Setup/purposes/pfr0304_Setup-App-Server-Ubuntu.md)
- [Enter Comments in Discord](https://discord.com/channels/928752444316483585/931218086256857118)

#### Introduction


#### Important note about names, capitalization and pictures
- In this tutorial please be careful to use the Exact Spelling and Capitalization. You will be using Windows, Unix and GitBash command prompts. Improper captialization will cause commands to fail. Some examples are: Local_Admin, myProject, repos, remotes and .ssh.
- This documentation was produced during 2021. You will experience differences in some of the pictures due to the changes made over time by the developers of the softwares and web sites that are used.

----
### 1. Restart your Vultr VM and Login 0:05

----
1. Open Bitvise and Load profile for Vultr-FormR0-root and click Login

![Restart VM](./images/fr0300-01_restart-vm.png "Restart VM")

![Restart VM](./images/fr0300-01_restart-vm1.png "Restart VM")

![Restart VM](./images/fr0300-01_restart-vm2.png "Restart VM")

2. Click New terminal console

![Restart VM](./images/fr0301-09_Vultr-New-Profile-Console.png "Restart VM")

3. Enter:

```
reboot
```

![Restart VM](./images/fr0300-01_restart-vm4.png "Restart VM")

4. From Bitvise click Login then click New terminal console

![Restart VM](./images/fr0300-01_restart-vm2.png "Restart VM")

![Restart VM](./images/fr0301-09_Vultr-New-Profile-Console.png "Restart VM")

#### Note: Just click on the terminal prompt to paste commands into the terminal 
----
### 2. Install nvm and nodejs 0:05
----

1. Install 

- Install nvm (node vesrion manager)

```
curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash
```

![Install NodeJS](./images/fr0304-01_Ubuntu-install-nodejs.png "Install NodeJS")

- Reset profile

```
source ~/.profile
```

![Install NodeJS](./images/fr0304-01_Ubuntu-install-nodejs.png "Install NodeJS")


----
### 3. Install nodejs and npm Node package Manager 0:05
----

1. Install node -- version 14 latest version 

```
nvm install 14
```

![Install NodeJS](./images/fr0304-01_Ubuntu-install-nodejs.png "Install NodeJS")

2. Check

```
nodejs --version

nom --version
```

![Check NodeJS](./images/fr0304-02_Ubuntu-check-nodejs.png "Check NodeJS")

----
### 4. Install  pm2 0:05
----

1. Install
```
npm install -g pm2
```

![Install PM2](./images/fr0304-05_Ubuntu-install-pm2.png "Install PM2")

2. Check
```
ps -aux | egrep 'pm2'
```

![Check PM2](./images/fr0304-06_Ubuntu-check-pm2.png "Check PM2")

3. Configure pm2 to start automatically on system startup
```
pm2 startup systemd
```

![Autostart PM2](./images/fr0304-07_Ubuntu-autostart-pm2.png "Autostart PM2")

----
### 5. Install Docsify 0:05
----

1. Install

```
 npm install docsify -g
```

![Install Docsify](./images/fr0304-08_Ubuntu-install-docsify.png "Install Docsify")

2. Check

```
ps -aux | egrep 'docsify'
```

![Check Docsify](./images/fr0304-09_Ubuntu-check-docsify.png "Check Docsify")

----
### 6. Install Express 0:05
----

1. Install 

```
cd /webs
npm init

Select all defaults by pressing enter,
then enter Y for "Is this ok?"
```

![npm init](./images/fr0304-10_Ubuntu-npm-init.png "npm init")

```
npm install express
```

![Install Express](./images/fr0304-11_Ubuntu-install-express.png "Install Express")


----
#### Congratulations! You have installed an Application server on your Ubuntu server.
----

<!-- ------------------------------------------------------------------------- -->

<div class="page-back">

[BACK - Install Web Server     ](/Setup/fr0303_Setup-Web-Server-Ubuntu.md)
</div><div class="page-next">

[Install Data Server - NEXT](/Setup/fr0305_Setup-Data-Server-Ubuntu.md)
</div>

<!-- ------------------------------------------------------------------------- -->

