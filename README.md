Java 11 + JavaFX 11 Test Project

## Why? How?

I wanted to test how to include JavaFX, which is no longer a part of the JDK beginning with Java 11.
So I went to the [JavaFX 11 EA download page](http://jdk.java.net/openjfx/) and extracted the zip into my project directory.
Then I created a simple demo application and compiled it with [JDK 11](http://jdk.java.net/11/).

For some reason my `maven-compiler-plugin` didn't want to use any language level higher than 9... I don't use any specific Java 10+ features, though.

## Build

Run `mvn clean package`.

This invokes jlink to produce a custom runtime image under `target/Runtime`.

## Run

Inside of `target/Runtime` simply invoke `./bin/java de.skymatic.javafx11test.Main`.