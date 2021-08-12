# MongoDB Compass Dark Mode
No longer do you need have your retinas burned by the unchangable light mode in MongoDB Compass on Mac OS! 

The app.asar file is the original app file plus 2 additions. The darkreader.js file from the dark reader chrome addon, and the script tag in the html. No other modifications have been made.

This file is simply hosted here to make it easier to drag and drop dark mode. Dark mode has no settings or toggle, it is just on.

Original idea for Linux/Windows from [Reddit](https://www.reddit.com/r/mongodb/comments/mj1zr0/successfully_achieved_darkmode_for_mongodb_compass/) \
Linux Users: [This guy's script might work](https://github.com/Pragalbha-Patil/mongodb-compass-dark-mode) \
Windows Users: The zip file should work, just paste it into the correct MongoDB Compass directory for Windows

TLDR (Mac file path); 
* Download file 
* navigate to /Applications/MongoDB Compass/Contents/Resources 
* rename app.asar (to make backup), unzip app.asar.zip 
* drag and drop app.asar file into /Applications/MongoDB Compass/Contents/Resources 

# Walkthrough (Mac file path):

* Download MongoDB Compass from https://www.mongodb.com/try/download/compass (tested on v 1.28.1 MacOS 10.15.7)
* Download the dark mode asar.zip from this repo (original asar + dark reader chrome addon)
* Once installed, go to the finder and click your /Applications folder
* Find MongoDB Compass in the list and right click it > show package contents
* Click /Contents
* Click /Resources
* rename the original app.asar in /Resources to app_original.asar
* copy the app.asar that you downloaded from this repo and paste it into the /Resources folder
* Restart MongoDB Compass and it will be dark!

# Failed?
If you want to revert back, simply **delete** the file _app.asar_ and **rename** the original _app_original.asar_ back to _app.asar_. \
Then Restart MongoDB Compass \
You can always delete the app and install it again

__*Script Coming Soon*__
