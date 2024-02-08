Depricated
=====================
This plugin was created when Jenkins pipeline was still maturing and the functionality of triggering job from all upstream dependencies run was missing in jenkins 1.x

The function of this plugin can be easily created using jenkins groovy an [reference](https://stackoverflow.com/questions/8884166/how-do-i-dynamically-trigger-downstream-builds-in-jenkins) of how this can be achived. If you think this can't be achieved via groovy please raise such request at [Report issue](https://www.jenkins.io/participate/report-issue).

=====================
Job FanIn Plugin
=====================
[![Build Status](https://jenkins.ci.cloudbees.com/buildStatus/icon?job=plugins/job-fan-in-plugin)](https://jenkins.ci.cloudbees.com/job/plugins/job/job-fan-in-plugin/)

See [Wiki page](https://wiki.jenkins-ci.org/display/JENKINS/JobFanIn+Plugin) for more information.
Description
--------------------
* Trigger downstream projects based on build stability of multiple upstream projects.

  _Example_: 'Job Z' will be triggered if and only if 'Job A', 'Job B' and 'Job C' are build and stable
![alt tag](https://raw.githubusercontent.com/jenkinsci/job-fan-in-plugin/master/fanin.png)

* Trigger can check stability of upstream jobs **recursively**
 
  _Example_: 'Job Z' will be triggered if and only if Job A, B, C, P1, P2, P3 and P4 are build and stable
![alt tag](https://raw.githubusercontent.com/jenkinsci/job-fan-in-plugin/master/fanin-hierarchy.png)

* Configuration is done on downstream job very simple
![alt tag](https://raw.githubusercontent.com/jenkinsci/job-fan-in-plugin/master/job-fan-in-plugin.png)
