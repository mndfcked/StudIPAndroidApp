Stud.IP Android App
===================

A mobile Stud.IP client application for the Android plattform which utilizes the studip-rest.ip Rest-API Plugin [studip/studip-rest.ip][2]
for communication with a Stud.IP backend.

NOTE: This app is in alpha stadium and not intended to be used in an productive enviroment.

If you want to contribute to this project, feel free to do so. For more information on how to do this read the Contributing section below.

Setup
-----
* Clone the project. All external library projects are imported as git submodules.
Run ```git submodule init``` and ```git submodule update```,
otherwise it will not compile.

### Gradle (Android Studio)
* Under Quick Start click ```Import Project..``` and choose the cloned project root
* Choose ```Use gradle wrapper (recommended)```
* Press Ok and let Gradle do the rest
* If you want to learn more about Gradle and Android Studio, you can find further information [here][9]

### Eclipse with Maven (Legacy: Some manual work needed)
* Make sure you've installed Eclipse with Maven and EGit.
* Install the Maven Android plugin as described [here][3]
* In Eclipse just use `File->Import->Check out existing Maven repository from scm`
* Maven will take care of the rest

NOTE: To test it with your own installation of the studip-rest.ip plugin,
you need to create your own ```TempServerDeclares``` in the ```de.elanev.studip.android.app.backend.net.oauth```
package. See the ```TempServerDeclaresExample.java``` for more details.

Contributing
------------
* Improve the code
	* Fork it, make your changes, commit them and open a Pull Request. We will take care of the rest.
* Create issues for bugs, feature requests and other ideas
* Contribute to the wiki

Libs
---------
* [oauth-signpost][4]
* [Jackson JSON Processor][5]
* [ActionBarSherlock][6]
* [Google Volley HTTP][7]
* [Square Picasso][10]

Developed By
------------
* [ELAN e.V][8]

License
-------
    Copyright (c) 2013 ELAN e.V.

	All rights reserved. This program and the accompanying materials
    are made available under the terms of the GNU Public License v3.0
    which accompanies this distribution, and is available at
    http://www.gnu.org/licenses/gpl.html

[1]: https://github.com/uol-studip/StudIPAndroidApp
[2]: https://github.com/studip/studip-rest.ip
[3]: http://code.google.com/p/maven-android-plugin/wiki/GettingStarted
[4]: http://code.google.com/p/oauth-signpost/
[5]: http://wiki.fasterxml.com/JacksonHome
[6]: http://actionbarsherlock.com/
[7]: https://android.googlesource.com/platform/frameworks/volley/
[8]: http://www.elan-ev.de/
[9]: http://developer.android.com/sdk/installing/studio.html
[10]: http://square.github.io/picasso/
