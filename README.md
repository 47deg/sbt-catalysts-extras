
[comment]: # (Start Badges)

[![Maven Central](https://img.shields.io/badge/maven%20central-0.13.3-green.svg)](https://repo1.maven.org/maven2/com/47deg/sbt-org-policies_2.12_1.0) [![License](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://raw.githubusercontent.com/47degrees/sbt-org-policies/master/LICENSE) [![GitHub Issues](https://img.shields.io/github/issues/47degrees/sbt-org-policies.svg)](https://github.com/47degrees/sbt-org-policies/issues)

[comment]: # (End Badges)
# sbt-org-policies (ABANDONED)

### DEPRECATION NOTICE

**sbt-org-policies** was an SBT plugin that used to enforce some organization policies and sharing settings across all the Scala projects. However, with Github actions, as well as other fantastic sbt plugins like sbt-ci-release, sbt-mdoc, sbt-github, ... you can achieve the same in a more natural, and maintainable way. We recommend using that approach.

47 Degrees has therefore discontinued the development and maintenance of this library. The source code is left here for those interested in studying it.

## Installation

[comment]: # (Start Replace)
Add the following line to `project/plugins.sbt`:

```scala
addSbtPlugin("com.47deg" % "sbt-org-policies" % "0.12.0-M1")
```

[comment]: # (End Replace)

## Creating New Org Project

1. Create a new project from our g8 template:

```scala
sbt new 47degrees/org-template.g8
```

2. Fill the required information (you can see an example below):

```bash

...

name [Project Name]: Test
projectDescription [Project Description]:
project [project-name]: org-test
package [com.fortysevendeg]:
startYear [2017]:
organization_web [http://47deg.com]:
github_owner [47degrees]:
github_repo [org-test]:
sbt_org_policies_version [0.4.18]:
Skipping existing file: ./test/.gitignore
Skipping existing file: ./test/build.sbt
Skipping existing file: ./test/project/build.properties
Skipping existing file: ./test/project/plugins.sbt

Template applied in ./test
```

The new project will be created in the `test` folder, with the basic structure and basic sbt configuration based on the sbt-org-policies plugin.

3. Create the organization files, to do so, from the project folder, you could just run:

```scala
sbt orgCreateFiles
```

[comment]: # (Start Copyright)
# Copyright

sbt-org-policies is designed and developed by 47 Degrees

Copyright (C) 2017-2020 47 Degrees. <http://47deg.com>

[comment]: # (End Copyright)
