<!-- ---------------------------------------------------------------------- -->
<div class="page-back">

[<-- BACK](/FRApps/fr020100_My-HTML-Custom)

</div><div class="page-next">

<!-- ---------------------------------------------------------------------- -->

___

HTML

```html

<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="ie=edge">
        <title>HTML Custom Apps</title>
        <link rel="shortcut icon" href="favicon.png">
        <link rel="stylesheet"    href="https://fonts.googleapis.com/css?family=Bookman Old Style" >
        <link rel="stylesheet"    href="index_v1.css">
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

CSS


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
    width: 100%; /*was 300px*/
    height: 10%; /*was 100px*/
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
/*-----------------------------------------
The .header h2 override properties
------------------------------------------*/
.header h2 {
    padding: 1rem;
}

/* REPLACE Point - section1 */
/*-----------------------------------------
The .section1 properites
------------------------------------------*/
.section1 {
    background: var(--section1-color);
    width: 100%; /*was 300px*/
    height: 40%; /*was 100px*/
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
    width: 100%; /*was 300px*/
    height: 40%; /*was 100px*/
    position: relative;
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
.footer properites
------------------------------------------*/
.footer {
    background: var(--footer-color);
    width: 100%; /*was 300px*/
    height: 10%; /*was 100px*/
    position: relative;
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