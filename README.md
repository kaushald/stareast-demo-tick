# TICK Stack Demo

> A quick way to get a sample TICK stack up at STAREAST 2018

* [Pre-requisites](#pre-requisites)
* [Run](#run)

---

## Pre-requisites

To get started you need a running docker installation. If you don't have one, you can download Docker for [Mac](https://www.docker.com/docker-mac) or [Windows](https://www.docker.com/docker-windows), or follow the installation instructions for Docker CE for your [Linux distribution](https://docs.docker.com/engine/installation/#server).

---

### Run

To run the `sandbox`, simply use the convenient cli:

```bash
$ ./sandbox
sandbox commands:
  up           -> spin up the sandbox environment
  down         -> tear down the sandbox environment
  restart      -> restart the sandbox
  influxdb     -> attach to the influx cli

  enter (influxdb||kapacitor||chronograf||telegraf||ifql) -> enter the specified container
  logs  (influxdb||kapacitor||chronograf||telegraf||ifql) -> stream logs for the specified container

  delete-data  -> delete all data created by the TICK Stack
  docker-clean -> stop and remove all running docker containers
  rebuild-docs -> rebuild the documentation container to see updates
```

To get started just run `./sandbox up`. You browser will open two tabs:

* `localhost:8888` - Chronograf's address. You will use this as a management UI for the full stack
* `localhost:3010` - Documentation server. This contains a simple markdown server for tutorials and documentation.

---
