---
title: Use tokens
seotitle: Use an authentication token in InfluxDB
description: Use an authentication token in InfluxDB using the InfluxDB UI or the `influx` CLI.
aliases:
  - /influxdb/v2.0/users/tokens/create-token/
menu:
  influxdb_2_0:
    name: Use a token
    parent: Manage tokens
weight: 201
---

## Use tokens

Tokens are used to authenticate all requests to InfluxDB, whether writing, querying, or managing data and resources.

This includes

- using the `influx` command line
- sending raw API requests

### Example

```sh
influx write -t <token> -b BUCKET -o org-name <DATA>
```

### Example

```
export INFLUX_TOKEN=my-token
influx write -b bucket -org org <DATA>
```

### Example

```
curl
```

See Postman for another way to work with the API.

## Influx configurations

To automatically manage and use tokens from the CLI, create a configuration in your local environment.
See the [`influx config`] documentation for more.
