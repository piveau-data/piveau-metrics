# piveau metrics

**PREVIEW VERSION** 

piveau metrics is an Open Data metadata quality assessment service based on Semantic Web technologies

## Installation

### Prerequisites
- Java JDK 11
- Node 10.15.0
- npm 6.4.1
- Docker and Docker Compose
- Maven

### Get the Code
```
$ git clone https://github.com/piveau-data/piveau-metrics-persistence
$ git clone https://github.com/piveau-data/piveau-metrics-service
$ git clone https://github.com/piveau-data/piveau-metrics-url-checker
$ git clone https://github.com/piveau-data/piveau-metrics-similarity-service
$ git clone https://github.com/piveau-data/piveau-metrics-reporter
$ git clone https://github.com/piveau-data/piveau-metrics-ui
```
### Build the Backend
```
$ cd piveau-metrics-persistence
$ mvn clean package -U -DskipTests
$ cd ..
$ cd piveau-metrics-service
$ mvn clean package -U -DskipTests
$ cd ..
$ cd piveau-metrics-url-checker
$ mvn clean package -U -DskipTests
$ cd ..
$ cd piveau-metrics-similarity-service
$ mvn clean package -U -DskipTests
$ cd ..
$ cd piveau-metrics-reporter
$ mvn clean package -U -DskipTests
$ cd ..
```
### Build the Frontend
```
$ cd piveau-metrics-ui
$ npm install
$ npm run build
```

### Run it
```
$ docker-compose up --build
```

## Quick Manual

### Frontend
- The frontend is accessible via `http://localhost:8080`

### APIs
- Metrics endpoint: `http://localhost:8083`
