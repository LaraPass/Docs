# Basic Setup - Teams Version

Basic Setup required for installing `LaraPass v2 Teams Version` on your server.

---

- [Requirements](#requirements)
- [Hosting & Host Manager](#hosting)
- [Digital Ocean Setup](#do)
- [<a href="https://github.com/larapass/docs/edit/master/resources/docs/teams/basic-setup.md" target="_blank"><i class="fa fa-edit"></i> Help us improve this page!</a>](#)

> {primary} The Basic Setup and Installation Steps for Teams and Personal Versions are identical. If you have experience installing the Personal Version, the experience with the Teams Version will be no different.

<a name="requirements"></a>
## Requirements

```php
PHP >= 7.4
Following PHP Extensions:
 - BCMath
 - Ctype
 - Fileinfo
 - JSON
 - Mbstring
 - OpenSSL
 - PDO
 - Tokenizer
 - XML
 - Zip Module
NGINX or Apache
MySQL or MariaDB
SSH Access (Recommended)
```
> {success} You can download the LaraPass v2 Compatibility Tester from [`here`](https://github.com/LaraPass/CompatibilityTester) and confirm whether your server supports it or not.

---

<a name="hosting"></a>
## Hosting & Host Manager

> {primary} **LaraPass** works best on a `VPS` with SSH Access. 

Below are some of the reputable and amazingly cheap VPS Providers -

**
<a href="https://refs.spargon.tech/digital-ocean" target="_blank">Digital Ocean</a>, <a href="https://refs.spargon.tech/vultr" target="_blank">Vultr</a>, <a href="https://aws.amazon.com/free/" target="_blank">Amazon AWS</a>
**

Since these VPS provide raw server with resources, we will need a server manager to run our PHP applications such as LaraPass. Some of the suggested are - 

**
<a href="https://refs.spargon.tech/ploi" target="_blank">Ploi</a>, <a href="https://refs.spargon.tech/runcloud" target="_blank">RunCloud</a>, <a href="https://refs.spargon.tech/serverpilot" target="_blank">ServerPilot</a>, <a href="https://forge.laravel.com/" target="_blank">Laravel Forge</a>, <a href="https://refs.spargon.tech/cloudways" target="_blank">Cloudways</a>
**

All of these service have slightly different pricing and features, so you can check them out and decide for your self. we personally would recommend the combination of <a href="https://refs.spargon.tech/digital-ocean" target="_blank">**Digital Ocean**</a> & <a href="https://refs.spargon.tech/ploi" target="_blank">**Ploi**</a> to get the most out of your investment.

We also recommend downloading & installing **`Bitvise SSH Client`** or any other of your choice so you can connect to your server easily.

> {warning} *While it does work, we do not recommend running **LaraPass v2** using Shared Hosting as Shared servers are not Secure and may create issues down the line (especially with respect to permissions).*

If you are still interested in using the cheaper Shared Hosting services, we recommend using <a href="https://refs.spargon.tech/a2-hosting" target="_blank">**`A2Hosting`**</a> and use coupon code **``SOFAST!``** for 51% Off.

[![img](https://affiliates.a2hosting.com/accounts/default1/banners/b33b2977.png)](https://www.a2hosting.com?aid=larapass&amp;bid=b33b2977)

> {success} Visit the [``cPanel Installation Guide Page``](setup/cpanel) for details on how to successfully install **LaraPass v2** on cPanel powered server.

---

<a name="do"></a>
## Digital Ocean Setup

 Setting up a VPS server provided by <a href="https://refs.spargon.tech/digital-ocean" target="_blank">**`Digital Ocean`**</a> or any other from the above list is very simple and straight forward. These steps are general and are not specific to **LaraPass**. If you already know how to provision a DO server, then just skip this section. If you are using <a href="https://refs.spargon.tech/cloudways" target="_blank">**`Cloudways`**</a>, then you don't need to register at DO, they will handle everything (albeit at an extra premium).

 **Step # 1 -** Visit <a href="https://refs.spargon.tech/digital-ocean" target="_blank">**`Digital Ocean`**</a>  
 **Step # 2 -** Create an account. Use coupon/promo code **`DO10`** to get Free Credit to Launch your first server.  
 **Step # 3 -** Go to **`Create Droplets`**. Select Distritutions/OS as **`Ubuntu 20.04 (LTS) x64`**.  
 **Step # 4 -** Select any size as per your budget, larapass works fine even with the **`$5/mo - 1GB Droplet Size`** & Select a **`region`** as per your desire.  
 **Step # 5 -** Choose a **`Hostname`** and Click **`Create`** and wait for the server to get provisioned.  
 **Step # 6 -** Once the server is provisioned, you will get an Email with the Server IP & the root password.  
 **Step # 7 -** If you haven't already, then you need to point your Domain Nameservers to DigitalOcean <a href="https://www.digitalocean.com/community/tutorials/how-to-point-to-digitalocean-nameservers-from-common-domain-registrars" target="_blank">Read More</a>.  
 **Step # 8 -** Go to **`Networking -> Domains`** and Add your Domain.  
 **Step # 9 -** Lastly, create 2 new records for your domain as listed below:

 ```php
 Hostname : @
 Will direct to : your-server-ip-address
 TTL : 1800

 Hostname : www
 Will direct to : your-server-ip-address
 TTL : 1800
 ```

---
<br />
<larecipe-feedback message="Thankyou for your feedback!">
</larecipe-feedback>