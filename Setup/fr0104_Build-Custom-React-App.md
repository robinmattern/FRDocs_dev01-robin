<!-- ------------------------------------------------------------------------- -->

<div class="page-back">

[BACK - Clone First React Apps](/Setup/fr0102_Clone-First-React-Apps.md)
</div><div class="page-next">

[Vultr Ubuntu - NEXT](/Setup/fr0301_Setup-Vultr-Ubuntu.md)
</div><div style="margin-top:35px">&nbsp;</div> 
 
<!-- ------------------------------------------------------------------------- -->

## 1.4 Build Custom React App 0:45
- [Purpose and Background](../Setup/purposes/pfr0104_Build-Custom-React-App.md)
- [Enter Comments in Discord](https://discord.com/channels/928752444316483585/931216956827250709)

#### Introduction  
- Blah

- More Blah


#### Important note about names, capitalization, pictures and code copying
- In this tutorial please be careful to use the Exact Spelling and Capitalization. You will be using Windows, Unix and GitBash command prompts. Improper captialization will cause commands to fail. Some examples are: Local_Admin, myProject, repos, remotes and .ssh.
- This documentation was produced in 2021-2022. You will experience differences in some of the pictures due to the changes made over time by the developers of the softwares and web sites that are used.
- We recommend that you cut and paste code snippets from the Documentation into your workstation/server. This will reduce the errors caused by hand typing.


----


### 1. Copy 5c-my-react-app to 6c-my-custom-app 0:05
----

1. Right click on the client/5c-my-react-app folder and click Copy

![FRApps-Clone69](images/fr0103-FRApps-Clone-69.png "FRApps-Clone-69")


2. Right click on the client/5c-my-react-app folder and click Paste

![FRApps-Clone69](images/fr0103-FRApps-Clone-69-1.png "FRApps-Clone-69")


3. Right click on the client/5c-my-react-app-copy folder and click Rename

![FRApps-Clone69](images/fr0103-FRApps-Clone-69-2.png "FRApps-Clone-69")

- Enter:

```
6c-my-custom-app
```

![FRApps-Clone69](images/fr0103-FRApps-Clone-69-3.png "FRApps-Clone-69")

4. From 6c-my-custom-app folder, click to open the .env file

![FRApps-Clone69](images/fr0103-FRApps-Clone-69-4.png "FRApps-Clone-69")

- Change PORT to 50166

```
PORT=50166
```
![FRApps-Clone69](images/fr0103-FRApps-Clone-69-5.png "FRApps-Clone-69")

5. From 6c-my-custom-app folder, click toopen the package.json file

![FRApps-Clone69](images/fr0103-FRApps-Clone-69-6.png "FRApps-Clone-69")

- Make the following 3 changes

```
  "name": "6c-my-custom-app",

  "homepage": "/6c-my-custom-app",

   "prod": "node serveProd.js 51166",
```

![FRApps-Clone69](images/fr0103-FRApps-Clone-69-7.png "FRApps-Clone-69")

----
### 2. Run Client 6c-my-custom-app application 0:05
----

1. Right click on the client/6c-my-custom-app folder
2. Click Open in Integrated Terminal, then 

![FRApps-Custom-01](images/fr0103-FRApps-Custom-01.png "FRApps-Custom-01") 

```
npm start
```

![FRApps-Custom-01a](images/fr0103-FRApps-Custom-01a.png "FRApps-Custom-01a")

- If you are prompted, click Allow Access

![FRApps-Clone-22a](images/fr0103-FRApps-Clone-22a.png "FRApps-Clone-22a")

![FRApps-Custom-01b](images/fr0103-FRApps-Custom-01b.png "FRApps-Custom-01b")

![FRApps-Custom-01c](images/fr0103-FRApps-Custom-01c.png "FRApps-Custom-01c")

----
### 3. Install and test React-Bootstrap component library 0:05
----

[React-Bootstrap Reference](https://react-bootstrap.github.io/forms/overview/)

<br/>

1. Right click on the client/ folder
2. Click Open in Integrated Terminal, then 

![FRApps-Custom-02](images/fr0103-FRApps-Custom-02.png "FRApps-Custom-02")

```
npm install react-bootstrap bootstrap
```

![FRApps-Custom-02](images/fr0103-FRApps-Custom-02a.png "FRApps-Custom-02")

3. Check for production vulnerabilities

```
npm audit --production
```

![FRApps-Custom-02](images/fr0103-FRApps-Custom-02b.png "FRApps-Custom-02")

3. Open src/App.js and add a Primary Button

<br/>

- Add the following import statement to App.js

```
import Button from 'react-bootstrap/Button';
```

![FRApps-Custom-02](images/fr0103-FRApps-Custom-02c.png "FRApps-Custom-02")

- Add the following code snippet to App.js

```
      <p>
        <Button variant="primary">
          Primary Button
        </Button>
      </p>
```

![FRApps-Custom-02](images/fr0103-FRApps-Custom-02d.png "FRApps-Custom-02")


4. Run or refresh http://localhost:50166/6c-my-custom-app on your browser

![FRApps-Custom-02](images/fr0103-FRApps-Custom-02e.png "FRApps-Custom-02")


----
### 4. Add Carousel component 0:05
----








<!-- ------------------------------------------------------------------------- -->

<div class="page-back">

[BACK - Clone First React Apps](/Setup/fr0102_Clone-First-React-Apps.md)
</div><div class="page-next">

[Vultr Ubuntu - NEXT](/Setup/fr0301_Setup-Vultr-Ubuntu.md)
</div>


