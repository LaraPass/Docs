# System Settings

Admin System Settings page of `LaraPass v2 Personal Version`

---

- [Overview](#overview)
- [Maintenance Mode](#maintenance)
- [Application Settings](#app-settings)
- [Social Logins](#social)
- [Google reCaptcha](#recaptcha)
- [Access Settings](#access)
- [<a href="https://github.com/larapass/docs/edit/master/resources/docs/personal/admin/system-settings.md" target="_blank"><i class="fa fa-edit"></i> Help us improve this page!</a>](#)

<a name="overview"></a>
## Overview

You can manage your app's system settings including Maintenance Mode, Application, Social Login, Google reCaptcha and Access Settings from this page.  
<br/>

![screenshot](/screenshots/admin/settings/system-1.png)  

---

<a name="maintenance"></a>
## Maintenance Mode

LaraPass has a build-in maintenace mode that you can activate while performing any backups, maintenance or scheduled downtime.   

You can display a **`custom`** maintenace message to the user (the input accepts basic html styling).

Once the maintenance mode is active, you can access the app using the **`secret`** url. By default it a random string but you can custom the url accordingly - ex: **`http://yourapp.com/secretaccess`**  
<br/>

<p>  
    <img src="/screenshots/admin/settings/system-maintenance-1.png" width="250" alt="system-maintenance-1"/></a>
    <img src="/screenshots/admin/settings/system-maintenance-2.png" width="250" alt="system-maintenance-2"/></a>
    <img src="/screenshots/admin/settings/system-maintenance-3.png" width="250" alt="system-maintenance-3"/></a>
</p>
<br/>

If you somehow forget the secret url or are unable to access the site during the maintenance period, you can manually disable the **`maintenance mode`** in 2 ways -
 + If you have access to **console**, navigate to the larapass directory and run the command **`php artisan up`**
 + If you do not have access to **console**, open the `larapass/storage/framework` directory and delete the file titled **`down`**

---

<a name="app-settings"></a>
## Application Settings

Set your app's default vault configuration/limitations here - 
+ Set the default membership name.
+ Set the no. of vaults each user can create.
+ Set the no. of folders each user can create.
+ Set the no. of sites each user can add.
+ Set the no. of notes each user can add.
+ Set whether the system should send users `email` notifications when they reach their account limits or not.

<img src="/screenshots/admin/settings/system-app-1.png" width="500" alt="system-app-settings"/></a> 

---

<a name="social"></a>
## Social Logins

> {primary} Instructions on how to get the Client ID / Secret Key for Github, Facebook & Twitter are available [`here`](../misc/social-logins)

Add the client id and secret key for social logins using OAuth here - 

+ Enable Github / Facebook / Twitter.
+ Add Client ID & Secret Key respectively.
+ Update Settings.

<img src="/screenshots/admin/settings/system-social-1.png" width="700" alt="system-social-settings"/></a>   
<br/>

+ Login page when all the social logins are enabled -

<img src="/screenshots/admin/settings/system-social-2.png" width="700" alt="system-social-login"/></a> 

> {warning} Social Logins are only available / visible to users when the app is set to **`PUBLIC`** mode.

---
<br />
<larecipe-feedback message="Thankyou for your feedback!">
</larecipe-feedback>