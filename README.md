Java 11 + JavaFX 11 Test Project

## Why? How?

This is just a sandbox to play around with the packaging tools required to create and customize self-contained applications with JDK and OpenJFX 11.

## Prerequisites

Get a [backport of jpackager](https://mail.openjdk.java.net/pipermail/openjfx-dev/2018-September/022500.html) and adjust its path in the `pom.xml`.

## Build

Run `mvn clean package`.

This invokes jpackager and jlink to produce an application with a custom runtime image under `target/package`.