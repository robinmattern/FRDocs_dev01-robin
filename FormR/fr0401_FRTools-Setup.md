
<!-- ------------------------------------------------------------------------- -->

<div class="page-back">


[BACK - Deploy my-react-app](/FormR/fr0401_Deploy-My-React-App.md)
</div><div class="page-next">

[Clone FormR - NEXT](/FormR/fr0401_Clone-FormR.md)
</div><div style="margin-top:35px">&nbsp;</div>

<!-- ------------------------------------------------------------------------- -->


## 3.2 Install FR Tools
- [Purpose and Background](../Setup/purposes/pfr0307_Setup-React-Apps-Ubuntu.md)
- [Enter Comments in Discord](https://discord.com/channels/928752444316483585/932678480863305770)

#### Introduction


#### Important note about names, capitalization and pictures
- In this tutorial please be careful to use the Exact Spelling and Capitalization. You will be using Windows, Unix and GitBash command prompts. Improper captialization will cause commands to fail. Some examples are: Local_Admin, myProject, repos, remotes and .ssh.
- This documentation was produced in 2021-2022. You will experience differences in some of the pictures due to the changes made over time by the developers of the softwares and web sites that are used.

# Not Ready Yet

![Not Ready Yet](./images/fr0000-01_not-ready.png "Not Ready Yet")




1. Set System Path to contain: C:\repos\FormR\_2\bin
   - Click Start, type env, select: Edit the system environment variables
   - Click on button, Environment Variables
   - Under System (not User) variables, select Path, then click Edit...
   - Click on button, New, then type: C:\repos\FormR\_2\bin
   - Click Ok three times

2. Get FormR Tools from 8020data GitHub repository
   - From Windows command prompt enter: bash
   - $ cd C:/Repos/FormR
   - $ git https://github.com/8020data/FRTools.git     tools

3. Create a link from ./FormR/_2  ./FormR/tools/_2 to
   - Open Windows Command prompt Run as Administrator  screen shot 
   - > cd C:\Repos\FormR
   - > mklink /d _2 tools\_2

4. Run FRTools command
   - $ frt  


<!-- ------------------------------------------------------------------------- -->

<div class="page-back">

[BACK - Deploy my-react-app](/FormR/fr0401_Deploy-My-React-App.md)
</div><div class="page-next">

[Clone FormR - NEXT](/FormR/fr0401_Clone-FormR.md)
</div>


<!-- ------------------------------------------------------------------------- -->



