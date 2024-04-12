## Pact Consumer Test Project

This project is a simple example of how to use Pact to test a consumer.

### Running the tests
The pact tests are run as part of the Maven build. To run the tests, simply run `mvn clean install` from the root of the project.
The pact files are generated into the `target/pacts` directory.

### Running the broker
To run the Pact Broker, run `docker-compose up` from the docker directory in the project. This will start the Pact Broker on `http://localhost:9292`.

### Publishing the pacts
The pacts can be published to a Pact Broker by running `mvn pact:publish`. This will publish the pacts to the broker at `http://localhost:9292`.
