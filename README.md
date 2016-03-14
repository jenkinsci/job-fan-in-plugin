Job FanIn Plugin
=====================

Description
--------------------
* Trigger downstream projects based on build stability of multiple upstream projects.

  _Example_: 'Job Z' will be triggered if and only if 'Job A', 'Job B' and 'Job C' are build and stable
![alt tag](https://raw.githubusercontent.com/yogeshlonkar/job-fan-in/master/fanin.png)

* Trigger can check stability of upstream jobs **recursively**
 
  _Example_: 'Job Z' will be triggered if and only if Job A, B, C, P1, P2, P3 and P4 are build and stable
![alt tag](https://raw.githubusercontent.com/yogeshlonkar/job-fan-in/master/fanin-hierarchy.png)

* Configuration is done on downstream job very simple
![alt tag](https://raw.githubusercontent.com/yogeshlonkar/job-fan-in/master/job-fan-in-plugin.png)

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
