# Custom Debian Live System

Configuration and scripts for building a custom Debian "Buster" live system

## Building with Docker

The builds can run entirely within Docker, and have been tested on OSX and Debian hosts. Docker Compose is used to orchestrate this, and mount a cache volume.

```sh
make build
```

*Note:* Due to network timeouts or races, the first build on a fresh system without a cache may fail. This is normal, and it should be run again.

### Building with Debian

The builds can also be performed on a Debian (or any Debian family with `live-build` package installed).

```sh
cd config
./build.sh
```
