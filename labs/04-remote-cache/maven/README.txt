Lab 04: Remote build cache
==========================

NOTE: To view the build scans, use the credentials provided in the slides

- Open `.mvn/gradle-enterprise.xml`, note that the remote cache is enabled but not the local cache

- Build the project

    ./mvnw clean test

- Go to Performance > Build cache in the build scan. If you have cache hits:
    - Find the `test` goal in the Timeline view and inspect its details. Click the “View origin scan” link to see the build scan of the originating build
    - Make a change to `src/test/java/example/ExampleTest.java`
    - Build your project again, notice that tests had to be recompiled but production classes were reused

- If you do not have any cache hits, ask the instructor on how to diagnose the misses with inputs comaprison
