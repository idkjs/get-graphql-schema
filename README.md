# get-graphql-schema [![npm version](https://badge.fury.io/js/get-graphql-schema.svg)](https://badge.fury.io/js/get-graphql-schema)

Fetch and print the GraphQL schema from a GraphQL HTTP endpoint. (Can be used for Relay Modern.)


> **Note**: Consider using [`graphql-cli`](https://github.com/graphcool/graphql-cli) instead for improved workflows.

## Install

```sh
npm install -g get-graphql-schema
```

## Usage

```sh
  Usage: get-graphql-schema [OPTIONS] ENDPOINT_URL > schema.graphql

  Fetch and print the GraphQL schema from a GraphQL HTTP endpoint
  (Outputs schema in IDL syntax by default)

  Options:
    --header, -h    Add a custom header (ex. 'X-API-KEY=ABC123'), can be used multiple times
    --json, -j      Output in JSON format (based on introspection query)
    --version, -v   Print version of get-graphql-schema

```

## Usage With Header from terminal

```sh
  # watch your formatting

  export BEARER_TOKEN=eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6Ik9FWTJSVGM1UlVOR05qS
  export ENDPOINT_URL=https://api.endpoint.com/learn/graphql
  npx get-graphql-schema ENDPOINT_URL -j -h "Authorization=Bearer $BEARER_TOKEN" > graphql_schema.json
```

## Help & Community [![Slack Status](https://slack.graph.cool/badge.svg)](https://slack.graph.cool)

Join our [Slack community](http://slack.graph.cool/) if you run into issues or have questions. We love talking to you!

![](http://i.imgur.com/5RHR6Ku.png)
