# Modules Manager

Admin Modules Management page of `LaraPass v2 Personal Version`

---

- [Overview](#overview)
- [Two Factor Auth](#two-factor)
- [Social Logins](#social)
- [Google reCaptcha](#recaptcha)
- [<a href="https://github.com/larapass/docs/edit/master/resources/docs/personal/admin/modules-manager.md" target="_blank"><i class="fa fa-edit"></i> Help us improve this page!</a>](#)

<a name="overview"></a>
## Overview

You can manage your app's modules including Two Factor Authentication, Social Logins, and Google reCaptch from this page. We are building several other modules including first-party services to integrate with LaraPass v2 which will be released in due time.  
<br/>  

![screenshot](/screenshots/admin/modules-manager/overview.png)  

---

<a name="two-factor"></a>
## Two Factor Authentication Module

This module is **`Enabled`** by default and allows the users' of your app to setup, activate and use Two Factory Authentication using their Authenticator (TOTP) apps like Google Authenticator, Authy, etc.
<br/>  
You can disable this module anytime you like. Disabling it will remove the option to confirm Two Factor Code for the users regardless of whether they had activated it previously or not. This will be applicable site-wide to all the users. 
<br/>  
You can also configure whether or not to show the Provider Key to the users' (default is `show`). This allows users to add the TFA Access to their apps without having to scan the QR code (by entering the provider key) - ideally for users' mainly on mobile devices (since they can't scan the QR code). Disabling it will hide the Key from users.

> {warning} For security reasons, we recommend to always keep this module active and never turn it off.

---

<a name="social"></a>
## Social Logins Module

This module is **`Disabled`** by default as it requires additional configuration. You can enable it by following the steps below. 

> {primary} Instructions on how to get the Client ID / Secret Key for Github, Facebook & Twitter are available [`here`](../misc/social-logins)

Add the client id and secret key for social logins using OAuth here - 

+ Select Enable for Github / Facebook / Twitter.
+ Add Client ID & Secret Key respectively.
+ Update Settings.

<img src="/screenshots/admin/settings/system-social-1.png" width="700" alt="system-social-settings"/></a>   

> {warning} Social Logins are only available / visible to users when the app is set to **`PUBLIC`** mode.  

+ Login page when all the social logins are enabled -

<img src="/screenshots/admin/settings/system-social-2.png" width="700" alt="system-social-login"/></a> 

> {danger} Beaware - if you `disable` this module, any users that registered on your app via OAuth (Github, FB, Twitter), will no longer be able to login.

---
<br />
<larecipe-feedback message="Thankyou for your feedback!">
</larecipe-feedback>