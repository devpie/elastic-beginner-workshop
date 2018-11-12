# Get your Elastic environment up and running
We will use docker-compose and docker in order to get the elastic stack up and running.
In the next steps you will download this data set, that will be read by logstash and put into your local dockerized elasticsearch instance.
With you local Kibana instance, you then will be able to see the 1 million documents. 

## Getting the data set
Preferably download the data set by Signal Media with 1 million documents: https://research.signalmedia.co/datasets/signal1m.html

The gzipped jsonl file you will be downloading has a size of round about 1 GB. Unzipped the jsonl file is 2.6 GB in size.

## Unzipping
Unzip the signalmedia-1m.jsonl.gz file into the ```<repo-dir>/infra/logstashInput``` and rename it to ```inputfile.jsonl```

## Start your Elastic Stack
```
cd <repo-dir>/infra
docker-compose up -d
```
