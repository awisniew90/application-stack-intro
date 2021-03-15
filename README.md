<!-- PROJECT LOGO -->

<p align="center">
  <a href="https://openliberty.io/">
    <img src="https://openliberty.io/img/spaceship.svg" alt="Logo">
  </a>
</p>
<p align="center">
  <a href="https://openliberty.io/">
    <img src="https://github.com/OpenLiberty/open-liberty/blob/master/logos/logo_horizontal_light_navy.png" alt="title" width="400">
  </a>
</p>
<br />

[![License](https://img.shields.io/badge/License-ASL%202.0-green.svg)](https://opensource.org/licenses/Apache-2.0)

# application-stack-intro

NOTE: This branch does not include a devfile and is intended to demonstrate how the stack's devfile can be downloaded automatically from the devfile registry. 

This app is a simple but complete JAX-RS sample for use with the Open Liberty application stack. It includes a basic REST API, integration tests, and the MicroProfile Config, Health, and Metrics features.

### Getting Started

> It's recommended to use the latest version of OpenShift Do (odo). You can install odo using [these instructions](https://odo.dev/docs/installing-odo/)

1. Perform an `oc login` to your cluster.

1. Clone the application-stack-intro repository

    ```shell
    git clone -b blog-demo git@github.com:OpenLiberty/application-stack-intro.git
    cd application-stack-intro
    ```

1. Create your odo component

    ```shell
    odo create java-openliberty my-component
    ```

1. Push the sample application to OpenShift

    ```shell
    odo push
    ```
1. Wait for tests to complete

    ```shell
    odo log -f
    ```

For more details on using the Open Liberty application-stack, check out https://github.com/OpenLiberty/application-stack

For more details on using odo, check out https://odo.dev
