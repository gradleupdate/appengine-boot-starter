# Spring Boot + Kotlin + App Engine

A template project of Spring Boot and Kotlin on App Engine Java 8 Standard Environment.

This contains followings:

- Spring Boot
- Thymeleaf
- Kotlin
- Gradle


## How to Run

Google Cloud SDK is required.
See [Quickstart for Java 8 for App Engine Standard Environment](https://cloud.google.com/appengine/docs/standard/java/quickstart-java8).

```sh
# Run dev server
./gradlew appengineRun

# Deploy
./gradlew appengineDeploy
```


## How it works

This template contains:

1. Apply [Google App Engine plugin](https://github.com/GoogleCloudPlatform/app-gradle-plugin)
1. Apply Kotlin plugin
1. Apply war and disable repackaging tasks
1. Remove Tomcat dependencies
1. Add SLF4J to JUL dependency and remove Logback dependencies
1. Improve logging pattern on local dev server
