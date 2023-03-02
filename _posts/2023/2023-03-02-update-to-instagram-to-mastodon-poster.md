---
title: Instagram to Mastadon Crossposter update!
categories:
- Geek
tags:
- mastadon
- instagram
- postman
- geek
---
Irony of ironies, now that I have pointed out my [Instagram to Mastodon Crossposter]({{ "/2019/12/16/how-to-post-instagram-posts-on-mastodon-using-ifttt.html" | relative_url }}) in my [previous article]({{ "/2022/11/11/on-migrating-from-twitter-to-mastadon.html"| relative_url }}), someone has messaged me to say it's stopped working! As expected, it was due to changes in the Mastodon API in the three years since I last touched it, so here is an updated version of how to auto-post your latest Instagram images on Mastodon using If This Then That (IFTTT) <!--more-->

## Requirements

What you will need is:

1. An Instagram account. (Obviously!)
2. An account at [If This Then That](https://ifttt.com/). (Referred to through the rest of this post as "IFTTT".)
3. The root URL of your Mastodon instance.
4. An API key from your Mastodon instance. (We'll cover this in the next section.)

## Getting the API key

This is very important, as you will need this key to post to Mastodon. Note that you need to get this key from your **own Mastodon instance**.

1. Log in to your Mastodon instance, and select "Edit my profile".
2. On the left hand menu, select "Development", and then from the top right, select "New Application".
3. Fill in the form as follows:
   - Name: Anything you like, but I suggest "Instagram to Mastodon Crossposter".
   - Website: As the request is coming from IFTTT, put "https://ifttt.com" here.
   - Redirect URI: You don't need to change this.
4. The next part of the form concerns the "Permissions" of the application. You can select "Read"
   and "Write" permissions, and uncheck "Follow". If you *really* want to be careful with the permissions, you could restrict permissions to "Read:statuses" and "Write:statuses".
5. Select the "Save Changes" button at the bottom of the page.
6. You will now see the application you just created on the "Your applications" page. Click the link to enter the page.
7. At the top of the page you will see your access token listed as , approppriately enough,  "Your access token". Take a copy of this, as you will need this for the next section.

## Creating an App in IFTTT

***NOTE**: If you're upgrading your old crossposter in order to fix it, you can skip this part. Go to the app's "Settings".*

* Log into IFTTT.
* Select the "Create" button.

### Instagram integration

**If you have not added Instagram:**

* Select the "Add" button on this "If This..." panel.
* On the "Choose a service" page, search for "Instagram" and pick it. There is a search bar underneath the "All services" menu, so if you type `instag` into it, you'll see the instagram service.
* On the "Choose a trigger" page, select "Any new photo by you".
* On the next page you connect to your Instagram account. This will require logging in to your
  Instagram account, and giving permission to IFTTT to see your posts.
* Finall select "Create trigger" to complete the process.

**If you have added Instagram:**
If you are updating your old crossposter, you will already have Instagram added. However, the access key may have expired. So it's worth going to the "edit" link on the "If This..." panel, and checking. You may need to select "reconnect account" to re-authorise IFTTT to access your Instagram account. This will require logging in to your Instagram account, and giving permission to IFTTT to see your posts.

### Mastodon integration

The nice thing about IFTTT is that it's a way to interrogate API and RSS services without having to mess with complicated coding solutions. We just used one of IFTTT's built-in services to connect to Instagram's API. Unfortunately, there is no such service for Mastodon, and unless IFTTT works out a way to connect to individual Mastodon instances, there probably never will be one. However, we can work around this by using IFTTT's "Webhooks" service to connect to our Mastodon instance, which unfortunately is a bit more like coding, but it works if you know what your are doing.

* Select the "Add" button on this "Then That..." panel.
* On the "Choose a service" page, search for "webhooks" and pick it. There is a search bar
  underneath the "All services" menu, so if you type `webh` into it, you'll see the webhooks service.
* On the "Choose an action" page, select "Make a web request".

#### Setting up the web request

You will want the following values set in the form:

* URL: `https://[URL OF YOUR MASTODON INSTANCE]/api/v1/statuses`
* Method: `POST`
* Content Type: `application/x-www-form-urlencoded`
* Additional Headers: `Authorization: Bearer [YOUR_ACCESS_TOKEN]`
* Body: `status=New on Instagram: {% raw %}{{Caption}} {{Url}}{% endraw %}`
  You can customise the text in the body, but you will need to keep the `status=` part, as this is the part that tells Mastodon what to post. You can also add other fields, such as `visibility=unlisted` to make the post unlisted, or `sensitive=true` to mark the post as sensitive. You can find out more about the options for posting statuses in the Mastodon API [here](https://docs.joinmastodon.org/api/rest/statuses/).
* Select "Create action" to complete the process.

### Testing the app

After creating or updating the app, you will return to the app's home page. Check that the "Connected" slider button is set to "on". You can now test that the app is working, by selecting the "Check now" button near the bottom of the page. When clicked there will be a pause, then the  banner "Check completed" should appear. If there's a problem you'll get an error message.

If there's an error, there are two areas in which to check.

* Check that IFTTT can still connect to Instagram.
* Check the values in the Web Request. On this front, I used [Postman](https://getpostman.com) to debug the API call to my Mastodon instance.

---

So after all, that I now have brought back my crossposter back to life, and hopefully more of my photos from Instagram will reach my followers in the Fediverse!
