# Basic Setup

Basic Setup required for installing `LaraPass v2 Personal Version` on your server.

---

- [Requirements](#requirements)
- [Setup](#setup)
- [VPS Server](#vps)
- [VPS Manager](#manager)
- [<a href="https://github.com/larapass/LaraPass-v2-Docs/edit/master/resources/docs/personal/basic-setup.md" target="_blank"><i class="fa fa-edit"></i> Help us improve this page!</a>](#)

<a name="requirements"></a>
## Requirements

```php
PHP >= 7.3
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

---

<a name="setup"></a>
## Setup

> {primary} **LaraPass** works best on a `VPS` with SSH Access. 

Below are some of the reputable and amazingly cheap VPS Providers -

**
[Digital Ocean](https://refs.spargon.tech/digital-ocean), [Vultr](https://refs.spargon.tech/vultr), [Amazon AWS](https://aws.amazon.com/free/)
**

Since these VPS provide raw server with resources, we will need a server manager to run our PHP applications such as LaraPass. Some of the suggested are - 

**
[Ploi](https://refs.spargon.tech/ploi), [RunCloud](https://refs.spargon.tech/runcloud), [ServerPilot](https://refs.spargon.tech/serverpilot), [Laravel Forge](https://forge.laravel.com/), [Cloudways](https://refs.spargon.tech/cloudways)
**

All of these service have slightly different pricing and features, so you can check them out and decide for your self. we personally would recommend the combination of **[Digital Ocean](https://refs.spargon.tech/digital-ocean)** & **[Ploi](https://refs.spargon.tech/ploi)** to get the most out of your investment.

We also recommend downloading & installing **`Bitvise SSH Client`** or any other of your choice so you can connect to your server easily.

> {warning} *While it does work, we do not recommend running **LaraPass v2** using Shared Hosting as Shared servers are not Secure and may create issues down the line (especially with respect to permissions).*

If you are still interested in using the cheaper Shared Hosting services, then we recommend using [**``A2Hosting``**](https://refs.spargon.tech/a2-hosting) and use coupon code **``SOFAST!``** for 51% Off.

[![img](https://affiliates.a2hosting.com/accounts/default1/banners/b33b2977.png)](https://www.a2hosting.com?aid=larapass&amp;bid=b33b2977)

> {success} Visit the [``cPanel Installation Guide Page``](cpanel) for details on how to successfully install **LaraPass v2** on cPanel powered server.

---

<a name="vps"></a>
## VPS Server

 Setting up a VPS server provided by [**`Digital Ocean`**](https://m.do.co/c/1b88e7535dea) or any other from the above list is very simple and straight forward. These steps are general and are not specific to **LaraPass**. If you already know how to provision a DO server, then just skip this section. If you are using [**Cloudways**](https://www.cloudways.com/en/?id=94888), then you don't need to register at DO, they will handle everything (albeit at an extra premium).

 **Step # 1 -** Visit [**`DigitalOcean.com`**](https://m.do.co/c/1b88e7535dea)  
 **Step # 2 -** Create an account. Use coupon/promo code **`DO10`** to get Free Credit to Launch your first server.  
 **Step # 3 -** Go to **`Create Droplets`**. Select Distritutions/OS as **`Ubuntu 18.04 x64`**.  
 **Step # 4 -** Select any size as per your budget, we recommend the **`$10/mo - 2GB Droplet Size`** & Select a **`region`** as per your desire.  
 **Step # 5 -** Choose a **`Hostname`** and Click **`Create`** and wait for the server to get provisioned.  
 **Step # 6 -** Once the server is provisioned, you will get an Email with the Server IP & the root password.  
 **Step # 7 -** If you haven't already, then you need to point your Domain Nameservers to DigitalOcean [Read More](https://www.digitalocean.com/community/tutorials/how-to-point-to-digitalocean-nameservers-from-common-domain-registrars).  
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

<a name="manager"></a>
## VPS Manager

A VPS always comes as a barebones pc, as such in order to run web applications or websites on them we need to use a VPS Manager. For **LaraPass** we will be going with [**Ploi**](https://ploi.io/register?referrer=GTVyGH2vz2N3tN84XxW7) because unlike others, it comes with a Free Option (along with Free SSL) which allows you to manage your LaraPass site for **`Free`**. For more details visit [**Ploi.io**](https://ploi.io/register?referrer=GTVyGH2vz2N3tN84XxW7). These steps are general and not specific to **LaraPass**. If you already know how to link your VPS with a Manager, then just skip this section.

**Step # 1 -** Go to [**`Ploi.io`**](https://ploi.io/register?referrer=GTVyGH2vz2N3tN84XxW7) & Sign Up.  
**Step # 2 -** Click on **`Create Server`**.  
**Step # 3 -** Click on **`Custom VPS`** under Select Provider.  
**Step # 4 -** Copy the **`Command`** shown under `"You can also use this one-liner to add the authorized key:"`, its something like this - (do not copy the command below, its just a dummy one)

```php
mkdir -p /root/.ssh && touch /root/.ssh/authorized_keys && echo "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQC6BBCdgfd/8FblBAwAuZYFQti4xOub2BxlMMwjMajI+JM91bD81B6xBA19gBTrc194SuoD1L/T7tna66XQsBUchC2YBF/akdwyyduSBJh/yK98JCMNZyNcE0qZ/g9MhCfkYI3ZkFLOeoTYsDEUpkzNKePu9r6egBSFQj0TGNAKyZ3wohnM469CoCS0Jh6kbOOa+kp7OLr0jXRY5l7f8MCEjPcVldkYFhXhxIFQ6GZnGdnayqnlBVRpN4/4q1X+HTsMOWKcTtJembJ8wThaKnAUhsZjNOitD9edhsDu+K9JeZU8egnP8tz28i+8pFcuPykoeqUJOCgMCiuHuvMhu2iL ploi-worker" >> /root/.ssh/authorized_keys
```
**Step # 5 -** Login to your VPS Server as **`root`** using **`Bitvise SSH Client`** or **`CyberDuck`** or directly from Digital Ocean Server Panel.  
**Step # 6 -** **`Paste`** the **`Command`** you copied in **Step # 4**.  
**Step # 7 -** Come back to **`Ploi`**, enter your `Server Name`, `IP Address`, `Select OS`, `PHP Version as 7.3`, `MySQL Version as 5.7` and click on **`Create Server`** and wait for it to provision.  
**Step # 8 -** Once done, head over to your server on ploi, click on add sites, add your domain name and in the directory add /public (since its a laravel installation).  
**Step # 9 -** All done. Visit the Installation Page to get started with installing LaraPass on your server.

> {info} If you are unfamiliar with setting up a VPS server and deploying a site or don't have time for it, we can do complete setup and installation (via TeamViewer) for you at an extra charge. Contact **`support@larapass.net`** for more details and exact quote.

[DO & PLOI Setup Video]