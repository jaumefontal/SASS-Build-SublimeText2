SASS build system for Sublime Text 2
====================================

**Note: I'm working in a portable version of the SASS build with all the libraries included & ready to use. It will be available (I hope!) the next week.**

Description
-----------

Provides a Build system for SASS files.


Prerequisites
-------------

Requires **Ruby** & **SASS** libraries.

Step by step:

1. Install Ruby library

	**Windows**: Download and install Ruby. You can find it here:
	http://rubyinstaller.org/downloads/

	Reboot after install it.

	**IMPORTANT**: Don't forget to mark the option '*Add Ruby executables to your PATH*'.
	If you don't check the option, you will have to modify the path in the Build file afterwards.

	**OS X & Linux**: It's already installed. Easy! :)


2. Installing SASS

	Open your console ('*Command promp with Ruby*' on Windows) and execute the following command:

	`gem install sass`


Installing
----------
**With the Package Control plugin**

The easiest way to install this package is through Package Control.

1. Download and install the [Package Control Plugin](http://wbond.net/sublime_packages/package_control).
Follow the instructions on the website.

2. Open the command panel: `Control+Shift+P` (Linux/Windows) or `Command+Shift+P` (OS X) and select '**Package Control: Install Package**'.
3. When the packages list appears type '**SASS**' and you'll find the **SASS Build System**. Select to install it.

4. Now you can compile your SASS files! Launch your build with `Control+B` (Linux/Windows) or `Command+B` (OS X)-

5. Enjoy your coding =)


**With Git**

Clone the repository in your Sublime Text "Packages" directory:

    git clone git://https://github.com/jaumefontal/SASS-Build-SublimeText2.git SASS-build

You can find your 'Packages' inside the following directories:

* OS X:
    `~/Library/Application Support/Sublime Text 2/Packages/`
* Windows:
    `%APPDATA%/Sublime Text 2/Packages/`
* Linux:
    `~/.Sublime Text 2/Packages/`

**Without Git**

Download the latest source zip from [Github](https://github.com/jaumefontal/SASS-Build-SublimeText2) and extract it into a new folder named `SASS-Build` in your Sublime Text "Packages" folder.


Recommendations
---------------

* Is recommended to use this build with the [SASS plugin](https://github.com/nathos/sass-textmate-bundle).
* Also, I recomend the plugin [SublimeOnSaveBuild](https://github.com/alexnj/SublimeOnSaveBuild). Just save your SASS files and transform them into CSS!


Author
------

Created by **Jaume Fontal** ([@jaumefontal](http://www.twitter.com/jaumefontal)).

If you need more info you can find me on Twitter!