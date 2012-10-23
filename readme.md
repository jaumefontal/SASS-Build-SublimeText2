SASS build system for Sublime Text 2
====================================

**Note: I'm working in a portable version of the SASS build with all the libraries included & ready to use. It will be available (I hope!) the next week.**

Description
-----------

Provides two Build system for SASS files (with and without compression)


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
**OPTION 1 - With the Package Control plugin (recommended)**

The easiest way to install this package is through Package Control.

1. Download and install the [Package Control Plugin](http://wbond.net/sublime_packages/package_control).
Follow the instructions on the website.

2. Open the command panel: `Control+Shift+P` (Linux/Windows) or `Command+Shift+P` (OS X) and select '**Package Control: Install Package**'.
3. When the packages list appears type '**SASS**' and you'll find the **SASS Build System**. Select to install it.

4. Now you can compile your SASS files! Launch your build with `Control+B` (Linux/Windows) or `Command+B` (OS X).

5. Enjoy your coding =)


**OPTION 2 - With Git**

Clone the repository in your Sublime Text "Packages" directory:

    git clone git://https://github.com/jaumefontal/SASS-Build-SublimeText2.git SASS-build

You can find your 'Packages' inside the following directories:

* OS X:
    `~/Library/Application Support/Sublime Text 2/Packages/`
* Windows:
    `%APPDATA%/Sublime Text 2/Packages/`
* Linux:
    `~/.Sublime Text 2/Packages/`

**OPTION 3 - Without Git**

Download the latest source zip from [Github](https://github.com/jaumefontal/SASS-Build-SublimeText2) and extract it into a new folder named `SASS-Build` in your Sublime Text "Packages" folder.


Using the build
---------------

After installing the package you will find two new options in `Tools > Build system` of your  Sublime menu: **SASS** and **SASS - Compressed**.

By default your `.scss` and `.sass` files will be builded using the **SASS build** (not compressed).

And remember, always you can launch the selected build with `Control+B` (Linux/Windows) or `Command+B` (OS X).


Recommendations
---------------

* Is recommended to use this build with one of the next plugins: [SASS plugin](https://github.com/nathos/sass-textmate-bundle) or [SCSS.tmbundle](https://github.com/kuroir/SCSS.tmbundle).
* Also, I recomend the plugin [SublimeOnSaveBuild](https://github.com/alexnj/SublimeOnSaveBuild). Just save your SASS files and transform them into CSS!
* If you want to change the default folder of your generated CSS files into another one, you can edit the build:

  **Exemple:** Save your CSS files into a `css` folder:
  `"cmd": ["sass", "--update", "$file:${file_path}/../css/${file_base_name}.css"],`


Author
------

Created by **Jaume Fontal** ([@jaumefontal](http://www.twitter.com/jaumefontal)).

If you need more info you can find me on Twitter!

Acknowledgements
----------------

Thanks to the collaboration of [@hdennison](http://www.twitter.com/hdennison) with the testing in MacOS.