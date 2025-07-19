
## Steps to deploy a Laravel application with its database to Vercel
Once you've build your Laravel application and you want to share your app to others colleagues/client, you can deploy it on Vercel. Here are steps to follow.

##### **Step 1**

Ensure that Vercel CLI is installed on your computer. Type the following command in the terminal

npm install -g vercel



After the installation, check the current version by typing "vercel --version"



Login into Vercel using command line "vercel login"





##### **Step 2**

Create a new folder "api" and add a new file "index.php"



##### **Step 3**

Write Following in the file

``` php
<?php  

require \_\_DIR\_\_ . "/../public/index.php";
```



##### **Step 4**

Create a new file "vercelignore" and add this

/vendor



##### **Step 5**

Create new file "vercel.json" and add the content of attached file



##### **Step 6**

Create empty folder "dist"



##### **Step 7**

Deploy the project in local, type in the terminal "vercel ."





&nbsp;   Set up and deploy “folder/yourprojectname”? \[Y/n] select Y



&nbsp;   Which scope do you want to deploy to? press ENTER



&nbsp;   Link to existing project? \[y/N] optional



&nbsp;   Whats your projects name? yourprojectname



&nbsp;   In which directory is your code located? ./



&nbsp;   Setting up project…



&nbsp;   Want to modify these settings? \[y/N] optional



##### **Step 8**

After the build, you'll get the error "The output directory 'dist' is empty."



##### **Step 9**

Go to your vercel dashboard [https://vercel.com/dashboard](https://vercel.com/dashboard) 

Go to your project

Go to tab settings

Go to Build \& Development Settings, then checklist Output Directory and type public, then click button save



##### **Step 10**

Redeploy again your project with type on command "vercel ."





##### **Step 11**

Create an online database to host your data.
Go to [https://www.freesqldatabase.com](https://www.freesqldatabase.com)

Or go to [https://supabase.com](https://supabase.com)  

Or anyone database hosting service



##### **Step 12**

Get your online database credentials and put them in your .env file



##### **Step 13**

Redeploy your project with the command "vercel ."
