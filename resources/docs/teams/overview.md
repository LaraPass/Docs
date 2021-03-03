# LaraPass v2 Teams Version

A Self-Hosted Password Manager for Teams.

---

- [Overview](#overview)
- [Features](#features)
- [Credits](#credits)
- [Contribute](#contribute)
- [<a href="https://github.com/larapass/docs/edit/master/resources/docs/teams/overview.md" target="_blank"><i class="fa fa-edit"></i> Help us improve this page!</a>](#)

<a name="overview"></a>
## Overview

**LaraPass v2** is a self-hosted password manager for teams that allows you to store all of your important site login details and information into secure vaults on your own servers and share them among your team members thereby guaranteeing highest level of security and discretion 😏. **LaraPass v2** is build using the amazing Laravel PHP Framework (v8.x) and the beautiful, responsive UI is powered by the Stisla Template (by *Muhamad Nauval Azhar*) using Bootstrap 4, along with powerful Livewire Components.

---

<a name="features"></a>
## Features

**LaraPass v2 Teams Version** comes with a plethora of features right out of the box.  
  
**`For Users`**
+ Secure Vaults to store sites, notes, etc (Add extra layer of protection by password protecting individual vaults).
+ Store Site Login Info in Encrypted form along with notes & custom fields.
+ Two Factor Authentication System (using an Authenticator App) for increased Security.
+ Get notified via Email whenever you log in from a new device.
+ Password Generator - Custom build Password Generator to generate strong, highly secured password strings with just one-click.
+ Beautiful and responsive layout for immersive user experience.
+ Easily copy account details with just one-click.
+ Folders - Allows you to organize sites in separate folders to avoid any unnecessary confusion.
+ Receive Custom Emails for Verification, Welcome, Password Reset, New Device Login, Team Invite, etc.  
+ Create New Teams or Join any existing Teams through an Invite.
+ Quick and robust search system to search through your catelog of sites from different personal or team vaults.

**`For Teams`**
+ Create separate teams and invite registered members to join your team.
+ Separate team vaults for each team. Keep your team's site data isolated from other teams.
+ Assign teams roles (Team Admin, Team Member, Team Intern) and manage permissions (per user): 
    + **Team Admin** - Access to all of the team settings and data. Can invite, update (roles) or remove members from the team. Can view team logs and if needed, Delete the entire team.
    + **Team Member** - Can access team vaults, sites and folders. Update data if required. Cannot invite or remove members from the team.
    + **Team Intern** - Very limited access. Can only view data of the vaults, sites and folders in it. Cannot update, share, move or delete any of the team's data.
  
**`For Admins`**
+ LaraPass Installer included for simple few clicks installation experience.
+ Overview - Get quick stats of the app.
+ Announcements - Send app wide announcements to all users of the app.
+ Pages Manager - Manage custom static pages (currently only Terms & Privacy Pages available).
+ User Manager - View, Add, Update, Verify, Suspend, Ban or Delete Users.
+ Team Manager - View, Update or Delete Teams or Team Members.
+ Admin Manager - Manage General, Email, System & Automation Settings:
    + **General Settings** - Manage App name, email, address, logo, favicon, language, footer, and theme settings among others.
    + **Email Settings** - Manage output email services (smtp, mailgun api, etc).
    + **System Settings** - Manage Maintenance Mode, default storage, Public/Private mode & database settings.
    + **Automation Settings** - Manage Backups, Optimization & Automated Scheduled Tasks (thru cron jobs).
+ Module Manager - Enable/Disable & Manager 1st Party Modules:
    + **Teams Module** - Enable teams module to enable the teams functionality in your app. Manage general configuration for teams (max. members allow, max. vaults, max. sites, etc).
    + **Two Factor Authentication Module** - Enable TFA Module to allow users to setup Two Factor Authentication (TOTP Based) using an Authenticator App like Google Authenticator.
    + **Google reCaptcha Module** - Add Google reCaptcha Check to the registration page to prevent bot/spam registrations. Adivsed for apps opening Public Registrations.
    + **Social Logins Module** - Allow users to register/login using their social media account. Currently supports Github, Facebook & Twitter.

---

<a name="credits"></a>
## Credits

**LaraPass** uses internally some open-source third-party libraries/packages, many thanks to the web community:

+ **`Laravel`** - Open source full-stack framework.
+ **`Muhamad Nauval Azhar`** - Thanks for the Stisla Template.
+ **`Bootstrap 4`** - Open source front end framework.
+ **`Livewire`** - A full-stack framework for Laravel by Caleb Porzio.
+ **`Spatie`** - Various amazing packages from Spatie.be.
+ **`spargon/laravel-auth-logger`** - Sends notifications when logging-in on new system/location.
+ **`techtailor/rpg`** - Random Password Generator & Encrypter for Laravel.
+ **`pragmarx/google2fa`** - Google TwoFactor Authentication Library.

---

<a name="contribute"></a>
## Contribute

**LaraPass v2** **Docs** are designed to guide our users through the installation process and help inform them of all the amazing features that **LaraPass v2** offers in detail. If you think there is anything missing in the docs, or you could make it more readable and better understandable for others, then visit the github page below and start contributing. Any contribution would be much appreciated & fully credited.

> {primary} **LaraPass v2 Docs Repository** &nbsp; <a href="https://github.com/LaraPass/Docs" target="_blank">**`https://github.com/LaraPass/Docs`**</a>