# System Settings - Teams Version

Admin System Settings page of `LaraPass v2 Teams Version`

---

- [Overview](#overview)
- [Maintenance Mode](#maintenance)
- [Application Settings](#app-settings)
- [Access Settings](#access)
- [<a href="https://github.com/larapass/docs/edit/master/resources/docs/teams/admin/system-settings.md" target="_blank"><i class="fa fa-edit"></i> Help us improve this page!</a>](#)

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

###  You can checkout our demo video of our build-in maintenance mode in action below: 
<a href="https://youtu.be/shjxnSlqA8c" target="_blank">
    <img src="/screenshots/installation/maintenance-demo.jpg" alt="Installation-Demo-Video" width="240" height="180" border="10" />
</a>

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
<br />
<larecipe-feedback message="Thankyou for your feedback!">
</larecipe-feedback>