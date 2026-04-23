# cp-maven-common-bom

`uk.gov.justice:maven-common-bom`

The central dependency bill of materials (BOM) for all CPP framework projects. It pins the versions of every third-party library used across the framework so that all projects agree on the same set of versions.

## Position in the hierarchy

```
maven-parent-pom
└── maven-common-bom  ← this project
```

`maven-framework-parent-pom` imports this BOM via `<scope>import</scope>`, making all version definitions available to `cp-framework-libraries`, `cp-microservice-framework`, `cp-event-store`, and `cp-cake-shop`.

## What this BOM pins

Dependency versions only — no actual dependencies are added to any project. A project must still declare its own `<dependencies>` but omits `<version>` tags for anything listed here.

**Jakarta EE 10 APIs**
- `jakarta.jakartaee-api` 10.0.0
- CDI 4.0.1, JMS 3.1.0, JSON-P 2.1.3, Persistence 3.1.0, Servlet 6.0.0, Transactions 2.0.1, JAXB 4.0.0

**Server / container**
- WildFly 34.0.1.Final
- RESTEasy 6.2.15.Final
- Apache ActiveMQ Artemis 2.40.0
- Hibernate ORM 6.6.1.Final
- Weld SE 5.1.2.Final (CDI for tests)
- Apache TomEE / OpenEJB 10.1.4 (embedded EJB for tests)

**Data**
- PostgreSQL driver 42.3.2
- Liquibase 4.10.0
- Apache Commons DBCP2 2.14.0

**Jackson**
- `jackson-databind` 2.15.4 (aligned to WildFly 32's bundled version)
- `jackson-dataformat-yaml` 2.14.3 (pinned at last snakeyaml 1.x compatible version — 2.15+ breaks the raml-parser Maven plugin)

**JSON**
- Parsson 1.1.7, Johnzon 2.0.2, everit json-schema 1.6.0

**Logging**
- Log4j 2.25.4 (full BOM import), SLF4J 2.0.17

**Testing**
- JUnit Jupiter 5.14.3, Mockito 5.23.0, Hamcrest 2.2, WireMock 3.13.2
- Awaitility 4.3.0, Rest Assured 5.5.7, Cucumber 7.34.3
- Weld JUnit 5 1.2.2.Final, OpenEJB JUnit 5 10.1.4

**Utilities**
- Apache Commons (lang3, io, codec, collections, beanutils, cli, validator, dbcp2)
- Guava 33.5.0-jre, Jackson, Jolt 0.1.8, ClassGraph 4.8.184
- Micrometer BOM 1.16.4 (including Azure Monitor and Prometheus registry)

## Usage

Import in your project's `<dependencyManagement>`:

```xml
<dependency>
    <groupId>uk.gov.justice</groupId>
    <artifactId>maven-common-bom</artifactId>
    <version>${maven-common-bom.version}</version>
    <type>pom</type>
    <scope>import</scope>
</dependency>
```

All projects that inherit from `maven-framework-parent-pom` get this import automatically.
