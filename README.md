This is a Java wrapper around the MailChimp API. Checkout [Example.groovy](src/example/groovy/com/mailchimp/Example.groovy) for a simple demo.

[ ![Codeship Status for PaeDae/mailchimp-java](https://app.codeship.com/projects/dc564a50-aa43-0136-c433-6e7b034bdf95/status?branch=master)](https://app.codeship.com/projects/309075)

## Running the Demo

    ./gradlew example

In [Example.groovy](src/example/groovy/com/mailchimp/Example.groovy) you need to set your credentials and a mailchimp list id.

## Testing

There is a test suite that hits the MailChimp API. To run it, enter your MailChimp API key, list ID, and test email address in `test.properties` and then `./gradlew build`. Unfortunately MailChimp will flag your email address for being resubmitted if you run the test more than a few times, and tests will fail as a result. So it isn't a great fit for the CI environment.

## Maven / Gradle

This library can be included from Maven, e.g using gradle:

    dependencies {
        implementation 'com.github.micheal-swiggs:mailchimp-java:0.5.4'
    }

### Installing

    ./gradlew install

OR

    ./gradlew publish
