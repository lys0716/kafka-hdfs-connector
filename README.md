# kafka-hdfs-connector

## Dependencies install[working...]
```sh
pip install -r requirements.txt
```

## Set up enviroment
Please check if you have kafka, zookeeper and schema-registry already exist locally. If yes, delete them.
```sh
docker-compose up
```

## avro-data-producer.py
Implement a kafka AvroProducer, fetch stock price from Yahoo finance and store as avro format in kafka.

### Dependecies[working...]
googlefinance   https://pypi.python.org/pypi/googlefinance
kafka-python    https://github.com/dpkp/kafka-python
schedule        https://pypi.python.org/pypi/schedule

### Run
```sh
python avro-data-producer.py AAPL stock-analyzer 192.168.99.100:9092 http://localhost:8081
```

## Sink to hdfs[working...]

## Register on hive meta server[working...]
