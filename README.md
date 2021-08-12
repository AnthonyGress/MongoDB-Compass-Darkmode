# Mac MongoDB Compass Dark Mode
No longer do you need have your retinas burned by the unchangable light mode in MongoDB Compass on Mac OS.

TLDR; Download file, rename original app.asar, drag and drop new file into /Applications/MongoDB Compass/Contents/Resources

* Download MongoDB Compass from https://www.mongodb.com/try/download/compass (tested on v 1.28.1 MacOS 10.15.7)
* Download the dark mode addon (basically added dark reader chrome addon js)
https://drive.google.com/file/d/1CYOGvTqIDde-J4psfEiqbFa1dnZKuuA4/view?usp=sharing
* Once installed, go to the finder and click your /Applications folder
* Find MongoDB Compass in the list and right click it > show package contents
* Click /Contents
* Click /Resources
* rename the original app.asar in /Resources to app_original.asar
* copy the app.asar that you downloaded from the google drive and paste it into the /Resources folder
* Restart MongoDB Compass and it will be dark!

Failed?
If you want to revert back, simply **delete** the file _app.asar_ and **rename** the original _app_original.asar_ back to _app.asar_.
Restart MongoDB Compass

__*Script Coming Soon*__
