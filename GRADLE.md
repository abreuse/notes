Gradle
====

### Basics

Gradle is a dependency manager like Maven.  
It can fetch dependencies, build and test project.  
It can also configure project settings and plugins.  

#### Wrapper

You can use Gradle Wrapper to have the same gradle across project collaborators.

    gradle wrapper --gradle-version 6.5.1  
    ./gradlew clean  
    ./gradlew build  
  
#### Daemon

Gradle has a daemon running in the background.  
It stays in `IDLE` mode when not running.  
This allows the build to not start a new JVM each time it is running. (faster build time)  

#### Gradle options

    org.gradle.caching=true  
    
Allows build to be _much_ faster ! It caches the build in a local directory.  
A remote cache can also be used for larger organizations.  

    org.gradle.parallel=true

Build will be faster.  
Nice with multi module project.  
