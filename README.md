# Maven repository for NASA World Wind JAVA SDK 1.5

As WWJ is not available in public maven repositories you must install it manually via `mvn install` to your local maven repository.
All that belongs to the past.

## Prerequisites
Eclipse

Maven + Maven Plugin 4 Eclipse

Installed NASA World Wind Libraries


If not check these install instructions: https://github.com/jimjonesbr/de.ifgi.europa/wiki

## Instructions

First you have to copy the following snippet to you pom.xml of your maven project. If your pom.xml contains a repositories tag
just copy what´s inside.

```
<repositories>
    <repository>
        <id>NASA Worldwind for Java Repo</id>
        <url>https://github.com/mpfeil/mvn-repo/raw/master</url>
    </repository>
</repositories>
```

After copying the repository you have to add the following dependencies also to the pom.xml file. Same as above if your pom.xml contains a dependencies tag just copy what´s inside.

```
<dependencies>
    <dependency>
        <groupId>de.ifgi.nasa.wwj</groupId>
        <artifactId>gdal</artifactId>
        <version>1.5</version>
    </dependency>
    <dependency>
        <groupId>de.ifgi.nasa.wwj</groupId>
        <artifactId>gluegen</artifactId>
        <version>1.5</version>
    </dependency>
    <dependency>
        <groupId>de.ifgi.nasa.wwj</groupId>
        <artifactId>worldwind</artifactId>
        <version>1.5</version>
    </dependency>
    <dependency>
        <groupId>de.ifgi.nasa.wwj</groupId>
        <artifactId>worldwindx</artifactId>
        <version>1.5</version>
    </dependency>
    <dependency>
        <groupId>de.ifgi.nasa.wwj</groupId>
        <artifactId>jogl</artifactId>
        <version>1.5</version>
    </dependency>
<dependencies>
```

Now you´re almost done. Save your pom.xml file and the maven repository is updating.
