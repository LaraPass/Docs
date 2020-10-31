# cPanel Installation Guide

LaraPass Installation Guide for cPanel powered Shared/VPS Hosting Servers.

---

- [Downloading](#downloading)
- [Setup cPanel](#setup_cpanel)
- [Uploading](#uploading)
- [Setup Database](#setup_database)
- [Installing](#installing)
- [<a href="https://github.com/larapass/LaraPass-v2-Docs/edit/master/resources/docs/personal/misc/cpanel.md" target="_blank"><i class="fa fa-edit"></i> Help us improve this page!</a>](#)

<a name="downloading"></a>
## Downloading

Download all the files you get after purchasing **Larapass** from **`CodeCanyon`** (Envato). 

> {primary} Keep the License File (with License/Purchase Code) safely as you will need it to `activate` LaraPass. 

Extract all the files into a safe location. Also extract the **`laravel_source`** zip_file into a folder (it contains all the main files we will be uploading to our server).

---

<a name="setup_cpanel"></a>
## Setup cPanel

Open cPanel in your browser, usually available at the url address **``yourdomain.com:2082``** .

Navigate to your **``Domains``**, **``Addon Domains``** or **``Sub-domains``** depending on which type of domain you want to install LaraPass on. For this example we will be using a sub-domain, so click on the Sub-Domains Page in your cPanel (the proceedure is almost same for all types of domains).

![screenshot](/screenshots/misc/cpanel/sub.png)

* **Pick a new subdomain, in our case,** **``demo``**

* **Select the domain name, in our case,** **``larapass.net``**

* **Document Root -** **``larapass/public``** (remove the default document root that pops up)

* **Click** **``Create``**

![screenshot](/screenshots/misc/cpanel/sub_added.png)

> {info} *Becareful - larapass app should always be placed in or point towards a directory in the root/home directory of your server and not be accessible using the publicly available directory*

---

<a name="uploading"></a>
## Uploading

Open File Manager in cPanel or login to your server using an FTP program such as FileZilla or CyberDuck.

Navigate to the larapass directory and open it (should be present in the root or home directory).

![screenshot](/screenshots/misc/cpanel/larapass.png)

Upload all the files & folders you got from the **`laravel_source`** zip_file into the server directory.

> {warning} *Becareful not to miss any file or interrupt when uploading to server.*

![screenshot](/screenshots/misc/cpanel/lp.png)

---

<a name="setup_database"></a>
## Setup Database

Open MySQL Databases in your cPanel.

* **Create a new database.**

![screenshot](/screenshots/misc/cpanel/mysqldb.png)

* **Create a new user (with a unique password).**

![screenshot](/screenshots/misc/cpanel/mysqlusers.png)

* **Add the newly created user to the larapass database and**

![screenshot](/screenshots/misc/cpanel/mysqldbuser.png)

* **add ALL PRIVILIGES to that user.**

![screenshot](/screenshots/misc/cpanel/mysqluserpriv.png)

> {success} Note down the ``Database Name``, ``Username`` and ``Password`` to be used in the next step for Installation.

---

<a name="installing"></a>
## Installing LaraPass

Follow the instructions [**here**](../installation/overview#installing)

---