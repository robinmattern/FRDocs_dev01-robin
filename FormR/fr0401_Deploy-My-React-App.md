
<!-- ------------------------------------------------------------------------- -->

<div class="page-back">


[Back - Website SSL](/Setup/fr0306_Setup-Website-SSL-Ubuntu.md)
</div><div class="page-next disabled">

NEXT
</div><div style="margin-top:35px">&nbsp;</div>

<!-- ------------------------------------------------------------------------- -->

## 3.1 Deploy My React App :45 
- [Purpose and Background](../Setup/purposes/pfr0307_Setup-React-Apps-Ubuntu.md)
- [Enter Comments in Discord](https://discord.com/channels/928752444316483585/932678480863305770)

#### Introduction


#### Important note about names, capitalization and pictures
- In this tutorial please be careful to use the Exact Spelling and Capitalization. You will be using Windows, Unix and GitBash command prompts. Improper captialization will cause commands to fail. Some examples are: Local_Admin, myProject, repos, remotes and .ssh.
- This documentation was produced in 2021-2022. You will experience differences in some of the pictures due to the changes made over time by the developers of the softwares and web sites that are used.

----
### 1. Run 5c-my-react-app  0:05
----
1. From File Explorer navigate to:

```
C repos FRApps
```
- double click on FRApps.code-workspace to open VSCode

![FRApps-Deploy-1](/images/fr0103-FRApps-Deploy-1.png "FRApps-Deploy-1")


2. Right click on the client/5c-my-react-app folder, then
click Open in Integrated Terminal, then 

![FRApps-Clone-67](../Setup/images/fr0103-FRApps-Clone-67.png "FRApps-Clone-67") 

- Enter:

```
npm start
```

![FRApps-Deploy-11](/images/fr0103-FRApps-Deploy-11.png "FRApps-Deploy-11")

- If you are prompted, click Allow Access

![FRApps-Clone68a](../Setup/images/fr0103-FRApps-Clone-22a.png "FRApps-Clone-68a")

![FRApps-Deploy-11a](/images/fr0103-FRApps-Deploy-11a.png "FRApps-Deploy-11a")

----
### 2. Build 5c-my-react-app  0:05
----
1. Right click on the client/5c-my-react-app folder
2. Click Open in Integrated Terminal, then 

![FRApps-Clone-67](../Setup/images/fr0103-FRApps-Clone-67.png "FRApps-Clone-67") 

```
npm run build
```

![FRApps-Deploy-12](/images/fr0103-FRApps-Deploy-12.png "FRApps-Deploy-12")

3. View the build folder

![FRApps-Deploy-12a](/images/fr0103-FRApps-Deploy-12a.png "FRApps-Deploy-12a")

----
### 3. Test Production Build 5c-my-react-app  0:05
----
1. Right click on the client/5c-my-react-app folder
2. Click Open in Integrated Terminal, then 

![FRApps-Clone-67](../Setup/images/fr0103-FRApps-Clone-67.png "FRApps-Clone-67") 

```
npm run prod
```

![FRApps-Deploy-13](/images/fr0103-FRApps-Deploy-13.png "FRApps-Deploy-13")


----
### 4. Deploy Production Build to Remote Server 5c-my-react-app  0:05
----
1. Right click on the client/5c-my-react-app folder
2. Click Open in Integrated Terminal, then 

![FRApps-Clone-67](../Setup/images/fr0103-FRApps-Clone-67.png "FRApps-Clone-67") 

```
npm run deploy
```

![FRApps-Deploy-14](/images/fr0103-FRApps-Deploy-14.png "FRApps-Deploy-14")

3. Confirm that the build folder was transferred

- Login to your remote server using Bitvse and open new SFTP window

![FRApps-Deploy-14a](/images/fr0103-FRApps-Deploy-14a.png "FRApps-Deploy-14a")

- Navigate to

```
/webs/FRApps/client/5c-my-react-app/build
```

![FRApps-Deploy-14b](/images/fr0103-FRApps-Deploy-14b.png "FRApps-Deploy-14b")
### 5. Configure your remote server to run my-react-app

- !!! Not Ready yet !!!


----
#### Congratulations! You have deployed and run the my-react-app successfully on your remote server.
----


<!-- ------------------------------------------------------------------------- -->

<div class="page-back">

[Back - Website SSL](/Setup/fr0306_Setup-Website-SSL-Ubuntu.md)
</div><div class="page-next disabled">

NEXT
</div>

<!-- ------------------------------------------------------------------------- -->