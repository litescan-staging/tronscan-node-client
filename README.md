<h1 align="center">
  Litescan Client
  <br>
</h1>

<h4 align="center">
  Node Client for the <a href="https://github.com/litescan/litescan-frontend/blob/dev2019/document/api.md">Litescan.org API</a>
</h4>

<p align="center">
  <a href="#how-to-use">How to Use</a>
</p>

# How to use

## Requirements

* Node v9.8.0

## Running tests

```bash
> npm test
```

## Usage

Install the package

```bash
> npm install @litescan/client
```

Use the HTTP Client

```javascript
import {Client} from "@litescan/client";

const client = new Client();

let recentBlocks = await client.getBlocks({
  sort: '-number',
  limit: 10,
});
```
