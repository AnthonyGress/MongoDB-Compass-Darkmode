# MongoDB Compass Dark Mode
No longer do you need have your retinas burned by the unchangable light mode in MongoDB Compass on Mac OS! 

## Modifications
The app.asar file is the original app file plus 2 additions. The darkreader.js file from the dark reader chrome addon, and the script tag in the html. No other modifications have been made.

This file is simply hosted here to make it easier to drag and drop dark mode.

Original idea for Linux/Windows from [Reddit](https://www.reddit.com/r/mongodb/comments/mj1zr0/successfully_achieved_darkmode_for_mongodb_compass/)

Linux Users: your directory would looks something like `/usr/lib/mongodb-compass/resources` 
[This guy's script might also work](https://github.com/Pragalbha-Patil/mongodb-compass-dark-mode)

Windows Users: The zip file should work, just paste it into the correct MongoDB Compass directory for Windows

## TLDR (Mac file path); 
1. Download file 
2. navigate to `/Applications/MongoDB Compass/Contents/Resources` 
3. rename _app.asar_ (to make backup)
4. unzip `app.asar.zip` 
5. drag and drop `app.asar` file into `/Applications/MongoDB Compass/Contents/Resources` 

## Walkthrough (Mac file path):

1. Download MongoDB Compass from https://www.mongodb.com/try/download/compass (tested on v 1.28.1 MacOS 10.15.7)
2. Download the dark mode `asar.zip` from this repo (original asar + dark reader chrome addon)
3. Once installed, go to the finder and click your `/Applications` folder
4. Find MongoDB Compass in the list and right click it > show package contents
5. Click `/Contents`
6. Click `/Resources`
7. rename the original `app.asar` in `/Resources` to `app_original.asar`
8. copy the app.asar that you downloaded from this repo and paste it into the `/Resources` folder
9. Restart MongoDB Compass and it will be dark!

## Usage
Dark mode has no settings or toggle, it is just on.

## Failed?
If you want to revert back, simply **delete** the file _app.asar_ and **rename** the original _app_original.asar_ back to _app.asar_. \
Then Restart MongoDB Compass \
You can always delete the app and install it again

__*Script Coming Soon*__
