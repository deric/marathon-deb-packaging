# Marathon deb packaging


usage:
```
 ./build_marathon --repo https://github.com/mesosphere/marathon.git?ref=v0.7.3 --version "0.7.3"
```

By default init.d/upstart are used for starting Marathon service. For starting service with `runit` use `--start-with` flag:

```
./build_marathon --ref v0.7.5 --version "0.7.5" --start-with runit
```

## Options

  * `ref` - referring tag in Marathon repository
  * `version` - package version, usually same as referring tag
  * `start-with` - mechanism used for starting service (default: `system` -- depends of OS service startup system)

## Requirements for building

  * `apt-get install dpkg-dev git`
  * some Java
     - e.g. `apt-get install openjdk-7-jdk`
     - Oracle JDK
  * Ruby
     - FPM `gem install fpm`
  * install SBT, e.g. from here:

    http://www.scala-sbt.org/release/tutorial/Installing-sbt-on-Linux.html

