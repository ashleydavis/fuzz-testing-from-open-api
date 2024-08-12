# fuzz-testing-from-open-api

An example of fuzz testing a REST API with data generated from an Open API spec.

Built on:
- Fuzzmatic to generate the data from the JSON schema.
- Express.js to implement the REST API.
- MongoDB for the database.
- Jest for running the tests and matching expectations.
- Jest is used to mock MongoDB for the automated fuzz tests.
- Axios for making the HTTP requests.
- Ajv for testing the REST API response against the JSON schema in the test spec.
- Yaml for parsing the test spec.

## Test spec

See the open api spec here: [./openapi.yaml](./openapi.yaml).

See the fuzz testing here: [./test/fuzz-tests.test.js](./test/fuzz-tests.test.js).

## Setup

```bash
git clone https://github.com/ashleydavis/fuzz-testing-from-open-api
cd fuzz-testing-from-open-api
npm install
```

## Run tests

```bash
npm test
```

Note: Testing uses a mocked version of MongoDB.

## Run the REST API

```bash
npm start
```

Note: This includes an instant development database.

