# Set up your site

## Change Favicon

1. Login as admin
2. Go to Settings->images
3. Upload your favicon

## Change the project logo and default images

Go to your project and login as admin.\
In the settings page, you will be able to change the project logo and the default images for the menu items and the cover image in the restaurant menu.

## Change email send by the system

If you go to this folder **app/Notifications**

There are list of PHP files that represent the content of the email And inside them, there is function called **toMail**

You can modify the strings there.

If you want to change the layout, ex, include some CSS for the email you can edit the blade file here **resources/views/vendor/notifications/email.blade.php**

## **Change the content of the front page**

The landing page code is located in **modules/Privacygen/Resources/views/landing/home.blade.php** **.** If you want to do structural changes you can edit those files there. In our updates, we try not to change these files as much as possible. But for just in case, make a backup of them when you have done your changes.

If you want to change the css, the best way to do that will be throught the option to add custom CSS inside Admin->Setting->CSS and JS. There you can define your own CSS and JS, so if we have an update on our CSS or JS doesn't discard your changes.

To modify the images, you can do that from Admin->Settings->Images.

To change the text, you can do that via the inline editing tool on the front page if you login as admin.
