# Parking System &middot; [![Build Status](https://travis-ci.com/np111/P4_parking_system.svg?branch=master)](https://travis-ci.com/np111/P4_parking_system) [![codecov.io](https://codecov.io/github/np111/P4_parking_system/coverage.svg?branch=master)](https://codecov.io/github/np111/P4_parking_system?branch=master)

A command line app for managing the parking system. 
This app uses Java to run and stores the data in Mysql DB.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

- Install **Java 1.8**
  [(link)](https://docs.oracle.com/javase/8/docs/technotes/guides/install/install_overview.html)
- Install **Maven 3.6.2**
  [(link)](https://maven.apache.org/install.html)
- Install and configure **Mysql 8.0.17**
  - Download and install mysql [(link)](https://dev.mysql.com/downloads/mysql/),
    set the root password to `rootroot` and import `resources/Data.sql`.
  - *--- or ---*
  - Use the docker-compose development environment (it automatically setup everything):
    ```bash
    ./dev.sh docker up -d
    ```

### Running App

```bash
mvn package
java -jar target/parking-system-1.0-SNAPSHOT-jar-with-dependencies.jar
```

### Testing

```bash
mvn verify
```

## Notes
This is a school project (for OpenClassrooms).

The goal is to fix and add some features to an existing application ([see the sprint board](https://www.notion.so/727631bfc99b456f996e9b9780ee4383?v=bc18814b128d476d9fa8979409c80330)).
