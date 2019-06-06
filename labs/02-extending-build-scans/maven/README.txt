Lab 02: Extending build scans
=============================

NOTE: To view the build scans, use the credentials provided in the slides

- Open `.mvn/gradle-enterprise.xml`, find the code adding the tags, values and links

- Open `pom.xml`, find the code configuring use of a Groovy script

- Open `buildScanUserData.groovy`

- Run a build to publish a build scan

    ./mvnw clean test

- Follow the link in the console output to view your build scan

- Find the tags, links and values in your build scan

- Run another build adding a tag at build time

    ./mvnw clean test -Dscan.tag.TEST

- Go to the scan list and find your scan with this tag
