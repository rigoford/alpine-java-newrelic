# alpine-java-newrelic
An Alpine Linux docker image based on `java:8-alpine` with the
[New Relic](https://newrelic.com/) Java agent installed into `/opt/newrelic`.


## Usage

Mount (or copy) the `newrelic.yml` configuration file into `/opt/newrelic`. At
a minimum the `license_key` and `app_name` settings must be updated.

Add `-javaagent:/opt/newrelic/newrelic.jar` as a JVM Option.


## Further details

Refer to https://docs.newrelic.com/docs/agents/java-agent for further details.
