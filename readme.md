Sass build system for Sublime Text
==================================


Description
-----------

This is a plugin for Sublime Text 2/3 providing four build systems for Sass/SCSS files:
 * `Nested` (default)
 * `Compressed`
 * `Compact`
 * `Expanded`



Prerequisites
-------------

Requires **Ruby** & **Sass** libraries.

####Step-by-step library installation guide: 
---

1. Install Ruby library

	**Windows**: Download and install Ruby. You can find it here: http://rubyinstaller.org/downloads/

	Reboot after installing it.

	**IMPORTANT**: Don't forget to mark the option '*Add Ruby executables to your PATH*'.
	If you don't check this option, you will have to modify the path in the Build file afterwards.

	**OS X & Linux**: It's already installed. Easy! :)


2. Installing Sass

	Open your console (_`Command prompt with Ruby`_ on Windows or _`Terminal`_ on Mac) and execute the following command:

	`gem install sass`

	Depending on your user permissions, the above command may not work. If that is the case, try executing this command:

	`sudo gem install sass`


Installing
----------
**OPTION 1 - With the Package Control plugin (recommended)**

The easiest way to install this package is through Package Control.

1. Download and install the [Package Control Plugin](http://wbond.net/sublime_packages/package_control).
Follow the instructions on the website.

2. Open the command panel: `Control+Shift+P` (Linux/Windows) or `Command+Shift+P` (OS X) and select '**Package Control: Install Package**'.
3. When the packages list appears type '**Sass**' and you'll find the **Sass Build System**. Select to install it.

4. Now you can compile your Sass files! Launch your build with `Control+B` (Linux/Windows) or `Command+B` (OS X).

5. Enjoy your coding =)


**OPTION 2 - With Git**

Clone the repository in your Sublime Text "Packages" directory:

    git clone git://github.com/jaumefontal/Sass-Build-SublimeText2.git Sass-build

Depending on your version of Sublime Text, you can find your 'Packages' inside the following directories:

* OS X:
    `~/Library/Application Support/Sublime Text 2/Packages/`
    `~/Library/Application Support/Sublime Text 3/Packages/`
* Windows:
    `%APPDATA%/Sublime Text 2/Packages/`
    `%APPDATA%/Sublime Text 3/Packages/`
* Linux:
    `~/.Sublime Text 2/Packages/`
    `~/.Sublime Text 3/Packages/`

**OPTION 3 - Without Git**

Download the latest source zip from [Github](https://github.com/jaumefontal/Sass-Build-SublimeText2) and extract it into a new folder named `Sass-Build` in your Sublime Text "Packages" folder.


Using the build
---------------

After installing the package you will find four new options in `Tools > Build system` option in your Sublime menu: `Sass — Nested`, `Sass - Compressed`,  `Sass — Expanded`, and `Sass - Compact`.

By default, your `.scss` and `.sass` files will be built using the **Sass — Nested** setting. Additionally, the files will be saved into the same directory as the Sass file. For information on how to change this setting, please see the **Recommendations** section below.

And remember, always you can launch the selected build with `Control+B` (Linux/Windows) or `Command+B` (OS X).


Recommendations
---------------

* This plugin will work best when combined with either the [Sass plugin](https://github.com/nathos/sass-textmate-bundle) or [SCSS.tmbundle](https://github.com/kuroir/SCSS.tmbundle).
* Also, I recommend the plugin [SublimeOnSaveBuild](https://github.com/alexnj/SublimeOnSaveBuild). When you save your Sass files, they will transformed into CSS!

####Changing the default folder for generated CSS

If you want to change the default folder of where your CSS is generated, you can edit the `.sublime-build` files, found in the `Sass-build` folder of the 'Packages' directory. In Sublime Text 3, you can easily access this directory through the `Preferences > Browse Packages` option in the Sublime menu:

  **Example:** Save your CSS files into a `css` folder:
  `"cmd": ["sass", "--update", "$file:${file_path}/../css/${file_base_name}.css"],`

  If you are using partials and running into issues, David Kiv [suggests](http://blog.hovercraft.ie/post/61592756918/update-sass-build-plug-in-for-sublime-text-2-to) putting this code in the `.sublime-build` files:

  **Windows** 
  		* `"cmd": ["sass", "--update", "${project_path}\\scss\\styles.scss:${project_path}\\css\\styles.css", "--stop-on-error", "--no-cache"],`
  		
  **Mac** 
	 * `"cmd": ["sass", "--update", "${project_path}/scss/styles.scss:${project_path}/css/styles.css", "--stop-on-error", "--no-cache"],`



Author
------

Created by **Jaume Fontal** ([@jaumefontal](http://www.twitter.com/jaumefontal)).

If you need more info you can find me on Twitter!

Acknowledgments
----------------

Thanks to the collaboration of [@hdennison](http://www.twitter.com/hdennison) with the testing in MacOS.
