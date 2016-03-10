Job FanIn Plugin
=====================

Building the Project
--------------------

### Dependencies
* [Apache Maven][maven] 3.0.4 or later

### Targets
```shell
  $ mvn clean install
```

Installing Plugin Locally
-------------------------
1. Build the project to produce `target/job-fan-in.hpi`
2. Remove any installation of the JobFanIn in `$user.home/.jenkins/plugins/`
3. Copy `target/job-fan-in.hpi` to `$user.home/.jenkins/plugins/`
4. Start/Restart Jenkins


[maven]: https://maven.apache.org/
