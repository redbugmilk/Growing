# Get start Java Application with Maven

## SetUp Project
- New Maven project
- Define:
    - GroupId: uniquely identifies your project across all projects and it starts with a reversed domain name you control. Group or organization that the project belongs to. Often expressed as an inverted domain name. [Java's package name rules](https://docs.oracle.com/javase/specs/jls/se6/html/packages.html#7.7). Eg: org.apache.commons;
    - ArtifactId: is the name of the jar without version. If you created it, then you can choose whatever name you want with lowercase letters and no strange symbols. If it's a third party jar, you have to take the name of the jar as it's distributed. Eg: commons-math

## Cheat sheet

- Check version: 
```
mvn -v
```

## POM
- <packaging> - How the project should be packaged. Defaults to "jar" for JAR file packaging. Use "war" for WAR file packaging.

