A project to download (http) and install in local maven repository jme3 (java monkey engine 3.0) and some jme3 contributions (lemur).

Then the libs can be used by project using maven, gradle, ivy, sbt, ... to manage dependencies.

Contributions (PR) are  welcomes (it's my first gradle project).

# Instructions

to install jme3

```
# require java available in PATH
cd jme3
../gradlew downloadJme unzipJme install
```

Then artifact (jar) is available :
```
 group : com.jme3
 version: 3.0+2014-04-25
```
Change `jmeRev` in jme3/build.gradle to use an other download than 2014-04-25 from http://updates.jmonkeyengine.org/stable/3.0/engine/ .

# Limitations

* I didn't port every libs.
* *-sources.jar and *-javadoc.jar are not installed.
* not battle tested

Pull Request welcome.
