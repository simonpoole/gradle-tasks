# Collection of useful gradle tasks

## eclipse-android

Create classpath for android style project layouts, iirc based on something from stackoverflow, a bit hacky but works. For sub projects it will use the roots project name plus the path to the subject as the eclipse project name to avoid naming clashes.

Include in build.gradle with 
       
       apply from: 'https://raw.githubusercontent.com/simonpoole/gradle-tasks/master/eclipse-android'
       
## publish-on-bintray-android

Publish an android library on bintray including source and javadoc jars so that it can be published on jCenter 

Expects GROUP, ARTIFACT_ID, NAME, REPO, to be set and BINTRAY_USER BINTRAY_KEY to be in the environment.

Include in build.gradle with
       
       apply from: 'https://raw.githubusercontent.com/simonpoole/gradle-tasks/master/publish-on-bintray-android'