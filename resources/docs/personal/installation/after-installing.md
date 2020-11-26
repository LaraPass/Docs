# After Installing

After Installation Guide for `LaraPass v2 Personal Version`.

---

- [Outgoing Mailer](#mailer)
- [Privacy & Terms Pages](#pages)
- [<a href="https://github.com/larapass/docs/edit/master/resources/docs/personal/installation/after-installing.md" target="_blank"><i class="fa fa-edit"></i> Help us improve this page!</a>](#)

<a name="mailer"></a>
## Outgoing Mailer

LaraPass v2 sends allot of transactional emails for a variety of reasons such as - email verification, password reset, account information, limit notifications, personal data requests, etc., as such an outgoing mailer needs to be setup and configured. If you don't setup one, several critical functions of LaraPas v2 won't work (during testing/development you can set the mailer as `log` and all outgoing mails will be stored in `/storage/logs/laravel.log` file).  

> {primary} Detailed instructions on how to setup your mailer can be found [`here`](../admin/email-settings) 

---

<a name="pages"></a>
## Privacy & Terms Pages

LaraPass v2 comes with a build in page manager out of the box with a WYSIWYG editor. We have inserted placeholders for your app's Privacy & Terms of Service Pages which you can easily edit and update with your terms and wordings by opening the pages manager here - 

```php
yourdomain.com/admin/pages
```
and clicking on the `Edit` button under the Privacy Page or the Terms of Service Page.

> {primary} Detailed instructions on how to manage your pages can be found [`here`](../admin/pages-manager) 

---
<br />
<larecipe-feedback message="Thankyou for your feedback!">
</larecipe-feedback>

