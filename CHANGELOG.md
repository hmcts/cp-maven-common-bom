# Change Log

All notable changes to this project will be documented in this file, which follows the guidelines
on [Keep a CHANGELOG](http://keepachangelog.com/). This project adheres to
[Semantic Versioning](http://semver.org/).

## [Unreleased]
### Security
- Update Jackson version to **2.15.0** to fix **security vulnerability CVE-2025-52999**
  Detail: https://cwe.mitre.org/data/definitions/121.html
- Update commons.beanutils version to **1.11.0** to fix **security vulnerability CVE-2025-48734**
  Detail: https://cwe.mitre.org/data/definitions/284.html
- Update resteasy version to **3.15.5.Final** to fix **security vulnerability CVE-2023-0482**
  Detail: https://cwe.mitre.org/data/definitions/378.html
- Update classgraph version to **4.8.112** to fix **security vulnerability CVE-2021-47621**
  Detail: https://cwe.mitre.org/data/definitions/611.html


## [17.103.1] - 2025-07-11
### Changed
- Update maven-parent-pom to 17.103.0

## [17.103.0] - 2025-05-28
### Added
  - Add dependencies for Micometer Metrics 1.15.0

## [17.102.1-M1] - 2025-04-08
### Changed
- Github migration to HMCTS Organisation

## [17.102.0] - 2025-02-26
### Added
- Add dependency for commons-codec 1.17.2

## [17.101.1] - 2025-01-09
### Changed
- Update commons.io to 2.18.0 to fix **security vulnerability CVE-2024-47554**
  Detail: https://nvd.nist.gov/vuln/detail/CVE-2024-47554 and https://cwe.mitre.org/data/definitions/400.html

## [17.101.0] - 2025-01-08
### Changed
- Update maven-parent-pom to 17.101.0 
- Update postgresql.driver.version to 42.3.2 (through maven-parent-pom)

## [17.5.2] - 2024-07-16
### Added
- Add junit-jupiter-engine dependency

## [17.6.1] - 2024-07-11
### Added
- Add dependency for weld-junit5 1.2.2.Final
- Add dependency for org.owasp.encoder 1.2.3

## [17.5.1] - 2024-06-21
### Added
- Add dependency for org.ow2.asm version 9.3

## [17.6.0] - 2024-06-20
### Changed
- Bumped version to match master branches of framework post java 17 code
### Added
- Add dependency for weld-junit5 1.2.2.Final

## [17.5.0] - 2024-06-20
### Security
- Update com.jayway.json-path to version 2.9.0 to fix **security vulnerability CWE-787**
  Detail: https://cwe.mitre.org/data/definitions/787.html

## [17.2.2] - 2024-06-12
### Added
- Add maven-sonar-plugin to pluginManagement (through maven-parent-pom)

## [17.2.1] - 2023-11-27
### Added
- Added undefined version property name for jaway rest-assured dependency
- Added dependency on jackson-datatype-joda
             
## [17.2.0] - 2023-11-03
### Changed
- Centralise all generic library dependencies and versions into this common-bom
### Removed
- Removed dependency on apache-drools as it's not used by any of the framework code
### Security
- Update org.json to version 20231013 to fix **security vulnerability CVE-2023-5072**
    Detail: https://nvd.nist.gov/vuln/detail/CVE-2023-5072
- Update plexus-codehaus to version 3.0.24 to fix **security vulnerability CVE-2022-4244**
    Detail: https://nvd.nist.gov/vuln/detail/CVE-2022-4244
- Update apache-tika to version 1.28.3 to fix **security vulnerability CVE-2022-30973**
    Detail: https://nvd.nist.gov/vuln/detail/CVE-2022-30973
- Update google-guava to version 32.0.0-jre to fix **security vulnerability CVE-2023-2976**
    Detail: https://nvd.nist.gov/vuln/detail/CVE-2023-2976

## [17.1.2] - 2023-07-11
### Changed
- Update to JUnit 5
- Update maven-parent-pom to 17.1.0
- Update junit dependencies
  - Cucumber to 7.12.1
  - Mockito to 5.3.1
  - Servlet.api to 4.0.1
  - Wiremock version to 3.0.0-beta-10
### Security
  - Update Guava to 32.0.0-jre
### Removed
  - Removed net.trajano.commons:commons-testing

## [17.0.1] - 2023-06-14
### Security
- Update org.json to version 20230227 to fix **security vulnerability CVE-2022-45688** 
   Detail: https://nvd.nist.gov/vuln/detail/CVE-2022-45688

## [17.0.0] - 2023-05-05
### Changed
- Update to Java 17
### Added
- Add byte-buddy 1.12.22 as a replacement for cglib
### Removed
- Remove illegal-access argument from surefire plugin from plugin management (through parent pom release)
- Remove illegal-access argument from surefire plugin

## [11.0.1] - 2023-02-01
### Changed
- Downgraded maven minimum version to 3.3.9 until the pipeline maven version is updated

## [11.0.0] - 2023-01-25
### Changed
- Update to Java 11
- Updated to JEE 8
- Bumped the version number to 11.0.0 to match the java 11 versions of the framework
- Updated apache.commons-dbcp2 version to 2.9.0
- Updated artemis.jms version to 2.24.0
- Updated awaitility version to 4.1.0
- Updated commons-io to 2.7 to fix security vulnerability in commons-io
- Updated commons.lang3 version to 3.12.0
- Updated deltaspike version to 1.9.6
- Updated glassfish-json version to 1.1.4
- Updated guava version to 30.1-jre
- Updated hamcrest version to 2.2
- Updated httpclient to version 4.5.13
- Updated Jackson version to 2.10.5.1
- Updated jaxb version to 2.3.1
- Updated jaxb-core version to 2.3.0.1
- Updated jboss-logging version to 3.5.0.Final
- Updated jsonassert version to 1.2.3
- Updated jsonpath version to 2.6.0
- Updated log4j.version to 2.17.2
- Updated mockito version to 4.11.0
- Updated of liquibase to 4.10.0
- Updated OpenEjb to version 8.0.6 to match JEE 8.0
- Updated openejb version to 8.0.13
- Updated restassured version to 4.4.0
- Updated RestEasy to version 3.12.1.Final which matches the version that Wildfly 20.6.1 uses
- Updated resteasy-client version to 4.5.7.Final
- Updated slf4j version to 2.0.6
- Updated slf4j/log4j bridge jar from slf4j-log4j12 to slf4j-reload4j
- Updated snakeyaml to version 1.26
- Updated weld.version to 3.1.4.Final
- Updated wildfly.version to 26.1.2.Final
- Moved snakeyaml.version to maven-parent-pom as it is now a liquibase dependency
### Added
- Dependency for io.rest-assured:rest-assured
- com.lmax.disruptor version 3.4.4 required by Jmx Command Client
- Added dependency for deltaspike-test-control-module-impl
- Added dependency for xbean-asm7-shaded version 4.11
- Jaxb libraries needed for java 11 as they're no longer included by default -->
  - com.sun.xml.bind:jaxb-core
  - javax.xml.bind:jaxb-api
  - com.sun.xml.bind:jaxb-impl
- Added classgraph as a replacement for reflections.org
### Removed
- Removed all old hamcrest libraries
- Removed log4j-over-slf4j as it is now replaced by slf4j-reload4j
### Security
- Updates to various libraries to address security alerts:
  - Updated to log4j2. All log4j 1 libraries removed or updated
  - hibernate version to 5.4.24.Final
  - jackson.databind version to 2.12.7.1
  - jackson libraries to 2.12.7
  - wildfly to version 26.1.2.Final
  - artemis to version 2.20.0
  - resteasy-client to version 4.7.7.Final
  - log4j2 version to 2.17.2 to fix critical security violation
  
## [7.1.1] - 2020-10-14
### Changed
- Updated various library dependencies to fix security vulnerabilities:
    - junit:                4.12 ->   4.13.1      https://github.com/advisories/GHSA-269g-pwp5-87pp
    - commons.beanutils:    1.9.2 ->   1.9.4       https://github.com/advisories/GHSA-6phf-73q6-gh87
    - commons.guava:        19.0 ->   29.0-jre    https://github.com/advisories/GHSA-mvr2-9pj6-7w5j
    - apache.tika:          1.20 ->   1.22        https://github.com/advisories/GHSA-mm7m-xg4h-6m52

## [7.1.0] - 2020-09-23
### Changed
- Updated parent maven-parent-pom to version 2.0.0
- Moved to new Cloudsmith.io repository for hosting maven artifacts
- Updated encrypted properties in travis.yaml to point to cloudsmith

## [7.0.3] - 2020-06-02
### Changed
- Update Drools to 6.5.0.Final

## [7.0.2] - 2020-05-27
### Added
- Cucumber version and dependencies

## [7.0.1] - 2020-05-21
### Changed
- added dependencies required by Embedded Artemis in framework-libraries

## [7.0.0] - 2020-05-20
### Added
- Added diff.utils version 1.3.0
- Added jolt version 0.1.1
### Changed
- Jumped version to 7.0.0 to match Framework and associated libraries

## [2.5.0] - 2020-02-17
### Removed
- 1.5.1 of org.everit.json.schema dependency, this is causing conflicts

## [2.4.0] - 2019-07-11
### Added
- Added commons.cli version 1.2
### Changed
- wildfly-client-all now has default exclusions to allow for running Jmx Clients

## [2.3.0] - 2019-06-25
### Changed
- Revert jackson version 2.9.8 to 2.8.11
- Update jackson.databind to version 2.8.11.3
- Update jackson-dataformat-csv to version 2.8.11

## [2.2.0] - 2019-05-13
### Changed
- Updated apache tika to version 1.20

## [2.1.0] - 2019-05-13
### Changed
- Update jackson to version 2.9.8

## [2.0.2] - 2019-05-01
### Changed
- Revert Deltaspike version to 1.6.1, due to issues with Deltaspike when testing

## [2.0.1] - 2019-05-01
### Changed
- Revert Deltaspike version to 1.6.1, due to issues with Deltaspike when testing

## [1.31.0] - 2019-04-30
## Removed
- org.elasticsearch.client:rest:5.2.2
- org.elasticsearch:elasticsearch:5.2.2
- org.elasticsearch.plugin:transport-netty4-client:5.2.2

## [1.30.0] - 2019-02-07
## Added
- io.github.classgraph:classgraph:4.6.32

## [1.29.0] - 2019-02-01
## Changed
- Update Deltaspike version 1.7.0

## [1.28.0] - 2018-07-25
### Changed
- Update Jackson dataformat YAML to Jackson version 2.8.11

## [1.27.0] - 2018-06-20
### Changed
- Upgrade Apache Tika to 1.18

## [1.26.0] - 2018-05-16
### Changed
- Downgraded Jackson version to 2.8.11 to fix bug with single argument constructors

## [1.25.0] - 2018-05-15
### Changed
- Updated Jackson version to 2.9.5

## [1.24.0] - 2018-04-13
### Added
- jackson-dataformat-yaml 2.8.7

## [1.23.0] - 2018-04-09
### Added
- jglue-cdi-unit version 4.0.1
- jboss.weld.se version 2.4.5.Final

## [1.22.0] - 2017-11-06
### Added
- javax.mail version 1.5.0

## [1.21.0] - 2017-11-01
### Changed
- Updates to fix OWASP vulnerabilities
    - Exclude johnzon-core from artemis-jms-client
### Added
- Updates to fix OWASP vulnerabilities
    - johnzon-core version 1.0.0 dependency

## [1.20.0] - 2017-10-31
### Changed
- Updates to fix OWASP vulnerabilities
    - Update artemis-jms to 1.5.5
    - glassfish-json to 1.0.4

## [1.19.0] - 2017-10-18
### Changed
- org.json:json to version 20170516

## [1.18.0] - 2017-09-26
### Added
- jboss-vfs
- github repo based everit

## [1.17.0] - 2017-07-28
### Changed
- Updated to use parent
  POM [1.6.0](https://github.com/CJSCommonPlatform/maven-parent-pom/releases/tag/release-1.6.0)
- Use bintray for releases
- Improve Travis build process (use common one)

## [1.16.0] - 2017-06-14
### Changed
- Upgrade to use parent
  POM [1.5.0](https://github.com/CJSCommonPlatform/maven-parent-pom/releases/tag/release-1.5.0)
- Revert Wiremock to 1.x for backwards compatibility
- Upgrade JSON Schema library to 1.5.1 so forked version is no longer required
- Upgrade RAML parser to 0.8.18
- Exclude logging dependencies where appropriate

## [1.15.0] - 2017-04-28
### Changed
- Upgrade to use parent
  POM [1.4.1](https://github.com/CJSCommonPlatform/maven-parent-pom/releases/tag/release-1.4.1)
- Uplift wiremock to the forked version

## [1.14.0] - 2017-03-15
### Added
- add Http Mime

## [1.13.0] - 2017-03-10
### Added
- Add Apache Tika

## [1.12.0] - 2017-03-02
### Removed
- Remove JBoss exclusions

## [1.11.0] - 2017-03-02
- Failed release; do not use

## [1.10.0] - 2017-02-22
### Added
- Uplift RESTEasy version and exclude conflicting dependencies

## [1.9.0] - 2017-02-14
### Added
- Add maven-plugin-annotations

## [1.8.0] - 2017-02-13
### Added
- dependency on rest easy-multipart
- dependencies used by raml maven plugin

## [1.7.0] - 2017-02-10
### Added
- maven-plugin-testing-harness
- maven-compat
- maven-core

## [1.6.0] - 2017-01-19
### Added
- Postgres driver, apache.commons-dbcp2 and hamcrest library versions

## [1.5.1] - 2016-12-15
### Changed
- Update org.json version to 20160810

## [1.5.0] - 2016-12-01
### Changed
- Depend on MoJ forked json schema library as it has fix for date-time format

## [1.4.0] - 2016-11-14
### Added
- Add hamcrest regex library
### Changed
- Resolved logging transitive dependency conflicts

## [1.3.0] - 2016-11-02
### Added
- Add jolokia dependencies
### Changed
- Dependencies to resolve maven enforcer conflicts
- Property ordering and removing duplicate declarations

## [1.2.0] - 2016-10-05
### Changed
- Changed artemis.jms.client.version from 1.2.0 to 1.3.0
### Added
- Add artemis.jms.version 1.3.0
- Add artemis-ra library
- Add artemis-jms-server library
- Add artemis-service-extensions library
- Add wildfly-client-all library
- Add javassist version
- Add hamcrest date library
- Dropwizard metrics core
- Weld 2.4.0.Final
- JCommander 1.48

## [1.1.0] - 2016-08-18
### Added
- Add java 8 matchers version

## [1.0.0] - 2016-07-28
### Added
- Initial release of common BOM
