### Kilim IP Multicast

[kilim](https://github.com/kilim/kilim) is a continuation and actor library for java.
[my fork is planned to be kilim 2.0](https://github.com/nqzero/kilim)

this project builds upon kilim to provide IP multicast support

- [ChiaHung Lin](https://github.com/chl501) submitted https://github.com/kilim/kilim/pull/4
- the kilim team was unable to test this code (no multicast environment set up),
  so rather than integrate it into kilim it was broken out into a separate project
- [CHL's original commit](https://github.com/chl501/kilim/tree/9f14f11e05a15e99b974b9f69837bdabae9776c3)
- [discussion on google groups](https://groups.google.com/forum/?hl=en#!topic/kilimthreads/k7QIf2Cn4qM)
- the code looks reasonable, builds, and weaves, the (minimal) included tests pass,
  and `kilim.examples.aio.Multicast` runs (but does nothing since i don't have multicast enabled)
- CAVEAT EMPTOR ... use at your own risk, this project exists primarily to preserve the code
  and is completely unmaintained and unsupported (the original author CHL is no longer active on github)
- MIT License (the same as kilim)


##### Maven

the artifact has not been published, so you'll need to `mvn package` locally to use it

```
    <dependency>
        <groupId>org.db4j</groupId>
        <artifactId>kilim-multicast</artifactId>
        <version>0.1</version>
    </dependency>
```




