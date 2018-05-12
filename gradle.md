#Gradle

Main project should have 2 files:
- build.gradle (include dependencies, define tasks)
- settings.gradle (define subprojects - `include 'subprojectName'`)
```
./gradlew tasks --all
./gradlew tasks
./gradlew :supermonitor:tasks
```

###Axion plugin
```
./gradlew currentVersion --info
./gradlew cV
```

###Overriding version
Push just a new tag
```
./gradlew markNextVersion -Prelease.version=1.6.7
```
or do release with provided tag
```
./gradlew release -Prelease.forceVersion=1.6.7
```

###Examples
Axion [examples](http://axion-release-plugin.readthedocs.io/en/latest/examples/examples.html)
###Test run
```
./gradlew :superapp:release -Prelease.dryRun
```