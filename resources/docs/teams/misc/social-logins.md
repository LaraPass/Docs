# Social Logins using OAuth

Guide to setup Social Logins using OAuth for your App.

---

- [Overview](#Overview)
- [Enable Social Logins](#enable)
- [Github Login Setup](#github)
- [Facebook Login Setup](#facebook)
- [Twitter Login Setup](#twitter)
- [<a href="https://github.com/larapass/docs/edit/master/resources/docs/teams/misc/social-logins.md" target="_blank"><i class="fa fa-edit"></i> Help us improve this page!</a>](#)

> {warning} The Social Logins Setup Steps for all versions of LaraPass v2 are identical. You do not have to make any special changes for the Teams Version.

<a name="overview"></a>
## Overview

LaraPass v2 uses OAuth for enabling Social Logins. OAuth (2.0) is the industry-standard protocol for authorization. It allows for easy flow of information (as much authorized) from one-point-to-another, in our case, from the social media site to your LaraPass v2 App.

---

<a name="enable"></a>
## Enable Social Logins

Details on how/where to add your OAuth credentials can be found [**`here`**](../admin/modules-manager#social) On this page, we will be focusing on learning how to get the credentails (an API Key & a Secret Key) from the social netwrok (Github, FB, Twitter, etc).

---

<a name="github"></a>
## Github Login Setup

Follow the steps below to create an OAuth app on Github and get your API & Secret Key.

`+` **`Step # 1`** - Login to your Github account - you can use your personal account or your organizations' account (imo using an official organization account brings legitimacy).
  
`+` **`Step # 2`** - Go to **Developer Settings**. For personal accounts you can find it here - `https://github.com/settings/developers`, for organization accounts, you will find it here - `https://github.com/organizations/your_organization/settings/applications`
  
`+` **`Step # 3`** - Click on **Register a new application** or **New OAuth App**.
  
`+` **`Step # 4`** - Enter your app name (something thats recognizable by users).
  
`+` **`Step # 5`** - The URL of your app, ex: for our demo its `https://personal-demo.larapass.net`
  
`+` **`Step # 6`** - A few words describing your app/site.
  
`+` **`Step # 7`** - **Authorization callback URL** - Take the app url from **Step # 5** and add **`/login/github/callback`** at the end. This is important. Ex: in our demo the Callback URL is **`https://personal-demo.larapass.net/login/github/callback`**.
  
`+` **`Step # 8`** - Once created, you can add your app's logo (improves identification) and done. You will now have access to your OAuth App Client ID and Secret Key (as shown below).
  
`+` **`Step # 9`** - Enter these in the Social Logins Module, Enable it and voila, you are good to go.

![screenshot](/screenshots/misc/social/github-creds.png)


---

<a name="facebook"></a>
## Facebook Login Setup

Coming Soon!

---

<a name="twitter"></a>
## Twitter Login Setup

Coming Soon!

---
<br />
<larecipe-feedback message="Thankyou for your feedback!">
</larecipe-feedback>
