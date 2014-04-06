AndroidStudio-LocaleAPI
=======================
A version of the API library used by the Tasker and Locale apps for plugin development built in Android Studio.

Why?
----
Locale allows you to change device settings when certain outside conditions are met. Tasker allows you automate certain tasks on your phone. It's nice that they both use the same API, but it's built using Eclipse, which can be a real pain to try to get working right (I know I had trouble!). Considering I'm an Android Studio fanboy, it was only natural that I should rebuild it there.

Usage
-----
[This site provides a very straightforward method of using AAR files in Android Studio](http://geekgarage.labasland.net/local-aar-android-library/). You essentially add a new directory to your project, include it as a flat repository, and add it to your dependencies in Gradle.

Building
--------
If the normal build button doesn't work, open the terminal tab in Android Studio and type the following:

Windows:

    gradlew.bat clean
    gradlew.bar aR

Others:

	./gradlew clean
	./gradlew aR

Credit
------
All credit goes to two forty four a.m. LLC. I merely created a new project and tweaked the settings so that it would build an AAR library that could be imported in Android Studio projects.

Copyright 2013 two forty four a.m. LLC <http://www.twofortyfouram.com>

License
-------
Under the same license as the API: Apache License, version 2.0.
