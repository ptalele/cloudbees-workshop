Lab 02: Extending build scans
=============================

NOTE: To view the build scans, use the credentials provided in the slides

- Open `build.gradle`, find the code adding the tags, values and links

- Run a build to publish a build scan

      ./gradlew build

- Follow the link in the console output to view your build scan

- Find the tags, links and values in your build scan

- Run another build adding a tag at build time

    ./gradlew build -Dscan.tag.TEST

- Go to the scan list and find your scan with this tag
