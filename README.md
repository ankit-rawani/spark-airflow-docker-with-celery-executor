# **Docker based setup of Spark and Airflow**

To setup the project, clone this repo and run the following commands -
```bash
mkdir -p ./dags ./logs ./plugins ./config
echo -e "AIRFLOW_UID=$(id -u)" > .env
docker compose pull
docker compose build
docker compose up airflow-init
docker compose up
```