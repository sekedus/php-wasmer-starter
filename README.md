# PHP Basic Starter + Wasmer

This example shows how to run a bare-bones [PHP](https://php.org/) script on **Wasmer Edge** using the built-in development server.


## How it Works

The entrypoint [app/index.php](./app/index.php) is intentionally simple:

* Builds an associative array containing a greeting, a few numbers, and `phpversion()`.
* Iterates over the array, printing each key/value pair with tab separators.

Swap this logic for your own endpoints or templates, Wasmer simply executes the PHP script for each request.


## Running Locally

You can run things locally with:

```bash
php -t app -S localhost:8080
```

Or you can also use [wasmer run](https://wasmer.io/help/reference#:~:text=wasmer%20run) to run it locally (check out the [Wasmer install guide](https://docs.wasmer.io/install)):

```bash
wasmer run .
```

Open [http://localhost:8080](http://localhost:8080) with your browser to see the result.


## Deploy to Wasmer

The easiest way to deploy your PHP app is to use the [Wasmer Edge](https://wasmer.io/products/edge).

Live example: https://php-starter-wasmer-examples.wasmer.app/

Run this commmand to deploy to Wasmer Edge:

```bash
wasmer deploy
```

## Docs
- https://docs.wasmer.io/edge/guides/php
- https://docs.wasmer.io/edge/learn/volumes
