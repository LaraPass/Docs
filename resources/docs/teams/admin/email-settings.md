# Email Settings (Transactional Emails) - Teams Version

Admin Email Settings page of `LaraPass v2 Teams Version`

---

- [Overview](#overview)
- [Recommended Mailers](#recommended)
- [Configuration](#configuration)
- [Send Test Mail](#test)
- [<a href="https://github.com/larapass/docs/edit/master/resources/docs/teams/admin/email-settings.md" target="_blank"><i class="fa fa-edit"></i> Help us improve this page!</a>](#)

<a name="overview"></a>
## Overview

You can update your mailer for sending notifications and update emails from here.

![screenshot](/screenshots/admin/settings/email-1.png)

---

<a name="recommended"></a>
## Recommended Mailers

We recommend the following mailing services as best for sending transactional emails. However, you are free to use any 3rd-Party service that allows outgoing SMTP services (ex: Gmail, etc).

<p float="left">
  <a href="https://refs.spargon.tech/mailgun"><img src="/brands/mg_logo.png" width="180" alt="mailgun"/></a> &nbsp;
  <a href="https://refs.spargon.tech/elastic-email"><img src="/brands/ee_logo.png" width="180" alt="elastic-email"/></a> &nbsp;
  <a href="https://refs.spargon.tech/send-grid"><img src="/brands/sg_logo.png" width="180" alt="send-grind"/></a> &nbsp;
  <a href="https://refs.spargon.tech/send-in-blue"><img src="/brands/sib_logo.png" width="180" alt="send-in-blue"/></a>
</p>
---

<a name="configuration"></a>
## Configuration

LaraPass mailer offers 3 types of mail drivers for sending outgoing emails - 
+ **`Log`** (all emails/notifications sent are logged into the laravel.log file in the local storage) - Only use this for testing.
+ **`SMTP`** (use any 3rd party service that provides smtp for outgoing emails and add credentials for that here).
+ **`Mailgun API`** (setup mailgun and get their API & Secret Key and add it here).  
<br/>

After selecting the **`Mail Driver`**, configure the mailer accordingly - 

+ Enter the **Mail Host Address** you get from your mailing service provider (only when using the SMTP Driver).
+ Enter the **Mail Port** - usually 587 (only when using the SMTP Driver).
+ Select **Mail Encryption** - usually START/TLS (only when using the SMTP Driver).
+ Enter the **Mail Username** - your smtp login username (only when using the SMTP Driver).
+ Enter the **Mail Password** - your smtp login password (only when using the SMTP Driver).
+ Enter the **Mail From Address** - The `sent from email` to be shown in the emails (required for all drivers).
+ Enter the **Mail From Name** - The `sent from name` to be shown in the emails (required for all drivers).
+ Enter the **Mailgun Domain** - your mailgun domain (only when using the Mailgun API Driver).
+ Enter the **Mailgun Secret Key** - your mailgun secret key (only when using the Mailgun API Driver).

---

<a name="test"></a>
## Send Test Mail

After configuring the mailer, click on the **`Send Test Mail`** button to test and verify whether the email is being sent and received as expected or not. The *test* email will be sent to the email address stored as `App Email` in the [**General Settings**](general-settings).

---
<br />
<larecipe-feedback message="Thankyou for your feedback!">
</larecipe-feedback>  