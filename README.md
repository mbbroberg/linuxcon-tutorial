# LinuxCon Tutorial
Hey LinxuCon! :wave:

I want to walk through learning cool things about telemetry using Snap, the open telemetry framework I've been working on.

**We want to get to:**
* Snap v0.15.0 running on your laptop
* A time-series database configured to collect telemetry
* Grafana configured to visualize this telemetry

You have a few ways to do that. I'll share them from easiest to hardest.

## Easiest
You get:
  * Reusable demo environment safely living in containers
  * 1 VM with InfluxDB and Grafana ready to deploy in Docker
  * 1 or more VMs with Snap running as a service and in Tribe Mode

### How to get going
  * `git clone` [this repository](https://github.com/nanliu/snap-demo-velocity#velocity-2016-snap-demo)
  * Install the dependencies
  * `vagrant up` and `vagrant ssh`

## Intermediate
You get:
  * Snap packages installed on your OS of choice
  * InfluxDB and Grafana up and running in Docker

### How to get going
  * Download latest package from [snap-telemetry.io](http://snap-telemetry.io/download.html)
  * Install for your OS ([syntax in the docs](docs/install-snap.md))
  * `git clone` the [Snap framework](https://github.com/intelsdi-x/snap)
  * `cd` to `examples/influxdb-grafana`
  * `docker-compose up -d`


## Hardest: Build from Source
You get:
  * Experience building Snap from source
  * Further experience being a CLI sorcerer

### How you get going
  * `git clone` or `go get -d github.com/intelsdi-x/snap`
  * `git clone` or `docker run` Grafana
  * Same for InfluxDB (or whatever other persistence you want to use as long as a publisher is in [the Plugin Catalog](http://snap-telemetry.io/plugins.html))
