FROM apache/airflow:2.9.1-python3.10

USER root

RUN apt-get update \
&& apt-get install -y --no-install-recommends \
    vim \
    git \
    iputils-ping \
    net-tools \
    telnet \
    curl \
    wget \
    unzip \
&& apt-get autoremove -yqq --purge \
&& apt-get clean \
&& rm -rf /var/lib/apt/lists/*

USER airflow

# Set working directory to /airflow
WORKDIR /airflow

# Copy requirements file and install dependencies
COPY requirements.txt .

RUN pip install -r requirements.txt

# Uncomment if you have dags to copy
# COPY /dags ./dags

# Change to airflow user
USER default

# Expose necessary ports
EXPOSE 8080
EXPOSE 8793
EXPOSE 5555
