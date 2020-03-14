# GraalVM Main Information.





## Contents at a Glance.
* [About](#about)
* [Documentation.](#documentation)
* [Pros.](#pros)
* [Articles.](#articles)
* [Conferences.](#conferences)
* [Conference Speakers.](#conference-speakers)
* [Help](#help)





## About.





## Documentation.
* [GraalVM.](https://www.graalvm.org/)
* [GraalVM GitHub.](https://github.com/graalvm/)
* [GraalVM GitHub. Oracle.](https://github.com/oracle/graal)
* [GraalVM Oracle.](https://www.oracle.com/technetwork/graalvm/overview/index.html)
* [GraalVM Native Image Compatibility and Optimization Guide. Limitations.](https://github.com/oracle/graal/blob/master/substratevm/LIMITATIONS.md)
* [Generation platform dependent code.]()
* [Closed World Assumption.](https://www.google.com/search?q=Closed+World+Assumption+graalvm&oq=Closed+World+Assumption+graalvm&aqs=chrome..69i57.10634j0j7&sourceid=chrome&ie=UTF-8)
* [GraalVM Truffle Framework.](https://www.google.com/search?newwindow=1&safe=active&sxsrf=ALeKk02vlhAcgyEQTVt7y28S9id8Bs2TNg%3A1583845303865&ei=t49nXtypNKuMlwTTkZqQCw&q=graalvm+truffle+framework&oq=graalvm+truffle+framework&gs_l=psy-ab.3..0i8i30.91737.91787..92689...0.3..0.102.180.1j1......0....1..gws-wiz.......0i71.5-HfWuvuk2w&ved=0ahUKEwic4dzF-4_oAhUrxoUKHdOIBrIQ4dUDCAs&uact=5)
* [Native Executables and Private Members.](https://quarkus.io/guides/cdi-reference#native-executables-and-private-members)



## Pros.
1. High-Performance modern Java.
2. Low-footprint, fast-startupJava.
3. Combine Java, R, JavaScript, Ruby.
4. Run native languages on the JVM.
5. Tools that work across all languages.
6. Extend a JVM-based application.
7. Extend a native application.
8. Java code as a native library.
9. Polyglot in the database.
10. Create you own language.





## Static Initializer - things not to do.
* Start application threads that continue to run in the background.
* Load native libraries using 'java.lang.Runtime.load(String)'.
* Open files or sockets, or ...
* Allocate C memory, e.g., 'java.nio.ByteBuffer.allocateDirect(int)'.





## Static Initializers.
* Writ your own initialization methods and call them explicitly from your main entry point.

## Static Initializers delay.
* `--delay-class-initialization-to-runtime=class,list`





## Dynamic classloading.
* Image build time - yes.
* Image run time - no.





## Reflection.
* Reflection Config File. Describe which classes are needed for reflection.
* `-H:ReflectionConfigurationFiles=`





## Java Native Interfaces (JNI).
* `-H:+JNI`
* `-H:+JNIConfigurationFiles=`





## Finalizers.
* Finalizers - no.
* Reference and ReferenceQueues - yes 80%.
* Reference.enqueue() and Reference.isEnqueued() - no.





## Resources.
* `-H:IncludeResources=<regex>`
* `-H:IncludeResources="application.yml|META-INF/services/*.*`





## Unsafe.





## Substitutions.





## java.langNoClassDefFoundError.
* `-H:ReportUnsupportedElementsAtRuntime`





## Articles.
* [The GraalVM frenzy.](https://medium.com/@jponge/the-graalvm-frenzy-f54257f5932c)
* [Instant Netty Startup using GraalVM Native Image Generation.](https://medium.com/graalvm/instant-netty-startup-using-graalvm-native-image-generation-ed6f14ff7692)





## Conferences.
* [Олег Шелаев — Компилируем Java ahead of time с GraalVM. Russian version.](https://www.youtube.com/watch?v=tPezgDSD1Bk&t=1448s)





## Conference Speakers.
* [Oleg Šelajev](https://twitter.com/shelajev?lang=en)





## Help.
