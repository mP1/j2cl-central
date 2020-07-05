# j2cl-central
Not really a code repo but a faq, collection of texts and links to j2cl libraries created/forked by me that work with the j2cl javascript runtime.



## Maven plugin
Maven plugin required to build other libraries in the family.

- [j2cl-maven-plugin](https://github.com/mP1/j2cl-maven-plugin)



## Minimal JRE emulation

- [j2cl-uber](https://github.com/mP1/j2cl-uber) Include all the minimal bootclass, JRE and runtime libraries
- [j2cl-uber-test](https://github.com/mP1/j2cl-uber-test) Includes junit test support



## JRE emulation

The following additions are available, for further details of support and unsupported APIs refer to each project.

- [j2cl-java-io](https://github.com/mP1/j2cl-java-io)
- [j2cl-java-net](https://github.com/mP1/j2cl-java-net)
- [j2cl-java-text](https://github.com/mP1/j2cl-java-text)
- [j2cl-java-time](https://github.com/mP1/j2cl-java-time)
- [j2cl-java-util-Base64](https://github.com/mP1/j2cl-java-util-Base64)
- [j2cl-java-util-Calendar](https://github.com/mP1/j2cl-java-util-Calendar)
- [j2cl-java-util-Currency](https://github.com/mP1/j2cl-java-util-Currency)
- [j2cl-java-util-Locale](https://github.com/mP1/j2cl-java-util-Locale)
- [j2cl-java-util-StringTokenizer](https://github.com/mP1/j2cl-java-util-StringTokenizer)
- [j2cl-java-util-TimeZone](https://github.com/mP1/j2cl-java-util-TimeZone)



## Supporting annotation processors

- [j2cl-java-text-annotation-processor](https://github.com/mP1/j2cl-java-text-annotation-processor)
- [j2cl-java-util-currency-annotation-processor](https://github.com/mP1/j2cl-java-util-currency-annotation-processor)
- [j2cl-java-util-Locale-annotation-processor](https://github.com/mP1/j2cl-java-util-Locale-annotation-processor)
- [j2cl-java-util-TimeZone-annotation-processor](https://github.com/mP1/j2cl-java-util-TimeZone-annotation-processor)
- [j2cl-locale](https://github.com/mP1/j2cl-locale)
- [walkingkooka-resource-annotation-processor](https://github.com/mP1/walkingkooka-resource-annotation-processor)



## Maven

- There are no versions or releases only snapshots with the latest.
- Nothing is pushed to maven-central
- There are no sources.jar, java source is always included with the jar file containing the binaries.
- All projects require JDK 9 to build and execute tests, other versions may work but some tests (such as those extracting locale data) will fail because they make assumptions to verify against specific JREs.
- New JDK than 9 should work, but have not been tested.



### Maven repository

Use the following repo to grab the latest builds/snapshots.

```xml
<repository>
  <id>github-mp1-appengine-repo</id>
  <url>https://maven-repo-254709.appspot.com</url>
</repository>
```

This simple maven repo is hosted on Google App Engine using Cerrato Renaud's [appengine-maven-repository](https://github.com/renaudcerrato/appengine-maven-repository), which is very easy and quick to setup and just works.