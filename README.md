gradle-build-for-target-environment
===================================

A build.gradle that can build a Java project targetted at a dev, cert or prod environment

How to use
---
```
git clone git@github.com:Pance/gradle-build-for-target-environment.git

# Run gradle targeted at a development environment
$ gradle -Penv=dev
**Selected environment is: DEV
**Loaded SourceSets for resources:
[.../gradle-build-for-target-environment/src/main/resources/global, .../gradle-build-for-target-environment/src/main/resources/dev]

# Run gradle targeted at a certification environment
$ gradle -Penv=cert
**Selected environment is: CERT
**Loaded SourceSets for resources:
[.../gradle-build-for-target-environment/src/main/resources/global, .../gradle-build-for-target-environment/src/main/resources/cert]

# Run gradle targeted at a production environment
$ gradle -Penv=prod
**Selected environment is: PROD
**Loaded SourceSets for resources:
[.../gradle-build-for-target-environment/src/main/resources/global, .../gradle-build-for-target-environment/src/main/resources/prod]

# Without the given env parameter, the build.gradle defaults to DEV
$ gradle
**Selected environment is: DEV
**Loaded SourceSets for resources:
[.../gradle-build-for-target-environment/src/main/resources/global, .../gradle-build-for-target-environment/src/main/resources/dev]
```
