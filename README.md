## Setup 

**Prerequisites**:

1. [docker](https://docs.docker.com/engine/install/) & [docker compose](https://docs.docker.com/compose/)
2. Atleast 4GB (preferably 8GB or more) memory

Start the container by opening a terminal in the downloaded project folder and starting the containers

```bash

docker compose up --build -d 
sleep 30
```

Open Jupyter lab at **[http://localhost:8888/lab/](http://localhost:8888/lab/)**.

Stop containers with

```bash
docker compose down -v
sudo rm -rf ./minio_data/*
sudo rm -rf ./notebooks/data/*
```

## Licensing & Attribution

### MinIO
This course uses [MinIO](https://min.io) for object storage demonstrations. MinIO is open source software licensed under GNU AGPL v3.

### Stack Overflow Dataset
This course uses the Stack Overflow dataset for examples and exercises.

**Dataset:** Stack Overflow questions and answers  
**Source:** [ClickHouse Example Datasets](https://clickhouse.com/docs/getting-started/example-datasets/stackoverflow)  
**Original Data:** © Stack Exchange Inc.  
**License:** [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)  

The Stack Overflow data is user-contributed content from the Stack Exchange network, made available under the Creative Commons Attribution-ShareAlike 4.0 International License.

**Note** 
Code archived with 

```bash
zip -r archive.zip . \
  -x "*.git/*" -x ".git/*" \
  -x "*.minio.sys/*" -x ".minio.sys/*" \
  -x "*.Trash-*/*" -x ".Trash-*/*" \
  -x "*.ipynb_checkpoints/*" -x ".ipynb_checkpoints/*" \
  -x "*__pycache__/*" -x "__pycache__/*"
```
