# Llanfair
I'm mainly working on this as I run under Linux. LiveSplit One is not enough, I need global keybinds (haven't checked in a while so feel free to prove me wrong) and there isn't really many other solutions.

---

Llanfair is a free software that helps speedrunners keep track of their run. Released in August 2012, its capacity for customization and its portability allowed it to garner some recognition in the scene. Developed in Java, Llanfair can run on Windows, MacOS, or nix* systems.

The original author Xavier "Xunkar" Sencert was kind enough to release the sources 
(see [here](https://twitter.com/Xunkar/status/671042537134624768) and [here](https://twitter.com/Xunkar/status/671099823563632641))
I will be extending the original application as best I can by adding some missing features here and 
there and fixing bugs as needed.

## Download

Check the [releases page](releases) for downloadable JARs. 

Llanfair requires Java 11 or later to run. Java 11 is recomeneded currently as there are issues running it on later versions.
  
## Building

Llanfair currently requires Java 11 or later to build and Gradle 6.8.3

Deprecated options used within [build.gradle](blob/master/build.gradle) were removed in Gradle 7.0 and newer and I'm not familar enough with gradle to get this up to date. **Any help here would be appreciated!**

### Command Line Building
To build:
```xl
gradle build
```
If you receive an error about using the incorrect Java version to build you must give the path to a JDK versioned 11 or newer. You can do this by passing the path to the location of your JDK
```xl
gradle build -Dorg.gradle.java.home="/path/to/java/jdk/"
```