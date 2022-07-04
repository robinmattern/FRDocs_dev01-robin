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

You will find in VSCode a folder "0c1_my-basic-blocks."  In this folder are the empty index.<b>html</b> and index.<b>css</b> files, along with a favicon.png image file. There is an "assets" folder that holds an "images" folder with the needed images to build your final project for this HTML Custom App course.

___

<img class="shadow-border" src="FRApps/assets/images/md-images/IntroductionImage1.jpg">

___


- Your Final Web Site Preview
<br>
The below preview will have a fixed (secured) header and footer, navigation links and a "wiggle" button, an image with a font-based overlay, and a formR logo.
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


----
### 1. Basic Blocks
----

- We will begin this Custom App by simply copying & pasting the code below into  your empty html and css files.  The results will be 4 very basic blocks that sit on top of each other.  Let's start by reviewing the files in your [repos]itory.


#### 1. Review Files

-  Using VSCode, in a folder called "0c1_my-basic-blocks", open:
    - index.<b>html</b> and
    - index.<b>css</b>
    
Both should be empty.

#### 2. Code - index.html

<br>

> <span style="font-size: 25px"><b>SHORTCUT</b></span><br>
Mouse over the "HTML" in the upper right corner of the code block to quickly copy all the code.
<img src="FRApps/assets/images/md-images/BasicBlocksImage0a.jpg">
<img src="FRApps/assets/images/md-images/BasicBlocksImage0.jpg">

- Click on and open the index.<b>html</b> file from VSCode. Copy and paste the entire below code to Line 1 of the empty index.<b>html</b> file:

```HTML
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="ie=edge">
        <title>HTML Custom Apps</title>
        <link rel="shortcut icon" href="favicon.png">
        <link rel="stylesheet"    href="https://fonts.googleapis.com/css?family=Bookman Old Style" >
        <link rel="stylesheet"    href="index.css">
    </head>
    <body>
        <!-- REPLACE Point - header -->
        <div class="header">
            <h2>header</h2>
        </div>
        <!-- INSERT Point - mobile nav -->
        <!-- REPLACE Point - section1 -->
        <div class="section1">
           <h2>section 1</h2>
        </div>
        <div class="section2">
            <h2>section 2</h2>
        </div>
        <!-- REPLACE Point - footer -->
        <div class="footer">
            <h2>footer</h2>
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

> <span style="font-size: 25px"><b>SHORTCUT</b></span><br>
The css code can be quickly and fully copied the same way you did above with the html code. <br>
<img src="FRApps/assets/images/md-images/BasicLargeBlocksImage0.jpg">

```css
/* Basic Blocks Custom App */
@import url('https://fonts.googleapis.com/css?family=Bookman Old Style');

/* REPLACE Point - Root Variables */
/*-----------------------------------------
:root selector for variables
-------------------------------------------*/
:root {
    --header-color: red;
    --section1-color: blue;
    --section2-color: lightgray;
    --footer-color: green;
    --h2-text-color-light: white;
    --h2-text-color-dark: black;
    --nav-list-item-hover-color: white;
    --h2-font-size: 1.5rem;
    --nav-list-font-size: 1.2rem;
    --footer-list-font-size: .9rem;
} 

/*-----------------------------------------
The html properites
------------------------------------------*/
html {
    background: #b3b3b3;
    height: 100%;
    text-align: center;
}

/* REPLACE Point - Body */
/*-----------------------------------------
The body properites
------------------------------------------*/
body {
    background: white;
    height: 100%;
    margin: 0;
}

/* REPLACE Point - h2 */
/*-----------------------------------------
<h2> tag properties
-------------------------------------------*/
h2 {
    margin: 0;
    font-size: var(--h2-font-size) ;
    color: var(--h2-text-color-light);
    padding: 1.5rem;
    text-align: center;
  }

/* REPLACE point - .header */
/*-----------------------------------------
The .header properites
------------------------------------------*/
.header {
    background: var(--header-color);
    width: 300PX;
    height: 100PX;
    position: relative;
}

/* INSERT Point - .formr-logo */

/* INSERT Point - .header-logo */

/* INSERT Point - .header-logo:first-letter */

/* INSERT Point - .nav-list */

/* INSERT Point - .nav-list-item a */

/* INSERT Point - .nav-list-item a:hover
                  .nav-list-item a:active */

/* INSERT Point - .nav-list-item-cta a */

/* INSERT Point - .nav-list-item-cta */

/* INSERT Point - @keyframes wiggle */

/* INSERT Point - .header h2 */
/* DELETE Point - .header h2 */

/* REPLACE Point - section1 */
/*-----------------------------------------
The .section1 properites
------------------------------------------*/
.section1 {
    background: var(--section1-color);
    width: 300PX;
    height: 100PX;
    position: relative;
}

/* INSERT Point - .image-text */

/* INSERT Point - .image-text::first-letter */

/* REPLACE Point - section2 */
/*-----------------------------------------
The .section2 properites
------------------------------------------*/
.section2 {
    background: var(--section2-color);
    width: 300PX;
    height: 100PX;
    position: relative;
}

/* INSERT Point - section2 h2 */
/* DELETE Point - section2 h2 */

/* REPLACE Point - footer */
/*-----------------------------------------
.footer properites
------------------------------------------*/
.footer {
    background: var(--footer-color);
    width: 300PX;
    height: 100PX;
    position: relative;
}

/* INSERT Point - footer h2 */
/* DELETE Point - footer h2 */

/* INSERT Point - .footer-text */

/* INSERT Point - .footer-list */

/* INSERT Point - .footer-list-item a */

/* INSERT Point - .footer-list-item a:hover
                  .footer-list-item a:active */

/* INSERT Point - All Responsive Code */                  

/* END */
```

___


#### 4.  Basic Blocks Web Page      

- Please check your Chrome browser. 

<br>
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicBlocksImage3.jpg"><br><br>

> We will build from this basic page to create a web site with a fixed header and footer, links with a "wiggle" button, and an image with a text overlay.<br><br>
From there, the next course we will move on to add some magic with JavaScript (JS) to this web page.

___

#### 5. Understanding CSS        <!-- .(20615.01.2 RAM Changed to ### 4. Was #### --> 
<br>
To understand a little of this CSS code, let's look at the .header properties.
<br>
<br>
<font color='green'>** Notes:</font>
<br>

```css
/*-----------------------------------------
The .header properites
------------------------------------------*/
.header {
    background: var(--header-color);
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

#### 6.  [View Full Code For Basic Blocks](/FRApps/code/fr020101_basic-blocks-code.md "Full Code")

- <span style="font-size: 20px"><b>CONGRATULATIONS!!</b></span> You have just created a simple html page with a cascading style sheet (CSS) which makes 4 *basic blocks.*  


----
### 2. Large Blocks  
----

- Next, we will add to your existing code in the index.<b>css</b> file to continue building on our basic web page.
<br><br>
Note: The index.**html** file will remain unchanged.

#### 1. index.css - Body

- Body

In the <font color='green'>body</font> section we will ADD the following:<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<b><font color=#A81966>width</font></b>: 100%; 

Copy <font color='green'>body</font> code below... 

```css
/*-----------------------------------------
The body properites
------------------------------------------*/
body {
    background: white;
    height: 100%;
    width: 100%;
    margin: 0;
}

```
...AND make certain you paste it BELOW this *<u>REPLACE point</u>* comment in your index.**css** file:


> /* REPLACE Point - Body */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage1.jpg">

___


#### 2. .header &#60;h2&#62; Override


- We must override (OvR) the padding for this &#60;h2&#62; tag in the <font color='green'>.header</font> & <font color='green'>.footer</font> with the following, placed under each, respectively.

Copy the <font color='green'>. header h2</font> below...

```css
/*-----------------------------------------
The .header h2 override properties
------------------------------------------*/
.header h2 {
    padding: 1rem;
}

```
...AND make certain you paste it BELOW this *INSERT Point/DELETE Point* comment in your index.**css** file:

> /* INSERT Point - .header h2 */
<br>
  /* DELETE Point - .header h2 */

<br>

Like this:

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage3.jpg">

___

#### 3. .footer &#60;h2&#62; Override

- AND<font color='green'>.footer</font> class.

Copy the <font color='green'>. footer h2</font> below...

```css
/*-----------------------------------------
The .footer h2 override properties
------------------------------------------*/
.footer h2 {
    padding: 1rem;
}

```
...AND make certain you paste it BELOW this *INSERT Point/DELETE Point* comment in your index.**css** file:

> /* INSERT Point - .footer h2 */
<br>
  /* DELETE Point - .footer h2 */

<br>

Like this:

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage4.jpg">

___

#### 4. .section2 &#60;h2&#62; Override

- We must override (OvR) the font color for this &#60;h2&#62; tag in the <font color='green'>.section2</font> with the following:

Copy the below code block and paste it below this... 

```css
/*-----------------------------------------
The .section2 h2 properites
------------------------------------------*/
.section2 h2 {
    color: var(--h2-text-color-dark);
}

```
...AND make certain you paste it BELOW this *INSERT Point/DELETE Point* comment in your index.**css** file:

> /* INSERT Point - .section2 h2 */<br>
  /* DELETE Point - .section2 h2 */

Like this:
<br>
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage4e.jpg">

___

#### 5. .header
<br>

- In the <font color='green'>.header</font> section we will MODIFY the following:<br>

    + <b><font color=#A81966>width</font></b>: 100%; 
    + <b><font color=#A81966>height</font></b>: 10%;

Copy <font color='green'>.header</font> code below... 

```css
/*-----------------------------------------
The .header properites
------------------------------------------*/
.header {
    background: var(--header-color);
    width: 100%; /*was 300px*/
    height: 10%; /*was 100px*/
    position: relative;
}
```
...AND make certain you paste it BELOW this *<u>REPLACE point</u>* comment in your index.**css** file:


> /* REPLACE Point - .header */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage4a.jpg">

___


#### 6. .section 1 & 2

- In <font color='green'>section1</font> <b>AND</b> <font color='green'>section2</font>, CHANGE

    + <b><font color=#A81966>width</font></b> to 100%  
    + <b><font color=#A81966>height</font></b> to 40%
<br>

___

<font color='green'><u>section1</u></font>

- Copy <font color='green'>.section1</font> code below... 

```css
The .section1 properites
------------------------------------------*/
.section1 {
    background: var(--section1-color);
    width: 100%; /*was 300px*/
    height: 40%; /*was 100px*/
    position: relative;
}

```

...AND make certain you paste it BELOW this *<u>REPLACE point</u>* comment in your index.**css** file:


> /* REPLACE Point - .section1 */

<br>
Like this
<br><br>

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage4b.jpg">

___

<font color='green'><u>section2</u></font>

- Copy <font color='green'>.section</font> code below... 

```css
The .section2 properites
------------------------------------------*/
.section2 {
    background: var(--section2-color);
    width: 100%; /*was 300px*/
    height: 40%; /*was 100px*/
    position: relative;
}

```

...AND make certain you paste it BELOW this *<u>REPLACE point</u>* comment in your index.**css** file:


> /* REPLACE Point - .section2 */

<br>
Like this
<br><br>

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage4c.jpg">

___

#### 7. .footer
<br>

- In the <font color='green'>.footer</font> section we will ADD the following:<br>

    + <b><font color=#A81966>width</font></b> to 100% <br>AND 
    + <b><font color=#A81966>height</font></b> to 10%

Copy <font color='green'>.footer</font> code below... 

```css
/*-----------------------------------------
The .footer properites
------------------------------------------*/
.footer {
    background: var(--footer-color);
    width: 100%; /*was 300px*/
    height: 10%; /*was 100px*/
    position: relative;
}
```
...AND make certain you paste it BELOW this *<u>REPLACE point</u>* comment in your index.**css** file:


> /* REPLACE Point - .footer */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage4d.jpg">

___


#### 8. Large Blocks Web Page       <!-- .(20615.01.1 RAM This seems a little out of place --> 
- Please check your Chrome browser to see your web page so far.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage5.jpg">

<br><br>
<span style="font-size: 25px"><b>CONGRATULATIONS</b></span>! You have built a full page with four distinct blocks using your Basic Blocks index.<b>css</b> code. In the next section. we will add/modify code to secure (fix) the header in one spot.   
<br>

<!--## 6. View Full Code  <!-- {docsify-ignore} -->

#### 9. [View Full Code For Basic Blocks](/FRApps/code/fr020102_basic-large-blocks-code.md "Full Code")

___

----
### 3. Fixed Header 
----

- Next, we will add to your existing code in  both index.<b>html</b> AND index.<b>css</b> files to continue building on our basic web page.

___

#### index.html

#### 1. <font color='green'>header</font> class
<br>

- In the <font color='green'>header</font> class section we will REPLACE the code within the <br>
&#60;div class="header"&#62; & &#60;/div&#62; tags:<br><br>

Copy <font color='green'>header</font> code below... 

```html
<div class="header">
    <span class="header-logo">My Logo</span>
    <ul class="nav-list">
        <li class="nav-list-item"><a href=#>Links</a></li>
        <li class="nav-list-item"><a href=#>Cards</a></li>
        <li class="nav-list-item"><a href=#>FAQs</a></li>
        <li class="nav-list-item-cta"><a href=#>Sign In</a></li>
    </ul>
</div>
```
...AND make certain you paste it BELOW this *<u>REPLACE point</u>* comment in your index.**html** file:


> &#60;!-- REPLACE Point - header --&#62;

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage1.jpg">
<br><br>
Great! Now we move to the index**.css** file.

___


#### index.css

___

#### 1. .header
<br>
First and foremost in the <font color='green'>.header</font> section we will CHANGE & ADD the following:<br>

- CHANGE the <font color=#A81966>position</font>: from relative to <b>fixed</b>
- ADD 
    + <font color=#A81966>z-index</font>: 100; 
    + <font color=#A81966>display</font>: flex; 
    + <font color=#A81966>justify-content</font>: space-between;

Copy <font color='green'>.header</font> code below... 

```css
/*-----------------------------------------
The .header properites
------------------------------------------*/
.header {
    background: var(--header-color);
    width: 100%;
    height: 10%;
    position: fixed;  /*was relative*/
    z-index: 100;
    display: flex;
    justify-content: space-between;
}

```
...AND make certain you paste it BELOW this *<u>REPLACE point</u>* comment in your index.**css** file:


> /* REPLACE Point - .header */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage1b.jpg">

___

#### 2. .header h2
<br>

- When we made the changes within the &#60;div class="header"&#62; & &#60;/div&#62; tags in the index.**html** we removed the &#60;h2&#62; tag.  We now do not need the .header h2 class in our index.**css** file.


Go there and delete the entire code block.

```css
/* INSERT Point - .header h2 */
/* DELETE Point - .header h2 */
/*-----------------------------------------
The .header h2 override properties
------------------------------------------*/
.header h2 {
    padding: 1rem;
}
```

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage2.jpg">

___

Look at your Chrome browser! The above steps "fixed" the header into a stationary position.

We still need to:

1. Get rid of the "Unwanted Space" at the bottom 
2. Fix the "My Logo" in the left corner of the header.
3. Fix the links in the right corner of the header 


<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage3.jpg">
<br><br>
To handle the Unwanted Space, we need to adjust Sections 1 & 2 and the Footer.  It's easy, we will 'code' each to have a <font color=#A81966>top</font> of 10%.  
<br><br>

ADD 
- <font color=#A81966>top</font>: 10%;

at the bottom of <font color=green>.section1</font>, <font color=green>.section2</font> and <font color=green>.footer</font>

&nbsp;&nbsp;&nbsp;&nbsp;AND

MODIFY in <font color=green>section1</font> & <font color=green>section2</font> to: 

- <font color=#A81966>height</font>: 50%;

Let's start with <font color=green>.section1</font> below.
___

#### 3. .section1

- In the <font color='green'>.section1</font> class, copy the code below...

```css
/*-----------------------------------------
The .section1 properites
------------------------------------------*/
.section1 {
    background: var(--section1-color);
    width: 100%;
    height: 50%;
    position: relative;
    top:10%; /*<---ADD to adjust the top position*/
}

```
...AND make certain you paste it BELOW this *<u>REPLACE point</u>* comment in your index.**css** file:


> /* REPLACE Point - .section1 */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage0a.jpg">

___
#### 4. .section2

- In the <font color='green'>.section2</font> class, copy the code below...

```css
/*-----------------------------------------
The .section2 properites
------------------------------------------*/
.section2 {
    background: var(--section2-color);
    width: 100%;
    height: 50%;
    position: relative;
    top:10%; /*<---ADD to adjust the top position*/
}

```
...AND make certain you paste it BELOW this *<u>REPLACE point</u>* comment in your index.**css** file:


> /* REPLACE Point - .section2 */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage0b.jpg">

___

#### 5. .footer

- In the <font color='green'>.footer</font> class, copy the code below...

```css
/*-----------------------------------------
The .footer properites
------------------------------------------*/
.footer {
    background: var(--footer-color);
    width: 100%;
    height: 10%;
    position: relative;
    top:10%; /*<---ADD to adjust the top position*/
}

```
...AND make certain you paste it BELOW this *<u>REPLACE point</u>* comment in your index.**css** file:


> /* REPLACE Point - .footer */

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


#### 6. .header-logo

- Now, let's fix that ugly "My Logo" on the left side of the header. To do this, we add some new classes to our CSS file.
<br>

Copy and paste the following 2 classes, and place below respective /*REPLACE Point*/ markers.
<br><br>
First <font color='green'>.header-logo</font> class. Copy the below code and paste it below: 
<br><br>

> /* INSERT Point - .header-logo*/


```css
/*-----------------------------------------
The .header-logo properites
------------------------------------------*/
.header-logo {
    font-family: "Bookman Old Style", sans-serif;
    font-size: 30px;
    font-weight: bolder;
    color: blue;
    text-shadow: 2px 2px 12px #000000;
    padding-left: 20px;
}
```

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage0d.jpg">

___


- Next <font color='green'>.header-logo::first-letter</font> class. Copy the below code and paste it below: 
<br>

> /* INSERT Point - .header-logo::first-letter*/


```css
/*-----------------------------------------
The .header-logo::first-letter properites
------------------------------------------*/

.header-logo::first-letter {
    font-size: 150%;
    color: cornflowerblue;
}
```

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage0e.jpg">

___

Now check Chrome
<br>

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage5.jpg">

___


This takes the boring "My Logo" and turns it into a nice "font-based" logo (with large shadowed blue letters and a lighter blue first letter).  Note the font is one of Google's special fonts, called "Bookman Old Style."  We linked to that from the very top of the index.<b>css</b> file.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage6.jpg">

___

#### 7. header nav-bar


- Now, let's focus on the stack of links on the right side of the header.  

- We will be INSERTING 3 new classes:

    + <font color='green'>.nav-list</font>

    + <font color='green'>.nav-list-item a</font>
    + <font color='green'>.nav-list-item a:hover</font><br>
    <font color='green'>.nav-list-item a:active</font>

In the <font color='green'>.nav-list</font>, copy the code below...

```css
/*-----------------------------------------
The .nav-list properites
------------------------------------------*/
.nav-list {
    list-style: none;
    margin-right: 30px;
    padding: 0;
    display: flex;
    flex-direction: row;
    align-items: center;
    font-size: var(--nav-list-font-size);
}

```
...AND make certain you paste it BELOW this *<u>REPLACE point</u>* comment in your index.**css** file:


> /* INSERT Point - .nav-list */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage0g.jpg">

___

- In the <font color='green'>.nav-list-item a</font>, copy the code below...

```css
/*-----------------------------------------
The .nav-list-item a properites
------------------------------------------*/
.nav-list-item a {
    color: black;
    font-weight: bold;
    text-decoration: none;
    margin: 8px 0;
    padding: 25px;
}

```
...AND make certain you paste it BELOW this *<u>REPLACE point</u>* comment in your index.**css** file:


> /* INSERT Point - .nav-list-item a */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage0h.jpg">

___


- In the 

    + <font color='green'>.nav-list-item a:hover,</font><br>
    <font color='green'>.nav-list-item a:active</font> 

copy the code below...

```css
/*-----------------------------------------
The .nav-list-item a properites
------------------------------------------*/
.nav-list-item a:hover,
.nav-list-item a:active {
    color: var(--nav-list-item-hover-color);
}

```
...AND make certain you paste it BELOW this *<u>INSERT point</u>* comment in your index.**css** file:


> /* INSERT Point - .nav-list-item a:hover<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
.nav-list-item a:active */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage0i.jpg">

___

Go back to Chrome and see the results. Notice that the 3 links on the right will to a light gray (#ccc) when you mouse over them. They are also aligned side-by-side properly.

<br>

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage8.jpg">

___

#### 8. cta button
<br>

> cta stands for Call to Action

<br>
Now, let's do something about that "Sign In" link. Using CSS, we can turn it into a nice blue button. We will copy the below code...<br>


```css
/*-----------------------------------------
The .nav-list-item-cta a properties
------------------------------------------*/
.nav-list-item-cta a {
    color: white;
    background: blue ;
    padding: 0.5rem 1rem;
    border-radius: 8px;
}

```
...AND make certain you paste it BELOW this *<u>INSERT point</u>* comment in your index.**css** file:


> /* INSERT Point - .nav-list-item-cta a */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage0j.jpg">

___

Again, go see it in your Chrome browser.  

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage10.jpg">

___

You have completed this part of the Fixed Header.  Later, we will add an image for a logo instead of the font-based logo. <br>
<img src="FRApps/assets/images/md-images/BasicFixedHeaderImage11.jpg">

AND add some code to make the "**Sign In**" button wiggle!
___


#### Fixed Header Web Page       <!-- .(20615.01.1 RAM This seems a little out of place --> 
<br>


<span style="font-size: 25px"><b>CONGRATULATIONS!</b></span> You have just added to your Basic Blocks code which built a full web page with a fixed header along with links, a "wiggle" button, and a font-based logo. In the next section, we will add/modify code that will secure the footer with links.   
<br>
Please check your Chrome browser to see your web page thus far.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage12.jpg">

___

<!--## 6. View Full Code  <!-- {docsify-ignore} -->

####  [View Full Code For Basic Blocks](/FRApps/code/fr020103_basic-with-fixed-header-code.md "Full Code")

___

----
### 4. Fixed Footer 
----

- Next, we will add to your existing code in both the index.<b>html</b> AND index.<b>css</b> files to continue building on our basic web page. We will add some links to the footer and "secure" the position of the footer as we did with the header.
___

#### index.html

#### 1. <font color='green'>footer</font> class

- In the <font color='green'>footer</font> class section we will REPLACE the code within the <br>
&#60;div class="footer"&#62; & &#60;/div&#62; tags:<br><br>

Copy <font color='green'>footer</font> code below... 

```html
<div class="footer">
    <ul class="footer-list">
        <li class="footer-list-item"><a href=#>Support</a></li>
        <li class="footer-list-item"><a href=#>Terms Of Use</a></li>
    </ul>
</div>
```
...AND make certain you paste it BELOW this *<u>REPLACE point</u>* comment in your index.**html** file:


> &#60;!-- REPLACE Point - footer --&#62;

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage1.jpg">
<br><br>

Good job! Now we move to the index<b>.css</b> file.


___

#### index.css

___


#### 1. footer
<br>
First, in the .footer class:

- CHANGE the <font color=#A81966>position</font>: from relative to <b>fixed</b>
- ADD 
    + <font color=#A81966>z-index</font>: 99; 
    + <font color=#A81966>bottom</font>: 0; 
- REMOVE the <font color=green>top</font> property<br><br>
  You can comment-out a line of code with the /* (slash asterisk) at the 
  beginning of the line and an */ (asterisk slash) at the end.<br><br>
  Example:<br>
  <b>/ * top: 10%;</b>  Removed in place of the bottom property*/

In the <font color='green'>.footer</font> class, copy the code below...

```css
/*-----------------------------------------
The .footer properites
------------------------------------------*/
.footer {
  background: var(--footer-color);
  width: 100%; 
  /*top: 10%;  Removed in place of the bottom property*/
  bottom: 0;
  position: fixed;
  z-index: 99;
}

```
...AND make certain you paste it BELOW this *<u>REPLACE point</u>* comment in your index.**css** file:


> /* REPLACE Point - .footer */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage3.jpg">

___

Also, we can remove the <font color='green'>.footer h2</font> class.  It is not needed because we replaced the &#60;h2&#62; tag with a &#60;ul&#62; tag in the index.<b>html</b> file.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage4.jpg">

___


Look on your Chrome browser! This "secured" the footer into a stationary position, but we need to fix the links in the left corner of the footer.


<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage6.jpg">

___

#### 2. nav-links

- Now, let's focus on the links on the left side of the header.  We will be INSERTING 4 new classes:

    + <font color='green'>.footer-text</font>

    + <font color='green'>.footer-list</font>
    + <font color='green'>.footer-list-item a</font>
    + <font color='green'>.footer-list-item a:hover</font><br>
    <font color='green'>.footer-list-item a:active</font>

<br>
We can do these quickly one at time.  

#### 3. .footer-text
<br>
For  <font color='green'>.footer-text</font> copy the below...


```css
/*-----------------------------------------
The .footer-text properties
------------------------------------------*/
.footer-text {
  font-size: x-large;
  text-align: right;
  padding: 0px 30px 0px 65%;
}
```

...AND make certain you paste it BELOW this *<u>INSERT point</u>* comment in your index.**css** file:


> /* INSERT Point - .footer-text */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage7a.jpg">

___

#### 4. .footer-list
<br>
For  <font color='green'>.footer-list</font> copy the below...


```css
/*-----------------------------------------
The .footer-list properties
------------------------------------------*/
.footer-list {
    list-style: none;
    margin: 20px;
    padding: 0;
    display: flex;
    flex-direction: row;
    justify-content: center;
    font-size: var(--footer-list-font-size);
  }
```

...AND make certain you paste it BELOW this *<u>INSERT point</u>* comment in your index.**css** file:


> /* INSERT Point - .footer-list */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage7b.jpg">

___

#### 5. .footer-list-item
<br>
For  <font color='green'>.footer-list-item a</font> copy the below...

```css
/*-----------------------------------------
The .footer-list-item a properties
------------------------------------------*/
.footer-list-item a {
    color: black;
    font-weight: bold;
    text-decoration: none;
    margin: 8px 0;
    padding: 12px;
  }
```

...AND make certain you paste it BELOW this *<u>INSERT point</u>* comment in your index.**css** file:


> /* INSERT Point - .footer-list-item a */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage7c.jpg">

___

#### 6. .footer-list-item a:hover
<br>

For  
- <font color='green'>.footer-list-item a:hover</font><br> 
<font color='green'>.footer-list-item a:active</font> 

copy the below...


```css
/*-----------------------------------------
The .footer-list-item a:hover,
    .footer-list-item a:active properties
------------------------------------------*/
.footer-list-item a:hover,
.footer-list-item a:active {
  color: var(--nav-list-item-hover-color);
}
```
...AND make certain you paste it BELOW this *<u>INSERT point</u>* comment in your index.**css** file:


> /* INSERT Point - .footer-list-item a:hover<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
.footer-list-item a:active */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage7d.jpg">

___

Again, go see it in your Chrome browser. The links are nicely centered and side-by-side, thanks to the CSS "flex" property. 

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage8.jpg">


#### 3. Fixed Footer Web Page       <!-- .(20615.01.1 RAM This seems a little out of place --> 
<br>


<span style="font-size: 25px"><b>CONGRATULATIONS!</b></span> You have just added to your Basic Blocks code which builds a full web page with a secured footer along with links. In the next section, we will add/modify code that will add an image and text overlay in <font color='green'>section1</font>.   
<br>
Please check your Chrome browser to see your web page thus far:

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage9.jpg">



####  [View Full Code For Basic Blocks](/FRApps/code/fr020104_basic-with-fixed-footer-code.md "Full Code")

___


----
### 5. With Image
----

- To add magic to your web site, we will include an image and text overlay.  This will require some modifications to your existing code in both the index.<b>html</b> AND index.<b>css</b> files.  

First, the index.<b>html</b> file.
___

#### index.html

#### 1. <font color='green'>section1</font> class

- In the <font color='green'>section1</font> class area we will REPLACE the code within the <br>
&#60;div class="section1"&#62; & &#60;/div&#62; tags:<br><br>

Copy <font color='green'>section1</font> code below... 

```html
        <div class="section1">
            <h2 class="image-text">My Image & Text</h2>
        </div>
```
...AND make certain you paste it BELOW this *<u>REPLACE point</u>* comment in your index.**html** file:


> &#60;!-- REPLACE Point - section1 --&#62;

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicWithImageImage1.jpg">
<br><br>
Notice. in CHROME, the "My Image & Text" within the &#60;h2&#62; tags.  This will become our text overlay.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicWithImageImage2.jpg">
<br><br>
Now, we move to the index.<b>css</b> file.

___

#### index.css

#### 1. .section1
<br>
This is where there is a large change to the .section1 code below.

- CHANGE the <font color=#A81966>background</font>: to include a url
- ADD 
    + <font color=#A81966>background-color</font>: blue; 
    + <font color=#A81966>background-repeat</font>: no-repeat; 
    + <font color=#A81966>background-size</font>: cover; 
    + <font color=#A81966>background-position</font>: center; 

> Notice how we are using CSS to add a link to .jpg
file (monaco-blue-soft.jpg) in "images" directory.
Please Google the other properties to see how they
allow to properly position the image.

<br>
In the <font color='green'>.section1</font> class, copy the code below...

```css
/*-----------------------------------------
The .section1 properites
------------------------------------------*/
.section1 {
  background: url("assets/images/monaco-blue-soft.jpg");
  background-color: blue;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  width: 100%;
  height: 50%;
  position: relative;
  top: 10%; 
}

```
...AND make certain you paste it BELOW this *<u>REPLACE point</u>* comment in your index.**css** file:


> /* REPLACE Point - .section1 */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicWithImageImage3.jpg">

___


Again, check your Chrome browser for the change; a nice blue image with the font overlay.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicWithImageImage4.jpg">

___


#### 2. .image-text

- For the <font color='green'>.image-text</font> class, copy the code below...

```css
/*-----------------------------------------
The .image-text properties
------------------------------------------*/
.image-text {
  font-family: "Bookman Old Style", sans-serif;
  font-size: 3rem;
  font-weight: bolder;
  color: blue;
  text-shadow: 2px 2px 12px #000000;
  padding: 80px 400px 20px 0px;
}


```
...AND make certain you paste it BELOW this *<u>INSERT point</u>* comment in your index.**css** file:


> /* INSERT Point - .image-text */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicWithImageImage5a.jpg">

___

#### 3. .image-text::first-letter

- For the <font color='green'>.image-text::first-letter</font> class, copy the code below...

```css
/*-----------------------------------------
The .image-text::first-letter properties
------------------------------------------*/
.image-text::first-letter {
  font-size: 150%;
  color: cornflowerblue;
}
```
...AND make certain you paste it BELOW this *<u>INSERT point</u>* comment in your index.**css** file:


> /* INSERT Point - .image-text::first-letter */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicWithImageImage5b.jpg">

___


#### With Image Web Page       <!-- .(20615.01.1 RAM This seems a little out of place --> 
<br>


<span style="font-size: 25px"><b>CONGRATULATIONS!</b></span>  You have <i><u>almost</u></i> completed your web page with a fixed header and footer, links, a "wiggly" button, an image, and a text overlay.   
<br>
Please check your Chrome browser to see your web page:


<img class="shadow-border" src="FRApps/assets/images/md-images/BasicWithImageImage6.jpg">

___


In the final section, we will change the font-based logo to a formR logo image file AND we will change the color of the blocks on the web page.  


<img src="FRApps/assets/images/md-images/formr-logo.gif">


<br>
<!--## 6. View Full Code  <!-- {docsify-ignore} -->

####  [View Full Code For Basic w/ Image](/FRApps/code/fr020105_basic-with-image-code.md "Full Code")

___


----
### 6. FINAL  

- As previoused mentioned, we will make some changes.  First, the font-based "My Logo" will be changed to our formR logo image file. We will also add some code to the index.**css** file to animate the "Sign In" button.  AND finally, because the next author would like to work with diffent colors for the blocks, we can easily change them.  

- Let's have some fun. This will require some modifications to your existing code in both the index.<b>html</b> AND index.<b>css</b> files.  

First, the index.<b>html</b> file.
___

#### index.html

#### 1. Replace logo

- In the index.<b>html</b> file we will change the header class to include a link to our formR logo and at the same time comment-out the "My Logo" &#60;span&#62; tag.
<br><br>

Copy the below code and...

```html
<div class="header">
    <img class="formr-logo" src="assets/images/formr-logo.gif"/>
    <!--<span class="header-logo">My Logo</span>-->
```


...AND make certain you paste it BELOW this *<u>REPLACE point</u>* comment in your index.**html** file:

> &#60;!-- REPLACE Point - header --&#62;

<br>
<img src="FRApps/assets/images/md-images/BasicBonusImage1.jpg">

___

#### index.css

#### 1. .formr-logo

- In the <font color='green'>.formr-logo</font> class, copy the code below...

```css
/*-----------------------------------------
The .formr-logo properites
------------------------------------------*/
.formr-logo {
  width: 210px;
  height: 60px;
  padding-left: 20px;
  padding-top: 10px;
}
```
...AND make certain you paste it BELOW this *<u>INSERT point</u>* comment in your index.**css** file:


> /* INSERT Point - .formr-logo */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicBonusImage3.jpg">

___


The web page should look like this.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicBonusImage4.jpg">

___

#### 2. Color Changes

- We were requested to change some colors for the next major lessons. No problem!
<br>

First, remember the <font color='green'>:root</font> in our index.<b>css</b> file.
<br>

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicBonusImage5a.jpg">

<br><br>
Well, it's very simple to make the requested color changes right here in four of the properties:

- --header-color<br>
    &nbsp;&nbsp;&nbsp;&nbsp;(requested change from red to #FF7034; [dark orange])
- --section1-color  
    &nbsp;&nbsp;&nbsp;&nbsp;(requested change from blue to whitesmoke)
- --section2-color<br>
    &nbsp;&nbsp;&nbsp;&nbsp;(requested change from lightgray to whitesmoke)
- --footer-color<br>
    &nbsp;&nbsp;&nbsp;&nbsp;(requested change from green to #FF7034; [dark orange])
<br><br>

In the <font color='green'>:root</font> section, copy the code below...

```css
/*-----------------------------------------
:root selector for variables
-------------------------------------------*/
:root {
    --header-color:  #FF7034; /*dark orange*/
    --section1-color: whitesmoke;
    --section2-color: whitesmoke;
    --footer-color: #FF7034; /*dark orange*/
    --h2-text-color-light: white;
    --h2-text-color-dark: black;
    --nav-list-item-hover-color: white;
    --h2-font-size: 2rem;
    --nav-list-font-size: 1.2rem;
    --footer-list-font-size: .9rem;    
}
```
...AND make certain you paste it BELOW this *<u>REPLACE point</u>* comment in your index.**css** file:


> /* REPLACE Point - :root variables */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicBonusImage5b.jpg">

___
 
Check it out in Chrome!  So easy and powerful with the <font color='green'>:root</font> variables.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicBonusImage6.jpg">

___

#### 3. "Wiggle" Button

- Our final snippets of code to the index.**css** file will bring to life our cta (Call to Action) button with a little wiggle animation.


In the <font color='green'>.nav-list-item-cta</font> class, copy the code below...

```css
/*-----------------------------------------
The .nav-list-item-cta properties
------------------------------------------*/
.nav-list-item-cta {
  animation     : wiggle 400ms 2s 8 ease-out none;
  }
```
...AND make certain you paste it BELOW this *<u>INSERT point</u>* comment in your index.**css** file:


> /* INSERT Point - .nav-list-item-cta */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicBonusImage5c.jpg">
<br>

> Note: the animation properties:<br>
>- wiggle   - specifies the action
>- 400ms    - specifies the speed of the wiggle
>- 2s       - specifies the delay after page has refreshed
>- 8        - specifies how many wiggles
>- ease-out none - specifies how to end
___

- AND FINALLY

In the <font color='green'>@keyframes wiggle</font> section, copy the code below...

```css
/*-----------------------------------------
The @keyframes wiggle properties
------------------------------------------*/
@keyframes wiggle {
    0% { transform: rotateZ(  0deg ); }
   50% { transform: rotateZ(-10deg ); }
  100% { transform: rotateZ( 10deg ); }
  }
```
...AND make certain you paste it BELOW this *<u>INSERT point</u>* comment in your index.**css** file:


> /* INSERT Point - /* INSERT Point - @keyframes wiggle */

<br>

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicBonusImage5d.jpg">

___

#### Final Version With formR logo, color changes and "wiggle" button.

___

<span style="font-size: 20px"><b>CONGRATULATIONS!!</b></span> You have completed My HTML Custom App.



<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFINALImage.jpg">


<!--## 6. View Full Code  <!-- {docsify-ignore} -->

####  [View Full Code For Basic Blocks](/FRApps/code/fr020106_basic-bonus-code.md "Full Code")


<!-- ------------------------------------------------------------------------- -->

<div class="page-back">

[BACK - Website SSL](/Setup/fr0306_Setup-Website-SSL-Ubuntu.md)
</div><div class="page-next">

[Custom FRApps React - NEXT](/Setup/fr0105_Custom-FR-Apps-React.md)
</div><br>
