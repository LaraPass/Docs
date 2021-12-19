# Modules Manager - Teams Version

Admin Modules Management page of `LaraPass v2 Teams Version`

---

- [Overview](#overview)
- [Teams Module](#teams)
- [Two Factor Auth](#two-factor)
- [Social Logins](#social)
- [Google reCaptcha](#recaptcha)
- [<a href="https://github.com/larapass/docs/edit/master/resources/docs/teams/admin/modules-manager.md" target="_blank"><i class="fa fa-edit"></i> Help us improve this page!</a>](#)

<a name="overview"></a>
## Overview

You can manage your app's modules including Two Factor Authentication, Social Logins, and Google reCaptch from this page. We are building several other modules including first-party services to integrate with LaraPass v2 which will be released in due time.  
<br/>  

![screenshot](/screenshots/admin/modules-manager/teams-overview.png)  

---

<a name="teams"></a>
## Teams Module

This module enables the **`Teams`** functionality of the app. This module is **`Disabled`** by default. You can configure and enable it according to your requirement. You can also **disable** this module in the future and all teams data and access with be closed off aswell (data will always be preserved).

**You can configure the following options in the Teams Module:**

+ **Allow Team by Default** - This configurations decides whether or not a new user should automatically be allowed to create new teams (configurable on per user basis aswell).
+ **Default Membership Name** - Name of the Plan / Membership to display on the teams page (doesn't have any effect of the functionality of the module).
+ **Default Member Role** - Which role should be assigned by default to all newly invited members:
    + Admin - This role have no restrictions and allows users to modify any aspect of the team (not recommended for new invites).
    + Member - This role gives the user unrestricted access to the Teams Vault and the data within it, but doesnt allow them to modify any aspect of the team itself (inviting members, changing roles, removing members, team logs, etc).
    + Intern - This role gives the user a read-only acceess, meaning they can access the team's vaults, sites, etc but cannit update or delete any content within the vault (ideal for new invites).
+ **Max. Teams** - This limits the no. of teams a user can create or join (configurable on per user basis from the User Management Menu).
+ **Max. Members** - This limits the no. of members a team can have (configurable on per team basis from the Team Management Menu).
+ **Max. Vaults** - This limits the no. of vaults a team can have (configurable on per team basis from the Team Management Menu).
+ **Max. Sites** - This limits the no. of sites a team can have (configurable on per team basis from the Team Management Menu).
+ **Max. Folders** - This limits the no. of folders a team can have (configurable on per team basis from the Team Management Menu).
+ **Max. Notes** - This limits the no. of notes or custom fields a team can have (configurable on per team basis from the Team Management Menu).
+ **Apply to Existing Teams - Selecting NO will only affect new teams created thereafter, however, selecting YES will overwrite all the teams related limits in the database. If you have made any manual changes to any individual teams limit, they will be overwritten.**
<br/><br/>
  
![screenshot](/screenshots/admin/modules-manager/teams-limits.png)  

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