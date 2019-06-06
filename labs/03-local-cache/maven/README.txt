Lab 03: Local build cache
=========================

NOTE: To view the build scans, use the credentials provided in the slides

- Open `.mvn/gradle-enterprise.xml`, note that local cache is not configured (enabled by default)

- Build the project

    ./mvnw clean test

- Build again, notice in the build scan the compilation and test goal outcomes are FROM-CACHE

    ./mvnw clean test

- Execute just a clean

    ./mvnw clean

- Then execute tests and notice the cache was not used

    ./mvnw test

- Build again with build cache disabled, notice the much longer build time

    ./mvnw clean test -Dgradle.cache.local.enabled=false
