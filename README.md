# OpenAPI SDK MCA

MCA OpenAPI SDK for Zerofinance.

## Requirements

- JDK 8 or newer
- Maven 3.9 or newer

## Dependency

```xml
<dependency>
    <groupId>com.zerofinance</groupId>
    <artifactId>openapi-sdk-mca</artifactId>
    <version>1.0.0</version>
</dependency>
```

## Build

```bash
mvn clean verify
```

## Publishing

Configure a Maven server with id `mavencenter-release` in `~/.m2/settings.xml` using a
Central Portal user token. The token and the GPG passphrase must not be committed.

For a final release:

```bash
mvn clean deploy -Prelease
```

The release profile requires a GPG private key whose public key is available from a
Central-supported keyserver. Maven Central releases are immutable.
