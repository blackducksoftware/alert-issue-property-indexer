## Overview ##
An application used for indexing issue properties to allow Alert to map notifications to the correct issue(s).

## Build ##

[![Build Status](https://travis-ci.org/blackducksoftware/alert-jira-property-indexer.svg?branch=master)](https://travis-ci.org/blackducksoftware/alert-jira-property-indexer)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
## Where can I get the latest release? ##

You can download the latest from GitHub: https://github.com/blackducksoftware/alert-issue-property-indexer/releases

## Documentation ##

This plugin only creates a database index inside of Jira. 


### Generating a security scanner report ###
Use the following commands to generate an OWASP security scanner report:

Atlassian SDK:
```
atlas-mvn verify
```
OR 

Maven:
```
mvn verify
```
These commands will create the `dependency-check-report.html` file in the target directory.

### Generating a Dependency Tree File ###

Atlassian SDK:
```
atlas-mvn dependency:tree -DoutputType=dot -DoutputFile=maven_dependency_tree.gv
```
OR

Maven: 
```
mvn dependency:tree -DoutputType=dot -DoutputFile=maven_dependency_tree.gv
```
These commands create a file `maven_dependency_tree.gv` file in the directory where the command is run.