<!-- ------------------------------------------------------------------------- -->

<div class="page-back">

[BACK - Website SSL](/Setup/fr0306_Setup-Website-SSL-Ubuntu.md)
</div><div class="page-next">

[Custom FRApps React - NEXT](/Setup/fr0105_Custom-FR-Apps-React.md)
</div><div style="margin-top:35px">&nbsp;</div> 
 
<!-- ------------------------------------------------------------------------- -->

## 3.1 My HTML Custom App h:mm <!-- {docsify-ignore} -->
- [Purpose and Background](../Setup/purposes/pfr020100_fr020100_My-HTML-Custom.md)
- [Enter Comments in Discord](https://discord.com/channels/928752444316483585/931216956827250709)


#### Introduction 
- You will be building a web site which starts with very simple index.**html** and index.**css** files.  Your repository will include both of those **empty** files plus the needed images. If you follow the directions and copy/paste each sections code you will end up with a still simple index.html but a rather complex index.css file.

- Tutorial Links 

We are not attempting to teach CSS (Cascading Style Sheets), but providing with some links below of very good tutorials. Hopefully, this exercise will encourage you to explore these links. (See Purpose and Background for details)

- Tools Used

1. Your completed workstation
2. Chrome web browser
3. Windows File Explorer
4. VS (Visual Studio) Code
5. Git Hub  

- Your Workspace

You will find in VSCode a folder "1c1_my-html-custom-app."  In this folder are the empty index.<b>html</b> and index.<b>css</b> files, along with a favicon.png image file. There is an "assets" folder that holds an "images" folder with the needed images to build your final project for this HTML Custom App course.

___

<img class="shadow-border" src="FRApps/assets/images/md-images/IntroductionImage1.jpg">

___

- Suggested method to set up your windows.  
    + VSCode taking up the right 1/2 of your screen
    + Chrome with your work instructions taking up the left 2/3 of your screen
    + A second Chrome window with your "live server" taking up the left 1/3 of your screen
- As you add code to your index.html and index.css files, you will be able to see immediate results in the "Live Server" portion of your screen

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicBlocksWorkstationImage1.jpg">

___

- Your Final CUSTOMIZED Web Site Preview
<br><br>
The below preview will have a fixed (secured) header and footer, navigation links and a "wiggle" button, an image with a font-based overlay, a formR logo, and is responsive (the page will react properly when small or large).
<br>
<br>
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFINALImage.jpg">

<!--
<img class="shadow-border" src="FRApps/assets/images/md-images/IntroductionImage2.jpg">
-->

#### Important note about names, capitalization, pictures and code copying <!-- {docsify-ignore} -->
- In this tutorial please be careful to use the Exact Spelling and Capitalization. You will be using Windows, Unix and GitBash command prompts. Improper captialization will cause commands to fail. Some examples are: Local_Admin, myProject, repos, remotes and .ssh.
- This documentation was produced in 2021-2022. You will experience differences in some of the pictures due to the changes made over time by the developers of the softwares and web sites that are used.
- We recommend that you cut and paste code snippets from the Documentation into your workstation/server. This will reduce the errors caused by hand typing.
- We will be Replacing, Inserting and Deleting blocks of code in both the index.html & index.css files.  Below is the KEY to aid in finding the place in the code for these actions in the index.**css** file:
    + **BR**:  Body Replace
    + **HR**:  Header Replace
    + **H**:   Header Insert/Delete
    + **S1R**: Section1 Replace
    + **S1**:  Section1 Insert
    + **S2R**: Section2 Replace
    + **S2**:  Section2 Insert
    + **FR**:  Footer Replace
    + **F**:   Footer Insert
    + **R**:   Responsive Insert

Example:

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicBlocksInsertKeyImage1.jpg">

- In some cases we will be copy/pasting large block of code. It will be noted as below: 


/*===========================================*/<br>
/* START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*INSERT CODE HERE*<br>
/* END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/<br>

<br>

> <u><b><i>LAYOUT vs CUSTOMIZATION</i></b></u>:  As we build upon the code in both index.html and index.css, we will create first a "Layout," then we will "Customize" it our way.  You will have the opportunity to customize your "Layout" as your "Custom HTML App" later.
<br><br>Below is our outline.
<br> 
- Layout
    + 1. Create Basic Blocks
    + 2. Modify to Large Blocks
    + 3. Add Fixed Header
    + 4. Add Fixed Footer
    + 5. Add Text Overlay
    + 6. Add "Wiggle" Button
    + 7. Add Responsiveness
- Customize
    + 1. Add Image to Section 1
    + 2. Add Image formR Logo
    + 3. Change Texts
    + 4. Change Colors

### *LAYOUT*
<br>
Like many web sites (pages) we like to start with a very simple sketch; pencil drawn on a sheet of paper.  Here was our initial thoughts to build a very simple "block" structured web page.  We came very close in achieving our goal.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicHTMLSketch.jpg">

<br>

----
### 1. Create Basic Blocks
----

- We will begin this Custom App by simply copying & pasting the code below into  your empty html and css files.  The results will be 4 very basic blocks that sit on top of each other.  Let's start by reviewing the files in your [repos]itory.


#### 1. Review Files

-  Using VSCode, in a folder called "0c1_my-basic-blocks", open:
    - index.<b>html</b> and
    - index.<b>css</b>
    
Both should be empty.

#### 2. Code - index.html

<br>

> <span style="font-size: 25px"><b>REMINDER</b></span><br>
Mouse over the "HTML" in the upper right corner of the code block to quickly copy all the code.<br>
<img width="15%" src="FRApps/assets/images/md-images/BasicHTMLCopyImage.jpg">

- Click on and open the index.<b>html</b> file from VSCode. Copy and paste the entire below code to Line 1 of the empty index.<b>html</b> file:

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <meta http-equiv="X-UA-Compatible" content="ie=edge">
        <title>HTML Custom Apps</title>
        <link rel="shortcut icon" href="favicon.png">
        <link rel="stylesheet"    href="https://fonts.googleapis.com/css?family=Bookman Old Style" >
        <link rel="stylesheet"    href="index.css">
    </head>

    <body>    

        <!-- REPLACE Point - Header -->
        <div class="Header">
        	<!-- INSERT Point - responsive -->
        	<h2>PH Header</h2>
        </div>

        <!-- REPLACE Point - Section1 -->
        <div class="Section1">
           <h2>PH Section 1</h2>
        </div>
        
        <!-- REPLACE Point - Section2 -->        
        <div class="Section2">
            <h2>PH Section 2</h2>
        </div>        
        
        <!-- REPLACE Point - Footer -->
        <div class="Footer">
            <h2>PH Footer</h2>
        </div>
    
    </body>

</html>
```

___

- From VSCode, right click on the file "index.<b>html</b>" and click on "Open In Live Server"

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicBlocksImage1.jpg">
<br><br>
If your Chrome browser is not already open, this command will open it and show the results of the above html code. 
<br><br>
Like this
<br>
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicBlocksImage2.jpg">
<br><br>

<span style="font-size: 25px"><b>This is our starting point.</b></span>  Let's move to the CSS code to add our blocks.

___

#### 3. Code - index.css  

- Click on the index.<b>css</b> file. Then copy and paste the below code, on to Line 1 of index.**css**</b>:
<br>

```css
/* Basic Blocks Custom App */
@import url('https://fonts.googleapis.com/css2?family=Frank+Ruhl+Libre:wght@700&display=swap');
@import url('https://fonts.googleapis.com/css?family=Bookman Old Style');

/*=======================================*/
/* root REPLACE Point - :root */
/*-----------------------------------------
:root selector for variables
-------------------------------------------*/
:root {
    --Header_background-color: red;
    --Header_hover-color: white;
    --HeaderLogo-image: "";
    /*--HeaderLogo-image: *url( 'assets/images/formr-logo-blue.gif' );*/
    --HeaderLogo_margin: 35px 0 0 0px;
    --HeaderList-font-size: 1.2rem;
  
    --Section1_background-color: blue;
    --Section1_background-image: url( 'assets/images/monaco-blue-soft.jpg' );
  
    --Section2_background-color: lightgray;
    --Section2Paragraph-font-color: #ff7034;  /* dark orange */
  
    --Footer_background-color:green;
    --Footer_hover-color: white;
    --FooterList-font-size: .9rem;  
    
    --GlobalFontFamily: "Bookman Old Style", "Frank+Ruhl+Libre:wght@700&display=swap";
} 


/*-----------------------------------------
The <html> tag properites (unchanged)
------------------------------------------*/
html {
    background: #b3b3b3;
    height: 100%;
    text-align: center;
}


/*-----------------------------------------
The body properites
------------------------------------------*/
body {
    background: white;
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
    width: 300PX;
    height: 100PX;
    position: relative;
}


/*===========================================*/
/* START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* H-1 INSERT Point - .HeaderNavBars */

/*     INSERT Point - .HeaderNavBars:focus */
/* END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/


/*===========================================*/
/* START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* H-2 INSERT Point - .HeaderLogo */

/*     INSERT Point - .HeaderLogo a */

/*     INSERT Point - .HeaderSpacer */
/* END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/


/*===========================================*/
/* START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* H-3 INSERT Point - .HeaderNavList */

/*     INSERT Point - .HeaderNavListItem a */

/*     INSERT Point  - .HeaderNavListItem a:hover
                       .HeaderNavListItem a:active */
/* END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/


/*=======================================*/
/* H-4 INSERT Point - .HeaderNavListItemCTA a */
/*----------------------------------------
The .HeaderNavListItemCTA a properties
-----------------------------------------*/


/*===========================================*/
/* START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* H-5 INSERT Point - .HeaderNavListItemCTA */

/* INSERT Point - @keyframes wiggle */
/* END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/


/*=======================================*/
/* S1R-1 REPLACE Point - Section1 */
/*-----------------------------------------
The .Section1 properites
------------------------------------------*/
.Section1 {
    background: var(--Section1_background-color);
    width: 300PX;
    height: 100PX;
    position: relative;
}


/*===========================================*/
/* START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* S1-1 INSERT Point - .Section1ImageText */

/*      INSERT Point - .Section1ImageText::first-letter */
/* END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/


/*=======================================*/
/* S2R-1 REPLACE Point - Section2 */
/*-----------------------------------------
The .Section2 properites
------------------------------------------*/
.Section2 {
    background: var(--Section2_background-color);
    width: 300PX;
    height: 100PX;
    position: relative;
}


/*=======================================*/
/* S2-1 INSERT Point - Section2 h2 */
/*      DELETE Point - Section2 h2 */
/*-----------------------------------------
The .Section2 h2 properites
------------------------------------------*/
.Section2 h2 {
    color: black;
    font-size: 1.5rem;
    padding: 1.5;
}


/*===========================================*/
/* START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* S2-2 INSERT Point - Section2Paragraph */

/*      INSERT Point - Section2Paragraph::first-letter/line */
/* END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/


/*=======================================*/
/* FR-1 REPLACE Point - Footer */
/*-----------------------------------------
.Footer properites
------------------------------------------*/
.Footer {
    background: var(--Footer_background-color);
    width: 300PX;
    height: 100PX;
    position: relative;
}


/*===========================================*/
/* START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* F-1 INSERT Point - .FooterNavList */

/*     INSERT Point - .FooterNavListItem a */

/*     INSERT Point - .FooterNavListItem a:hover
                      .FooterNavListItem a:active */
/* END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/


/*===========================================*/
/* START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* Responsive Code */  
/* R-1 INSERT Point - @media (responsive min-width)*/                

/*     @media (responsive max-width)*/ 
/* END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/


/* END */
```

___

#### 4.  Basic Blocks Web Page      

- Please check your Chrome browser. 

<br>
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicBlocksImage3.jpg"><br><br>

> We will build from this basic page to create a web site with a fixed header and footer, links with a "wiggle" button, and an image with a text overlay--in our customize section.<br><br>
From there, the next course we will move on to add some magic with JavaScript (JS) to this web page.

___

#### 5. Understanding CSS        <!-- .(20615.01.2 RAM Changed to ### 4. Was #### --> 
<br>
To understand a little of this CSS code, let's look at the .Header properties.
<br>
<br>
<font color='green'>** Notes:</font>
<br>

```css
/*-----------------------------------------
The .Header properites
------------------------------------------*/
.Header {
    background: var(--Header_background-color);
        ** Sets the background to the variable you set above
    width: 300px;
        ** Sets the width of the header block 300 pixels
    height: 100px;
        ** Sets the height of the header block 100 pixels
    position: relative;
        ** Places the header box relative to the html code
        *DOM (Document Object Model) reading from 
        the top to the bottom
        
}

```

&nbsp;&nbsp;&nbsp;&nbsp;*[DOM](https://www.w3.org/TR/WD-DOM/introduction.html "What Is DOM")

<!--<a href='/FRApps/code/fr020101_basic-blocks-code.md' title='Full Code'>View Full Code For Basic Blocks</a>-->

<!--
#### 6.  [View Full Code For Basic Blocks](/FRApps/code/fr020101_basic-blocks-code.md "Full Code") -->

- <span style="font-size: 20px"><b>CONGRATULATIONS!!</b></span> You have just created a simple html page with a cascading style sheet (CSS) which makes 4 *basic blocks.*  


----
### 2. Modify to Large Blocks  
----

- Next, we will add to your existing code in the index.<b>css</b> file to continue building on our basic web page.  We will fill the web page up with our 4 blocks; pefectly one block on top of the next block.  They will be "Large Blocks."
<br><br>

#### index.css

#### 1. .Header
<br>

- In the <font color='green'>.Header</font> section we will MODIFY the following:<br>

    + <b><font color=#A81966>width</font></b>: 100%; 
    + <b><font color=#A81966>height</font></b>: 10%;

Copy <font color='green'>.Header</font> code below... 

```css
/*-----------------------------------------
The .Header properites
------------------------------------------*/
.Header {
    background: var(--Header_background-color);
    width: 100%; /*was 300px*/
    height: 10%; /*was 100px*/
    position: relative;
}
```
...AND make certain you paste it BELOW this *<u>HR-1 REPLACE point - Header</u>* comment in your index.**css** file:


> /* HR-1 REPLACE Point - .Header */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage4a.jpg">

___

- Check out your live server on Chrome and see the difference the above .Header code made.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage4f.jpg">

___

#### 2. .Section 1 & 2

- In <font color='green'>Section1</font> <b>AND</b> <font color='green'>Section2</font>, CHANGE

    + <b><font color=#A81966>width</font></b> to 100%  
    + <b><font color=#A81966>height</font></b> to 40%
<br>

___

<font color='green'><u>Section1</u></font>

- Copy <font color='green'>.Section1</font> code below... 

```css
/*-----------------------------------------
The .Section1 properites
------------------------------------------*/
.Section1 {
    background: var(--Section1_background-color);
    width: 100%; /*was 300px*/
    height: 40%; /*was 100px*/
    position: relative;
}

```

...AND make certain you paste it BELOW this *<u>S1R-1 REPLACE point - .Section1</u>* comment in your index.**css** file:


> /* S1R-1 REPLACE Point - .Section1 */

<br>
Like this
<br><br>

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage4b.jpg">

___

<font color='green'><u>.Section2</u></font>

- Copy <font color='green'>.Section2</font> code below... 

```css
/*-----------------------------------------
The .Section2 properites
------------------------------------------*/
.Section2 {
    background: var(--Section2_background-color);
    width: 100%; /*was 300px*/
    height: 40%; /*was 100px*/
    position: relative;
}

```

...AND make certain you paste it BELOW this *<u>REPLACE point</u>* comment in your index.**css** file:


> /* REPLACE Point - .Section2 */

<br>
Like this
<br><br>

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage4c.jpg">

___

#### 3. .Footer
<br>

- In the <font color='green'>.Footer</font> section we will ADD the following:<br>

    + <b><font color=#A81966>width</font></b> to 100% <br>AND 
    + <b><font color=#A81966>height</font></b> to 10%

Copy <font color='green'>.Footer</font> code below... 

```css
/*-----------------------------------------
The .Footer properites
------------------------------------------*/
.Footer {
    background: var(--Footer_background-color);
    width: 100%; /*was 300px*/
    height: 10%; /*was 100px*/
    position: relative;
}
```
...AND make certain you paste it BELOW this *<u>FR-1 REPLACE point - .Footer</u>* comment in your index.**css** file:


> /* FR-1 REPLACE Point - .Footer */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage4d.jpg">

___

#### Index.html

#### 1. Section2 Paragraph
<br>
- In the <font color='green'>Section2</font> class section we will REPLACE the code within the <br>
&#60;div class="Section2"&#62; & &#60;/div&#62; tags:<br><br>

Copy <font color='green'>Section2</font> code below ... 

```html
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
```

...AND make certain you paste it BELOW this *<u>REPLACE point - Section2</u>* comment in your index.**html** file:


> &#60;!-- REPLACE Point - Section2 --&#62;

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage6.jpg">
<br><br>
This provides a paragraph text we can add some nice attributes later in the <i>Customization</i> section. 


#### Large Blocks Web Page       <!-- .(20615.01.1 RAM This seems a little out of place --> 
- Please check your Chrome browser to see your web page so far.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage5.jpg">

<br><br>
<span style="font-size: 25px"><b>CONGRATULATIONS</b></span>! You have built a full page with four distinct blocks using your Basic Blocks index.<b>css</b> code. In the next section. we will add/modify code to secure (fix) the header in one spot.   

<!--## 6. View Full Code  <!-- {docsify-ignore} -->

<!--#### 9. [View Full Code For Basic Blocks](/FRApps/code/fr020102_basic-large-blocks-code.md "Full Code")-->


----
### 3. Add Fixed Header 
----

- Next, we will add to your existing code in  both index.<b>html</b> AND index.<b>css</b> files to continue building on our basic web page.  In this section we will "fix" the Header so when you scroll, the Header stays in place.  We will do the same for the Footer in the next section.  Also, we will be "prettying up" the Navigation Bar on the right side of the Header.  Let's go...

___

#### index.html

#### 1. Header class


- In the <font color='green'>Header</font> class section we will REPLACE the code within the <br>
&#60;div class="Header"&#62; & &#60;/div&#62; tags:<br><br>

Copy <font color='green'>Header</font> code below ... 

```html
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
```
...AND make certain you paste it BELOW this *<u>REPLACE point - Header</u>* comment in your index.**html** file:


> &#60;!-- REPLACE Point - Header --&#62;

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage1.jpg">
<br>

___


Take a quick look at Chrome and the Header.  

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage1a.jpg">
<br><br>
We now need to go to the index.css file to clean this up.  We are using names like "PH_Link1" and "PH Logo" as <u><b>P</b></u>lace <u><b>H</b></u>olders for our final customization of our Web page.
<br><br>
Now we move to the index.css file.

___

#### index.css

___

#### 1. .Header
<br>
First and foremost in the <font color='green'>.Header</font> section we will CHANGE & ADD the following:<br>

- CHANGE 
    + <font color=#A81966>position</font>: from relative to <b>fixed</b>
    + <font color=#A81966>height</font>: from 10% to <b>100px</b>
- ADD 
    + <font color=#A81966>z-index</font>: 100; 
    + <font color=#A81966>display</font>: flex; 
    + <font color=#A81966>justify-content</font>: space-between;
    + <font color=#A81966>align-items: center;</font>: space-between;

Copy <font color='green'>.Header</font> code below... 

```css
/*-----------------------------------------
The .Header properites
------------------------------------------*/
.Header {
    background: var(--Header_background-color);
    width: 100%;
    height: 100px;
    position: fixed;  /*was relative*/
    z-index: 100;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

```
...AND make certain you paste it BELOW this *<u>HR-1 REPLACE point - .Header</u>* comment in your index.**css** file:


> /* HR-1 REPLACE Point - .Header */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage1b.jpg">

___

Look at your Chrome browser! The above steps "fixed" the header into a stationary position.

We still need to:

1. Get rid of the "Unwanted Space" at the bottom 
2. Fix the "PH Logo" in the left corner of the header.
3. Fix the links in the right corner of the header 


<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage3.jpg">
<br><br>
To handle the Unwanted Space, we need to adjust Sections 1 & 2 and the Footer.  It's easy, we will 'code' each to have a <font color=#A81966>top</font> of 10%.  
<br><br>

- ADD 
    + <font color=#A81966>top</font>: 10%; (at the bottom of <font color=green>.Section1</font>, <font color=green>.Section2</font> & <font color=green>.Footer</font>)

&nbsp;&nbsp;&nbsp;&nbsp;AND

- MODIFY in <font color=green>.Section1</font> & <font color=green>.Section2</font>
    + <font color=#A81966>height</font>: 50%;

Let's start with <font color=green>.Section1</font> below.
___

#### 2. .Section1

- In the <font color='green'>.Section1</font> class, copy the code below...

```css
/*-----------------------------------------
The .Section1 properites
------------------------------------------*/
.Section1 {
    background: var(--Section1_background-color);
    width: 100%;
    height: 50%;
    position: relative;
    top:10%; /*<---ADD to adjust the top position*/
}

```
...AND make certain you paste it BELOW this *<u>S1R-1 REPLACE point - .Section2</u>* comment in your index.**css** file:


> /* S1R-1 REPLACE Point - .Section1 */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage0a.jpg">

___
#### 3. .Section2

- In the <font color='green'>.Section2</font> class, copy the code below...

```css
/*-----------------------------------------
The .Section2 properites
------------------------------------------*/
.Section2 {
    background: var(--Section2_background-color);
    width: 100%;
    height: 50%;
    position: relative;
    top:10%; /*<---ADD to adjust the top position*/
}

```
...AND make certain you paste it BELOW this *<u>S2R-1 REPLACE point - .Section2</u>* comment in your index.**css** file:


> /* S2R-1 REPLACE Point - .Section2 */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage0b.jpg">

___

#### 4. .Footer

- In the <font color='green'>.Footer</font> class, copy the code below...

```css
/*-----------------------------------------
The .Footer properites
------------------------------------------*/
.Footer {
    background: var(--Footer_background-color);
    width: 100%;
    height: 10%;
    position: relative;
    top:10%; /*<---ADD to adjust the top position*/
}

```
...AND make certain you paste it BELOW this *<u>FR-1 REPLACE point</u>* comment in your index.**css** file:


> /* FR-1 REPLACE Point - .Footer */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage0c.jpg">

___

Back to Chrome. We now have all the blocks stacked in proper order with no "Unwanted Space" at the bottom. 
<br><br>
AND if you scroll up and down, you will have the "secured" header.

___

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage4.jpg">

___


#### 5. .HeaderLogo (PH Logo)

- Now, let's fix that ugly "PH Logo" on the left side of the header. To do this, we add a new class to our CSS file.
<br>


- We will be INSERTING 3 new classes as a block of code:

    + <font color='green'>.HeaderLogo</font>
    + <font color='green'>.HeaderLogo a</font>
    + <font color='green'>.HeaderLogo:focus</font><br>

In the <font color='green'>.HeaderLogo</font>, copy the code below...

> Note: In your css code you will see an area to copy a full BLOCK of code like this:
<br>/&#10035; START BLOCK &#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;/
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color=red>PLACE H-2 CODE HERE</font>
<br>/&#10035;&nbsp;END BLOCK ^^^^^^^^^^^^^^^^^^^&#10035;/ 


```css
/*=======================================*/
/* H2 INSERT Point - .HeaderLogo */
/*-----------------------------------------
The .HeaderLogo properites
------------------------------------------*/
.HeaderLogo {
    padding-left: 54px;
    font-size: 1.5rem;
    color:whitesmoke;
}

/*=======================================*/
/* INSERT Point - .HeaderLogo a */
/*-----------------------------------------
The .HeaderLogo a properites
------------------------------------------*/
.HeaderLogo a {
    text-decoration: none;
    color: white;
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
```
...AND make certain you paste it BELOW this *<u>START BLOCK</u>* and *<u>END BLOCK</u>* comment in your index.**css** file:

> NOTE<br><img class="shadow-border" src="FRApps/assets/images/md-images/BasicStartBlockImage1.jpg">

<br>
Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage0d.jpg">

___

Now check Chrome
<br>

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage5.jpg">

___


This takes the "PH Logo" and turns it into a nice "font-based" logo.  Note the font is one of Google's special fonts, called "Bookman Old Style."  We linked to that from the very top of the index.<b>css</b> file.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage6.jpg">
<br><br>
This PH Logo is for the *LAYOUT*.  We will replace this with a formR logo image in the *CUSTOMIZATION* section.

___

#### 6. .HeaderNavList - BLOCK


- Now, let's focus on the stack of links on the right side of the header.  

- We will be INSERTING 3 new classes as a block of code:

    + <font color='green'>.HeaderNavList</font>

    + <font color='green'>.HeaderNavListItem a</font>
    + <font color='green'>.HeaderNavListItem a:hover</font><br>
    <font color='green'>.HeaderNaveListItem a:active</font>

In the <font color='green'>.HeaderNavList</font>, copy the code below...

> Note: In your css code you will see an area to copy a full BLOCK of code like this:
<br>/&#10035; START BLOCK &#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;/
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color=red>PLACE H-3 CODE HERE</font>
<br>/&#10035;&nbsp;END BLOCK ^^^^^^^^^^^^^^^^^^^&#10035;/ 

```css
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
```
...AND make certain you paste it BELOW this *<u>START BLOCK</u>* and *<u>END BLOCK</u>* comment in your index.**css** file:

<br>
Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage0g.jpg">

___

Go back to Chrome and see the results. Notice that the 3 links on the right will to a light gray (#ccc) when you mouse over them. They are also aligned horozontally for our *LAYOUT*.

<br>

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage8.jpg">

___

#### 7. CTA button
<br>

> CTA stands for Call to Action

<br>
Now, let's do something about that "PH CTA" link. Using CSS, we can turn it into a nice blue button. We will copy the below code...<br>


```css
/*-----------------------------------------
The .HeaderNavListItemCTA a properties
------------------------------------------*/
.HeaderNavListItemCTA a {
    color: white;
    background: blue ;
    padding: 0.5rem 1rem;
    border-radius: 8px;
}

```
...AND make certain you paste it BELOW this *<u>H-4 INSERT point - HeaderNavListItemCTA a</u>* comment in your index.**css** file:


> /* H-4 INSERT Point - .HeaderNavListItemCTA a */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage0j.jpg">

___

Again, go see it in your Chrome browser.  

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage10.jpg">

___

- You have completed this part of the Fixed Header.  Later, we will add an image for a logo instead of the PH logo. <br>

- AND add some code to make the "**PH CTA**" a button that wiggles!
___


#### Fixed Header Web Page       <!-- .(20615.01.1 RAM This seems a little out of place --> 
<br>


<span style="font-size: 25px"><b>CONGRATULATIONS!</b></span> You have just added to your Basic Blocks code which built a full web page with a fixed header along with links, a "wiggle" button, and a font-based logo. In the next section, we will add/modify code that will secure the footer with links.   
<br>
Please check your Chrome browser to see your web page thus far.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage12.jpg">


<!--## 6. View Full Code  <!-- {docsify-ignore} -->

<!--
####  [View Full Code For Basic Blocks](/FRApps/code/fr020103_basic-with-fixed-header-code.md "Full Code")
-->


----
### 4. Add Fixed Footer 
----

- Next, we will add to your existing code in both the index.<b>html</b> AND index.<b>css</b> files to continue building on our basic web page *LAYOUT*. 

- We will add some links to the Footer and fix the position of the Footer as we did with the Header.
___

#### index.html

#### 1. <font color='green'>Footer</font> class

- In the <font color='green'>Footer</font> class section we will REPLACE the code within the <br>
&#60;div class="Footer"&#62; & &#60;/div&#62; tags:<br><br>

Copy <font color='green'>Footer</font> code below... 

```html
<div class="Footer">
    <ul class="FooterNavList">
        <li class="FooterNavListItem"><a href=#>PH Link1</a></li>
        <li class="FooterNavListItem"><a href=#>PH Link2</a></li>
    </ul>
</div>
```
...AND make certain you paste it BELOW this *<u>REPLACE Point - Footer</u>* comment in your index.**html** file:


> &#60;!-- REPLACE Point - Footer --&#62;

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage1.jpg">
<br><br>

Good job! Now we move to the index<b>.css</b> file.
___

#### index.css
___


#### 1. .Footer
<br>
First, in the .Footer class:

- CHANGE the <font color=#A81966>position</font>: from relative to <b>fixed</b>
- ADD 
    + <font color=#A81966>z-index</font>: 99; 
    + <font color=#A81966>bottom</font>: 0; 
- REMOVE the <font color=green>top</font> property<br><br>

>  You can comment-out a line of code in CSS with the /* (slash asterisk) at the 
  beginning of the line and an */ (asterisk slash) at the end.<br><br>
  Example:<br>
  <b>/ * top: 10%;</b>  Removed in place of the bottom property*/
  <br><br>But here we will copy and paste the full code

<br>
In the <font color='green'>.Footer</font> class, copy the code below...

```css
/*-----------------------------------------
The .Footer properites
------------------------------------------*/
.Footer {
  background: var(--Footer_background-color);
  width: 100%; 
  /*top: 10%;  Removed in place of the bottom property*/
  bottom: 0;
  position: fixed;
  z-index: 99;
}

```
...AND make certain you paste it BELOW this *<u>FR-1 REPLACE Point - .Footer</u>* comment in your index.**css** file:


> /* FR-1 REPLACE Point - .Footer */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage3.jpg">

<br><br>
Look on your Chrome browser! This fixed the Footer into a stationary position (same as the Header), but we need to fix the links in the center of the Footer. We will force them to be horizontal without the bullets on the left. We will also add the "hover" feature as we did in the Header.
<br>

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage6.jpg">

___

#### 2. .FooterNavList - BLOCK

- Now, let's focus on the links on the left side of the header.  We will be INSERTING 3 new classes in one copy/paste block of code:

    + <font color='green'>.FooterNavList</font><br><br>
    + <font color='green'>.FooterNavListItem a</font><br><br>
    + <font color='green'>.FooterNavListItem a:hover</font><br>
    <font color='green'>.FooterNavListItem a:active</font>

<br>
In the <font color='green'>.FooterNavList</font>, copy the code below...

> Note: In your css code you will see an area to copy a full BLOCK of code like this:
<br>/&#10035; START BLOCK &#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;/
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color=red>PLACE F-1 CODE HERE</font>
<br>/&#10035;&nbsp;END BLOCK ^^^^^^^^^^^^^^^^^^^&#10035;/ 

```css
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
```

...AND make certain you paste it BETWEEN the *<u>START BLOCK</u>*  and *<u>END BLOCK</u>* comment in your index.**css** file:

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage7a.jpg">

___


Again, go see it in your Chrome browser. The links are nicely centered and horozontal, thanks to the CSS "flex" property. 

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage8.jpg">


#### Fixed Footer Web Page       <!-- .(20615.01.1 RAM This seems a little out of place --> 
<br>


<span style="font-size: 25px"><b>CONGRATULATIONS!</b></span> You have just added to your Basic Blocks code which builds a full web page with a secured (fixed) footer, along with links. In the next section, we will add/modify code that will add a text overlay in <font color='green'>Section1</font>.   
<br>
Please check your Chrome browser to see your web page thus far:

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage9.jpg">

___

### 5. Add Text Overlay

- Now, let's focus on the Text Overlay. It will be another <u>P</u>lace <u>H</u>older (PH Text Overlay).  This will require some modifications to your existing code in both the index.<b>html</b> AND index.<b>css</b> files.  

First, the index.<b>html</b> file.

#### index.html

#### 1. <font color='green'>Section1</font> class

- In the <font color='green'>Section1</font> class area we will REPLACE the code within the <br>
&#60;div class="Section1"&#62; & &#60;/div&#62; tags:<br><br>

Copy <font color='green'>Section1</font> code below... 

```html
<div class="Section1">
    <h2 class="Section1ImageText">PH Text Overlay</h2>
</div>
```
...AND make certain you paste it BELOW this *<u>REPLACE point - Section1</u>* comment in your index.**html** file:


> &#60;!-- REPLACE Point - Section1 --&#62;

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicWithImageImage1.jpg">
<br><br>
Notice. in CHROME, the "PH Text Overlay" within the &#60;h2&#62; tags.  This will become our text overlay.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicWithImageImage2.jpg">
<br><br>


Now, we move to the index.<b>css</b> file.

___

#### index.css

#### 1. .Section1ImageText

- We will be INSERTING 2 new classes in one copy/paste block of code:

    + <font color='green'>.Section1ImageText</font><br>
    + <font color='green'>.Section1ImageText::first-letter</font><br>

<br>
In the <font color='green'>.Section1ImageText</font>, copy the code below...

> Note: In your css code you will see an area to copy a full BLOCK of code like this:
<br>/&#10035; START BLOCK &#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;/
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color=red>PLACE S1-1 CODE HERE</font>
<br>/&#10035;&nbsp;END BLOCK ^^^^^^^^^^^^^^^^^^^&#10035;/ 


```css
/*=======================================*/
/* S1-1 INSERT Point - .Section1ImageText */
/*-----------------------------------------
The .Section1ImageText properties
------------------------------------------*/
.Section1ImageText {
    font-size: 3rem;
    font-weight: bolder;
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
```
...AND make certain you paste it BETWEEN the *<u>START BLOCK</u>*  and *<u>END BLOCK</u>* comment in your index.**css** file:

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicWithImageImage5a.jpg">

___
#### Text Overlay
<br>
Check it out in Chrome. <br> 
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLAYOUTImage1.jpg">

___


### 6. Add "Wiggle" Button

#### index.css

#### 1. .HeaderNavListCTA & @keyframes wiggle

- With the use of only CSS code we can make the CTA button wiggle for a few seconds after the page opens or when it has been refreshed.  Again, we will use a Block of code containing 2 classes.

- We will be INSERTING these 2 new classes in one copy/paste block of code:

    + <font color='green'>.HeaderNavListCTA</font><br>
    + <font color='green'>@keyframes wiggle</font>

<br>
In the <font color='green'>.HeaderNavListCTA</font>, copy the code below...

> Note: In your css code you will see an area to copy a full BLOCK of code like this:
<br>/&#10035; START BLOCK &#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;/
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color=red>PLACE H-5 CODE HERE</font>
<br>/&#10035;&nbsp;END BLOCK ^^^^^^^^^^^^^^^^^^^&#10035;/ 

```css
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
```

...AND make certain you paste it BETWEEN the *<u>START BLOCK</u>*  and *<u>END BLOCK</u>* comment in your index.**css** file:

<br>

Like this
<br>

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicBonusImage5d.jpg">

___

#### Wiggle Button

- Now check out the "wiggle" when you refresh your page.  Note the CTA button will wiggle 8 times, 2 seconds after the refresh.  The <font color=#A81966><b>animation</b></font> property controls this motion. Remember, CTA stands for "Call To Action."  The wiggle certainly calls for the reader's attention.


<img class="shadow-border" src="FRApps/assets/images/md-images/BasicWiggleImage1.jpg">

___

### 7. Make Responsive

- A very smart programmer once told me that you code your web page for a hand-held device first, the desk top second.

- This is probably the most important section.  Learn this and you will use these skills to become very accomplished in HTML anf CSS. Go out and research "responsiveness."   

-  First let's look at our current web page on an iPhone7 Plus:

<img class="shadow-border" width=75% src="FRApps/assets/images/md-images/BasicResponsiveImage1.jpg">

___

- We have 2 problems here.
    + The Menu list is too big to properly display
    + All font sizes are too large


#### Developer Tools
<br>
Most all Internet browsers have a wonderful tool called "Developer Tools."

> To get to them, you can go to settings > More Tools > Developer Tools

<br>
Like below:

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicDevToolsImage1.jpg">

> Shortcut to Developer Tools on most browsers is press F12 key.

<br><br>
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicDevToolsImage1b.jpg">


> Example (above image): Click on the drop down and:<br>
    + (1) Select "iPhone IE"<br>
    + (2) Select the little <img src="FRApps/assets/images/md-images/BasicDevToolsIconImage.jpg"> icon <br>
    + (3) Select the "PH Logo" <br>
    + (4) See the information about this element. <br>
    Note the "padding: 0px 0pc 0px 54px;<br><br>
    *CSS padding property goes from (top, right, bottom, left)<br>
    We set only the left property to 54px* (below picture).

<br>
If you recall, when we set the padding-left: 54px; 

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicDevToolsImage3.jpg">
<br><br>

#### NavBar

- Let's focus on the Header and how we want it to appear on a smart phone.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicIPhoneImage1.jpg">

- We can set, using CSS, a certain width of the "viewpoint" to where we can make changes to the appearence.  In our code we will set it at 760px.  At that width we can make the NavList (horizontal links) DISAPPEAR; and a NavBar (commonly known as a hamburger) APPEAR.

- First we need to add the NavBar in both index.html and index.css.

#### index.html

#### HeaderNavBars Class
<br>
In the Header class section we will INSERT this code below the<br> 
"INSERT Point - responsive"
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicResponsiveImage1a.jpg">
<br><br>
Copy HeaderNavBars code below…

```html
<div class="HeaderNavBars">
    <object data="assets/images/hamburger.svg?fill=white"
            type="image/svg+xml" title="Toggle sidebar">
    </object>
</div>
```        
…AND make certain you paste it BELOW this INSERT Point - responsive comment in your index.html file:

> &#60;!-- INSERT Point - responsive --&#62;

<br>
Like this
<br>
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicResponsiveImage2.jpg">
<br><br>
 Take a look at Chrome.  We have successfully added our NavBars.
<br><br>
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicResponsiveImage3.jpg">
<br><br>

> Quick discussion on images.  Note in your assets/images directory you have 3 different images.<br>
    + formr-logo-blue.gif (our logo image)<br>
    + hamburger.svg (the NavBar we are working with now)<br>
    + monaco-blue-soft.jpg (an image we will use later in customization)<br>

<br><br>
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicResponsiveImage4.jpg">



Now let's move on to index.**css** to adjust the NavBar in a proper postion

#### index.css
#### 1. .HeaderNavBars

- We will be INSERTING 2 new classes in one copy/paste block of code:

    + <font color='green'>.HeaderNavBars</font><br>
    + <font color='green'>.HeaderNavBars:focus</font><br>

<br>
In the <font color='green'>.HeaderNavBars</font>, copy the code below...

> Note: In your css code you will see an area to copy a full BLOCK of code like this:
<br>/&#10035; START BLOCK &#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;/
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color=red>PLACE H-1 CODE HERE</font>
<br>/&#10035;&nbsp;END BLOCK ^^^^^^^^^^^^^^^^^^^&#10035;/ 


```css
/*=======================================*/
/* H-1 INSERT Point - .HeaderNavBars */
/*-----------------------------------------
The .HeaderNavBars (hamburger menu) properites
------------------------------------------*/
.HeaderNavBars {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    list-style: none;
    height: 24px;
    width: 24px;
    background: transparent;
    border: none;
    cursor: pointer;
    padding: 0px;
    box-sizing: border-box;
    margin-left: 20px;
    margin-top: 0px;
    align-items: center;
}

/*=======================================*/
/* INSERT Point - .HeaderNavBars:focus */
/*-----------------------------------------
The .HeaderNavBars:focus properites
------------------------------------------*/
.HeaderNavBars:focus {
    outline: none;
}
```
...AND make certain you paste it BETWEEN the *<u>START BLOCK</u>*  and *<u>END BLOCK</u>* comment in your index.**css** file:

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicResponsiveImage5.jpg">

___

Check it out in Chrome.  
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicResponsiveImage6.jpg">

___

#### 2. Responsive CSS Code


####  index.css

#### 1. @media (min-width) &  @media (max-width)

- Here is where the real magic happens.  With the use of @media query we can test the width of the view point of the screen your web page appears.  In our case we will make changes when the screen is greater than or less than 760 pixels. 

- Again, we will use a Block of code containing the 2 queries.

- We will be INSERTING these 2 new queries in one copy/paste block of code:

    + <font color='green'>@media (min-width)</font><br>
    + <font color='green'>@media (max-width)</font>

<br>
In the <font color='green'>/* Responsive Code */</font>, copy the code below...

> Note: In your css code you will see an area to copy a full BLOCK of code like this:
<br>/&#10035; START BLOCK &#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;/
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color=red>PLACE R-1 CODE HERE</font>
<br>/&#10035;&nbsp;END BLOCK ^^^^^^^^^^^^^^^^^^^&#10035;/ 


```css
/* Responsive Code */  
/* R-1 INSERT Point - @media (responsive min-width)*/ 
/*-----------------------------------------
The @media MIN-width query properties
=========================================*/
@media (min-width: 760px) {
    .HeaderNavBars {
      display: none;
    }
    .HeaderLogo {
      margin-left: 45px;
    }
  }
  
  /*=======================================*/
  /* INSERT Point - @media (responsive max-width)*/
  /*-----------------------------------------
  The @media MAX-width query properties
  =========================================*/
  
  @media (max-width: 760px) {
    .HeaderNavList {
        display: none;
    }
    .HeaderLogo {
        font-size: 1rem;
      }    
    .Section1ImageText {
      font-size: 1.5rem;
      padding: 80px 100px 20px 0px;
    }
    .Section2 h2 {
      font-size: 1.7rem;
    }
    .Section2Paragraph {
      font-size: 75%;
    }
  }
```

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicResponsiveImage7.jpg">

___


Check it out in Chrome.

The image on the left is when the Chrome window is greater than 760 pixels wide, the one on the right is less than 760.  That is "responsiveness!"


<img class="shadow-border" src="FRApps/assets/images/md-images/BasicResponsiveDualScreenImage1.jpg">

___

Now, check it out on iPhone 7 Plus. Remember, this is our LAYOUT.  Later, we will see how our CUSTOM web page looks on the iPhone. 

<img class="shadow-border" width="75%" src="FRApps/assets/images/md-images/BasicResponsiveIPhoneImage2.jpg">

___

Compare the 2 (before and after RESPONSIVE queries)

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicResponsiveIPhoneImage3.jpg">

___

#### Final LAYOUT
<br>
<span style="font-size: 25px"><b>CONGRATULATIONS!</b></span>  You have completed your web page *LAYOUT* with a fixed header and footer, links, a CTA button, an image and a text overlay.  All Place Holders in their correct positions.  AND responsive to the width size of the screen it is displayed.  
<br><br>

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFinalLayout.jpg">

<br><br>
You are now ready to *CUSTOMIZE*.  We will work together on our version of a formR web page.  Once complete, please go and *CUSTOMIZE* your own page with a different image, logo and links. 
<br>

####  [View Full Code For HTML Layout](/FRApps/code/fr020101_layout-code.md "Full Code")


___

___


### *CUSTOMIZATION*
----

- As previoused mentioned, we will make some changes to our LAYOUT.<br>We will:

    + Add an image (.jpg) file to Section 1
    + Change the font-based “PH Logo” to our formR logo image (.gif) file
    + Change all of the Place Holder (PH) text
    + Change some colors

- Let’s have some fun. This will require some modifications to your existing code in both the index.html AND index.css files.

___

### 1. Add Image to Section 1
----
- To add some pazzazz to your web site, we will include an image in Section 1.  This will require some modifications to your existing code in the index.<b>css</b> file.  
#### index.css

#### 1. .Section1
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

<!--
> Notice how we are using CSS to add a link to .jpg
file (monaco-blue-soft.jpg) in "images" directory. We are taking advantage of the variable we set in the :root section.
<br>
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicURLImage.jpg">
-->

<br>
In the <font color='green'>.Section1</font> class, copy the code below...

```css
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
    height: 50%;
    position: relative;
    top: 100px;
}
```
...AND make certain you paste it BELOW this *<u>S1R-1 REPLACE point</u>* comment in your index.**css** file:


> /* S1R-1 REPLACE Point - .section1 */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicWithImageImage3.jpg">
<br>

> Variables Discussion:<br><br>In the above .Section CSS code, there were 2 classes that named variables, which were created in the <b>[:root]</b> section at the top the file.<br><br>
The background: was set at<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"var(--Section1_background-image),"<br>
which is blue, as you can see in the [:root] for Section1 section.
<br><br>Also, the background: was set as a URL variable,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"var(--Section1_background-image)."<br>
In the <b>[:root]</b>, this variable was set as 'assets/images/monaco-blue-soft.jpg.'<br><br>Later in the <b><u>Customize</u></b> section, you will find this to be very powerful in changing areas of the web page.<br><br>
<img src="FRApps/assets/images/md-images/BasicWithImageImage3a.jpg">

___

#### Web Page With Image in Section 1
<br>
That's it! Check your Chrome browser for the changes; a nice blue image with the font overlay.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicWithImageImage4.jpg">


### 2. Change To formR Logo
<br>
Now lets add an image in place of the "PH Logo" in the Header. In the "assets/images directory there is a file (formr-logo-blue.gif) that we will add to the left side of the Header.
<br>
<img width=25% src="FRApps/assets/images/md-images/formr-logo.gif">
<br>

- This will require a change in both the index.html and index.css files.

- First the index.html

#### index.html
#### 1. Header
<br>
- In the <font color='green'>Header</font> class section we will REPLACE the code within the <br>
&#60;div class="Header"&#62; & &#60;/div&#62; tags:<br><br>

Copy <font color='green'>Header</font> code below ... 

```html
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
```
...AND make certain you paste it BELOW this *<u>REPLACE point - Header</u>* comment in your index.**html** file:


> &#60;!-- REPLACE Point - Header --&#62;

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicformRImage1.jpg">

___


#### index.css
<br>

#### 1. &#58;root
<br>

- In the <font color='green'>:root</font> section we will MODIFY the following:<br>

    + <b><font color=#A81966>--HeaderLogo-image:</font></b>: url('assets/images/formr-logo-blue.gif'); 
    + <b><font color=#A81966>--HeaderLogo-margin:</font></b>: 0px 0 0 0px;<br><br>

- Copy <font color='green'>:root</font> code below... 

```css
/*-----------------------------------------
:root selector for variables
-------------------------------------------*/
:root {
    --Header_background-color: red;
    --Header_hover-color: white;
    --HeaderLogo-image: url( 'assets/images/formr-logo-blue.gif' );
    --HeaderLogo_margin: 0px 0 0 0px;
    --HeaderList-font-size: 1.2rem;
  
    --Section1_background-color: blue;
    --Section1_background-image: url( 'assets/images/monaco-blue-soft.jpg' );
  
    --Section2_background-color: lightgray;
    --Section2Paragraph-font-color: #ff7034;  /* dark orange */
  
    --Footer_background-color:green;
    --Footer_hover-color: white;
    --FooterList-font-size: .9rem;  
    
    --GlobalFontFamily: "Bookman Old Style", "Frank+Ruhl+Libre:wght@700&display=swap";
} 
```

...AND make certain you paste it BELOW this *<u>root REPLACE Point - :root</u>* comment in your index.**css** file:


> /* root REPLACE Point - :root */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicformRImage2.jpg">

#### 2. .HeaderLogo
<br>

- We will be REPLACING 3 classes...

    + <font color='green'>.HeaderLogo</font>
    + <font color='green'>.HeaderLogo a</font>
    + <font color='green'>.HeaderSpacer</font><br><br>

- ... with 2 classes... 

    + <font color='green'>.HeaderLogo</font>
    + <font color='green'>.HeaderSpacer</font><br><br>

- ...as a block of code:

In the <font color='green'>.HeaderLogo</font>, copy the code below...

> Note: In your css code you will see an area to copy a full BLOCK of code like this:
<br>/&#10035; START BLOCK &#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;/
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color=red>PLACE H-2 CODE HERE</font>
<br>/&#10035;&nbsp;END BLOCK ^^^^^^^^^^^^^^^^^^^&#10035;/ 

```css
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
```
...AND make certain you paste it BELOW this *<u>START BLOCK</u>* and *<u>END BLOCK</u>* comment in your index.**css** file:

<br>
Like this
<br>
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicformRImage3.jpg">

#### Web Page with formR Logo
<br>
<span style="font-size: 25px"><b>CONGRATULATIONS!</b></span>  You have successsfully replaced the "PH Logo" with the image of our formR logo.   
<br><br>
Please check your Chrome browser to see your web page:
<br><br>
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicformRImage4.jpg">

___


### 3. Change Texts

- It is time to replace all of our <u><b>P</b></u>lace <u><b>H</b></u>older text.  We can do this by simply changing the texts in our index.**html** file. We will change the following:

<!--
- Header (Section)
    | Place Holder | New Text  |
    | -------------     | --------- |
    | "PH_Link1"        | "Links"     |
    | "PH_Link2"        | "Cards"     |
    | "PH_Link3"        | "FAQs"      |
    | "PH_CTA"          | "Sign In"   |
------------------------------------
- Section 1
    | Place Holder              | New Text  |
    | -------------         | --------- |
    | "PH Text Overlay"     | "My Image & Text" |
------------------------------------
- Section 2
    + Remove the "PH&#60;br&#62;" above the Paragraph
    | Place Holder  | New Text  |
    | ------------- | --------- |
    | "PH &#60;br&#62;"          | *null*        |    
------------------------------------
- Footer (Section)
    | Place Holder      | New Text  |
    | -------------     | --------- |
    | "PH Link1"        | "Support"     |
    | "PH Link2"        | "Terms Of Use"|
-->

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



___

#### index.html

- Open your index.html file and follow along as we are just going to edit the page, starting with the Header.

#### 1. <font color='green'>Header</font>

- In the &#60;li&#62; tags please make the 4 changes as shown in the below "before" and "after" images.

<span style="font-size: 25px"><b>BEFORE</b></span><br>
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicTextImage1.jpg"><br>
<span style="font-size: 25px"><b>AFTER</b></span><br>
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicTextImage2.jpg">

___

#### 2. <font color='green'>Section 1</font>

- In the &#60;h2&#62; tag please make the 1 change as shown in the below "before" and "after" images.

<span style="font-size: 25px"><b>BEFORE</b></span><br>
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicTextImage3.jpg"><br>
<span style="font-size: 25px"><b>AFTER</b></span><br>
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicTextImage4.jpg">
<br>

___

#### 3. <font color='green'>Section 2</font>

- In the &#60;p&#62; tag please make the 1 change as shown in the below "before" and "after" images. 

- Just remove the PH &#60;br&#62;.

<span style="font-size: 25px"><b>BEFORE</b></span><br>
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicTextImage5.jpg"><br>
<span style="font-size: 25px"><b>AFTER</b></span><br>
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicTextImage6.jpg">
<br>

___

#### 4. <font color='green'>Footer</font>
- In the &#60;li&#62; tags please make the 2 changes as shown in the below "before" and "after" images.

<span style="font-size: 25px"><b>BEFORE</b></span><br>
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicTextImage7.jpg"><br>
<span style="font-size: 25px"><b>AFTER</b></span><br>
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicTextImage8.jpg">
___

#### Web Page with Text Changes
<br>
Now let's see these changes in Chrome.  LOOKS GREAT!

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicTextFinalImage.jpg">
<br><br>
FINALLY, we will CUSTOMIZE with some color changes.

### 4. Change Colors

- We were requested to change some colors for the next major lessons. No problem!
<br>

- This can all be done in the index.**css** file.

#### index.css

#### 1. &#58;root

<br>
First, remember the <font color='green'>:root</font> section.
<br>

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicColorImage1.jpg">

<br><br>
Well, it's very simple to make the requested color changes right here in four of the properties:

- --Header_background-color<br>
    &nbsp;&nbsp;&nbsp;&nbsp;(requested change from red to #FF7034; [dark orange])
- --Section1_background-color  
    &nbsp;&nbsp;&nbsp;&nbsp;(requested change from blue to whitesmoke)
- --Section2_background-color<br>
    &nbsp;&nbsp;&nbsp;&nbsp;(requested change from lightgray to whitesmoke)
- --Footer_background-color<br>
    &nbsp;&nbsp;&nbsp;&nbsp;(requested change from green to #FF7034; [dark orange])
<br><br>

In the <font color='green'>:root</font> section, copy the code below...

```css
/*-----------------------------------------
:root selector for variables
-------------------------------------------*/
:root {
    --Header_background-color: #FF7034;
    --Header_hover-color: white;
    --HeaderLogo-image: url( 'assets/images/formr-logo-blue.gif' );
    --HeaderLogo_margin: 0px 0 0 0px;
    --HeaderList-font-size: 1.2rem;
  
    --Section1_background-color: whitesmoke;
    --Section1_background-image: url( 'assets/images/monaco-blue-soft.jpg' );
  
    --Section2_background-color: whitesmoke;
    --Section2Paragraph-font-color: #ff7034;  /* dark orange */
  
    --Footer_background-color:#FF7034;
    --Footer_hover-color: white;
    --FooterList-font-size: .9rem;  
    
    --GlobalFontFamily: "Bookman Old Style", "Frank+Ruhl+Libre:wght@700&display=swap";
} 

```
...AND make certain you paste it BELOW this *<u>root REPLACE Point - :root</u>* comment in your index.**css** file:


> /* root REPLACE Point - :root */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicColorImage2.jpg">

___
 
- Check it out in Chrome!  NICE!
- So easy and powerful with the <font color='green'>:root</font> variables.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicColorImage3.jpg">

___

There is one last touch for Section 2.  Let's pretty-up that paragraph.  It is done with the class "Section2Paragraph."

#### 2. .Section2Paragraph
<br>

- We will change the font color to that dark orange color we used for the header and footer background colors.
- We will make the first line larger than the rest of the lines.
- Finally we will make the first letter of the first line very large.
- In the <font color='green'>.Section2Paragraph</font> section we will INSERT the following:<br>

    + <b><font color=#A81966>Section2Paragraph</font></b>: 
    + <b><font color=#A81966>Section2Paragraph::first-line</font></b>:
    + <b><font color=#A81966>Section2Paragraph::first-letter</font></b>:

Copy <font color='green'>.Section2Paragraph</font> code below... 

> Note: In your css code you will see an area to copy a full BLOCK of code like this:
<br>/&#10035; START BLOCK &#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;&#10035;/
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color=red>S2-2 INSERT Point - Section2Paragraph</font>
<br>/&#10035;&nbsp;END BLOCK ^^^^^^^^^^^^^^^^^^^&#10035;/ 

```css

/*=======================================*/
/* S2-2 INSERT Point - Section2Paragraph */
/*-----------------------------------------
The .Section2Paragraph properites
------------------------------------------*/
.Section2Paragraph {
    font-family: "Bookman Old Style", sans-serif;
    margin-top: 0px;
    font-size: 1.3rem;
    color: var(--Section2Paragraph-font-color); /* dark orange*/
    font-weight: bolder;
    padding-top: 5rem;
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
```
<br>
...AND make certain you paste it BELOW this *<u>START BLOCK</u>* and *<u>END BLOCK</u>* comment in your index.**css** file:


> /* S2-2 INSERT Point - .Section2Paragraph */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicColorImage4.jpg">

#### Web Page with Color Changes

- Check out Chrome.  

<span style="font-size: 25px"><b>CONGRATULATIONS!!</b></span> 
- You have completed "My HTML Custom App."

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFINALImage.jpg">


#### Final Version With formR logo, text & color changes, "wiggle" button and responsive.

___

- Like the Layout version, your completed custom version is responsive at 760 pixels.  

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicResponsiveDualScreenImage2.jpg">

- And it looks great on an iPhone 7 Plus.

<img class="shadow-border" width=75% src="FRApps/assets/images/md-images/BasicFinaliPhoneImage.jpg">
<br><br>

Now you have all the tools to go back to your Layout and Customize it the way you would like.

- We saved your Layout in the 1c1_my-html-custom-app directory.  The files are:
    + index_final_layout.html
    + index_final_layout.css

- Here:

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicColorImage5.jpg">

> <span style="font-size: 25px"><b>IMPORTANT!</b></span> Remember to change your<br>  "&#60;link rel="stylesheet"    href="index_final_layout.css"&#62;"<br> reference in your index.html file to match the name of your relating index.css file. Like below:
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicColorImage6.jpg">



Your next journey will be to add some very cool functions to our web page using JavaScript.

Happy coding!

<!--## 6. View Full Code  <!-- {docsify-ignore} -->

####  [View Full Code For HTML Custom Apps](/FRApps/code/fr020101_custom-code.md "Full Code")
<br>

<!-- ------------------------------------------------------------------------- -->

<div class="page-back">

[BACK - Website SSL](/Setup/fr0306_Setup-Website-SSL-Ubuntu.md)
</div><div class="page-next">

[Custom FRApps React - NEXT](/Setup/fr0105_Custom-FR-Apps-React.md)
</div><br>
