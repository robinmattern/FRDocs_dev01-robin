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
- You will be building a web site which starts with very simple index.<b>html </b>and index.<b>css</b> files.  Your repository will include both of those <b>empty</b> files plus the needed images. If you follow the directions and copy/paste each sections code you will end up with a still simple index.html but a rather complex index.css file.

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


= Your Final Web Site Preview
<br>
The below preview will have a fixed (secured) header and footer, navigation links and a button, an image with a font-based overlay, and a formR logo.
<br>
<br>

<img class="shadow-border" src="FRApps/assets/images/md-images/IntroductionImage2.jpg">


#### Important note about names, capitalization, pictures and code copying <!-- {docsify-ignore} -->
- In this tutorial please be careful to use the Exact Spelling and Capitalization. You will be using Windows, Unix and GitBash command prompts. Improper captialization will cause commands to fail. Some examples are: Local_Admin, myProject, repos, remotes and .ssh.
- This documentation was produced in 2021-2022. You will experience differences in some of the pictures due to the changes made over time by the developers of the softwares and web sites that are used.
- We recommend that you copy and paste code snippets from the Documentation into your workstation/server. This will reduce the errors caused by hand typing.


NEXT -->


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

- Click on index.<b>html</b> file from VSCode. Copy and paste the entire below code to Line 1:
<br><br>

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

- From VSCode, right click on the file "index.<b>html</b>" and click on "Open In Live Server"

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicBlocksImage1.jpg">

If your Chrome browser is not already open, this command will open it and show the results of the above html code. 

Like this:

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicBlocksImage2.jpg">

<i>This is our starting point.</i>  Let's move to the CSS code to add our blocks.

#### 3. Code - index.css  

- Click on the index.<b>css</b> file. Then copy and paste the below code (ensure to grab the final curly bracket "<font color='green'><b>}</b></font>" ), on to Line 1 of index.<b>css</b>:
<br><br>

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

/* END */
^ copy to here

```


___


#### 4.  Basic Blocks Web Page      

- Please check your Chrome browser. 

> We will build from this basic page to create a web site with a fixed header and footer, links with a button, and an image.  From there, the next course we will move on to add some magic with JavaScript (JS) to this web page.

<br>
<img class="shadow-border" src="FRApps/assets/images/md-images/BasicBlocksImage3.jpg">


#### 5. Understanding CSS        <!-- .(20615.01.2 RAM Changed to ### 4. Was #### --> 
<br>
To understand a little of this CSS code, let's look at the .header properties.
<br>
<br>
<font color='green'>** Notes:</font>
<br><br>

<!--
> .header {
>      background: var(--header-color);
>        ** Sets the background to the variable you set above

>    width: 300px;
>        ** Sets the width of the header block 300 pixels
>    height: 100px;
>        ** Sets the height of the header block 100 pixels
>    position: relative;
>       ** Places the header box relative to the html code
>        *DOM (Document Object Model) reading from 
>        the top to the bottom  
>}



/*-----------------------------------------
root selector to create variables
-------------------------------------------*/
** In CSS you can describe variables, this is very 
powerful. For example, if it was decided that the 
header color should actually be salmon, not red,
it only needs changing here.  Several of the below 
variables are not used in this particular .css, but 
will be used in upcoming sessions.

NOTE: in the .header properties below exactly 
      how this variable is used.  We are setting
      the background color of the header to red
      with the variable called "--header-color"

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

-->

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



#### 6.  [View Full Code For Basic Blocks](/FRApps/code/fr020101_basic-blocks-code.md "Full Code")

- Congratulations, you have just created a simple html page with a cascading style sheet (CSS) which makes 4 *basic blocks.*  

NEXT -->

----
### 2. Basic Large Blocks  
----

- Next, we will add to your existing code in the index.<b>css</b> file to continue building on our basic web page.
<br><br>
Note: The index.<b>html</b> file will remain unchanged.

#### 1. index.css - Body

- Body

In the <font color='green'>body</font> section, ADD the following by copying<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<b><font color=#A81966>width</font></b>: 100%; 

and pasting it below the existing code for <b><font color=#A81966>height</font></b>.
<br><br>
Like this:

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage1.jpg">
<br><br> 
<b>ALTERNATIVELY</b> -- Copy/Paste <font color='green'>.body</font> code from below: 
<br>
(make certain you copy from <font color='green'>body ----- }</font> (curly bracket) ):
<br><br>

```css
body {
    background: white;
    height: 100%;
    width: 100%;  
    margin: 0;
}
^ copy to here

```

#### 2. index.css - &#60;h2&#62; tags

- The &#60;h2&#62; tags come with built-in margins which we must <b>override</b> for the blocks to sit perfectly on top of each other.  
<br><br>
Please copy this snippet of code and paste below the body properties.
<br><br>

```css

/*-----------------------------------------
Set global properties for the <h2> tags
It also overrides the intrinsic margin of
20 to 0--allowing to stack the blocks together.
CHANGE: padding
-------------------------------------------*/
h2 {
    margin: 0;
    font-size: var(--h2-font-size);
    color: var(--h2-text-color-light);
    padding: 6rem;
    text-align: center;
}
^ copy to here

```

Like this:

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage2.jpg">

___

#### 3. &#60;h2&#62; Override in Header

- <b>ALSO</b>, we must override the padding for this &#60;h2&#62; tag in the <font color='green'>.header</font> & <font color='green'>.footer</font> with the following, placed under each, respectively:

<br>

```css
/*-----------------------------------------
This is the first <h2> override
setting the padding from 6 to 1 rem
------------------------------------------*/
.header h2 {
    padding: 1rem;
}
^ copy to here

```

Like this:

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage3.jpg">


#### 4. &#60;h2&#62; Override in Footer

- <b>AND</b> for the <font color='green'>.footer</font>:
<br>

```css
/*-----------------------------------------
This is another <h2> override
setting the padding from 6 to 2 rem
------------------------------------------*/
.footer h2 {
    padding: 2rem;
}
^ copy to here

```

Like this:

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage4.jpg">

___


#### 5. Header

- In the <font color='green'>.header</font> section, CHANGE

 - <b><font color=#A81966>width</font></b> to 100% <br> AND 
 - <b><font color=#A81966>height</font></b> to 10%
<br><br>

```css
    width: 100%;    /*was 300px*/
    height: 10%;   /*was 100px*/
```
Like this:
```css
.header {
    background: var(--header-color);
    width: 100%; /*was 300px*/
    height: 10%; /*was 100px*/
    position: relative;
}
^ copy to here

```
___

#### 6. Sections 1 & 2

In <font color='green'>section1</font> <b>AND</b> <font color='green'>section2</font>, CHANGE
- <b><font color=#A81966>width</font></b> to 100% <br>AND 
- <b><font color=#A81966>height</font></b> to 40%
<br><br>

```css
    width:  100%;    /*was 300px*/
    height: 40%;   /*was 100px*/
```

Like this

```css
/*-----------------------------------------
The .section1 properites
CHANGE: width & height
------------------------------------------*/
.section1 {
    background: var(--section1-color);
    width: 100%; /*was 300px*/
    height: 40%; /*was 100px*/
    position: relative;
}

/*-----------------------------------------
The .section2 properites
CHANGE: width & height
------------------------------------------*/
.section2 {
    background: var(--section2-color);
    width: 100%; /*was 300px*/
    height: 40%; /*was 100px*/
    position: relative;
}
^ copy to here

```
___


#### 7. Footer

In the <font color='green'>.footer</font> section CHANGE the <b><font color=#A81966>width</font></b> to 100% 
- <b><font color=#A81966>width</font></b> to 100% <br>AND 
- <b><font color=#A81966>height</font></b> to 10%
<br><br>

```css
    width:  100%;    /*was 300px*/
    height: 10%;    /*was 100px*/
```

Like this

```css
/*-----------------------------------------
The .footer properites
CHANGE: width & height
------------------------------------------*/
.footer {
    background: var(--footer-color);
    width: 100%; /*was 300px*/
    height: 10%; /*was 100px*/
    position: relative;
}
```

#### 8. Basic Large Blocks Web Page       <!-- .(20615.01.1 RAM This seems a little out of place --> 
- Please check your Chrome browser to see your web page so far.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicLargeBlocksImage5.jpg">


<span style="font-size: 25px"><b>Congratulations</b></span>! You have built a full page with four distinct blocks using your "Basic Blocks index.<b>css</b> code." In the next section. we will add/modify code to secure the header in one spot.   
<br>

<!--## 6. View Full Code  <!-- {docsify-ignore} -->

#### 9. [View Full Code For Basic Blocks](/FRApps/code/fr020102_basic-large-blocks-code.md "Full Code")

___

NEXT -->

----
### 3. Basic Blocks with Fixed Header 
----

- Next, we will add to your existing code in  both index.<b>html</b> AND index.<b>css</b> files to continue building on our basic web page.

___

#### index.html

#### 1. Header Section

First, let's make some modifications to the index.<b>html</b> file.  The entire header section can be changed by replacing it with this code.

Like this
___

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
___

Replace the code, starting with line 12.

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage1.jpg">

<br>

Great! Now we move to the index.<b>css</b> file.

___

#### index.css

___



#### 1. header

First and foremost, do the following in the <font color='green'>.header</font> class:
- CHANGE the <font color=#A81966>position</font>: from relative to <b>fixed</b>
- ADD 
    + <font color=#A81966>z-index</font>: 100; 
    + <font color=#A81966>display</font>: flex; 
    + <font color=#A81966>justify-content</font>: space-between;

Like this<br><br>

```css
/*-----------------------------------------
The .header properites
CHANGES: position
ADDITION: z-index, display & justify-content
REMOVAL: .header h2 
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
^ copy to here

```

- REMOVE the <font color=green>.header h2</font> class


<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage2.jpg">


___

Look at your Chrome browser! The above steps "secure" the header into a stationary position.

We still need to:

1. Get rid of the "Unwanted Space" at the bottom 
2. Fix the links in the right corner of the header 
3. Fix the "My Logo" in the left corner of the header.


<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage3.jpg">


___



#### 2. sections 1 & 2, footer
<br>

To handle the Unwanted Space, we need to adjust Sections 1 & 2 and the Footer.  It's easy, we will code each to have a <font color=#A81966>top</font> of 10%.  

ADD 
- <font color=#A81966>top</font>: 10%;

at the bottom of <font color=green>.section1</font>, <font color=green>.section2</font> and <font color=green>.footer</font>

Like this

___

```css
/*-----------------------------------------
The .section1 properites
ADDITION: top
------------------------------------------*/
.section1 {
    background: var(--section1-color);
    width: 100%;
    height: 40%;
    position: relative;
    top:10%; /*<---ADD to adjust the top position*/
}

/*-----------------------------------------
The .section2 properites
CHANGE: height
ADDITION: top
------------------------------------------*/
.section2 {
    background: var(--section2-color);
    width: 100%; 
    height: 50%;  /*Added 10% for scrolling*/
    position: relative;
    top:10%; /*<---ADD to adjust the top position*/
}

/*-----------------------------------------
The .footer properites
ADDITION: top
------------------------------------------*/
.footer {
    background: var(--footer-color);
    width: 100%;
    height: 10%;
    position: relative;
    top:10%; /*<---ADD to adjust the top position*/
}
^ copy to here

```

Back to Chrome. We now have all the blocks stacked in proper order with no "Unwanted Space" at the bottom. 
<br><br>
AND if you scroll up and down, you will have the "secured" header.

___

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage4.jpg">

___


#### 3. header-logo
<br>
Now, let's fix that ugly "My Logo" on the left side of the header. To do this, we add some new classes to our CSS file.

Copy and paste the following 2 classes, and place below the <font color='green'>.header</font> class.
<br><br>
Like this
<br><br>

```css

/*-----------------------------------------
***NEW***
Sets all the properties for the font-based logo.
The font-family is special and explained below
this code. Notice how we add a shadow to the text.
------------------------------------------*/
.header-logo {
    font-family: "Bookman Old Style", sans-serif;
    font-size: 30px;
    font-weight: bolder;
    color: blue;
    text-shadow: 2px 2px 12px #000000;
    padding-left: 20px;
}

/*-----------------------------------------
***NEW***
Sets the properties for the first letter
of the font-based logo AND we increase the
size of the first letter by 150%.
------------------------------------------*/

.header-logo::first-letter {
    font-size: 150%;
    color: cornflowerblue;
}
^ copy to here

```

___

Check Chrome

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage5.jpg">

___


This takes the boring "My Logo" and turns it into a nice "font-based" logo (with large shadowed blue letters and a lighter blue first letter).  Note the font is one of Google's special fonts, called "Bookman Old Style."  We linked to that from the very top of the index.<b>css</b> file.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage6.jpg">

___

#### 4. header nav-bar
<br>
Now, let's focus on the stack of links on the right side of the header.  

Copy and paste the following 3 classes and place below the <font color='green'>.header-logo::first-letter</font> class.

<br>

```css

/*-----------------------------------------
***NEW***
Sets properties for the nav-bar
introducing the flex property. Again, we
use a variable to set the font size.
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

/*-----------------------------------------
***NEW***
Sets the properties for each nav-bar item.
The padding separates each 25px from each other.
------------------------------------------*/
.nav-list-item a {
    color: black;
    font-weight: bold;
    text-decoration: none;
    margin: 8px 0;
    padding: 25px;
}

/*-----------------------------------------
***NEW***
Sets the color of the nav-bar
items when you hover with a variable.
------------------------------------------*/
.nav-list-item a:hover,
.nav-list-item a:active {
    color: var(--nav-list-item-hover-color);
}
^ copy to here

```
Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage7.jpg">





Go back to Chrome and see the results. Notice that the 3 links on the right will to a light gray (#ccc) when you hover over them.

___

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage8.jpg">

___

#### 5. cta button
<br>
Now, let's do something about that "Sign In" link. Using CSS, we can turn it into a nice blue button. We will copy the below code and place it under the...<br>

&nbsp;&nbsp;&nbsp;<font color='green'>.nav-list-item a:hover,</font><br>
&nbsp;&nbsp;&nbsp;<font color='green'>.nav-list-item a:active</font> {<br>
class.


The "cta" stands for "Call to Action." It becomes the most important link.


```css

/*-----------------------------------------
***NEW***
Creates the blue button around the 'Sign In'
button.  -cta stands for 'Call To Action'
------------------------------------------*/
.nav-list-item-cta a {
    color: white;
    background: blue ;
    padding: 0.5rem 1rem;
    border-radius: 8px;
}
^ copy to here

```

___

Like this


<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage9.jpg">

___

Again, go see it in your Chrome browser.  

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage10.jpg">

___

You have completed this part of the Fixed Header.  Later, we will add an image for a logo instead of the font-based logo. <br>
<img src="FRApps/assets/images/md-images/BasicFixedHeaderImage11.jpg">

___


#### Basic Blocks w/ Fixed Header Web Page       <!-- .(20615.01.1 RAM This seems a little out of place --> 
<br>


<span style="font-size: 25px"><b>Congratulations!</b></span> You have just added to your Basic Blocks code which built a full web page with a fixed header along with links, a button, and a font-based logo. In the next section, we will add/modify code that will secure the footer with links.   
<br>
Please check your Chrome browser to see your web page thus far.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedHeaderImage12.jpg">

___

<!--## 6. View Full Code  <!-- {docsify-ignore} -->

####  [View Full Code For Basic Blocks](/FRApps/code/fr020103_basic-with-fixed-header-code.md "Full Code")

___

NEXT -->

----
### 4. Basic Blocks with Fixed Footer 
----

- Next, we will add to your existing code in both the index.<b>html</b> AND index.<b>css</b> files to continue building on our basic web page. We will add some links to the footer and "secure" the position of the footer as we did with the header.
___

#### index.html

#### 1. Footer Section

First, let's make some modifications to the index.<b>html</b> file.  The entire footer section can be changed by replacing it with this code.
___

```html
<div class="footer">
    <ul class="footer-list">
        <li class="footer-list-item"><a href=#>Support</a></li>
        <li class="footer-list-item"><a href=#>Terms Of Use</a></li>
    </ul>
</div>

```
___

Replace your code starting with line 27. 

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage1.jpg">

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage2.jpg">
<br><br>
Great! Now we move to the index.<b>css</b> file.

___

#### index.css

___



#### 1. footer

First and foremost, in the .footer class:
- CHANGE the <font color=#A81966>position</font>: from relative to <b>fixed</b>
- ADD 
    + <font color=#A81966>z-index</font>: 99; 
    + <font color=#A81966>bottom</font>: 0; 
- REMOVE the <font color=green>top</font> property<br><br>
  You can comment-out a line of code with the /* (slash asterisk) at the 
  beginning of the line and an */ (asterisk slash) at the end.<br><br>
  Example:<br>
  <b>/ * top: 10%; Removed in place of the bottom property*/</b>

Like this
<br><br>

```css
/*-----------------------------------------
The .footer properites
ADDITION: z-index, bottom
CHANGES: position
REMOVAL: top property; and .footer h2 class
------------------------------------------*/
.footer {
  background: var(--footer-color);
  width: 100%; 
  /*top: 10%;  Removed in place of the bottom property*/
  bottom: 0;
  position: fixed;
  z-index: 99;
}
^ copy to here

```

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage3.jpg">

___

Also, we can remove the <font color='green'>.footer h2</font> class.  It is not needed because we replaced the &#60;h2&#62; tag with a &#60;ul&#62; tag in the index.<b>html</b> file.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage4.jpg">

___


Look on your Chrome browser! This "secured" the footer into a stationary position, but we need to fix the links in the left corner of the footer.


<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage6.jpg">

___

#### 2. footer nav-links
<br>
Now, let's focus on the links on the left side of the header.  

Copy and paste the following 4 classes and place below the <font color='green'>.footer</font> class.

<br>

```css
/*-----------------------------------------
***NEW***
Sets properties for the footer text
------------------------------------------*/
.footer-text {
  font-size: x-large;
  text-align: right;
  padding: 0px 30px 0px 65%;}

/*-----------------------------------------
***NEW***
Sets properties for the footer nav list
introducing the flex property and the use
of a variable for the font size
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

/*-----------------------------------------
***NEW***
Sets the properties for each nav item
introducing the flex property
of the nav-bar items
------------------------------------------*/
.footer-list-item a {
    color: black;
    font-weight: bold;
    text-decoration: none;
    margin: 8px 0;
    padding: 12px;
  }

/*-----------------------------------------
***NEW***
Sets the color of the footer nav
items when you hover using a variable
------------------------------------------*/
.footer-list-item a:hover,
.footer-list-item a:active {
  color: var(--nav-list-item-hover-color);
}
^ copy to here

```
___

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage7.jpg">

___

Again, go see it in your Chrome browser. The links are nicely centered and side-by-side, thanks to the CSS "flex" property. 

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage8.jpg">


#### 3. Basic Blocks w/ Fixed Header Web Page       <!-- .(20615.01.1 RAM This seems a little out of place --> 
<br>


<span style="font-size: 25px"><b>Congratulations!</b></span> You have just added to your Basic Blocks code which builds a full web page with a secured footer along with links. In the next section, we will add/modify code that will add an image and text overlay in <font color='green'>section1</font>.   
<br>
Please check your Chrome browser to see your web page thus far:

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicFixedFooterImage9.jpg">



####  [View Full Code For Basic Blocks](/FRApps/code/fr020104_basic-with-fixed-footer-code.md "Full Code")

___

NEXT -->

----
### 5. Basic Blocks With Image
----

- To add magic to your web site, we will add an image and text overlay.  This will require some modifications to your existing code in both the index.<b>html</b> AND index.<b>css</b> files.  

First, the index.<b>html</b> file.
___

#### index.html

#### 1. Section 1

<br>

We will change this code that starts on line 21, from this...
<br><br>
```html
    <div class="section1">
        <h2>section 1</h2>
    </div>

```
...to this:

```html
    <div class="section1">
        <h2 class="image-text">My Image & Text</h2>
    </div>

```

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicWithImageImage1.jpg">

Notice the "My Image & Text" within the &#60;h2&#62; tags.  This will become our text overlay. Check your Chrome browser for this change.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicWithImageImage2.jpg">

Now, we move to the index.<b>css</b> file.
___

#### index.css

#### 1. section1

This is where you completely change the .section1 code with the below.  It should fall under <font color='green'>.nav-list-item-cta a</font>.
<br><br>

```css
/*-----------------------------------------
The .section1 properites
CHANGES:    background:
ADDITIONS:  background-color: 
            background-repeat:
            background-size: 
            background-position:
Notice how we are using CSS to add a link to .jpg
file (monaco-blue-soft.jpg) in "images" directory.
Please Google the other properties to see how they
allow to properly position the image.
------------------------------------------*/
.section1 {
  background: url("assets/images/monaco-blue-soft.jpg");
  background-color: blue;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  width: 100%;
  height: 45%;
  position: relative;
  top: 10%;  
}
^ copy to here

```

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicWithImageImage3.jpg">

Again, check your Chrome browser for the change; a nice blue image with the font overlay.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicWithImageImage4.jpg">

___


#### 2. image-text
<br>
Now, let's focus on the text overlay. By ADDING the following two classes: 

  - <font color='green'>.image-text</font> and 
  - <font color='green'>.image-text::first-letter</font> 

below the <font color='green'>.section1 code</font>, we will acheive a nice change to the overlay.<br><br>

```css
/*-----------------------------------------
Sets all the propterties for the font-based
text overlay (sits over top of the image above).
It uses the "Bookman Old Style" font and changes
it blue text.  The padding property positions
the text in the image.  Try adjusting this to 
see how it changes.
------------------------------------------*/
.image-text {
  font-family: "Bookman Old Style", sans-serif;
  font-size: 3rem;
  font-weight: bolder;
  color: blue;
  text-shadow: 2px 2px 12px #000000;
  padding: 80px 400px 20px 0px;
}

/*-----------------------------------------
Sets the properties for the first letter
of the font-based text overlay, above.
This makes the first letter a lighter blue
and increases its size to 150%.
------------------------------------------*/
.image-text::first-letter {
  font-size: 150%;
  color: cornflowerblue;
}
^ copy to here

```

Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicWithImageImage5.jpg">

#### Basic Blocks w/ Image Web Page       <!-- .(20615.01.1 RAM This seems a little out of place --> 
<br>


<span style="font-size: 25px"><b>Congratulations!</b></span>  You have just completed your web page with a fixed header and footer, links, a button, an image, and a text overlay.   
<br>
Please check your Chrome browser to see your web page:


<img class="shadow-border" src="FRApps/assets/images/md-images/BasicWithImageImage6.jpg">


#### Next Version With formR logo and color changes.
<br>

<img src="FRApps/assets/images/md-images/formr-logo.gif">

In the final section, we will change the font-based logo to a formR logo image file AND we will change the color of the blocks on the web page.  

<br>
<!--## 6. View Full Code  <!-- {docsify-ignore} -->

####  [View Full Code For Basic w/ Image](/FRApps/code/fr020105_basic-with-image-code.md "Full Code")

___

NEXT -->

----
### 6.  BONUS 

- As previoused mentioned, we will make some changes.  First, the font-based "My Logo" will be changed to our formR logo image file.  Then, because the next author would like to work with diffent colors for the blocks, we can easily change them.  Let's have some fun. This will require some modifications to your existing code in both the index.<b>html</b> AND index.<b>css</b> files.  

First, the index.<b>html</b> file.
___

#### index.html

#### 1. Replace logo

<br>
In the index.<b>html</b> file comment-out the below:<br><br>
&nbsp;&nbsp;&nbsp;&nbsp;<b>&#60;span class="header-logo">My Logo</span>&#62;</b><br><br>
using the &#60;!-- (Less-than exclamation dash dash) AND --&#62; (dash dash greater-than) at the beginning and end of this line of code.

Like this: &#60;!--&#60;span class="header-logo">My Logo</span>&#62;--&#62;

Then add:<br>
&nbsp;&nbsp;&nbsp;&nbsp;"&#60;img class="formr-logo" src="assets/images/formr-logo.gif"/&#62;"<br> below the &#60;div class="header"&#62;<br><br>
Like this:

<img src="FRApps/assets/images/md-images/BasicBonusImage1.jpg">

___

ALTERNATIVELY, Copy this code...

```html
<div class="header">
    <img class="formr-logo" src="assets/images/formr-logo.gif"/>
    <!--<span class="header-logo">My Logo</span>-->
```

...and paste below the <b>&#60;body&#62;</b> tag AND above <b>&#60;ul class="nav-list"&#62;</b>, to replace the existing code.

Like this

<img src="FRApps/assets/images/md-images/BasicBonusImage2.jpg">


#### index.css

#### 1. formr-logo


Then add the below css property (.formr-logo) below the 
<font color='green'>.header-logo::first-letter</font> css code.
___

```css
/*This replaces the action of the above css code*/
/*This sets the size and position of the formr.gif logo*/
.formr-logo {
  width: 210px;
  height: 60px;
  padding-left: 20px;
  padding-top: 10px;
}
^ copy to here

```
Like this

<img src="FRApps/assets/images/md-images/BasicBonusImage3.jpg">

___

The web page should look like this.

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicBonusImage4.jpg">

___

#### 2. Color Changes

We were requested to change some colors for the next major lessons. No problem!
<br><br>
First, remember the <font color='green'>:root</font> in our index.<b>css</b> file.
<br><br>

```css
/*-----------------------------------------
root selector to create variables
-------------------------------------------*/
** In CSS you can describe variables, this is very 
powerful. For example, if it was decided that the 
header color should actually be yellow, not red,
it only needs changing here.  NOTE in the .header
properties how this variable is used.

:root {
    --header-color: red;
    --section1-color: blue;
    --section2-color: lightgray;
    --footer-color: green;
    --h2-text-color-light: white;
    --h2-text-color-dark: black;
    --nav-list-item-hover-color: white;
    --h2-font-size: 2rem;
    --nav-list-font-size: 1.2rem;
    --footer-list-font-size: .9rem;    
}

```

Well, it's very simple to make the requested color changes right here in four of the properties:

- --header-color    (requested change from red to #FF7034; [dark orange])
- --section1-color  (requested change from blue to whitesmoke)
- --section2-color  (requested change from lightgray to whitesmoke)
- --footer-color    (requested change from green to #FF7034; [dark orange])
<br><br>

```css

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
Like this

<img class="shadow-border" src="FRApps/assets/images/md-images/BasicBonusImage5.jpg">
<br><br> 
Check it out in Chrome!  So easy and powerful with the <font color='green'>:root</font> variables.

___

#### Final Version With formR logo and color changes.
<br><br>
<span style="font-size: 20px"><b>CONGRATULATIONS!!</b></span> You have completed My HTML Custom App.



<img class="shadow-border" src="FRApps/assets/images/md-images/BasicBonusImage6.jpg">


<!--## 6. View Full Code  <!-- {docsify-ignore} -->

####  [View Full Code For Basic Blocks](/FRApps/code/fr020106_basic-bonus-code.md "Full Code")


<!-- ------------------------------------------------------------------------- -->

<div class="page-back">

[BACK - Website SSL](/Setup/fr0306_Setup-Website-SSL-Ubuntu.md)
</div><div class="page-next">

[Custom FRApps React - NEXT](/Setup/fr0105_Custom-FR-Apps-React.md)
</div><br>
