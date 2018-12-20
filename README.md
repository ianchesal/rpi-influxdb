# rpi-influxdb

Raspberry Pi compatible Docker base image with InfluxDB, an open source database written in Go specifically to handle time series data with high availability and high performance requirements.

Uses a nearly identical `Dockerbuild` file as the official InfluxDB Docker build flow but it uses Raspbian as the base file layer and s/wget/curl/ throughout.

### Build Details

#### Build the Docker Image
```bash
make build
```

#### Run the Docker Image and get the version of installed InfluxDB client
```bash
make version
```

#### Push the Docker Image to the Docker Hub
* First use a `docker login` with username, password and email address
* Second push the Docker Image to the official Docker Hub

```bash
make push
```

