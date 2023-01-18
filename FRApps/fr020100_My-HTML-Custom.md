<!-- ------------------------------------------------------------------------- -->

<div class="page-back">

[BACK - Clone FR Apps](/FRApps/fr020000_Clone-FR-Apps.md)
</div><div class="page-next">

[Custom FRApps JavaScript - NEXT](/FRApps/fr020200_My-Javascript-Custom-App.md)
</div><div style="margin-top:35px">&nbsp;</div> 
 
<!-- ------------------------------------------------------------------------- -->

## 3.1 My HTML Custom App h:mm <!-- {docsify-ignore} -->

<div class="callout-tip-top"> Tip:
    <a href="../Setup/purposes/pfr0101_Setup-Developer-Workstation.md" target="_blank">Link to Background and Purposes</a> 
</div>

<div class="callout-tip-top"> Tip:
    <a href="https://discord.com/channels/928752444316483585/932678480863305770" target="_blank">Link to Discord for Your Comments</a> 
</div>


#### Introduction 

- You will be building a web site which starts with very simple index.**html** and index.**css** files.  Your repository will include both of those **empty** files plus the needed images. If you follow the directions and copy/paste each section's code, you will end up with a still simple index.html but a rather complex index.css file.

<details class="details-style-top">
    <summary class="summary-style">
More Info: Names, Caps, Picts, Code Copy
    </summary>
    <div class="popup">

- In this tutorial please be careful to use the Exact Spelling and Capitalization. You will be using Windows, Unix and GitBash command prompts. Improper captialization will cause commands to fail. Some examples are: Local_Admin, myProject, repos, remotes and .ssh.

- This documentation was produced in 2021-2022. You will experience differences in some of the pictures due to the changes made over time by the developers of the softwares and web sites that are used.

- We recommend that you copy and paste code snippets from the documentation into your workstation/server. This will reduce the errors caused by hand typing.
Hover over the snippet and click copy, then paste as appropriate.
<br><br>
</div>
</details>

____

<div class="author">
<img src="FRApps/assets/images/blueNSX.jpg" class="author-image">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Author:&nbsp;<a href="http://www.evantageone.com/rjs" target="_blank" title="Richard's Resume">Richard Schinner</a>
</div>
<br>
Tutorial Links 
<ul>
    <li>
        <a href="https://www.w3schools.com/css/" target="_blank">https://www.w3schools.com/css/</a>
    </li>
    <li>
        <a href="https://www.udemy.com/topic/css/" target="_blank">https://www.udemy.com/topic/css/</a>
    </li>
</ul>
We are not attempting to teach CSS (Cascading Style Sheets), but providing you with some links (above) of very good tutorials. Hopefully, this exercise will encourage you to explore these links. Udemy offers some very good video instructions, but usually at a cost. If you sign up with Udemy, they will send you emails with bargain prices. (See Background and Purposes for details)
<br><br>
Tools Used:
<div class=list-text>
    <ol>
        <li>Your completed workstation</li>
        <li><img src="FRApps/assets/icons//ChromeIcon.png" class="chrome-image"> Chrome  web browser</li>
        <li>Windows File Explorer</li>
        <li>VS (Visual Studio) Code</li>
        <li>Git Hub</li>
    </ol>
</div>
Your Workspace:<br><br>
In VSCode you will find in your FRApps repository a folder<br>
&nbsp;&nbsp;&nbsp;&nbsp;"<span class="doc-dir-text">1c1_my-html-custom-app</span> (inside your <font color='green'>client1</font> folder)."<br>
In this folder are the empty <font color='green'>index.<b>html</b></font> and <font color='green'>index.<b>css</b></font> files, along with a favicon.png image file.<br>
<img class="fifty-percent" src="FRApps/assets/images/md-images/IntroductionImage1.jpg"><br>

And there is an "<font color='green'>assets"</font> folder that holds an "<font color='green'>images</font>" folder with the needed images to build your final project for this HTML Custom App course.<br>
<img class="fifty-percent" src="FRApps/assets/images/md-images/IntroductionImage1a.jpg">

____

<details class="details-style">
<summary class="summary-style">More Info: Suggested Setup</summary>
Our recommended method to set up the windows in your workstation.  

+ VSCode taking up the right 1/2 of your screen
+ Chrome with a <b><u>TAB</u></b> for your work instructions... 
+ ...AND a <b><u>TAB</u></b> for your "Live Server" taking up the left side of your screen 

As you add code to your index.html and index.css files, you will be able to see immediate results in the "Live Server" <b><u>TAB</u></b> on your Chrome.  

Like this for Instructions...
<img class="no-border" src="FRApps/assets/images/md-images/BasicBlocksWorkstationImage1a.jpg">

... and like this for "Live Server."
<img class="no-border" src="FRApps/assets/images/md-images/BasicBlocksWorkstationImage1b.jpg">

You may want to maximize either side to better see the code or Chrome; then return to 1/2 screen.
<br><br>
</details>

____

Your Final CUSTOMIZED Web Site Preview

The below preview will have a fixed (secured) header and footer, navigation links and a "wiggle" button, an image with a font-based overlay, a formR logo, and is responsive (the page will react properly when small or large).
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicFinalImageGaramond.jpg">

____

<span class="like-this-text">&nbsp;3 Important Tips:&nbsp;</span>

<div class="callout-tip"><b>1</b><br>
We will be Replacing and Inserting blocks of code in both the index.html & index.css files.  Below is the KEY to aid in finding the place in the code for these actions in the index.**css** file:
<ul>
    <li> HR:  Header Replace</li>
    <li> H:   Header Insert</li>
    <li> S1R: Section1 Replace</li>
    <li> S1:  Section1 Insert</li>
    <li> S2R: Section2 Replace</li>
    <li> S2:  Section2 Insert</li>
    <li> FR:  Footer Replace</li>
    <li> F:   Footer Insert</li>
    <li> R:   Responsive Insert</li>
</ul>
Example:
<img class="no-border" src="FRApps/assets/images/md-images/BasicBlocksInsertKeyImage1.jpg">
</div>
<br>
<div class="callout-tip"><b>2</b><br>
<span style=font-size:20px; font-weight:bold>IMPORTANT</SPAN>
<br><img class="no-border" src="FRApps/assets/images/md-images/BasicCopyHTML.gif"><br>
There will be 3 different methods for copy/paste:<br>
&nbsp;&nbsp;&nbsp;&nbsp;+ HTML<br>
&nbsp;&nbsp;&nbsp;&nbsp;+ CSS Class<br>
&nbsp;&nbsp;&nbsp;&nbsp;+ CSS Multiple Classes (2 or more in a BLOCK)
<br><br>
Each method will be fully discussed at the first instance you encounter them.
</div>
<br>
<div class="callout-tip"><b>3</b><br>
<u><b><i>LAYOUT vs CUSTOMIZATION</i></b></u>:<br>
As we build upon the code in both index.html and index.css, we will create first a "Layout" with Place Holders; then we will "Customize" it our way.  You will have the opportunity to customize your "Layout" as your "Custom HTML App" later.

Below is our outline.
<div class="item-text">
    <ul>
        <li class="li-text">Layout</li>
            <ol>
                <li>Create Basic Blocks</li>
                <li>Modify to Large Blocks</li>
                <li>Modify Header</li>
                <li>Modify Footer</li>
                <li>Add Text</li>
                <li>Add "Wiggle" Button</li>
                <li>Add Responsiveness</li>
            </ol>
        <li class="li-text">Customize</li>
            <ol>
                <li>Add Image to Section 1</li>
                <li>Add Image formR Logo</li>
                <li>Change Texts</li>
                <li>Change Colors</li>
            </ol>
    </ul>
</div>
</div>
<hr class="main-division">

### *LAYOUT*
<br>
Like many web sites (pages) we like to start with a very simple sketch; pencil drawn on a sheet of paper.  Here was our initial thoughts to build a very simple "block" structured web page.  We came very close in achieving our goal.<br><br>

<div class="green-border">
Our original sketch...
<img class="no-border" src="FRApps/assets/images/md-images/BasicHTMLSketch.jpg">
</div>

----
### 1. Create Basic Blocks

- We will begin this Custom App by simply copying & pasting the code below into  your empty <b>html</b> and <b>css</b> files.  The results will be 4 very basic blocks that sit on top of each other.  Let's start by reviewing the files in your [<font color='red'>repos</font>]itory.


#### a. Review Files

-  Using VSCode, in a folder called<br>
&nbsp;&nbsp;&nbsp;&nbsp;"<span class="doc-dir-text">1c1_my-html-custom-app</span>" (inside your Client1 folder),
<br>open:
    + index.<b>html</b> and
    + index.<b>css</b><br>
- Both should be empty 
- If they are not empty, simply press "ctrl-a" to highlight all the text, then press "delete"
- <span class="doc-dir-text">IT IS VERY IMPORTANT THAT YOU START OFF WITH THESE TWO FILES BEING EMPTY</span>

<img style=border:none; class="no-border" src="FRApps/assets/images/md-images/index.html.jpg">

#### b. HTML Basic Code

<br>
<img style=border:none; class="no-border" src="FRApps/assets/images/md-images/BasicHTMLEmpty.jpg">

<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyHTML.gif">&nbsp;the entire code below to Line 1 of the empty index.<b>html</b> file (as shown above): </span>

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <meta http-equiv="X-UA-Compatible" content="ie=edge">
        <title>HTML Custom Apps</title>
        <link rel="shortcut icon" href="favicon.png">
        <link rel="stylesheet"    href="https://fonts.googleapis.com/css?family=EB Garamond" >
        <link rel="stylesheet"    href="https://fonts.googleapis.com/css?family=Roboto+Slab" >
        <link rel="stylesheet"    href="index.css">
    </head>

    <body>    

    <!-- REPLACE Point - Header -->
        <div class="Header">
        	<!-- INSERT Point - responsive -->
        	<h2>PH Header</h2>
        </div>
    <!-- END REPLACE Point - Header -->

    <!-- REPLACE Point - Section1 -->
        <div class="Section1">
           <h2>PH Section 1</h2>
        </div>
    <!-- END REPLACE Point - Section1 -->

    <!-- REPLACE Point - Section2 -->        
        <div class="Section2">
            <h2>PH Section 2</h2>
        </div>        
    <!-- END REPLACE Point - Section2 -->

    <!-- REPLACE Point - Footer -->
        <div class="Footer">
            <h2>PH Footer</h2>
        </div>
    <!-- END REPLACE Point - Footer -->

    </body>

</html>
```
<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicHTMLImage.jpg">

From VSCode, right click on the file "index.<b>html</b>" and click on:
<br><span class="pic-text">&nbsp;Open In Live Server&nbsp;</span>

<img class="no-border" src="FRApps/assets/images/md-images/BasicBlocksImage1.jpg">
<br><br>
If your Chrome <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> browser is not already open, this command will open it and show the results of the above html code. 
<br><br>
<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="basic-image" src="FRApps/assets/images/md-images/BasicBlocksImage2a.jpg">
<br><br>

<div class="success">
<span style="font-size: 20px"><b>This is our starting point.</b></span>
<br>Let's move to the CSS code to add our blocks.
</div>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/index.css.jpg">

#### c. CSS Basic Code  

<br>
<img style=border:none; class="no-border" src="FRApps/assets/images/md-images/BasicCSSEmpty.jpg">

<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyCSS.gif">&nbsp;the entire code below to Line 1 of the empty index.<b>css</b> file (as shown above): </span>

```css
/* Basic Blocks Custom App */
@import url('https://fonts.googleapis.com/css?family=EB+Garamond');
@import url('https://fonts.googleapis.com/css2?family=Frank+Ruhl+Libre');
@import url('https://fonts.googleapis.com/css2?family=Roboto+Slab:wght@900&display=swap');

/*=======================================*/
/* root REPLACE Point - :root */
/*-----------------------------------------
:root selector for variables
-------------------------------------------*/
:root {
    --Body_background-color: #E5E4E2; /*platinum*/
   
    --Header_background-color: red;
    --Header_hover-color: white;
    --HeaderLogo-image: "";
    --HeaderLogo_margin: 35px 0 0 0px;
    --HeaderLogo-FontFamily: "Roboto Slab";
    --HeaderList-font-size: 1.2rem;
  
    --Section1_background-color: blue;
    --Section1_background-image: url( 'assets/images/monaco-blue-soft.jpg' );
  
    --Section2_background-color: lightgray;
    --Section2Paragraph-font-color: #ff7034;  /* dark orange */
  
    --Footer_background-color:green;
    --Footer_hover-color: white;
    --FooterList-font-size: .9rem;  
    
    --GlobalFontFamily: "Frank Ruhl Libre", "EB Garamond";

    --Button_Logo_font-color: whitesmoke;
} 
/* END REPLACE :root =====================*/


/*=======================================*/
/* HTML REPLACE Point */
/*-----------------------------------------
The <html> tag properites (unchanged)
------------------------------------------*/
html {
    background: var(--Body_background-color);
    height: 100%;
    text-align: center;
}
/* END HTML ============================*/


/*-----------------------------------------
The body properites
------------------------------------------*/
body {
    background: var(--Body_background-color);
    height: 100%;
    width: 100%;
    margin: 0;
    font-family: var(--GlobalFontFamily);
}

/*-----------------------------------------
The <h2> tag properties
-------------------------------------------*/
h2 {
    margin: 0;
    font-size: 1.5rem;
    color: white;
    padding: 1.5rem;
    text-align: center;
}

/*=======================================*/
/* HR-1 REPLACE Point - .Header */
/*-----------------------------------------
The .Header properites
------------------------------------------*/
.Header {
    background: var(--Header_background-color);
    width: 300px;
    height: 100px;
    position: relative;  /*was relative*/
}
/* END HR-1 .Header =====================*/


/*===========================================*/
/* H-1 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* H-1 INSERT Point - .HeaderNavBars */

/*     INSERT Point - .HeaderNavBars:focus */
/* H-1 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/


/*===========================================*/
/* H-2 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* H-2 INSERT Point - .HeaderLogo */

/*     INSERT Point - .HeaderLogo a */

/*     INSERT Point - .HeaderSpacer */
/* H-2 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/


/*===========================================*/
/* H-3 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* H-3 INSERT Point - .HeaderNavList */

/*     INSERT Point - .HeaderNavListItem a */

/*     INSERT Point  - .HeaderNavListItem a:hover
                       .HeaderNavListItem a:active */
/* H-3 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/


/*=======================================*/
/* H-4 INSERT Point - .HeaderNavListItemCTA a */
/*----------------------------------------
The .HeaderNavListItemCTA a properties
-----------------------------------------*/
/* END H-4 .HeaderNavListItemCTA a ======*/


/*===========================================*/
/* H-5 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* H-5 INSERT Point - .HeaderNavListItemCTA */

/* INSERT Point - @keyframes wiggle */
/* H-5 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/


/*=======================================*/
/* S1R-1 REPLACE Point - Section1 */
/*-----------------------------------------
The .Section1 properites
------------------------------------------*/
.Section1 {
    background: var(--Section1_background-color);
    width: 300px;
    height: 100px;
    position: relative;
}
/* END S1R-1 .Section1 =====================*/


/*===========================================*/
/* S1-1 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* S1-1 INSERT Point - .Section1ImageText */

/*      INSERT Point - .Section1ImageText::first-letter */
/* S1-1 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/


/*=======================================*/
/* S2R-1 REPLACE Point - Section2 */
/*-----------------------------------------
The .Section2 properites
------------------------------------------*/
.Section2 {
    background: var(--Section2_background-color);
    width: 300px;
    height: 100px;
    position: relative;
    color: black;
    font-family: var(--GlobalFontFamily);
    font-size: 1.2rem;
    font-weight: 600;
}
/* END S2R-1 .Section2 =====================*/


/*=======================================*/
/* S2-1 INSERT Point - Section2 h2 */
/*      DELETE Point - Section2 h2 */
/*-----------------------------------------
The .Section2 h2 properites
------------------------------------------*/
.Section2 h2 {
    padding: 1.5;
    color: black;
}
/* END S2-1 .Section2 h2==================*/


/*===========================================*/
/* S2-2 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* S2-2 INSERT Point - Section2Paragraph */

/*      INSERT Point - Section2Paragraph::first-letter/line */
/* S2-2 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/


/*=======================================*/
/* FR-1 REPLACE Point - Footer */
/*-----------------------------------------
.Footer properites
------------------------------------------*/
.Footer {
    background: var(--Footer_background-color);
    width: 300px;
    height: 100px;
    position: relative;
}
/* END FR-1 .Footer =====================*/


/*=============================================*/
/* F-1 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* F-1 INSERT Point - .FooterNavList */

/*     INSERT Point - .FooterNavListItem a */

/*     INSERT Point - .FooterNavListItem a:hover
                      .FooterNavListItem a:active */
/* F-1 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/


/*===========================================*/
/* R-1 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* Responsive Code */  
/* R-1 INSERT Point - @media (responsive min-width)*/                

/*     @media (responsive max-width)*/ 
/* R-1 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/

/* END CSS */

```

___

#### d. Basic Blocks Web Page      
<br>
Please check your <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome browser. 
<br>
<img class="basic-image" src="FRApps/assets/images/md-images/BasicBlocksImage3a.jpg"><br><br>

<div class="success">
<span style="font-size: 20px"><b>CONGRATULATIONS!!</b>
<br>
</span> You have just created a simple html page with a cascading style sheet (CSS) which makes <b><u>4 basic blocks</u></b>.<br><br>  
 We will build from this basic page to create a web site with a fixed header and footer, links with a "wiggle" button, and an image with a text overlay--in our customize section.<br><br>
From there, the next course we will move on to add some magic with JavaScript (JS) to this web page.
</div>

_____

<details class="details-style">
    <summary class="summary-style">
        More Info: Understanding CSS
    </summary>
<div class="popup">  
To understand a <u><i>little</i></u> of this CSS code, let's look at the .Header class properties.
<br><br>
/&ast;------------------------------------------------<br>
&nbsp;&nbsp;The .Header properites<br>
--------------------------------------------------&ast;/<br>
.Header {
<div class="list-text">
<ul>
<li>background: var(--Header_background-color);<br>
        &nbsp;&nbsp;&nbsp;&nbsp;<span style=color:red;>** Sets the background to the variable set above in the :root</span><br><br></li>
<li>width: 300px;<br>
        &nbsp;&nbsp;&nbsp;&nbsp;<span style=color:red;>** Sets the width of the header block 300 pixels</span><br><br>
<li>height: 100px;<br>
        &nbsp;&nbsp;&nbsp;&nbsp;<span style=color:red;>** Sets the height of the header block 100 pixels</span><br><br>
<li>position: relative;<br>
        &nbsp;&nbsp;&nbsp;&nbsp;<span style=color:red;>** Places the header box relative to the html code reading from the top to the bottom (DOM)</span></li><br><br>        
</ul>
</div>
</div>    
</details>

____

### 2. Modify to Large Blocks  

- Next, we will add to your existing code in the index.<b>css</b> file to continue building on our basic web page.  We will fill the web page up with our 4 blocks; one block on top of the next block.  They will be "Large Blocks."
<br><br>
<img style=border:none; class="no-border" src="FRApps/assets/images/md-images/index.css.jpg">

#### a. HTML

- In the <font color='green'>HTML</font>  section we will ADD the following:<br>

    + <b><font color=#A81966>max-width</font></b> to 1000px;   
    + <b><font color=#A81966>margin</font></b> to auto; 

<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyCSS.gif">&nbsp;<font color='green' style=font-weight:normal;>HTML</font> code below... </span>

```css
/*=====================================*/
/* HTML REPLACE Point */
/*---------------------------------------
The <html> tag properites (unchanged)
----------------------------------------*/
html {
    background: var(--Body_background-color);
    height: 100%;
    text-align: center;
    max-width: 1000px;
    margin: auto;
}
/* END HTML ===========================*/
```
<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<div class="multiple-equals-text">
/*=======================================*/<br>
/* HTML REPLACE Point */
<br><br>
 /* END HTML =======================*/<br> 
</div>
comments in your index.<b>css</b> file:
</div>
<br>
Replace the entire block with new code, like this.

<img class="no-border" src="FRApps/assets/images/md-images/BasicLargeBlocksHTMLImage.jpg"><br>

#### b. .Header

- In the <font color='green'>.Header</font> class section we will MODIFY the following:<br>

    + <b><font color=#A81966>width</font></b>: 100%; 
    + <b><font color=#A81966>height</font></b>: 80px;<br><br>

- and ADD: <br>

    + <b><font color=#A81966>position</font></b>: fixed; 
    + <b><font color=#A81966>z-index</font></b>: 100;
    + <b><font color=#A81966>max-width</font></b> to 1000px;  
    + <b><font color=#A81966>margin</font></b> to auto;

<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyCSS.gif">&nbsp;<font color='green' style=font-weight:normal;>.Header</font> code below... </span>

```css
/*=======================================*/
/* HR-1 REPLACE Point - .Header */
/*-----------------------------------------
The .Header properites
------------------------------------------*/
.Header {
    background: var(--Header_background-color);
    width: 100%; /*was 300px*/
    height: 80px;
    position: fixed;
    z-index: 100;
    max-width: 1000px;
    margin: auto;
}
/* END HR-1 .Header =====================*/
```
<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<div class="multiple-equals-text">
/*=======================================*/<br>
/* HR-1 REPLACE Point - .Header */
<br><br>
 /* END HR-1 .Header =======================*/<br> 
</div>
comments in your index.<b>css</b> file:
</div>
<br>
Like this, using the ctrl-v keys to paste the copied code.

<img class="no-border" src="FRApps/assets/images/md-images/BasicCopyPasteCSS_2.gif">

Replace the entire block with new code, like this.

<img class="no-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage4a.jpg"><br>

<div class="callout-note">
(for <b>css</b> files):<br><br>
This is the copy/paste method we will use throughout this exercise in the <b><u> index.css</u></b> file.<br><br>
The entire block will be replaced.
</div>

<br>
Check out your live server on <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome and see the difference the above .Header code made. OOPs, we seemed to have lost Section 1.  Have no fear we will bring it back shortly with more CSS.

<img class="no-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage4f.jpg">

___

#### c. .Section 1 & 2

- In <font color='green'>Section1</font> <b>AND</b> <font color='green'>Section2</font>, CHANGE
    + <b><font color=#A81966>width</font></b> to 100%  
    + <b><font color=#A81966>height</font></b> to 46%<br>
- and ADD:
    + <b><font color=#A81966>top</font></b> to 80px

<font color='green'><u>Section1</u></font>

<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyCSS.gif">&nbsp;<font color='green' style=font-weight:normal;>.Section1</font> code below... </span>

```css
/*=======================================*/
/* S1R-1 REPLACE Point - Section1 */
/*-----------------------------------------
The .Section1 properites
------------------------------------ ------*/
.Section1 {
    background: var(--Section1_background-color);
    width: 100%; /*was 300px*/
    height: 46%; /*was 100px*/
    position: relative;
    top: 80px; /*<---ADD to adjust the top position*/
}
/* END S1R-1 .Section1 =====================*/
```

Like this&nbsp;</span>
<br>
<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<div class="multiple-equals-text">
/*=======================================*/<br>
/* S1R-1 REPLACE Point - Section1 */
<br><br>
 /* END S1R-1 .Header =======================*/<br> 
</div>
comments in your index.<b>css</b> file:
</div>
<br>
<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage4b.jpg">
<br><br>
Follow your progress in <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome. No worries, those blocks will be put in their place soon, with CSS magic.

<img class="no-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage4f1.jpg">

____

<font color='green'><u>.Section2</u></font>

<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyCSS.gif">&nbsp;<font color='green' style=font-weight:normal;>.Section2</font> code below... </span>

```css
/*=======================================*/
/* S2R-1 REPLACE Point - Section2 */
/*-----------------------------------------
The .Section2 properites
------------------------------------------*/
.Section2 {
    background: var(--Section2_background-color);
    width: 100%;
    height: 46%;
    position: relative;
    color: black;
    font-family: var(--GlobalFontFamily);
    font-size: 1.2rem;
    font-weight: 600;
    top: 80px; /*<---ADD to adjust the top position*/
}
/* END S2R-1 .Section2 =====================*/
```


<br>
<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<div class="multiple-equals-text">
/*=======================================*/<br>
/* S2R-1 REPLACE Point - Section2 */
<br><br>
 /* END S2R-1 .Header =======================*/<br> 
</div>
comments in your index.<b>css</b> file:
</div>
<br>
<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>

<img class="no-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage4c.jpg">
<br><br>
Back to <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome.  Promise, that Footer will be next for proper placement.

<img class="no-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage4f2.jpg">

___

#### d. .Footer

- In <font color='green'>.Footer</font>, section we will CHANGE
    + <b><font color=#A81966>width</font></b> to 100%  
- REMOVE:
    + <b><font color=#A81966>top</font></b> in place of the bottom property
- and ADD:
    + <b><font color=#A81966>bottom</font></b> to 0
    + <b><font color=#A81966>position</font></b> to fixed  
    + <b><font color=#A81966>z-index</font></b> to 99  
    + <b><font color=#A81966>max-width</font></b> to 1000px   
    + <b><font color=#A81966>margin</font></b> to auto

<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyCSS.gif">&nbsp;<font color='green' style=font-weight:normal;>.Footer</font> code below... </span>

```css
/*=======================================*/
/* FR-1 REPLACE Point - Footer */
/*-----------------------------------------
The .Footer properites
------------------------------------------*/
.Footer {
    background: var(--Footer_background-color);
    width: 100%; 
    /*top: 80px;  Removed in place of the bottom property*/
    bottom: 0;
    position: fixed;
    z-index: 99;
    max-width: 1000px;
    margin: auto;
  } 
/* END FR-1 .Footer =====================*/
```
<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<div class="multiple-equals-text">
/*=======================================*/<br>
/* FR-1 REPLACE Point - .Footer */
<br><br>
 /* END FR-1 .Header =======================*/<br> 
</div>
comments in your index.<b>css</b> file:
</div>
<br>
<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage4d.jpg">


#### Large Blocks Web Page       <!-- .(20615.01.1 RAM This seems a little out of place --> 
<br>
Please check your <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome browser to see your web page so far.  Be sure to scroll up and down to see how we fixed both the Header and Footer in place.

<img class="no-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage5a.jpg">
<br><br>
<div class="success">
<span style="font-size: 20px"><b>CONGRATULATIONS!</b></span><br> You have built a full page with four distinct blocks using your Basic Blocks index.<b>css</b> code. We also secured (fixed) the header & footer in one spot.   
</div>

----

<details class="details-style">
    <summary class="summary-style">
        More Info: Max-Width
    </summary>
    <div class="popup">
    When you build a web site you want it to look good on any size screen. Especially on a full screen of a desktop or laptop. We added a couple properties in the index.css file that helps with this.
    <ul>
    <li>max-width: 1000px;</li>
    <li>margin: auto;</li>
    </ul>
    You will see this in 3 places:
    <ol>
    <li>html</li>
    <li>.Header</li>
    <li>.Footer</li>
    </ol>
<img class="no-border" src="FRApps/assets/images/md-images/BasicFullScreenCSSImage.jpg" style=border:none;>  <br><br> 
    Once this is done, the web site will look like this at full screen:
<img class="no-border" src="FRApps/assets/images/md-images/BasicFullScreenImage.jpg" style=border:none;>

Maximize your web site screen to see how this looks.  Return to your "working" screens to proceed.<br>
    </div>
    <br>
</details>


----
### 3. Modify Header 
<br>
<div class="callout-tip">
From our original sketch:
<img class="no-border" src="FRApps/assets/images/md-images/BasicSketchHeaderImage1a.jpg" style=border:none;>
<br>
We will add links (NavList) to the right and a font-based logo to the left.
<br>
</div>

<br>
We will add to your existing code in  both index.<b>html</b> AND index.<b>css</b> files to continue building on our basic web page.  In this section we will be "prettying up" the Navigation Bar on the right side of the Header.  Let's go...

<br>
<img style=border:none; class="no-border" src="FRApps/assets/images/md-images/index.html.jpg">

#### a. Header class
<br>
In the <font color='green'>Header</font> class section, we will replace the code.

<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyHTML.gif">&nbsp;<font color='green' style=font-weight:normal;>Header</font> code below... </span>

```html
    <!-- REPLACE Point - Header -->
        <div class="Header">
            <!-- INSERT Point - responsive -->
            <div class="HeaderLogo"><a href="/">PH Logo</a></div>
            <div class="HeaderSpacer"></div> 
            <ul class="HeaderNavList">
                <li class="HeaderNavListItem"><a href=#>PH_Link1</a></li>
                <li class="HeaderNavListItem"><a href=#>PH_Link2</a></li>
                <li class="HeaderNavListItem"><a href=#>PH_Link3</a></li>
                <li class="HeaderNavListItemCTA"><a href=#>PH_CTA</a></li>
            </ul>
        </div>
    <!-- END REPLACE Point - Header -->
```
<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<div class="replace-point-text">
&lt;!&dash;&dash; REPLACE Point - Header &dash;&dash;&gt; <br>
<br>
 &lt;!&dash;&dash; END REPLACE Point - Header &dash;&dash;&gt<br> 
</div>
comments in your index.<b>html</b> file:
</div>
<br>
<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicCopyPasteHTML.gif">
<br><br>
<div class="callout-tip"><br>
<img class="no-border" width=10% style=border:none; src="FRApps/assets/images/md-images/tabButton.jpg"><br>
Afterwards, you will most likely have to tab your lines over to properly align to other code.  Like this<br>
<img class="no-border" width=100% style=border:none; src="FRApps/assets/images/md-images/BasicTAB.gif">
</div>

<br>
Your work should look like this.

<img class="no-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage1.jpg">
<br><br>

<div class="callout-note">
 (for <b>html</b> files):<br><br>
This is the copy/paste method we will use throughout this exercise in the <b><u>index.html</u></b> file.<br><br>
The entire block will be replaced.
</div>
<br>
Take a quick look at <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome and the Header.  

<img class="no-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage1a.jpg">
<br><br>

<div class="callout-tip">
We are using names like "PH_Link1" and "PH Logo" as<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style=font-size:28px;><u><b>P</b></u>lace <u><b>H</b></u>olders</span><br>
for the final customization of our Web page.
</div>
<br><br>
Now we move to the index.css file.<br><br>


<img style=border:none; class="no-border" src="FRApps/assets/images/md-images/index.css.jpg">


#### b. .Header
<br>
First and foremost in the <font color='green'>.Header</font> section we will ADD the following:
 <ul>
    <li><font color=#A81966>display</font>: flex;</li> 
    <li><font color=#A81966>justify-content</font>: space-between;</li>
    <li><font color=#A81966>align-items: center;</font>: space-between;</li>
</ul>
<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyCSS.gif">&nbsp;<font color='green' style=font-weight:normal;>.Header</font> code below... </span> 

```css
/*=======================================*/
/* HR-1 REPLACE Point - .Header */
/*-----------------------------------------
The .Header properites
------------------------------------------*/
.Header {
    background: var(--Header_background-color);
    width: 100%;
    height: 80px;
    position: fixed;  /*was relative*/
    z-index: 100;
    max-width: 1000px;
    margin: auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
/* END HR-1 .Header =====================*/
```
<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<div class="multiple-equals-text">
/*=======================================*/<br>
/* HR-1 REPLACE Point - .Header */
<br><br>
 /* END HR-1 .Header =======================*/<br> 
</div>
comments in your index.<b>css</b> file:
</div>
<br>

<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage1b.jpg"><br>
Look at your <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome browser! 
<br>
We still need to:
<ol>
<li>Fix the "PH Logo" in the left corner of the header</li>
<li>Fix the links in the right corner of the header</li>
</ol>

<img class="no-border" style=border:none; src="FRApps/assets/images/md-images/BasicFixedHeaderImage3.jpg">


#### c. .HeaderLogo (PH Logo)
<br>
Now, let's fix that ugly "PH Logo" on the left side of the header. To do this, we add a new class to our CSS file.
<br><br>
We will be INSERTING 3 new classes as a BLOCK of code:
<ul>
    <li><font color='green'>.HeaderLogo</font></li>
    <li><font color='green'>.HeaderLogo a</font></li>
    <li><font color='green'>.HeaderSpacer</font></li>
</ul>
This will be the first time pasting into a large block of classes, in the index.css file (CSS Multiple Classes [2 or more]).<br><br>
Please follow the instructions closely.  We have created another small movie to demonstrate.

<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyCSS.gif">&nbsp;<font color='green' style=font-weight:normal;>.HeaderLogo</font> code below... </span>

```css
/*===============================================*/
/* H-2 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/*=======================================*/
/* H2 INSERT Point - .HeaderLogo */
/*-----------------------------------------
The .HeaderLogo properites
------------------------------------------*/
.HeaderLogo {
    margin-left: 45px;
    padding-left: 25px;
}

/*=======================================*/
/* INSERT Point - .HeaderLogo a */
/*-----------------------------------------
The .HeaderLogo a properites
------------------------------------------*/
.HeaderLogo a {
    text-decoration: none;
    font-size: 1.5rem;
    font-family: var(--HeaderLogo-FontFamily);
    font-weight: 600;    
    color: var(--Button_Logo_font-color);
    background: blue ;
    padding: 0.5rem .5rem;
    border-radius: 8px;
    box-shadow: 4px 4px black;
}

/*=======================================*/
/* INSERT Point - .HeaderSpacer */
/*-----------------------------------------
The .HeaderSpacer properites
------------------------------------------*/
.HeaderSpacer {
    flex: 1;
}
/* H-2 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
```

<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<div class="replace-point-text">
/&ast;===================================&ast;/<br>
/* H-2 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
<br><br>
/* H-2 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/<br> 
</div>
comments in your index.<b>css</b> file:
</div>
<br>
<span class="like-this-text">Like this</span>, using the ctrl-v keys to paste the copied code.

<img class="no-border" src="FRApps/assets/images/md-images/BasicCopyPasteBlock.gif">


<br>
Replace the entire block with new code, like this.

<img class="no-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage0d.jpg"><br>

<div class="callout-note">
 (for large blocks in the css file):<br><br>
This is the copy/paste method we will use throughout this exercise in the <b><u>index.css</u></b> file, for large blocks of code entailing 2 or more classes.<br><br>
The entire block will be replaced. From START BLOCK to END BLOCK.</div>
<br>
Now check <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome
<br>

<img class="no-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage5.jpg">

___

<details class="details-style">
    <summary class="summary-style">
        More Info: Google Fonts
    </summary>
We changed the "PH Logo" into a nice "font-based" logo.<br><br>
Note the font is one of Google's special fonts, called "EB Garamond."
<br><br>
We linked to that from the very top of the index.<b>css</b> file...
<br><br>
@import url('https://fonts.googleapis.com/css?family=EB Garamond');
<br><br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage6b.jpg">
<br><br>
... and we also linked to it from the very top of the index.<b>html</b> file.
<br><br>
&lt; link rel="stylesheet" href="https://fonts.googleapis.com/css?family=EB Garamond" &gt;

<img class="no-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage6a.jpg">
<br><br>
This PH Logo is for the *LAYOUT*.  We will replace this with a formR logo image in the *CUSTOMIZATION* section.<br><br>
</details>

____

#### d. .HeaderNavList - BLOCK
<br>
Now, let's focus on the stack of links on the right side of the header.  
<br><br>
We will be INSERTING 3 new classes as a BLOCK of code:
<ul>
    <li><font color='green'>.HeaderNavList</font></li><br>
    <li><font color='green'>.HeaderNavListItem a</font></li><br>
    </li><font color='green'>.HeaderNavListItem a:hover</font></li>
    <li><font color='green'>.HeaderNavListItem a:active</font></li>
</ul>
<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyCSS.gif">&nbsp;<font color='green' style=font-weight:normal;>.HeaderNavList</font> code below... </span>

```css
/*==============================================*/
/* H-3 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/*========================================*/
/* H-3 INSERT Point - .HeaderNavList */
/*-----------------------------------------
The .HeaderNavList (horizontal menu) properites
------------------------------------------*/
.HeaderNavList {
    list-style: none;
    margin-right: 30px;
    padding: 0;
    display: flex;
    flex-direction: row;
    align-items: center;
    font-size: var(--HeaderList_font-size);
}

/* INSERT Point .HeaderNavListItem a */
/*-----------------------------------------
The .HeaderNavListItem a properites
------------------------------------------*/
.HeaderNavListItem a {
    color: black;
    font-weight: bold;
    text-decoration: none;
    margin: 8px 0;
    padding: 25px;
}

/* INSERT Point .HeaderNavListItem a:hover
                .HeaderNavListItem a:active */
/*-----------------------------------------
The .HeaderNavListItem a properites
------------------------------------------*/
.HeaderNavListItem a:hover,
.HeaderNavListItem a:active {
    color: var(--Header_hover-color);
}
/* H-3 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/

```

<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<font color='green'>
/&ast;=======================================&ast;/<br>
/* H-3 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
<br><br>
/* H-3 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/<br> 
</font>
comments in your index.<b>css</b> file:
</div>
<br>
<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage0g.jpg">
<br><br>
Go back to <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome and see the results. Notice that the 3 links on the right will change to a light gray (#ccc) when you mouse over them. They are also aligned horizontally for our *LAYOUT*.
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage8.jpg">

____

<details class="details-style">
    <summary class="summary-style">
        More Info: FLEX
    </summary>
        <div class="popup">
        One of the more powerful CSS properties is "FLEX."  We used it above to place the stacked links horizontally; in the Header and later in the Footer. Like this:<br><br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicConceptColumnToRow.jpg" style=border:none><br><br>  
        Below is a short discussion on the basics of FLEX.<br>   
        <h3>Basic concepts of flexbox</h3><br>
        The Flexible Box Module, usually referred to as flexbox, was designed as a one-dimensional layout model, and as a method that could offer space distribution between items in an interface and powerful alignment capabilities. This article gives an outline of the main features of flexbox.<br><br>
        When we describe flexbox as being one dimensional we are describing the fact that flexbox deals with layout in one dimension at a time — either as a row or as a column.<br>
        <h3>The two axes of flexbox</h3><br>
        When working with flexbox you need to think in terms of two axes — the main axis and the cross axis. The main axis is defined by the flex-direction property, and the cross axis runs perpendicular to it. Everything we do with flexbox refers back to these axes.  Here we will discuss the Main Axis.<br>
        <h3>The Main Axis</h3><br>
        The main axis is defined by flex-direction, which has four possible values:<br>
            - row<br>
            - row-reverse<br>
            - column<br>
            - column-reverse<br><br>
        Should you choose row or row-reverse, your main axis will run along the row in the inline direction.
<img class="no-border" src="FRApps/assets/images/md-images/BasicConceptsFlexRow.jpg"><br><br>
        Choose column or column-reverse and your main axis will run from the top of the page to the bottom — in the block direction.
<img class="no-border" src="FRApps/assets/images/md-images/BasicConceptFlexColumn.jpg"><br><br>
<a href='https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox' target='_blank' title='Citation for Flex (MDN WEB DOCS)'>Citation</a>
        </div>
        <br>
</details>

____

#### e. CTA button
<br>
<div class="callout-tip">
CTA stands for Call to Action
</div>
<br>
Now, let's do something about that "PH CTA" link. Using CSS, we can turn it into a nice blue button.

 <span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyCSS.gif">&nbsp;<font color='green' style=font-weight:normal;>.HeaderNavListItemCTA </font> code below... </span>


```css
/*=======================================*/
/* H-4 INSERT Point - .HeaderNavListItemCTA a */
/*-----------------------------------------
The .HeaderNavListItemCTA a properties
------------------------------------------*/
.HeaderNavListItemCTA a {
    color: var(--Button_Logo_font-color);
    background: blue ;
    padding: 0.5rem 1rem;
    border-radius: 8px;
    text-decoration: none;
    font-family: var(--GlobalFontFamily);
    font-weight: 600;
}
/* END H-4 .HeaderNavListItemCTA a ======*/
```
<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<div class="multiple-equals-text">
/*=======================================*/<br>
/* H-4 INSERT Point - .HeaderNavListItemCTA a */
<br><br>
/* END H-4 .HeaderNavListItemCTA a ==========*/<br>
</div>
comments in your index.<b>css</b> file:
</div>
<br>
<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage0j.jpg">

Again, go see it in your <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome browser.  
<img class="no-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage10.jpg">


You have completed this part of modifying the Header.  Later, we will add an image for a logo instead of the PH logo. <br>

AND, add some code to make the <img class="wiggle-me" src="FRApps/assets/images/md-images/WiggleButtonPH-CTA.jpg"> button wiggle!

___


#### Modified Header Web Page       <!-- .(20615.01.1 RAM This seems a little out of place --> 
<br>

Please check your <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome browser to see your web page thus far.

<img class="no-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage12.jpg">
<br><br>
<div class="success">
<span style="font-size: 20px"><b>CONGRATULATIONS!</b></span><br> You have just added to your Basic Blocks code which built a full web page with a fixed header along with links, a "CTA" button, and a font-based logo. In the next section, we will add/modify code that will add links to the footer.   
</div>

----
### 4. Modify Footer 
<br>
<div class="callout-tip">
From the original sketch:
<img class="no-border" src="FRApps/assets/images/md-images/BasicSketchFooterImage.jpg">
<br>
We will add links (NavList) to the center.
</div>

<br>
Next, we will add to your existing code in both the index.<b>html</b> AND index.<b>css</b> files to continue building on our basic web page *LAYOUT*. 
<br><br>
We will add some links to the Footer and fix the position of the Footer as we did with the Header.


<img style=border:none; class="no-border" src="FRApps/assets/images/md-images/index.html.jpg">


#### a. <font color='green'>Footer</font> class
<br>
<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyHTML.gif">&nbsp;<font color='green' style=font-weight:normal;>Footer</font> code below... </span>

```html
<!-- REPLACE Point - Footer -->
    <div class="Footer">
        <ul class="FooterNavList">
            <li class="FooterNavListItem"><a href=#>PH Link1</a></li>
            <li class="FooterNavListItem"><a href=#>PH Link2</a></li>
        </ul>
    </div>
    <!-- END REPLACE Point - Footer -->
```
<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<div class="replace-point-text">
&lt;!&dash;&dash; REPLACE Point - Footer &dash;&dash;&gt; <br>
<br>
&lt;!&dash;&dash; END REPLACE Point - Footer &dash;&dash;&gt<br> 
</div>
comments in your index.<b>html</b> file:
</div>
<br>

<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage1.jpg">
<br><br>

Let's take a quick look at <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome.

<img class="no-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage1a.jpg">

<br>
Good job! Now we move to the index<b>.css</b> file.


<img style=border:none; class="no-border" src="FRApps/assets/images/md-images/index.css.jpg">


#### b. .FooterNavList - BLOCK

- Now, let's focus on the links on the left side of the header.  We will be INSERTING 3 new classes in one copy/paste block of code:

    + <font color='green'>.FooterNavList</font><br><br>
    + <font color='green'>.FooterNavListItem a</font><br><br>
    + <font color='green'>.FooterNavListItem a:hover</font><br>
    <font color='green'>.FooterNavListItem a:active</font>

<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyCSS.gif">&nbsp;<font color='green' style=font-weight:normal;>.FooterNavList</font> code below... </span>

```css
/*=============================================*/
/* F-1 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/*=======================================*/
/* F1 INSERT Point - .FooterNavList */
/*-----------------------------------------
The .FooterNavList properties
------------------------------------------*/
.FooterNavList {
    list-style: none;
    margin: 20px;
    padding: 0;
    display: flex;
    flex-direction: row;
    justify-content: center;
    font-size: var(--FooterList-font-size);
}

/*=======================================*/
/* INSERT Point - .FooterNavListItem a */
/*-----------------------------------------
The .FooterNavListItem a properties
------------------------------------------*/
.FooterNavListItem a {
    color: black;
    font-weight: bold;
    text-decoration: none;
    margin: 8px 0;
    padding: 12px;
}

/*=======================================*/
/* INSERT Point - .FooterNavListItem a:hover
                  .FooterNavListItem a:active */
/*-----------------------------------------
The .FooterNavListItem a:hover,
    .FooterNavListItem a:active properties
------------------------------------------*/
.FooterNavListItem a:hover,
.FooterNavListItem a:active {
  color: var(--Footer_hover-color);
}
/* F-1 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
```

<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<font color='green'>
/&ast;======================================&ast;/<br>
/* F-1 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
<br><br>
/* F-1 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/<br> 
</font>
comments in your index.<b>css</b> file:
</div>
<br>

<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage7a.jpg">
<br>
Again, go see it in your <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome browser. The links are nicely centered and horizontal, thanks to the CSS "flex" property. 
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage8.jpg">


#### Modified Footer Web Page       <!-- .(20615.01.1 RAM This seems a little out of place --> 
<br>

Please check your Chrome browser to see your web page thus far:

<img class="no-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage9.jpg">
<br><br>
<div class="success">
<span style="font-size: 20px"><b>CONGRATULATIONS!</b></span><br> You have just added to your Basic Blocks code which builds a full web page with links in the secured (fixed) footer. In the next section, we will add/modify code that will add a text overlay in Section1.   
</div>

____

### 5. Add Text

#### Add Text Overlay
<br>
<div class="callout-tip">
From Original Sketch:
<img class="no-border" src="FRApps/assets/images/md-images/BasicSketchSection1Image1.jpg">
<br>
We will add a Text Overlay to Section 1
</div>
<br>
Now, let's focus on the Text Overlay. It will be another <u>P</u>lace <u>H</u>older (PH Text Overlay).  This will require some modifications to your existing code in both the index.<b>html</b> AND index.<b>css</b> files.  
<br><br>
First, the index.<b>html</b> file.


<img style=border:none; class="no-border" src="FRApps/assets/images/md-images/index.html.jpg">


#### a. <font color='green'>Section1</font> class
<br>
<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyHTML.gif">&nbsp;<font color='green' style=font-weight:normal;>Section1</font> code below... </span>

```html
    <!-- REPLACE Point - Section1 -->
        <div class="Section1">
            <h2 class="Section1ImageText">PH Text Overlay</h2>
        </div>
    <!-- END REPLACE Point - Section1 -->
```

<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<div class="replace-point-text">
&lt;!&dash;&dash; REPLACE Point - Section1 &dash;&dash;&gt; <br>
<br>
&lt;!&dash;&dash; END REPLACE Point -Section1 &dash;&dash;&gt; <br> 
</div>
comments in your index.<b>html</b> file:
</div>
<br>

<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicWithImageImage1.jpg">
<br><br>
Notice. in <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome, the "PH Text Overlay" within the &#60;h2&#62; tags.  This will become our text overlay.
<br><br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicWithImageImage2.jpg">
<br>
Now, we move to the index.<b>css</b> file.


<img style=border:none; class="no-border" src="FRApps/assets/images/md-images/index.css.jpg">


#### b. .Section1ImageText

- We will be INSERTING 2 new classes in one copy/paste block of code:

    + <font color='green'>.Section1ImageText</font><br>
    + <font color='green'>.Section1ImageText::first-letter</font><br>

<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyCSS.gif">&nbsp;<font color='green' style=font-weight:normal;>.Section1ImageText</font> code below... </span>

```css
/*===========================================*/
/* S1-1 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/*=======================================*/
/* S1-1 INSERT Point - .Section1ImageText */
/*-----------------------------------------
The .Section1ImageText properties
------------------------------------------*/
.Section1ImageText {
    font-family: var(--GlobalFontFamily);
    font-size: 3rem;
    font-weight: 800;
    color: lightgray;
    text-shadow: 1px 1px 3px #000000;
    padding: 80px 350px 20px 0px;
}

/*=======================================*/
/* INSERT Point - .Section1ImageText::first-letter */
/*-----------------------------------------
The .Section1ImageText::first-letter properties
------------------------------------------*/
.Section1ImageText::first-letter {
    font-size: 150%;
    color: cornflowerblue;
}
/* S1-1 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
```
<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<font color='green'>
/&ast;======================================&ast;/<br>
/* S1-1 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
<br><br>
/* S1-1 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/<br> 
</font>
comments in your index.<b>css</b> file:
</div>
<br>
<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicWithImageImage5a.jpg">

___
#### c. Text Overlay
<br>
Check it out in <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome. <br> 
<img class="no-border" src="FRApps/assets/images/md-images/BasicLAYOUTImage1.jpg">

___

#### Add Text Paragraph
<br>

We will add a Text Paragraph to Section 2

<div class="callout-tip">
From the original sketch:
<img class="no-border" style=border:none; src="FRApps/assets/images/md-images/BasicSketchSection2Image.jpg">
<br>
We will add some text.
</div>
<br>Now, let's focus on the Text Paragraph. It will be another <u>P</u>lace <u>H</u>older.  This will require some modifications to your existing code in the index.<b>html</b> file.  

<img style=border:none; class="no-border" src="FRApps/assets/images/md-images/index.html.jpg">

<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyHTML.gif">&nbsp;<font color='green' style=font-weight:normal;>Section2</font> code below... </span>

```html
    <!-- REPLACE Point - Section2 -->        
        <div class="Section2">
            <h2></h2>
            <p class="Section2Paragraph">
                PH<br>
                The quick brown fox jumped over the lazy dog.<br>
                The quick brown fox jumped over the lazy dog.<br>
                The quick brown fox jumped over the lazy dog.<br>
                The quick brown fox jumped over the lazy dog.
            </p>  
        </div>
    <!-- END REPLACE Point - Section2 -->       
```

<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<div class="replace-point-text">
&lt;!&dash;&dash; REPLACE Point - Section2 &dash;&dash;&gt; <br>
<br>
&lt;!&dash;&dash; END REPLACE Point - Section2 &dash;&dash;&gt;<br> 
</div>
comments in your index.<b>html</b> file:
</div>
<br>

<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage6.jpg">
<br><br>

Check <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome.  This provides a paragraph text we can add some nice attributes later in the <i>Customization</i> section. 

<img class="no-border" src="FRApps/assets/images/md-images/BasicLAYOUTImage2.jpg">

___

### 6. Add "Wiggle" Button <!--<img class="wiggle-me" style="width:20%;" src="FRApps/assets/images/md-images/WiggleButtonPH-CTA.jpg">-->
<br>

<div class="callout-tip">
From the original sketch:<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicSketchWiggleImage.jpg"><br>
We eventually want this button in the NavList to be special.<br>
We will add some code to make it "wiggle."
</div>
<br>

<img style=border:none; class="no-border" src="FRApps/assets/images/md-images/index.css.jpg">


#### a. .HeaderNavListCTA & @keyframes wiggle

- With the use of only CSS code we can make the CTA button wiggle for a few seconds after the page opens or when it has been refreshed.  Again, we will use a Block of code containing 2 classes.

- We will be INSERTING these 2 new classes in one copy/paste block of code:

    + <font color='green'>.HeaderNavListCTA</font><br>
    + <font color='green'>@keyframes wiggle</font>


<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyCSS.gif">&nbsp;<font color='green' style=font-weight:normal;>.HeaderNavListCTA</font> code below... </span>

```css
/*===========================================*/
/* H-5 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* H-5 INSERT Point - .HeaderNavListItemCTA */
/*-----------------------------------------
The .HeaderNavListItemCTA properties
------------------------------------------*/
.HeaderNavListItemCTA {
  animation     : wiggle 400ms 2s 8 ease-out none;
  }

/*=======================================*/
/* INSERT Point - @keyframes wiggle */
/*-----------------------------------------
The @keyframes wiggle properties
------------------------------------------*/
@keyframes wiggle {
    0% { transform: rotateZ(  0deg ); }
   50% { transform: rotateZ(-10deg ); }
  100% { transform: rotateZ( 10deg ); }
}
/* H-5 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
```

<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<font color='green'>
/&ast;======================================&ast;/<br>
/* H-5 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
<br><br>
/* H-5 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/<br> 
</font>
comments in your index.<b>css</b> file:
</div>
<br>
<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>

<img class="no-border" src="FRApps/assets/images/md-images/BasicBonusImage5d.jpg">

___

#### b. Wiggle Button

- Now check out the "wiggle" when you refresh your page.  Note the CTA button will wiggle 8 times, 2 seconds after the refresh.  The <font color=#A81966><b>animation</b></font> property controls this motion. Remember, CTA stands for "Call To Action."  The wiggle certainly calls for the reader's attention.

<div class="callout-tip"><br>
<img class="no-border" style=border:none; src="FRApps/assets/images/md-images/refreshButtonGray.jpg"> You may have to refresh your screen to activate the wiggle button for the first time.
</div>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicWiggleImage1.jpg">

___

### 7. Make Responsive

- A very smart programmer once told me that you code your web page for a hand-held device first, the desk top second.

- This is probably the most important section.  Learn this and you will use these skills to become very accomplished in HTML and CSS. Go out and research "responsiveness."   

-  First let's look at our current web page on an iPhone7 Plus:

<img class="no-border" width=75% src="FRApps/assets/images/md-images/BasicResponsiveImage1.jpg">


We have 3 problems here.
<ul class="three-problems">
    <li>-The Menu list is too big to properly display</li>
    <li>-All font sizes are too large</li>
    <li>-The Logo is scrunched up</li>
</ul>
We will fix this using "responsive" code in our index.css file with the magic of a <font color='blue'>@media</font> query.

____

<details class="details-style">
    <summary class="summary-style">
        More Info: Developer's Tools
    </summary>
<div class="popup">    
Most all Internet browsers have a wonderful tool called "Developer Tools."
<br><br>
<p class="popup-tip"><br>
    To get to them, you can go to <img class="no-border" width=5% style=border:none; valign=bottom src="FRApps/assets/images/md-images/BasicSettingsButtons.jpg"> settings > More Tools > Developer Tools <br>
</p>
Like below:

<img class="no-border" src="FRApps/assets/images/md-images/BasicDevToolsImage1.jpg">
<br><br>
<p class="popup-tip"><br>
    Shortcut 1: Right-click anywhere on the screen and pick "Inspect."
    <br><br>
    Shortcut 2: On most browsers press F12 key.
</p>
<img class="no-border" src="FRApps/assets/images/md-images/BasicDevToolsImage1b.jpg">
<br><br>
<p class="popup-tip">
Example (above image): Click on the drop down and:<br>
    + (1) Select "iPhone IE"<br>
    + (2) Select the little <img src="FRApps/assets/images/md-images/BasicDevToolsIconImage.jpg"> icon <br>
    + (3) Select the "PH Logo" <br>
    + (4) See the information about this element. <br>
    Note the "padding: 0px 0pc 0px 54px;<br><br>
    *CSS padding property goes from (top, right, bottom, left)<br>
    We set only the left property to 54px* (below picture).
</p>
Go look in index.css for ".HeaderLogo."
<br>
We set the padding-left:&nbsp;25px; 
<br>
<img class="no-border" width=50% src="FRApps/assets/images/md-images/BasicDevToolsImage3.jpg">
</div>
<br>
</details>

____

#### a. NavBars 
<br>

<div class="callout-tip">
From the original sketch:
<img class="no-border" style=border:none; src="FRApps/assets/images/md-images/BasicSketchHeaderImage1b.jpg"><br>
We will add our NavBars (Hamburger)
</div>

<br>
Let's focus on the Header and how we want it to appear on a smart phone.

<img class="no-border" style=border:none; src="FRApps/assets/images/md-images/BasiciphoneImage1.jpg">

We can set, using CSS, a certain width of the "viewpoint" to where we can make changes to the appearence.  In our code we will set it at 760px.  At that width we can make the NavList (horizontal links) DISAPPEAR; and a NavBars (commonly known as a hamburger) APPEAR. And fix that scrunched up Logo.

First we need to add the NavBars (hamburger) in both index.html and index.css.

<img style=border:none; class="no-border" src="FRApps/assets/images/md-images/index.html.jpg">


#### b. HeaderNavBars Class
<br>
<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyHTML.gif">&nbsp;<font color='green' style=font-weight:normal;>Header</font> code below... </span>

```html
    <!-- REPLACE Point - Header -->
        <div class="Header">
            <!-- INSERT Point - responsive -->
            <div class="HeaderNavBars">
                <object data="assets/images/hamburger.svg?fill=white"
                        type="image/svg+xml" title="Toggle sidebar">
                </object>
            </div>
            <div class="HeaderLogo"><a href="/">PH Logo</a></div>
            <div class="HeaderSpacer"></div> 
            <ul class="HeaderNavList">
                <li class="HeaderNavListItem"><a href=#>PH_Link1</a></li>
                <li class="HeaderNavListItem"><a href=#>PH_Link2</a></li>
                <li class="HeaderNavListItem"><a href=#>PH_Link3</a></li>
                <li class="HeaderNavListItemCTA"><a href=#>PH_CTA</a></li>
            </ul>
        </div>
    <!-- END REPLACE Point - Header -->

``` 

<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<div class="replace-point-text">
&lt;!&dash;&dash; REPLACE Point - Header &dash;&dash;&gt; <br>
<br>
&lt;!&dash;&dash; END REPLACE Point - Header &dash;&dash;&gt;<br> 
</div>
comments in your index.<b>html</b> file:
</div>
<br>

<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicResponsiveImage2.jpg">
<br><br>
 Take a look at <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome.  We have successfully added our NavBars.
<br><br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicResponsiveImage3.jpg">
<br><br>
____

<details class="details-style">
<summary class="summary-style">More Info: Your Images</summary>
<div class="popup">
Note in your assets/images directory you have 3 different images.<br>
    &nbsp;&nbsp;&nbsp;&nbsp;+ formr-logo-blue.gif<br>
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(our logo image)<br>
    &nbsp;&nbsp;&nbsp;&nbsp;+ monaco-blue-soft.jpg<br> 
       &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;(an image we will use later in customization)<br>
    &nbsp;&nbsp;&nbsp;&nbsp;+ hamburger.svg<br>
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(the NavBars we are working with now)
<br><br>These images will be used in your code. The first 2 as variables in the :root section of the index.css file.  The last will be referenced directly in the Header section of the index.html file. 

<br>
<img class="no-border" width="30%" src="FRApps/assets/images/md-images/BasicResponsiveImage4.jpg">
</div>
</details>

____

Now let's move on to index.**css** to adjust the NavBars in a proper postion

<img style=border:none; class="no-border" src="FRApps/assets/images/md-images/index.css.jpg">


#### c. .HeaderNavBars

- We will be INSERTING 2 new classes in one copy/paste block of code:

    + <font color='green'>.HeaderNavBars</font><br>
    + <font color='green'>.HeaderNavBars:focus</font><br>

<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyCSS.gif">&nbsp;<font color='green' style=font-weight:normal;>.HeaderNavBars</font> code below... </span>

```css
/*===========================================*/
/* H-1 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* H-1 INSERT Point - .HeaderNavBars */
/*-----------------------------------------
The .HeaderNavBars (menu) properites
------------------------------------------*/
.HeaderNavBars {
  display: none;
  height: 24px;
  width: 24px;
  background: transparent;
  border: none;
  cursor: pointer;
  padding: 0px;
  box-sizing: border-box;
  margin-left: 20px;
  margin-top: 0px;
}

/*=======================================*/
/* INSERT Point - .HeaderNavBars:focus */
/*-----------------------------------------
The .HeaderNavBars:focus properites
------------------------------------------*/
.HeaderNavBars:focus {
    outline: none;
}
/* H-1 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
```

<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<font color='green'>
/&ast;======================================&ast;/<br>
/* H-1 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
<br><br>
/* H-1 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/<br> 
</font>
comments in your index.<b>css</b> file:
</div>

<br>

<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicResponsiveImage5.jpg">

Check it out in <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome.  
<img class="no-border" src="FRApps/assets/images/md-images/BasicResponsiveImage6.jpg">

<div class="callout-oops">
The hamburger is missing?  That is because we set its display to none in the CSS code we pasted in.  
<img class="no-border" src="FRApps/assets/images/md-images/BasicResponsiveImage6a.jpg"><br>
We will take care of this momentarily...
</div>

___

#### d. Responsive CSS Code
<br>

#### e. @media (max-width)

- Here is where the real magic happens.  With the use of <font color=cornflowerblue>@media</font> query we can test the width of the viewpoint of the screen your web page appears.  In our case we will make changes when the screen is at 760 pixels wide (typical tablet) AND 420 pixels wide (typical smart phone). 

- Again, we will use a Block of code containing the query.

- We will be INSERTING these new queries in one copy/paste block of code:

    + <font color='cornflowerblue'>@media</font> <font color=#A81966>(max-width)</font>

<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyCSS.gif">&nbsp;<font color='green' style=font-weight:normal;>/* Responsive Code */</font> code below... </span>

```css
/*===========================================*/
/* R-1 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* Responsive Code */  
/* R-1 INSERT Point - @media (max-width)*/ 
/*-----------------------------------------
The @media MAX-width (760px) query properties
=========================================*/
@media (max-width: 760px) {

    .HeaderLogo {
        font-size: 1.2rem;
        margin-left: 2px;
        background-size: 180px 51px;
    }
  
    .HeaderNavBars {
      display: flex;
    }
  
    .HeaderNavList {
        display: none;
    }
  
  .Section1ImageText {
        font-size: 2.5rem;
        padding: 80px 200px 20px 0px;
  }
  
    .Section2 h2 {
      font-size: 1.7rem;
    }
  
    .Section2Paragraph {
      font-size: 75%;
    }
  }

/*-----------------------------------------
The @media MAX-width (420px) query properties
=========================================*/
@media (max-width: 420px) {

    .HeaderLogo {
        font-size: .8rem;
        margin-left: 0px;
        margin-top: 0px;
        background-size: 144px 41px;
    }

    .Section1ImageText {
        font-size: 1.2rem;
        padding: 80px 100px 20px 10px;
      }
    
    .Section2Paragraph {
        font-size: 60%;
      }
}
  /* R-1 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
```
<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<font color='green'>
/&ast;======================================&ast;/<br>
/* R-1 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
<br><br>
/* R-1 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^/<br> 
</font>
comments in your index.<b>css</b> file:
</div>
<br>
<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicResponsiveImage7.jpg">

Check it out in <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome.

The image on the left is when the Chrome window is greater than 420 pixels wide, the one on the right is less than 420.  That is "responsiveness!"


<img class="no-border" style=border:none; src="FRApps/assets/images/md-images/BasicResponsiveDualScreenImage1.jpg">

Now, check it out on iPhone 7 Plus. Remember, this is our LAYOUT.  Later, we will see how our CUSTOM web page looks on the iPhone. 

<img class="no-border" width="75%" src="FRApps/assets/images/md-images/BasicResponsiveIPhoneImage2.jpg">

Compare the 2 (before and after RESPONSIVE queries)

<img class="no-border" style=border:none; src="FRApps/assets/images/md-images/BasicResponsiveIPhoneImage3.jpg">

### Final LAYOUT
<br>

<img class="no-border" src="FRApps/assets/images/md-images/BasicFinalLayoutGaramond.jpg">
<br><br>
<div class="success">
<span style="font-size: 20px"><b>CONGRATULATIONS!</b></span><br>You have completed your web page *LAYOUT* with a fixed header and footer, links, a CTA button, an image and a text overlay.  All Place Holders in their correct positions.  AND responsive to the width size of the screen it is displayed.  
<br><br>
You are now ready to *CUSTOMIZE*.  We will work together on our version of a formR web page.  Once complete, please go and *CUSTOMIZE* your own page with a different image, logo and links. 
</div>

###  [View Full Code For HTML / CSS Layout](/FRApps/code/fr020101_layout-code.md "Full Code")
<br>

<hr class="main-division">

### *CUSTOMIZATION*

- As previously mentioned, we will make some changes to our LAYOUT.<br>We will:
<div class="custom-list-text">    
    <ul>
        <li>Add an image (.jpg) file to Section 1</li>
        <li>Change the font-based “PH Logo” to our formR logo image (.gif) file</li>
        <li>Change all of the Place Holder (PH) text</li>
        <li>Change some colors</li>
    </ul>
</div>
- Let’s have some fun. This will require some modifications to your existing code in both the index.html AND index.css files.

___

### 1. Add Image to Section 1

- To add some pazzazz to your web site, we will include an image in Section 1.  This will require some modifications to your existing code in the index.<b>css</b> file.  

<img style=border:none; class="no-border" src="FRApps/assets/images/md-images/index.css.jpg">

#### a. .Section1
<br>
This is where there is a sizeable change to the .Section1 code below.

- CHANGE
    + <font color=#A81966>background</font>: to include a url<br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(this will come from the :root variables)
- ADD 
    + <font color=#A81966>background-color</font>: blue;<br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(this will come from the :root variables)
    + <font color=#A81966>background-repeat</font>: no-repeat; 
    + <font color=#A81966>background-size</font>: cover; 
    + <font color=#A81966>background-position</font>: center; 

<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyCSS.gif">&nbsp;<font color='green' style=font-weight:normal;>.Section1</font> code below... </span>

```css
/*=======================================*/
/* S1R-1 REPLACE Point - Section1 */
/*-----------------------------------------
The .Section1 properites
------------------------------------------*/
.Section1 {
    background: var(--Section1_background-image);
    background-color: var(--Section1_background-color);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
    width: 100%;
    height: 46%;
    position: relative;
    top: 80px;
}
/* END S1R-1 .Section1 =====================*/
```

<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<div class="multiple-equals-text">
/*=======================================*/<br>
/* S1R-1 REPLACE Point - .Section2 */
<br><br>
/* END S1R-1 .Section2 =====================*/<br> 
</div>
comments in your index.<b>css</b> file:
</div>
<br>
<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicWithImageImage3.jpg">
<br>

____

<details class="details-style">
    <summary class="summary-style">
        More Info: Variables
    </summary>
In the above .Section1 CSS code, there were 2 properties that named variables, which were created in the <b>[:root]</b> section at the top the file.<br><br>
The background: was set at<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"var(--Section1_background-color),"<br>
which is blue, as you can see in the [:root] for Section1 section.
<br><br>Also, the background: was set as a URL variable,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"var(--Section1_background-image)."<br>
In the <b>[:root]</b>, this variable was set as 'assets/images/monaco-blue-soft.jpg.'<br><br>Later in the <b><u>Customize</u></b> section, you will find this to be very powerful in changing areas of the web page.<br><br>
<img src="FRApps/assets/images/md-images/BasicWithImageImage3a.jpg">
<br><br>
</details>

____

#### Web Page With Image in Section 1
<br>
That's it! Check your <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome browser for the changes; a nice blue image with the font overlay.

<img class="no-border" src="FRApps/assets/images/md-images/BasicWithImageImage4.jpg">

____

### 2. Change To formR Logo
<br>
Now lets add an image in place of the "PH Logo" in the Header. In the "<span class="doc-dir-text">assets/images</span>" directory there is a file (formr-logo-blue.gif) that we will add to the left side of the Header.
<br>
<img width=25% src="FRApps/assets/images/md-images/formr-logo.gif">
<br>

- This will require a change in both the index.html and index.css files.

- First the index.html

<img style=border:none; class="no-border" src="FRApps/assets/images/md-images/index.html.jpg">


#### a. Header
<br> 
<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyHTML.gif">&nbsp;<font color='green' style=font-weight:normal;>Header</font> code below... </span>

```html
    <!-- REPLACE Point - Header -->
        <div class="Header">
            <!-- INSERT Point - responsive -->
            <div class="HeaderNavBars">
                <object data="assets/images/hamburger.svg?fill=white"
                        type="image/svg+xml" title="Toggle sidebar">
                </object>
            </div>
            <div class="HeaderLogo"><a href=""></a></div>
            <div class="HeaderSpacer"></div> 
            <ul class="HeaderNavList">
                <li class="HeaderNavListItem"><a href=#>PH_Link1</a></li>
                <li class="HeaderNavListItem"><a href=#>PH_Link2</a></li>
                <li class="HeaderNavListItem"><a href=#>PH_Link3</a></li>
                <li class="HeaderNavListItemCTA"><a href=#>PH_CTA</a></li>
            </ul>
        </div>
    <!-- END REPLACE Point - Header -->
```

<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<div class="replace-point-text">
&lt;!&dash;&dash; REPLACE Point - Header &dash;&dash;&gt; <br>
<br>
&lt;!&dash;&dash; END REPLACE Point - Header &dash;&dash;&gt;<br> 
</div>
comments in your index.<b>html</b> file:
</div>
<br>
<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicformRImage1.jpg">

> ...OR just follow along with the below video<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicHeaderPHLogoDelete.gif">

<br>

In <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome, we have made a mess of the logo.  Be patient, we will take care of this with CSS code.

<img class="no-border" src="FRApps/assets/images/md-images/BasicformRImage1a.jpg">
<br><br>

<img style=border:none; class="no-border" src="FRApps/assets/images/md-images/index.css.jpg">


#### b. &#58;root
<br>

In the <font color='green'>:root</font> section we will MODIFY the following:<br>

+ <b><font color=#A81966>--HeaderLogo-image:</font></b> url('assets/images/formr-logo-blue.gif'); 
+ <b><font color=#A81966>--HeaderLogo-margin:</font></b> 0px 0 0 50px;<br>

<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyCSS.gif">&nbsp;<font color='green' style=font-weight:normal;>:root</font> code below... </span>

```css
/*=======================================*/
/* root REPLACE Point - :root */
/*-----------------------------------------
:root selector for variables
-------------------------------------------*/
:root {
    --Body_background-color: #E5E4E2; /*platinum*/
   
    --Header_background-color: red;
    --Header_hover-color: white;
    --HeaderLogo-image: url( 'assets/images/formr-logo-blue.gif' );
    --HeaderLogo_margin: 0px 0 0 50px;
    --HeaderLogo-FontFamily: "Roboto Slab";
    --HeaderList-font-size: 1.2rem;
  
    --Section1_background-color: blue;
    --Section1_background-image: url( 'assets/images/monaco-blue-soft.jpg' );
  
    --Section2_background-color: lightgray;
    --Section2Paragraph-font-color: #ff7034;  /* dark orange */
  
    --Footer_background-color: green;
    --Footer_hover-color: white;
    --FooterList-font-size: .9rem;  
    
    --GlobalFontFamily: "Frank Ruhl Libre", "EB Garamond";

    --Button_Logo_font-color: whitesmoke;
} 
/* END REPLACE :root =====================*/
```
<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<div class="multiple-equals-text">
/*=======================================*/<br>
/* root REPLACE Point - :root */
<br><br>
/* END REPLACE :root ======================*/<br> 
</div>
comments in your index.<b>css</b> file:
</div>
<br>

<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicformRImage2.jpg">

#### c. .HeaderLogo

- We will be <u><b>REPLACING 3 classes</b></u>...

    + <font color='green'>.HeaderLogo</font>
    + <font color='green'>.HeaderLogo a</font>
        <br>&nbsp;&nbsp;&nbsp;(^ this class will be removed)
    + <font color='green'>.HeaderSpacer</font><br><br>

- ... <u><b>with 2 classes</b></u>... 

    + <font color='green'>.HeaderLogo</font>
    + <font color='green'>.HeaderSpacer</font><br><br>

- ...as a block of code:

<div class="callout-code-warning">
Take caution to assure that you replace threee (3) classes with just two (2).
</div>
<br>
<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyCSS.gif">&nbsp;<font color='green' style=font-weight:normal;>.HeaderLogo</font> code below... </span>

```css
/*===============================================*/
/* H-2 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/*=======================================*/
/* H-2 INSERT Point - .HeaderLogo */
/*-----------------------------------------
The .HeaderLogo properites
------------------------------------------*/
.HeaderLogo {
  width: 224px;
  height: 64px;
  margin-bottom: 0px;
  background-image: var(--HeaderLogo-image);
  background-size: 224px 64px;
  background-repeat: no-repeat;
  margin: var(--HeaderLogo_margin);
  font-size: 25px;
  font-weight: 600;
}

/*=======================================*/
/* INSERT Point - .HeaderSpacer */
/*-----------------------------------------
The .HeaderSpacer properites
------------------------------------------*/
.HeaderSpacer {
    flex: 1;
}
/* H-2 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
```
<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<font color='green'>
/&ast;======================================&ast;/<br>
/* H-2 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
<br><br>
/* H-2 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/<br> 
</font>
comments in your index.<b>css</b> file:
</div>
<br>

<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" style=border:none; src="FRApps/assets/images/md-images/BasicformRImage3.jpg">

____

#### d. @media (Slight change for responsiveness)

- In the <font color=cornflowerblue>@media</font> query
- Under <font color=cornflowerblue>@media</font> (max-width: 420px)<br><br>
- CHANGE in HeaderLogo:
    + <font color=#A81966>margin-left</font> from 0px to 15px
    + <font color=#A81966>margin-top</font> from 0px to 15px<br><br>
- ADD
    + <font color=green>h2</font> padding to 0

The easiest way to accomplish this is to copy/paste the entire Responsive BLOCK.<br> <span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyCSS.gif">&nbsp;<font color='green' style=font-weight:normal;>/* Responsive Code */</font> code below... </span>

```css

/*===========================================*/
/* R-1 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* Responsive Code */  
/* R-1 INSERT Point - @media (responsive max-width)*/
/*-----------------------------------------
The @media MAX-width query properties
=========================================*/
@media (max-width: 760px) {

    .HeaderLogo {
        font-size: 1.2rem;
        margin-left: 10px;
        background-size: 180px 51px;
    }
  
    .HeaderNavBars {
      display: flex;
    }
  
    .HeaderNavList {
        display: none;
    }
  
    .Section1ImageText {
        font-size: 2.5rem;
        padding: 120px 250px 20px 0px;
    }

    .Section2 h2 {
      font-size: 1.7rem;
    }
  
    .Section2Paragraph {
      font-size: 75%;
    }
  }

/*-----------------------------------------
The @media MAX-width (420px) query properties
=========================================*/
@media (max-width: 420px) {

    .HeaderLogo {
        font-size: .8rem;
        margin-left: 15px;
        margin-top: 15px;
        background-size: 144px 41px;
    }

    .Section1ImageText {
        font-size: 1.2rem;
        padding: 80px 100px 20px 10px;
      }
    
    .Section2Paragraph {
        font-size: 60%;
      }

    h2 {
        padding: 0;
    }
    
}
  /* R-1 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
```

<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<font color='green'>
/&ast;======================================&ast;/<br>
/* R-1 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
<br><br>
/* R-1 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^/<br> 
</font>
comments in your index.<b>css</b> file:
</div>
<br>

<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/
md-images/BasicResponsiveChange.jpg">

This will give the custom web page's formR logo the proper place in the header when viewing on an iPhone 7 Pro

<img class="no-border" src="FRApps/assets/images/
md-images/BasicFinaliPhoneHeaderImage.jpg">
____

#### Web Page with formR Logo
<br>
Please check your <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome browser to see your web page:
<br><br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicformRImage4.jpg">
<br><br>
<div class="success">
<span style="font-size: 20px"><b>CONGRATULATIONS!</b></span><br>You have successsfully replaced the "PH Logo" with the image of our formR logo.
</div>

___


### 3. Change Texts

- It is time to replace all of our <u><b>P</b></u>lace <u><b>H</b></u>older text.  We can do this by simply changing the texts in our index.**html** file. We will change the following:


- Header (Section)
    + "PH_Link1" ---> "Links"
    + "PH_Link1" ---> "Cards"
    + "PH_Link1" ---> "FAQs"
    + "PH_CTA"   ---> "Sign In"
- Section 1
    + "PH Text Overlay ---> "My Image & Text"
- Section2
    + "PH &#60;br&#62;" ---> *null*
- Footer (Section)
    + "PH Link1" ---> "Support"
    + "PH Link2" ---> "Terms Of Use"



<img style=border:none; class="no-border" src="FRApps/assets/images/md-images/index.html.jpg">


Open your index.html file and follow along as we are just going to edit some text in the page, starting with the Header class.

#### a. <font color='green'>Header</font>

- In the &#60;li&#62; tags please make the 4 changes as shown in the below "before" and "after" images.

> <span style="font-size: 25px"><b>BEFORE</b></span><br>
<img class="no-border" style=border:none; src="FRApps/assets/images/md-images/BasicTextImage1.jpg"><br>
<span style="font-size: 25px"><b>AFTER</b></span><br>
<img class="no-border" style=border:none; src="FRApps/assets/images/md-images/BasicTextImage2.jpg">

<br>
<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicHeaderTextEdit.gif">

____

#### b. <font color='green'>Section 1</font>

- In the &#60;h2&#62; tag please make the 1 change as shown in the below "before" and "after" images.

><span style="font-size: 25px"><b>BEFORE</b></span><br>
<img class="no-border" style=border:none; src="FRApps/assets/images/md-images/BasicTextImage3.jpg"><br>
<span style="font-size: 25px"><b>AFTER</b></span><br>
<img class="no-border" style=border:none; src="FRApps/assets/images/md-images/BasicTextImage4.jpg">
<br>

___

#### c. <font color='green'>Section 2</font>

- In the &#60;p&#62; tag please make the 1 change as shown in the below "before" and "after" images. 

- Just remove the PH &#60;br&#62;.

> <span style="font-size: 25px"><b>BEFORE</b></span><br>
<img class="no-border" style=border:none; src="FRApps/assets/images/md-images/BasicTextImage5.jpg"><br>
<span style="font-size: 25px"><b>AFTER</b></span><br>
<img class="no-border" style=border:none; src="FRApps/assets/images/md-images/BasicTextImage6.jpg">
<br>

___

#### d. <font color='green'>Footer</font>
- In the &#60;li&#62; tags please make the 2 changes as shown in the below "before" and "after" images.

> <span style="font-size: 25px"><b>BEFORE</b></span><br>
<img class="no-border" style=border:none; src="FRApps/assets/images/md-images/BasicTextImage7.jpg">&nbsp;<br>
<span style="font-size: 25px"><b>AFTER</b></span><br>
<img class="no-border" style=border:none; src="FRApps/assets/images/md-images/BasicTextImage8.jpg">
___

Here is what the final index.html page should look like:

<img class="no-border" style=border:none; src="FRApps/assets/images/md-images/BasicCustomHTMLFull.jpg">

#### Web Page with Text Changes
<br>
Now let's see these changes in <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome.  LOOKS GREAT!

<img class="no-border" src="FRApps/assets/images/md-images/BasicTextFinalImage.jpg">
<br><br>
FINALLY, we will CUSTOMIZE with some color changes.

### 4. Change Colors
<br>
We were requested to change some colors for the next major lessons. No problem!
<br><br>
This can all be done in the index.**css** file.

<img style=border:none; class="no-border" src="FRApps/assets/images/md-images/index.css.jpg">



#### a. &#58;root

<br>
First, remember the <font color='green'>:root</font> section.
<br>

<img class="no-border" src="FRApps/assets/images/md-images/BasicColorImage1.jpg">
<br><br>
Well, it's very simple to make the requested color changes right here in four of the properties:
<div class="list-text">
<ul>
<li>
    <font color=#A81966>--Header_background-color</font><br>
    &nbsp;&nbsp;(requested change from <span style="background-color:red;color:white">&nbsp;red&nbsp;</span> to <span style="background-color:#FF7034;color:white">&nbsp;dark orange&nbsp;</span>;<br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[hex: #FF7034])
</li><br>
<li>
    <font color=#A81966>--Section1_background-color</font><br>  
    &nbsp;&nbsp;(requested change from <span style="background-color:blue;color:white">&nbsp;blue&nbsp;</span> to <span style="background-color:whitesmoke;color:#424242">&nbsp;whitesmoke&nbsp;</span>)
</li><br>
<li>
    <font color=#A81966>--Section2_background-color</font><br>
    &nbsp;&nbsp;(requested change from <span style="background-color:lightgray;color:black">&nbsp;lightgray&nbsp;</span> to <span style="background-color:whitesmoke;color:#424242">&nbsp;whitesmoke&nbsp;</span>)
</li><br>
<li>
    <font color=#A81966>--Footer_background-color</font><br>
    &nbsp;&nbsp;(requested change from <span style="background-color:green;color:white">&nbsp;green&nbsp;</span> to <span style="background-color:#FF7034;color:white">&nbsp;dark orange&nbsp;</span>; <br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[hex: #FF7034])
</li>
</ul>
</div>
<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyCSS.gif">&nbsp;<font color='green' style=font-weight:normal;>:root</font> code below... </span>

```css
/*=======================================*/
/* root REPLACE Point - :root */
/*-----------------------------------------
:root selector for variables
-------------------------------------------*/
:root {
    --Body_background-color: #E5E4E2; /*platinum*/
   
    --Header_background-color: #FF7034; /*dark orange*/
    --Header_hover-color: white;
    --HeaderLogo-image: url( 'assets/images/formr-logo-blue.gif' );
    --HeaderLogo_margin: 0px 0 0 50px;
    --HeaderLogo-FontFamily: "Roboto Slab";
    --HeaderList-font-size: 1.2rem;
  
    --Section1_background-color: whitesmoke;
    --Section1_background-image: url( 'assets/images/monaco-blue-soft.jpg' );
  
    --Section2_background-color: whitesmoke;
    --Section2Paragraph-font-color: #ff7034;  /* dark orange */
  
    --Footer_background-color: #FF7034; /*dark orange*/
    --Footer_hover-color: white;
    --FooterList-font-size: .9rem;  
    
    --GlobalFontFamily: "Frank Ruhl Libre", "EB Garamond";

    --Button_Logo_font-color: whitesmoke;
} 
/* END REPLACE :root =====================*/

```
<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<div class="multiple-equals-text">
/*=======================================*/<br>
/* root REPLACE Point - :root */
<br><br>
/* END REPLACE :root ===================*/<br> 
</div>
comments in your index.<b>css</b> file:
</div>
<br>

<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicColorImage3.jpg">

 
Check it out in <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome!  NICE!<br>
So easy and powerful with the <font color='green'>:root</font> variables.

<img class="no-border" src="FRApps/assets/images/md-images/BasicColorImage3a.jpg">

___

There is one last touch for Section 2.  Let's pretty-up that paragraph.  It is done with the class "Section2Paragraph."

#### b. .Section2Paragraph
<br>

We will change the font color to that dark orange color we used for the header and footer background colors.<br>

We will make the first line larger than the rest of the lines.<br>

Finally we will make the first letter of the first line very large.<br>

In the <font color='green'>.Section2Paragraph</font> section we will INSERT the following:<br>
<ul>
    <li><b><font color='green'>Section2Paragraph</font></b>:</li><br> 
    <li><b><font color='green'>Section2Paragraph::first-line</font></b>:</li>
    <li><b><font color='green'>Section2Paragraph::first-letter</font></b>:</li>
</ul>
<span class="copy-code"><img class="copy-image" src="FRApps/assets/images/md-images/CopyCSS.gif">&nbsp;<font color='green' style=font-weight:normal;>.Section2Paragraph</font> code below... </span>

```css
/*===========================================*/
/* S2-2 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* S2-2 INSERT Point - Section2Paragraph */
/*-----------------------------------------
The .Section2Paragraph properites
------------------------------------------*/
.Section2Paragraph {
    font-family: var(--GlobalFontFamily);
    margin-top: 0px;
    font-size: 1.3rem;
    color: var(--Section2Paragraph-font-color); /* dark orange*/
    font-weight: bolder;
    padding-top: 1rem;
}

/*=======================================*/
/* INSERT Point - Section2Paragraph::firstLetter/line */
/*-----------------------------------------
The .Section2Paragraph::firstLetter/line properites
------------------------------------------*/
.Section2Paragraph::first-line {
  font-size: 125%;
  }
  
.Section2Paragraph::first-letter {
font-size: 150%;
}
/* S2-2 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
```
<div class="callout-code-warning">
<br><br>
...AND make certain you paste it <u>ENTIRELY WITHIN</u> these
<br>
<font color='green'>
/&ast;======================================&ast;/<br>
/* S2-2 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
<br><br>
/* S2-2 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/<br> 
</font>
comments in your index.<b>css</b> file:
</div>
<br>
<span class="like-this-text">&nbsp;Like this&nbsp;</span>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicColorImage4.jpg">

### Final CUSTOM

#### Web Page with Color Changes

<br>
<div class="success">
<span style="font-size: 20px"><b>CONGRATULATIONS!!</b></span>
    <div class="success-text">
    You have completed "My HTML Custom App."
    <ul>
        <li>GREAT JOB!</li>
        <li>Check out your work in <img src="FRApps/assets/icons//ChromeIcon.png" width="4%"> Chrome.</li>
    </ul>
    </div>  
</div>
<br>
<img class="no-border" src="FRApps/assets/images/md-images/BasicCustomWithWiggle.jpg">

#### Final Version With formR logo, text & color changes, "wiggle" button and responsive.

___

Like the Layout version, your completed custom version is responsive at 420 and 760 pixels.  

<img class="no-border" src="FRApps/assets/images/md-images/BasicResponsiveDualScreenImage2.jpg">
<br><br>
And it looks great on an iPhone 7 Plus.
<br><br>
<img class="no-border" width=75% src="FRApps/assets/images/md-images/BasicFinaliPhoneImage.jpg">
<br><br>

Now you have all the tools to go back to your Layout and customize it the way you would like.

<div class="save-code"><br><br>
We saved your Layout AND Custom files in the<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="callout-dir-text">"1c1_my-html-custom-app"</span> directory.<br<br><br><br>

The files are:<br>
+ index_final_custom.css
+ index_final_custom.html
+ index_final_layout.css
+ index_final_layout.html

Here:

<img class="seventy-five-percent" src="FRApps/assets/images/md-images/BasicColorImage5.jpg">
<br><br>
Please make modifications to the code in either set to help to create your own Custom HTML App.
<br><br>
</div>
<br><br>
<div class="callout-code-warning"><br>
Remember to change your<br>  
&nbsp;&nbsp;&nbsp;&nbsp;'&#60;link rel="stylesheet" href="<span class="css-link-text">index_final_layout.css</span>"&#62;'<br>
reference in your <u>index.<b>html</b></u> file to match the name of your relating <u>index*.css</u> file.
<br><br> Like below:
<img src="FRApps/assets/images/md-images/BasicColorImage6.jpg">
<!--</span>-->
</div>
<br>

<!--## 6. View Full Code-->  <!-- {docsify-ignore} -->

###  [View Full Code For HTML Custom Apps](/FRApps/code/fr020102_custom-code.md "Full Code") 

<br>

### *DEPLOY TO INTERNET*

### 1. Initial Clone 

- We will install the App that we just finshed on the Ubuntu server

#### 1. From VSCode, if you have made changes, Commit and Sync them from VSCode to your Github repository
<br>

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/commit.jpg">
<br><br>

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/sync.jpg">
<br><br>
 
- Note: If this is your first commit, please click Publish Branch instead of Sync <br>

<img class="fifty-percent" src="FRApps/assets/images/deploy/publish.jpg">
<br><br>

#### 2. Open VSCode new Terminal and connect to your remote Ubuntu server
<br>
<img class="seventy-five-percent" src="FRApps/assets/images/deploy/vscode-new-term.jpg">
<br><br>

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/vscode-new-term1.jpg">
<br><br>

- Connect to your Vultr server using your .ssh
vultr name (You created this in Build Workstation Step 3.) 

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/ssh-cong-vultr.jpg">
<br><br>

- enter into your new Terminal in VSCode

```
ssh vultr-formr0-nimda
```

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/vscode-term-ssh-login.jpg">
<br><br>

- From VSCode Terminal enter: 

```
cd /webs
```

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/terminal-cd-webs.jpg">
<br><br>

#### 3. Login to your Github repository for FRApps and click the Code button
<br>
<img class="seventy-five-percent" src="FRApps/assets/images/deploy/git-code.jpg">
<br><br>

- then click HTTPS and the copy button.

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/git-https-copy.jpg">
<br><br>

- then using Notepad enter and paste from clipboard:

```
git clone <paste herethe copied https link from your personal Github>
```

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/git-note-paste.jpg">
<br><br>

```
e.g. git clone https://github.com/brucetroutman-gmail/FRApps.git
```

- Copy from Notepad 

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/git-note-copy.jpg">
<br><br>

- and paste into the VSCode Terminal and execute the clone process.

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/term-clone.jpg">
<br><br>

#### 4. Using Bitvise Login and open an SFTP window 
<br>
<img class="seventy-five-percent" src="FRApps/assets/images/deploy/bitvise-login.jpg">
<br><br>

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/bitvise-sftp.jpg">
<br><br>


- Navigate to:

```
/etc/nginx/apps-enabled
```

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/sftp-apps-enabled.jpg">
<br><br>

#### 5. Copy this file name to the clipboard:

```
formr-xxx-00.com_my-html-remote-app.conf
```

- In the SFTP window right click in the white area and click Create file,

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/sftp-create-file.jpg">
<br><br>

- Paste into the new file

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/sftp-file-name.jpg">
<br><br>

#### 6. Right click on this file and click Edit
<br>
<img class="seventy-five-percent" src="FRApps/assets/images/deploy/sftp-file-edit.jpg">
<br><br>

- Paste the following into this file:

```
location    /my-html-remote-app {      

    alias       /webs/FRApps/client1/2c1_my-html-remote-app/;      

}   
```

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/sftp-note-paste-conf.jpg">
<br><br>

- Save the file

#### 7. In VSCode Terminal enter:

```
systemctl restart nginx 
```
then
```
pm2 restart app
```

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/term-restart.jpg">
<br><br>


#### 8. Browse to your server:

```
https://formr-cbt-00.com/my-html-remote-app
```
<img class="seventy-five-percent" src="FRApps/assets/images/deploy/browse-simp-my-html.jpg">
<br><br>


### 2. Update Your App

#### 1. Modify index.html in VSCode
<br>
Replace "My Image & Text" with (use your name)

```
"Welcome to Bruce's FormR..."
```

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/index-change-sect1.jpg">
<br><br>

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/index-change-sect1-1.jpg">
<br><br>

#### 2. Commit and Sync from VSCode to your Github repository
<br>
<img src="FRApps/assets/images/deploy/commit-sect1.jpg">
<br><br>

<img src="FRApps/assets/images/deploy/sync-sect1.jpg">
<br><br>

#### 3. In VSCode Terminal enter: 

```
cd /webs/FRApps/client1/2c1_my-html-remote-app
```

then

```
git pull
```

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/term-git-pull.jpg">
<br><br>

#### 4. Browse to your server:

```
https://formr-cbt-00.com/my-html-remote-app
```

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/browse-changed-sect1.jpg">
<br><br>

### 3. Change Your Home Page

- We will change your home page from simpleApp to my-html-remote-app

#### 1. From the SFTP window
<br>
- Navigate to:

```
/etc/nginx/apps-enabled
```

- then right click and edit 

formr-xxx-00.com_my-html-remote-app.conf

and replace everything with:

```
location      / {      

    alias       /webs/FRApps/client1/2c1_my-html-remote-app/;      

}   
```

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/conf-change-remote-app.jpg">
<br><br>

- Save the file

#### 2. From the SFTP window

- Navigate to:

```
/etc/nginx/apps-enabled
```
- then right click and edit 

formr-xxx-00.com_simpleApp.conf

and replace everything with:

```
location    =  /simpleapp  { 

    proxy_pass http://localhost:5000;

    } 
# ------------  --------------------------
   
```

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/conf-change-simple-app.jpg">
<br><br>

- Save the file

#### 3. In VSCode Terminal enter:

```
systemctl restart nginx 
```
then
```
pm2 restart app
```

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/term-restart.jpg">
<br><br>



#### 4. Browse to your server:

- To now get to simpleApp

```

https://formr-cbt-00.com/simpleapp

```
<img class="seventy-five-percent" src="FRApps/assets/images/deploy/browse-new-simple-app.jpg">
<br><br>


- Your homepage is now your html remote app

```

https://formr-cbt-00.com

```

<img class="seventy-five-percent" src="FRApps/assets/images/deploy/browse-new-home.jpg">
<br>

<hr>
Your next journey will be to add some very cool functions to our web page using JavaScript.
<br><br>

<div class="final">
    <span class="happy-coding">  
        <img class="happy-coding-percent" src="FRApps/assets/images/md-images/HappyCoding6.gif">
        <!--&nbsp;&nbsp;HAPPY CODING!-->
    </span>
</div>
<br>

<div class="page-back">

[BACK - Clone FR Apps](/FRApps/fr020000_Clone-FR-Apps.md)
</div><div class="page-next">

[Custom FRApps JavaScript - NEXT](/FRApps/fr020200_My-Javascript-Custom-App.md)
</div>
<br><br>
