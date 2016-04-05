# Devops delivery pipeline Kibana docker image

## Run from docker hub image

```
sudo docker run --name=box-kibana -p 9300:5601 -d -it -v /etc/hosts:/etc/hosts -e ELASTICSEARCH_URL=http://box-elastic.docker:9200 devopsru/training-kibana-image
```

## Build and run 

```
sudo docker build -t kibana .
sudo docker run --name=box-kibana -p 9300:5601 -d -it -v /etc/hosts:/etc/hosts -e ELASTICSEARCH_URL=http://box-elastic.docker:9200 kibana
```
