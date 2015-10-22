# FA Sceditor Emoji

This small plugin allows for the use of [Twitter Emojis](https://github.com/twitter/twemoji) in the SCEditor on Forumactif forums.

## Installation

To instsall this plugin go to Admin Panel > Modules > JavaScript codes management and create a new script with the following settings.

1. **Title :** Twemoji
2. **Placement :** In all the pages
3. Paste the [raw source](https://raw.githubusercontent.com/SethClydesdale/fa-sceditor-emoji/master/twemoji-button.js) into the textarea and click submit

Once you're finished, you should now be able to use Emojis in your messages on your forum.

![preview](http://i21.servimg.com/u/f21/18/21/41/30/captu111.png)

## Configuration

At the top of the script is an object called ``config`` which contains a few settings :

``emoji_size`` : Defines the default size of the emojis ; 16x16 by default. The sizes available are 16, 32, or 72. You can change this for larger or smaller emoji icons.

``emoji_list`` : Defines a list of twitter emojis in JavaScript Escaped Unicode Code Points. In this string you can edit the position of emojis, or remove ones you don't want. You can use this converter for converting characters and javascript escapes : https://r12a.github.io/apps/conversion/

``button_title`` : Defines the tooltip text displayed when you hover over the emoji button. 

``auto_close`` : Setting this option to ``true`` will automatically close the drop down once you've picked an emoji. Set this option to ``false`` if you don't want the drop down to close.

``async_load`` : This option is for performance. When set to ``true`` it will load one emoji after the other without making the browser wait. Setting this option to ``false`` may reduce performance, but it will load all emojis at once. However, this can make the browser unresponsive for a few seconds if there is a large amount of images.

For extended technical details and customization, please see the github page for twitter emojis : https://github.com/twitter/twemoji
