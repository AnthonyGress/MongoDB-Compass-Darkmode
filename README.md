# MongoDB Compass + Dark Mode (Dark Reader)

No longer do you need have your retinas burned by the unchangable light mode in MongoDB Compass on Mac OS! ... Why don't they have a dark mode..Anyways!

## Screenshot

<img width="1392" alt="MongoDB Compass Dark" src="https://user-images.githubusercontent.com/70029654/129631360-a317b486-a400-4567-977d-e6aaea86bcee.png">

## Modifications

The `app.asar.zip` file is the original app file plus 2 additions.

1. darkreader.js from the dark reader chrome addon
2. the <script> tag to link the javascript the html. No other modifications have been made.

_This file is simply hosted here to make it easier to drag and drop dark mode_

Original idea for Linux/Windows from [Reddit](https://www.reddit.com/r/mongodb/comments/mj1zr0/successfully_achieved_darkmode_for_mongodb_compass/)

Linux Users: your directory would look something like `/usr/lib/mongodb-compass/resources` -
[This guy's script might also work](https://github.com/Pragalbha-Patil/mongodb-compass-dark-mode)

Windows Users: The `app.asar` file should work, just paste it into the correct MongoDB Compass directory for Windows maybe `C:\Users\{YourUsername}\program files\MongoDB Compass\resources`

## TLDR (Mac file path);

1. Download file
2. navigate to `/Applications/MongoDB Compass/Contents/Resources`
3. rename _app.asar_ (to make backup)
4. unzip `app.asar.zip`
5. drag and drop `app.asar` file into `/Applications/MongoDB Compass/Contents/Resources`

## Walkthrough (Mac file path):

1. Download [MongoDB Compass](https://www.mongodb.com/try/download/compass) (tested on version 1.28.4 on MacOS 10.15.7)
2. Download the dark mode `asar.zip` from this repo (original asar + dark reader chrome addon)
3. Once installed, go to the finder and click your `/Applications` folder
4. Find MongoDB Compass in the list and right click `Show Package Contents`
5. Click `/Contents`
6. Click `/Resources`
7. Rename the original `app.asar` in `/Resources` to `app_original.asar`
8. Copy the `app.asar.zip` that you downloaded from this repo and paste it into the `/Resources` folder
9. Make sure to **unzip** the `app.asar.zip` file here.
10. Restart MongoDB Compass and it will be dark!

## Usage

Dark mode has no settings or toggle, it is just on. **This is the way**.

## Failed?

If you want to revert back, simply **delete** the file _app.asar_ and **rename** the original _app_original.asar_ back to _app.asar_.

Then Restart MongoDB Compass

You can always delete the app and install it again

## DIY

These are the commands i used to extract the file and repackage it with the modifications.

1. `npx asar extract app.asar destination_folder`
2. `npx asar pack destination_folder app.new.asar`

**_Mac Script Coming Soon_**
