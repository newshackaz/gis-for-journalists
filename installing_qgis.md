#Installing QGIS#


QGIS (Quantum GIS) is an open-source free software for Windows, Mac and Linux (also Android oddly enough). Installation instructions vary slightly depending on the operating system. The official installation instructions can be found [here](http://qgis.org/en/site/forusers/download.html). 

**IMPORTANT:** In order to install you need to have administrator privileges to your computer.

If you have any difficulty in installing the software, please report it [here](https://github.com/newshackaz/gis-for-journalists/issues). You should also check to see if someone else has had a similar issue.

###Windows###

Windows installation begins with downloading the software [here](http://qgis.org/en/site/forusers/download.html).

There are several options under the Windows heading. The software you want is listed under "Latest Release."

Select either the 32-bit or the 64-bit version depending on your operating system. To find out which operating system you are running, follow the directions [here](http://windows.microsoft.com/en-us/windows/32-bit-and-64-bit-windows#1TC=windows-7).

Click on the link to run the installation manager or download and then run it if it does not launch automatically.

If it asks you which installation you want, select the one that says something to the effect of "express install." Start the installation and follow any remaining prompts.

###Mac OS X###

Mac installation can be a bit more complicated. QGIS recommends downloading and installing the files from [KyngChaos](http://www.kyngchaos.com/software/qgis). It appears that this version supports Mac OS X Mountain Lion or newer. If you go this route, make sure to first download and install the requirements listed on the website - namely GDAL and Matplotlib.

If you are familiar with Homebrew, I recommend using that instead. Homebrew is a package manager that handles the installation and upgrade of multiple software packages. Many coders and developers rely on Homebrew to keep their machines up to date.

#####Working with Homebrew#####
Basic information about Homebrew can be found [here](http://brew.sh/). You may be prompted for your password during this process.
To install Homebrew, you need to access the terminal on your computer. To do so, click on Spotlight (the search icon on the upper right hand of your screen). Type in Terminal and press enter. This should open up a new window with a command line interface. Type (or just copy and paste) the following into your terminal and press enter:

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

And now that you have Homebrew installed you will need to tap [OSGEO](https://github.com/OSGeo/homebrew-osgeo4mac)'s  repository to install QGIS. This is down by entering the following into the terminal and pressing enter:

```
brew tap osgeo/osgeo4mac
```

This repository is maintained by the people at OSGEO and the QGIS software there is updated more frequently than in the regular Homebrew repository.

Next we install QGIS by entering the following into the command line:

```
brew install osgeo/osgeo4mac/qgis-28
```

This will install QGIS and all the other required software.
Installing QGIS this way may not make it visible in your Applications folder. To fix this, enter the following into your terminal:

```
brew link qgis-28
```

This will create a shortcut for QGIS in your Applications folder.

###Linux###

Installation can vary slightly depending on which flavor of Linux you are using. I use Ubuntu, so this is written with that in mind.

Launch Ubuntu's terminal program. If you can't find it, search for it in your computer. Once you open terminal, we should start by updating your repositories. You may be prompted for your password during this process. This is done by entering the following:

```
sudo apt-get update
```

Once it has completed updating you can then install QGIS by entering the following into the terminal:

```
sudo apt-get install qgis
```

That should complete the installation process.
