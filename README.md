# Gradle_alpha
Learning Gradle

### What is Gradle
- A build automation and project dependency management tool.
- Build using java, but the build process is done by groovy __ DSL (Domain Specific Language) __.
- Supports both maven and Ivy dependencies.
- Built by convention, Supports multi project builds.
- Supports not only java builds but also JavaScript and C++ builds.
- Easily customizable language, highly maintainable.
- Gradle has declarative build language which expresses the intent of the build language.
- We will say to Gradle what we would like to happen and not how it happens.

### Comparing Gradle to other build tools ANT, Maven
#### ANT - Another Neat Tool
- Made from XML, Hard to read and difficult to maintain.
- Do not have convention, Everything need to be specified
    - Where our source directory is present.
    - where to built classes, where to get libraries.
    - Where we are going to output the created files.
- We might have to right too many lines to specify, properties, targets (prepare, clean, build).
- These ant files can get very large, very quickly and unmaintainable.

#### Maven
- Several advantages over ANT, as we have so many conventions we don't have to specify everything.
- Supports dependency management. POM helps in resolving dependencies when we need them.
- Highly extensible, we have configurable plugins.
- As this is written in xml, can grow large in size and become unmaintainable.

#### Gradle
- As it uses language specific to domain here it is build domain.
- We can define the following.
    - Repositories
    - Dependencies
    - Plugins and many more things.
- Because of DSL, Gradle becomes largely self explanatory.

### Installing Gradle
- Can in done in 2 ways
    1) download from [Gradle](https://gradle.org/), place it in path you like.
        - Add Gradle/bin folder to path variable.
    2) Using GVM (Gradle environment manager), used for Linux and MAC operating systems.
        - Get GVM from [GVM](http://ww7.gvmtool.net/).
        - download using ``` curl -s get.gvmtool.net|bash ```
        - Add it to path using source command
        - install Gradle ``` gvm install gradle ```
- To check if Gradle is installed, just type ``` gradle ``` in command prmpt it will give a bunch of information about it.

### Creating initial Project Structure with Gradle
- use command ``` gradle init ``` it will ask the below options
- Select type of project to generate from (1:basic, 2:application, 3: library, 4:Gradle Plugins) we choose: 2.
- Select implementation language, we choose java.
- Select Build Script DSL, we choose groovy.
- Select Test Framework we choose Junit 4.
- Enter project name : we choose 'gradle_Initial'.
- Source package: we left it for default by clicking enter.

Then Gradle will create a basic folder structure for a java project as attached here.
> Like POM file for Maven, Gradle runs from build.gradle file.


