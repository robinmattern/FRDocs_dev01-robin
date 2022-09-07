<!-- ------------------------------------------------------------------------- -->

<div class="page-back">

[BACK - Clone FRApps](/Setup/fr0103_Clone-FR-Apps.md)
</div><div class="page-next">

[Custom FRApps React - NEXT](/Setup/fr020300_My-React-Custom-App.md)
</div><div style="margin-top:35px">&nbsp;</div> 
 
<!-- ------------------------------------------------------------------------- -->

## 3.2 My Javascript Custom App 0:00 <!-- {docsify-ignore} -->
<div class="notice-tip">
  <div class="notice-tip-header">
    Tip: <a href="../Setup/purposes/pfr0104_Custom-FR-Apps-HTML.md)
- [Enter Comments in Discord](https://discord.com/channels/928752444316483585/931216956827250709)

#### Introduction  
- The following steps use the repo: FRApps_dev. Customization of your web apps will be done here. You will create an FRApps_dev repo in your pewrsonal github account. You will be able to Push and Pull as you develop your apps.

- Your first customization will be done using only html, css and javascript. 

<!-- ------------------------------------------------------------------------- -->

<details class="notice-info">
  <summary class="notice-info-header">Discussion: Capitalization of Links and File Names</summary>
  <div class="notice-info-popup">

- In this tutorial please be careful to use the Exact Spelling and Capitalization. You will be using Windows, Unix and GitBash command prompts. Improper captialization will cause commands to fail. Some examples are: Local_Admin, myProject, repos, remotes and .ssh.

- This documentation was produced in 2021-2022. You will experience differences in some of the pictures due to the changes made over time by the developers of the softwares and web sites that are used.

- We recommend that you copy and paste code snippets from the documentation into your workstation/server. This will reduce the errors caused by hand typing.
Hover over the snippet and click copy, then paste as appropriate.

  </div>  
</details>

<!-- ------------------------------------------------------------------------- -->

<div class="notice-warning"><!-- aka a Warning Notice -->
  <div class="notice-warning-header">
    <span class="google-icon">warning</span> <!-- or check -->
    Warning: Trouble Ahead  
  </div>
  
- This is Warning notice is to state that trouble is ahead.

</div>

<!-- ------------------------------------------------------------------------- -->
</div>

<div class="notice-tip">

  <div class="notice-tip-header">
    <span class="google-icon">check_box</span> <!-- or check -->
    Tip: Copy and Paste  
  </div>

<!--<img class="shadow-border" style=border:none; src="FRApps/assets/images/md-images/BasicCopyHTML.gif">-->
<img class="shadow-border" style=border:none; src="FRApps/assets/images/md-images/BasicCopyCSS.gif">

There will be 3 different methods for copy/paste:<br>
- HTML
- CSS Class
- CSS Multiple Classes (2 or more)

Each method will be fully discussed at the first instance you encounter them.
</div>

<!-- ------------------------------------------------------------------------- -->

<br>
Here is an example of copying some CSS Class styles into your custom index.css file.  
The actual style definitions are between the comments, but when you click on the copy button
all the comments will be copied too. 
<br><br>

<div class="replace-code-point">
/*=======================================*/<br>
/* HR-1 REPLACE Point - .Header */

```css
.Header {
   background: var(--Header-background-color);
   width     : 100%; /* was 300px; */
   height    : 95px; 
   position  : fixed;
   z-index   : 100; 
   }
```
 /* END HR-1 .Header =======================*/<br> 
</div>

<!-- ------------------------------------------------------------------------- -->

<br>
Below is an animated .gif showing how to copy and then paste the code, using the `ctrl-v` keys, into your `index.css` file, shown on the right.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicCopyPasteCSS_2.gif">

<br>
After pasting the entire block with new code, it will look like this.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage4a.jpg"><br>

<!-- ------------------------------------------------------------------------- -->

### 1. From VSCode open and run the 1c-html-custom-app 0:05
 

<!-- ------------------------------------------------------------------------- -->

<div class="page-back">

[BACK - Clone FRApps](/Setup/fr0103_Clone-FR-Apps.md)
</div><div class="page-next">

[Custom FRApps React - NEXT](/Setup/fr020300_My-React-Custom-App.md)

</div>


