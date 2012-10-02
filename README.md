4sqWidget
=========

Foursquare Dashboard Widget for OSX.

Allows a User to easily check-in to a specified location.

Our company's website pulls a list of all users currently at the office via foursquare, 

this widget allows everyone to easily check-in to our office location so that they are listed

without the need to pull out their phone.

Opening the app after configuring it you will get the following screen

![Alt text](http://s12.postimage.org/4l8qlvcx9/Screen_Shot_2012_10_02_at_2_38_35_PM.png)

Clicking the info icon in the lower right will flip you to some minimal settings

![Alt text](http://s12.postimage.org/v7psol6i5/Screen_Shot_2012_10_02_at_2_39_16_PM.png)

Clicking authorize will take you to your callback URL where you will want to copy the string after access_token=

and enter it into the token box as shown above.

![Alt text](http://s12.postimage.org/4b5tg9not/Screen_Shot_2012_10_02_at_4_41_19_PM.png)

This is what you will look for after the redirect.



Configuration
=============

Clone the repo locally and open with Dashcode

Then press CMD+2 to open the source

look for an object called settings in main.js

```
var settings = {
  app_id: "",
  venue_name: "kohactive",
  venue_id: "4bc265a2f8219c74e0dab410",
  venue_longlat: "41.895347,-87.648072",
  permissions:  "public,twitter",
  redirect_url: "http://www.kohactive.com"
}
```

Here you can configure the app with long_lat, venue_id, venue name, callback url, and app_id

These are all things you acquire from http://foursquare.com/api when creating an app.

Good luck.


