# Data Storage Patterns for Data Warehouse 

Code for Blog at **[Coming Soon](https://www.startdataengineering.com/)**

## Setup 

**Prerequisites**:

1. [docker](https://docs.docker.com/engine/install/) & [docker compose](https://docs.docker.com/compose/)
2. Atleast 4GB (preferably 8GB or more) memory


Clone and start the containers using the command below on your terminal.

**Windows users**: please setup WSL and a local Ubuntu Virtual machine following [the instructions here](https://documentation.ubuntu.com/wsl/stable/howto/install-ubuntu-wsl2/#what-you-will-learn) until you get an ubuntu prompt.

```bash
git clone 
docker compose up --build -d 
sleep 30
```

* Open data storage pattern code notebook at **[storage_patterns.ipynb](http://localhost:8888/lab/tree/storage_patterns.ipynb)**
* Open Spark History Server at **[http://localhost:18080/](http://localhost:18080/)**
* Open Spark UI at **[http://localhost:4040/](http://localhost:4040/)**, and upto 4049 port (one SparkSessions UI per port from 4040 to 4049)
* Open Minio at **[http://localhost:9001](http://localhost:9001)** with `admin` and `password` as username and password.

Once done, stop containers with

```bash
docker compose down -v
sudo rm -rf ./minio_data/*
sudo rm -rf ./notebooks/data/*
```

## Licensing & Attribution

### MinIO
This course uses [MinIO](https://min.io) for object storage demonstrations. MinIO is open source software licensed under GNU AGPL v3.

