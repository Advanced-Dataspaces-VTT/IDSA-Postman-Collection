# Postman Collection for Data Offering and Consumption

This repository contains two Postman collections: `provide_offerings.postman_collection.json` and `consume_offerings.postman_collection.json`, and an environment file `connector.postman_environment.json`. These collections are used to simulate the process of providing and consuming data offerings.

## Setup

Before running the collections, you need to import the environment file:

1. Open Postman.
2. Click on the gear icon in the top right corner to manage environments.
3. Click on the "Import" button.
4. Select the `connector.postman_environment.json` file and click "Open".

## Provide Offerings

The `provide_offerings.postman_collection.json` collection is used to provide data offerings. 

To run this collection:

1. Open Postman.
2. Click on the "Runner" button at the top left.
3. Select the `provide_offerings.postman_collection.json` collection and the `connector.postman_environment.json` environment.
4. Click on the "Run" button.

The variables required by this collection will be automatically extracted from the responses and set for future requests.

## Consume Offerings

The `consume_offerings.postman_collection.json` collection is used to consume the data offerings provided by the `provide_offerings.postman_collection.json` collection.

To run this collection:

1. Open Postman.
2. Click on the "Runner" button at the top left.
3. Select the `consume_offerings.postman_collection.json` collection and the `connector.postman_environment.json` environment.
4. Click on the "Run" button.

The variables required by this collection will be automatically extracted from the responses and set for future requests.

Ensure that the option to persist the response body is enabled in the Postman settings. This will allow the final request, "Get Artifact", to display the data of the offering.

## Note

Make sure to run the `provide_offerings.postman_collection.json` collection before the `consume_offerings.postman_collection.json` collection, as the latter depends on the data provided by the former.