---
layout: docs
title: Download and Installation
meta_title: "How to Download and Install WireMock"
toc_rank: 13
description: WireMock is distributed in two flavours - a standard JAR containing just WireMock, and a standalone fat JAR containing WireMock plus all its dependencies.
---

WireMock is distributed in two flavours - a standard JAR containing just WireMock, and a standalone fat JAR containing
WireMock plus all its dependencies.

Most of the standalone JAR's dependencies are shaded i.e. they are hidden in alternative packages. This allows WireMock to be used in projects with
conflicting versions of its dependencies. The standalone JAR is also runnable (see [Running as a Standalone Process](/docs/running-standalone/)).

Additionally, versions of these JARs are distributed for both Java 7 and Java 8+.

The Java 7 distribution is aimed primarily at Android developers and enterprise Java teams still using JRE7. Some of its
dependencies are not set to the latest versions e.g. Jetty 9.2.x is used, as this is the last minor version to retain Java 7 compatibility.

The Java 8+ build endeavours to track the latest version of all its major dependencies.

> **note**
>
> The Java 7 version is now deprecated in the 2.x line and version 2.27.2 is the last release available. It's strongly
> recommended that you use the Java 8 releases if possible.


## 3.x beta

Maven:

```xml
<dependency>
    <groupId>com.github.tomakehurst</groupId>
    <artifactId>wiremock</artifactId>
    <version>{{ site.wiremock_beta_version }}</version>
    <scope>test</scope>
</dependency>
```

Maven (standalone):

```xml
<dependency>
    <groupId>com.github.tomakehurst</groupId>
    <artifactId>wiremock-standalone</artifactId>
    <version>{{ site.wiremock_beta_version }}</version>
    <scope>test</scope>
</dependency>
```

Gradle:

```groovy
testImplementation "com.github.tomakehurst:wiremock:{{ site.wiremock_beta_version }}"
```

Gradle (standalone):

```groovy
testImplementation "com.github.tomakehurst:wiremock-standalone:{{ site.wiremock_beta_version }}"
```



## Stable

Maven:

```xml
<dependency>
    <groupId>com.github.tomakehurst</groupId>
    <artifactId>wiremock-jre8</artifactId>
    <version>{{ site.wiremock_version }}</version>
    <scope>test</scope>
</dependency>
```

Maven (standalone):

```xml
<dependency>
    <groupId>com.github.tomakehurst</groupId>
    <artifactId>wiremock-jre8-standalone</artifactId>
    <version>{{ site.wiremock_version }}</version>
    <scope>test</scope>
</dependency>
```

Gradle:

```groovy
testImplementation "com.github.tomakehurst:wiremock-jre8:{{ site.wiremock_version }}"
```

Gradle (standalone):

```groovy
testImplementation "com.github.tomakehurst:wiremock-jre8-standalone:{{ site.wiremock_version }}"
```


## Java 7 (deprecated)

Maven:

```xml
<dependency>
    <groupId>com.github.tomakehurst</groupId>
    <artifactId>wiremock</artifactId>
    <version>2.27.2</version>
    <scope>test</scope>
</dependency>
```

Maven (standalone):

```xml
<dependency>
    <groupId>com.github.tomakehurst</groupId>
    <artifactId>wiremock-standalone</artifactId>
    <version>2.27.2</version>
    <scope>test</scope>
</dependency>
```

Gradle:

```groovy
testImplementation "com.github.tomakehurst:wiremock:2.27.2"
```

Gradle (standalone):

```groovy
testImplementation "com.github.tomakehurst:wiremock-standalone:2.27.2"
```

## Direct download

If you want to run WireMock as a standalone process you can
<a id="wiremock-standalone-download" href="https://repo1.maven.org/maven2/com/github/tomakehurst/wiremock-jre8-standalone/{{ site.wiremock_version }}/wiremock-jre8-standalone-{{ site.wiremock_version }}.jar">download the standalone JAR from
here</a>