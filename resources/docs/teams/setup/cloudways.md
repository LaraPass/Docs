# Cloudways Setup Guide

LaraPass v2 Setup Guide for Cloudways.

---

- [Sign Up](#sign-up)
- [Deploy](#deploy)
- [Setup](#setup)
- [Upload](#upload)
- [Installing](#installing)
- [Watch Demo Video](#video)
- [<a href="https://github.com/larapass/docs/edit/master/resources/docs/teams/setup/cloudways.md" target="_blank"><i class="fa fa-edit"></i> Help us improve this page!</a>](#)

<a href="https://refs.spargon.tech/cloudways" target="_blank"><img src="//www.cloudways.com/affiliate/accounts/default1/banners/61dde566.jpg" alt="The Ultimate Managed Hosting Platform" title="The Ultimate Managed Hosting Platform" width="728" height="90" /></a><img style="border:0" src="https://www.cloudways.com/affiliate/scripts/imp.php?id=94888&amp;a_bid=61dde566" width="1" height="1" alt="" />

<a name="sign-up"></a>
## Sign Up

If you don't already have one, then sign-up for a free Cloudways account by clicking <a href="https://refs.spargon.tech/cloudways" target="_blank">`here.`</a>

---

> {warning} The Cloudways Setup Steps for all versions of LaraPass v2 are identical. You do not have to make any special changes for the Teams Version.

<a name="deploy"></a>
## Deploy Your Server/Application

Login to your cloudways account. Click on `Server` option in the menu & click on the `Launch` button.

+ Select your Application >> PHP Custom App
+ Enter Name for the App and the Server & Select a Project for it.
+ Select your hosting provider (you can choose from Digital Ocean, Linode, Vultr, AWS & GoogleCloud) - Note: You don't need separate accounts for these, cloudways will pay for and manager all the servers.
+ Select the Server Size (you can start off with the smallest size and then upgrade to bigger servers when you start getting higher usage).
+ Select Location (the closest to you).
+ Click on Launch Now and watch the magic happen (this process will take 5-10 minutes to complete).  
<br/>  

![screenshot](/screenshots/setup/cloudways/configuration.png)

---

<a name="setup"></a>
## Setup

Prepare your server to run LaraPass v2.

+ Copy the IP Address of the newly deployed server.  
![screenshot](/screenshots/setup/cloudways/server.png)

+ Go to your Domain Manager and Add an A record to point your domain to this new server.
+ Open your App, Go to **Domain Management** and add your domain/website address there.  
![screenshot](/screenshots/setup/cloudways/domain.png)
+ Next > Go to SSL Certificate and Add a Let's Encrypt SSL (or if you are using a custom one, you can add that).  
![screenshot](/screenshots/setup/cloudways/ssl.png)
+ Lastly > Go to Application Settings & under **WEBROOT** add `public` and Save. The final directory would be `public_html/public` -  
![screenshot](/screenshots/setup/cloudways/webroot.png)

---

<a name="upload"></a>
## Upload

Upload LaraPass v2 files to your cloudways server.

+ Get the SFTP Login details from the **Access Details** Section.
+ Open Cyberduck (or any other SFTP program) & Login using said details.
+ Navigate to the `public_html` directory and delete any files inside there.
+ Upload all the files found in **`larapass_source`** folder (that you got from us) into the **`public_html`** directory.
+ And you are done. Navigate to `yourdoman.com` and you should see the Installation menu.
+ Lastly, don't forget to copy your MYSQL Database Username and Password from the **Access Details** page.

> {info} You can follow the installation instructions and installation demo video [`here`](../installation/overview#installing)

---

<a name="installing"></a>
## Installing LaraPass v2

Follow the instructions on the Installation page [**here.**](../installation/overview#installing)

---

<a name="video"></a>
## Watch Demo Video

Watch the demo of us setting up our cloudways account server.
<br>

<a href="https://youtu.be/iz6zqW67_eY" target="_blank">
    <img src="/screenshots/setup/cloudways/setup-demo.jpg" alt="Installation-Demo-Video" width="240" height="180" border="10" />
</a>

---
<br />
<larecipe-feedback message="Thankyou for your feedback!">
</larecipe-feedback>
