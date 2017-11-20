---
title: Installation
taxonomy:
    category: docs
---

To install Reel move the ``/addons/reel/`` directory to your ``/system/user/addons/`` folder. Also copy the ``/themes/user/reel/`` folder to the ``/themes/user/`` directory in your ExpressionEngine install. Login to your control panel and visit the Developer > Add-on Manager page, and click the Install link for Reel.

## Differences from Wyvern Video

Reel is the ExpressionEngine 3+ version of Wyvern Video. Many of the features found in Wyvern Video are available in Reel, however, due to the maintainability concerns, and general lack of use, one feature was removed, which is the ability to embed a video inside of a WYSIWYG editor (such as Wygwam, Wyvern, or the native RTE).

## Upgrading from Wyvern Video

If you are upgrading from ExpressionEngine 2 to 3 and previously used Wyvern Video, the upgrade process should be seemless. Simply install Reel in ExpressionEngine 3 once you have upgraded. All the Wyvern Video fields will be converted to Reel, then un-install Wyvern Video and delete its files.

## YouTube and Vimeo API keys

In order to use Reel you must provide YouTube and/or Vimeo API credentials:

### YouTube

Go to http://developers.google.com and read the Introduction section on who to obtain a Server API Key.

### Vimeo

Go to https://developer.vimeo.com/apps and create an API app so Reel can load videos from Vimeo. Once you create an app go to the authentication page where you will see the Client Identifier and Client Secrets created for your app. You will need to manually create an access token at the bottom of the Authentication page. Create a token with Public and Private access to your videos.

If you need to view private Vimeo videos you will need to use the numeric user ID, not friendly account handle found in the URL. You can find this ID in your Vimeo account page.

