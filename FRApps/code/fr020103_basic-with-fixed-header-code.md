<!-- ---------------------------------------------------------------------- -->
<div class="page-back">

[<-- BACK](/FRApps/fr020100_My-HTML-Custom)

</div><div class="page-next">

<!-- ---------------------------------------------------------------------- -->
HTML

___


```html
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
            <span class="header-logo">My Logo</span>
            <ul class="nav-list">
                <li class="nav-list-item"><a href=#>Links</a></li>
                <li class="nav-list-item"><a href=#>Cards</a></li>
                <li class="nav-list-item"><a href=#>FAQs</a></li>
                <li class="nav-list-item-cta"><a href=#>Sign In</a></li>
            </ul>
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

CSS

___

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
    --h2-font-size: 2rem;
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
    width: 100%;
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
    width: 100%;
    height: 10%;
    position: fixed;  /*was relative*/
    z-index: 100;
    display: flex;
    justify-content: space-between;
}


/* INSERT Point - .formr-logo */

/* INSERT Point - .header-logo */
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

/* INSERT Point - .header-logo:first-letter */
/*-----------------------------------------
The .header-logo::first-letter properites
------------------------------------------*/

.header-logo::first-letter {
    font-size: 150%;
    color: cornflowerblue;
}

/* INSERT Point - .nav-list */
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

/* INSERT Point - .nav-list-item a */
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

/* INSERT Point - .nav-list-item a:hover
                  .nav-list-item a:active */
/*-----------------------------------------
The .nav-list-item a properites
------------------------------------------*/
.nav-list-item a:hover,
.nav-list-item a:active {
    color: var(--nav-list-item-hover-color);
}

/* INSERT Point - .nav-list-item-cta a */
/*-----------------------------------------
The .nav-list-item-cta a properties
------------------------------------------*/
.nav-list-item-cta a {
    color: white;
    background: blue ;
    padding: 0.5rem 1rem;
    border-radius: 8px;
}

/* INSERT Point - .nav-list-item-cta */

/* INSERT Point - @keyframes wiggle */

/* REPLACE Point - section1 */
/*-----------------------------------------
The .section1 properites
------------------------------------------*/
.section1 {
    background: var(--section1-color);
    width: 100%;
    height: 40%;
    position: relative;
    top:10%; /*<---ADD to adjust the top position*/
}

/* INSERT Point - .image-text */

/* INSERT Point - .image-text::first-letter */

/* REPLACE Point - section2 */
/*-----------------------------------------
The .section2 properites
------------------------------------------*/
.section2 {
    background: var(--section1-color);
    width: 100%;
    height: 50%;
    position: relative;
    top:10%; /*<---ADD to adjust the top position*/
}

/* INSERT Point - section2 h2 */
/* DELETE Point - section2 h2 */
/*-----------------------------------------
The .section2 h2 properites
------------------------------------------*/
.section2 h2 {
    color: var(--h2-text-color-dark);
}

/* REPLACE Point - footer */
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

/* INSERT Point - footer h2 */
/* DELETE Point - footer h2 */
/*-----------------------------------------
The .footer h2 override properties
------------------------------------------*/
.footer h2 {
    padding: 2rem;
}

/* INSERT Point - .footer-text */

/* INSERT Point - .footer-list */

/* INSERT Point - .footer-list-item a */

/* INSERT Point - .footer-list-item a:hover
                  .footer-list-item a:active */

/* INSERT Point - All Responsive Code */                  

/* END */
```
___