To get started with Axxion ROM, you'll need to get
familiar with [Git and Repo](http://source.android.com/download/using-repo).

To build Axxion you need to first create a directory for the source code using "mkdir" an example would be:

    mkdir android/Axxion
    
You must the change directory or "cd" so run:

    cd android/Axxion
    
To initialize your local repository using the Axxion trees, use a command like this:

    repo init -u git://github.com/Axxion-Team/android.git -b pop

    or for omap4 use:

    repo init -u git://github.com/Axxion-Team/android.git -b omap

Then to sync up:

    repo sync -j4
    
Or be lazy and run it all in one with:

    mkdir (directory) && cd (directory) && repo int -u git://github.com/Axxion-Team/android.git -b (pop/omap) && repo sync -j4

Then to build:

    . build/envsetup.sh && time brunch
