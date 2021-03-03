# Google reCaptcha

Setting Up Google Invisible reCaptcha to work with your LaraPass App.

---

- [Sign Up](#signup)
- [Register Your Site](#register)
- [Add Keys to App](#keys)
- [Activate reCaptcha](#activate)
- [<a href="https://github.com/larapass/docs/edit/master/resources/docs/teams/misc/recaptcha.md" target="_blank"><i class="fa fa-edit"></i> Help us improve this page!</a>](#)

> {warning} The Google reCaptcha Setup Steps for all versions of LaraPass v2 are identical. You do not have to make any special changes for the Teams Version.

<a name="signup"></a>
## Sign Up

Go to [**`www.google.com/recaptcha/admin`**](https://www.google.com/recaptcha/admin) and Sign Up for Google's reCaptcha Services.


> {primary} Google reCaptcha is a **`Free`** service provided by Google. You can use your regular google/gmail account for the same. 

---

<a name="register"></a>
## Register Your Site

Once signed-up, you will be asked to register your site.

![screenshot](/screenshots/misc/recaptcha/register.png)

Enter a Label/Name for the Key (for self-identification)

Under reCAPTCHA Type - Select reCAPTCHA v2 & then Select Invisible reCAPTCHA Badge as shown below - 

![screenshot](/screenshots/misc/recaptcha/v2.png)

Add your domains & sub-domains. Add localhost if you to test larapass on your localhost system under "Domains"

![screenshot](/screenshots/misc/recaptcha/domains.png)

Accept Terms & Click on Submit.

> {info} Once you click on submit, you will get your ``reCAPTCHA`` keys. Store the ``SITE_KEY`` & ``SECRET_KEY`` safely.

---

<a name="keys"></a>
## Add reCaptcha Keys to your App

Go to Admin Menu -> Settings. Under ``Application Settings`` you have two fields for **Google reCaptcha Site Key** and **Google reCaptcha Secret Key**.

Take the Site & Secret Keys you got from Google Console and add it here & click on update.

Google Invisible reCaptcha Service is now active.

Visit ``yourapp.com/register`` to test it out.

---
<br />
<larecipe-feedback message="Thankyou for your feedback!">
</larecipe-feedback>
