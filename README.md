A project to download (http) and install in local maven repository jme3 (java monkey engine 3.0) and some jme3 contributions (lemur).

Then the libs can be used by project using maven, gradle, ivy, sbt, ... to manage dependencies.

Contributions (PR) are  welcomes (it's my first gradle project).

# Instructions

## to install jme3

```
# require java available in PATH
cd jme3 && ../gradlew downloadJme unzipJme publishToMavenLocal && cd ..
```

Then artifact (jar) is available :
```
 group : com.jme3
 version: 3.0.10
```
Change `jmeRev` (and `jmeVersion`) in jme3/build.gradle to use an other download than 2014-06-12 from http://updates.jmonkeyengine.org/stable/3.0/engine/ .

## to install lemur, zay-es

```
cd zay-es && ../gradlew install && cd ..
cd lemur && ../gradlew install && cd ..
```

# Limitations

* I didn't port every libs.
* *-sources.jar and *-javadoc.jar are not installed.
* not battle tested

Pull Request welcome.
