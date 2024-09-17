# Mailgun

Setting Up Mailgun to work with your LaraPass installation

---

- [Sign Up](#sign-up)
- [Add Domain](#add)
- [DNS Settings](#dns)
- [Wait For DNS](#wait-dns)
- [Ready to Use](#ready) 
- [Credit](#credit)
- [<a href="https://github.com/larapass/docs/edit/master/resources/docs/teams/misc/mailgun.md" target="_blank"><i class="fa fa-edit"></i> Help us improve this page!</a>](#)

> {warning} The Mailgun Setup Steps for all versions of LaraPass v2 are identical. You do not have to make any special changes for the Teams Version.

<a name="sign-up"></a>
## Sign Up

Go to [**`www.mailgun.com`**](https://refs.spargon.tech/mailgun) and SignUp for a Free Account.


> {primary} Mailgun Offers **`5,000 Emails/month`** for Free per month for 3 months. 

---

<a name="add"></a>
## Add Domain

In your **Mailgun** Control Panel, go to **`Domains`** & then click on **`Add New Domain`**

Enter a domain you own. Please note that you can use this one domain with many services.

Follow the 4 Steps shown on the page to complete the setup. If you are finding difficulty in following them, then go [**here**](http://code.krister.ee/mailgun-digitalocean/) for a more detailed guide

> {info} We are using **`mg.domain.com`** subdomain just to separate concerns. Its actually easier and more practical to just use your main **`domain.com`** instead.

![screenshot](/screenshots/misc/mailgun/add-domain.gif)

---

<a name="dns"></a>
## DNS Settings

Now Mailgun should have directed you to the DNS settings page. To find it manually, go to the Domains tab and select your domain. Here's a sample cropped image :

![screenshot](/screenshots/misc/mailgun/add-dns.png)  
&nbsp;
##### Log into DigitalOcean and select the Networking tab on the left.
&nbsp;

![screenshot](/screenshots/misc/mailgun/do.gif)
&nbsp;

##### * Select your **`mydomain.com`** (no need to create separate subdomain).  
&nbsp;
##### * Use the **`Add record`** button to add all the necessary information.  
&nbsp; 

![screenshot](/screenshots/misc/mailgun/record.gif)

&nbsp;  

##### Basically you need to convert the Mailgun provided data into this:

![screenshot](/screenshots/misc/mailgun/converted.png)

### **Things to notice when entering data**
+ the txt details may need to be in double quotes: **`v=spf...`**
+ Domain values need dots at the end (DigitalOcean will tell you this)
+ the **`v=spf`** part needs an **`@`** in front, not your domain, as Mailgun instructs.
+ Mailgun domains use the extension **`.org!`**

---

<a name="wait-dns"></a>
## Wait for DNS records to update

Usually this takes about 24 hours. If you're in a hurry you're welcome to go insane with the "Check DNS Records Now" button.

---

<a name="ready"></a>
## Ready to Use

You can now configure your LaraPass app to send emails using Mailgun.

Open Email Settings at `https://yourdomain.com/admin/settings/email`
+ Select Mail Driver as SMTP if you want to use Mailgun SMTP Credentials.
+ Add the SMTP Credentails you got from Mailgun & Save.
+ or Select Mailgun API if you want to use Mailgun API.
+ Add the Mailgun API Key & Secret you got from Mailgun & Save.
+ Click on **Send Test Mail** to verify your mailer is setup properly.

---

<a name="credit"></a>
## Credit

This Mailgun tutorial was borrowed from **`Krister Viirsaar`**. You can check out his original post [**`here`**](http://code.krister.ee/mailgun-digitalocean/)

---
<br />
<larecipe-feedback message="Thankyou for your feedback!">
</larecipe-feedback>