init : 
	mkdir -p ./dags ./logs ./plugins ./config
	
build:
	docker build -t apache/apache-airflow:test . && export AIRFLOW_IMAGE_NAME=apache/apache-airflow:test &&  docker compose up -d