# Unit_1_2025

A simple Java HelloWorld program with testing infrastructure.

## Running the Program

```bash
javac HelloWorld.java
java HelloWorld
```

## Running the Tests

First, download the JUnit dependencies:

```bash
mkdir -p lib
cd lib
curl -L -o junit-platform-console-standalone-1.9.3.jar https://repo1.maven.org/maven2/org/junit/platform/junit-platform-console-standalone/1.9.3/junit-platform-console-standalone-1.9.3.jar
cd ..
```

Then compile and run the tests:

```bash
javac -cp ".:lib/junit-platform-console-standalone-1.9.3.jar" HelloWorld.java HelloWorldTest.java
java -jar lib/junit-platform-console-standalone-1.9.3.jar --class-path . --scan-class-path
```