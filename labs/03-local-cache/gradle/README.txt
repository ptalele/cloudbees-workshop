Lab 03: Local build cache
=========================

NOTE: To view the build scans, use the credentials provided in the slides

- Open `gradle.properties`, note that caching is enabled
    - verbose console is enabled to make seeing the effects of caching easier

- Build the project

    ./gradlew build

- Build again with clean, notice in the build scan the compilation and test task outcomes are FROM-CACHE

    ./gradlew clean build

- Build again with clean and build cache disabled, notice the much longer build time

    ./gradlew clean build --no-build-cache
