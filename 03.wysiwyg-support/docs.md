---
title: WYSIWYG Support
taxonomy:
    category: docs
---

## Using Wyvern Video in a WYSIWYG editor

When inserting a video into the WYSIWYG editor of your choice (hopefully you are using Wyvern), it will insert an image place holder into the editing field. Upon saving of the entry it will replace the image with the full iframe embed code. Only Wyvern will provide extra options in the field settings page. Wygwam and Expresso do not have access to define a video size, instead it will default to the 360x240 dimensions, however, users can change these values when selecting their video in the pop-up window.

## Wyvern Support
To configure Wyvern to use Wyvern Video:

1. Move the plugins/video folder from the Wyvern Video package into into themes/third_party/wyvern/plugins/video directory.
2. Edit and save the toolbar(s) you want to add the video button to and select the Video toolbar button.

## Wygwam Support
To configure Wygwam to use Wyvern Video:

1. Move the plugins/video folder from the Wyvern Video package into into themes/third_party/wygwam/lib/ckeditor/plugins/ directory.
2. Edit the toolbar(s) you want to add the video button to. Select the extraPlugins option in the configuration list, and in the field value enter video. <a href="http://boldminded.com/assets/images/uploads/wv-wygwam-config.png">It should look like this</a>. Save the toolbar, then you should now see the Wyvern Video button at the end of the button list on your publish entry page.

## Expresso Support
To configure Expresso to use Wyvern Video:

1. Make sure the Video toolbar button is selected in the fieldtype settings page.
2. Move the plugins/video folder from the Wyvern Video package into themes/third_party/expresso/ckeditor/plugins/ directory. A video folder will already exist there, just save over it.
3. Open themes/third_party/expresso/javascript/expresso.js and find the extraPlugins: “header”, line and change it to extraPlugins: “headers,video”,