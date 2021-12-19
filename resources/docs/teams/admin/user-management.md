# User Management - Teams Version

Overview of Admin User Management System build in `LaraPass v2 Teams Version`

---

- [Overview](#overview)
- [User Profile](#user-profile)
- [Manage Plan / Limits](#manage-limits)
- [Change Email](#change-email)
- [View IP Logs](#view-ip-logs)
- [Ban User](#ban-user)
- [<a href="https://github.com/larapass/docs/edit/master/resources/docs/teams/admin/user-management.md" target="_blank"><i class="fa fa-edit"></i> Help us improve this page!</a>](#)

<a name="overview"></a>
## Overview

Quick overview list of all the registered users of your app.

![screenshot](/screenshots/admin/user-management/overview.png) 

---

<a name="user-profile"></a>
## User Profile

View the user account information and their stats (vaults, sites, etc owned). Also perform a variety of actions such as - changing email address (will require email verification by user), viewing IP logs, verifying support pin and banning user account.  
<br>

![screenshot](/screenshots/admin/user-management/teams-profile.png) 

---

<a name="manage-limits"></a>
## Manage User Plan / Limits

You can either manage User Plan & Limits globally through the Admin Settings page [`here`](/teams/admin/system-settings#app-settings) or update limits assigned to each user individually from the User's Profile page. 

**Available Options are:** 
+ Allowing Users to Create New Teams.
+ Maximum no. of Teams a user can create.
+ Maximum no. of vaults a user can create.
+ Maximum no. of folders a user can create (in total).
+ Maximum no. of sites a user can add (in total), and
+ Maximum no. of notes/custom fields a user can add (in total).

---

<a name="change-email"></a>
## Change User Email

You can change a user's email address on request by the user themselves. You will need to provide the current email address (on the account), the new email address (to be updated to) and the user's Support PIN. Without the Support PIN from the user (inaccessible to admin's themselves), the email address on the user's account cannot be changed. This has been done to ensure users' that admin wont be able to modify their access without authorization.  
<br> 

<img src="/screenshots/admin/user-management/change-email.png" height="400px" width="400px" />

Once the email address is updated, the system wil send a new verification email to the new email address. The user won't be able to access their account until they verify their email address.

---

<a name="view-ip-logs"></a>
## View IP Logs

You can view the IP address, device, platform and browser used by a user whenever they login into your app. The same data is also available to the user themselves so they can monitor any authorize or irregular access of their account.   
<br> 

<img src="/screenshots/admin/user-management/ip-logs.png" height="400px" width="400px" />

---

<a name="ban-user"></a>
## Ban / Un-Ban User

You can ban any user account by providing a reason. Once an account is banned, the user will receive an email stating when their account was banned, the reason for it and a way to appeal if they feel the ban was unwarranted.
<br/>

<p>  
    <img src="/screenshots/admin/user-management/ban-option.png" width="250" alt="ban-option"/></a>
    <img src="/screenshots/admin/user-management/ban-email.png" width="250" alt="ban-email"/></a>
    <img src="/screenshots/admin/user-management/ban-screen.png" width="250" alt="ban-screen"/></a>
</p>

You can also un-ban or revoke ban on an account and the users will be informed of the same.  
<br/>  

<p>  
    <img src="/screenshots/admin/user-management/banned-user.png" width="250" alt="banned-user"/></a>
    <img src="/screenshots/admin/user-management/unban-option.png" width="250" alt="unban-option"/></a>
    <img src="/screenshots/admin/user-management/unban-email.png" width="250" alt="unban-email"/></a>
</p>


---
<br />
<larecipe-feedback message="Thankyou for your feedback!">
</larecipe-feedback>