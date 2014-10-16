# Marathon deb packaging

## Requirements

  * `apt-get install dpkg-dev git`
  * some Java
     - e.g. `apt-get install openjdk-7-jdk`
     - Oracle JDK
  * install SBT, e.g. from here:

    http://www.scala-sbt.org/release/tutorial/Installing-sbt-on-Linux.html

usage:
```
 ./build_marathon --repo https://github.com/mesosphere/marathon.git?ref=v0.7.3 --version "0.7.3"
```
