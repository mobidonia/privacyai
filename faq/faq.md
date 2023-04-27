---
description: Frequently Asked Questions (FAQs)
---

# FAQ - Technical

## Install the project in subdomain

When you want to run your project in subdomain, you need to declare this subdomain in your Settings. To do that, you will need to go to Site setting->Setup->Subdomains and add your domain there. Ex, if you want to run the project in app.domain.com.

![](https://i.imgur.com/k6uuMa2.jpg)

## Notification translation

One really common problem is that the emails is no received correctly. Password or email is missing. and here is the reason why. Please check this [video](https://www.loom.com/share/112938a8fa31418386b5ae2c8c71303b)



## Error 500

**Problem**\
You get a white screen with Error 500 as on this screen.

![](https://i.imgur.com/HZmpG35.png)

**Reason**\
This is a general error, meaning something wrong happened in the system. And it can be from different causes. it can be a bug or misconfiguration.

**Option 1: Enable debug mode from admin**\
First, we need to see why this error happens,\
Enable debug mode, so you can see what is behind the 500 error. To do that

1. Login as admin
2. Go In **Setting**
3. Select **Setup** tab
4. Select **APP\_DEBUG**

Then try to reproduce the problem. Now, you will see a lot more information about the problem. If you do understand the message, you get, you may fix the problem on your own. Some common ones are SMTP are Stripe Misconfiguration. For these ones you may try to fix on your own, by going in settings to check if what you have entered is correct.

**Option 2: Enable debug mode from cPanel file manager**\
In case you are not able to login, you have the option to manually enable debug mode.

1. Go to your cPanel file manager
2. Find the file **.env** and edit it. This file is hidden so you may need to [show hidden file in cPanel](https://www.plothost.com/kb/show-hidden-files-htaccess-cpanel-file-manager/)
3. Locate APP\_DEBUG=false and change it to
4. APP\_DEBUG=true
5. Now you have debug mode ON

Then try to reproduce the problem. Now, you will see a lot more information about the problem. If you do understand the message, you get, you may fix the problem on your own. Some common ones are SMTP are Stripe Misconfiguration. For these ones you may try to fix on your own, by going in settings to check if what you have entered is correct.

**Share a link to the error** For some other reported errors, don't hesitate to contact us with a link of the Flare Error of the problem here [https://help.mobidonia.com/](https://help.mobidonia.com)

Here is how you can obtain a link.

![](https://i.imgur.com/pfxNCqH.png)



## Error on uploading an image

**Error**

"PHP Fileinfo extension must be installed

**Reason**\
"PHP Fileinfo extension must be installed/enabled to use Intervention Image."

The project needs the [fileinfo](https://i.stack.imgur.com/vhN3E.png) extension.

**Solution**

As you can see on the [image](https://i.stack.imgur.com/vhN3E.png), it can be enabled from PHP Selector. But if there is no PHP Selector you should have access to **WHM**.

**IN WHM**

Initially, we login to WHM and navigate as follows,

Software >> EasyApache 4 >> Customize >> PHP extensions.

Here we search for **fileinfo** and enable phpx.x-php-fileinfo for all versions. Finally, we click on Review and Provision.

This enables the file extension for all the PHP websites in the server.

Let me know about this.

## How to force HTTPS

In order to force your site to run only in HTTPS login as admin, then go in "Site Setting" and in "Setup" tab locate the "App environment". And set it to "Production".

This is what can be done on the Project level. Make sure you have valid SSL and that you have set the HTTPS force on the hosting level also.

## How to enable PHP Extension

If you get an error like this one

![](https://i.imgur.com/EXp59rL.png)

This indicates that the INTL extension - or depending on the problem, another one is not enabled.

Here is a good video on how you can enable it. If you can't. Please speak with your hosting provider.

{% embed url="https://www.youtube.com/watch?v=kYwRtMwWerQ" %}
