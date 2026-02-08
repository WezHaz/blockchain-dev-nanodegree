# Project #3. Connect Private Blockchain to Front-End Client via APIs

## Overview

This project exposes the private blockchain from Project 2 through a REST API built with Express. It provides basic read/write access to the chain and serves as the foundation for later service and validation workflows.

## Objectives

- Wrap blockchain operations in a web service
- Support block retrieval by height
- Support block creation via HTTP POST

## Endpoints

- `GET /block/:height`
- `POST /block`

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

Node.js runtime environment is required.

### Installing

Install all required dependencies

```
$ npm install
```

Run server

```
$ node server.js
```

The API listens on `http://localhost:8000`.

## GET Block Endpoint

This endpoint has a GET request which uses a URL path with a block height parameter. The response for this endpoint provides block object in JSON format.

REQUEST:

```
TYPE: GET
URL: http://localhost:8000/block/[blockheight]
Example URL path:
http://localhost:8000/block/0, where '0' is the block height
```

RESPONSE:

```
{
    "hash": "19eb3cd3c81b45457ded2ecfb6c9b0ccd9e7ab493c7f0b3c5e6dd551cd3736f8",
    "height": 0,
    "body": "First block in the chain - Genesis block",
    "time": "1556966325",
    "previousBlockHash": ""
}
```

## POST Block Endpoint

This endpoint posts a new block with data payload option to add data to the block body. The block body supports a string of text. The response for the endpoint provides block object in JSON format.

REQUEST:

```
TYPE: POST
URL: http://localhost:8000/block
HEADER: { Content-Type: application/json }
Example BODY:
{
    "body": "Test Block 1"
}
```

RESPONSE:

```
{
    "hash": "fba83a7cfbda11b31e788ecd7c25bb45622b1be485d64d0cd3eee4791325f3df",
    "height": 1,
    "body": "Test Block 1",
    "time": "1556971343",
    "previousBlockHash": "19eb3cd3c81b45457ded2ecfb6c9b0ccd9e7ab493c7f0b3c5e6dd551cd3736f8"
}
```

## Built With

* [level](https://www.npmjs.com/package/level) - A Node.js-style LevelDB wrapper for Node.js
* [crypto-js](https://www.npmjs.com/package/crypto-js) - JavaScript library of crypto standards
* [Express](https://expressjs.com/) - Web framework for Node.js

## Notes

- The service reads and writes to the local LevelDB database, so data persists between runs.
- Use a tool like `curl` or Postman to exercise the API.
