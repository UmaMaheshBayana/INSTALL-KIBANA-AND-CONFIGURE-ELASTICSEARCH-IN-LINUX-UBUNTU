# INSTALL KIBANA AND CONFIGURE ELASTICSEARCH IN LINUX UBUNTU

***After Elasticsearch install please follow the below setps to install and configure KIBANA***

***Command to install Kibana*** 

```
sudo apt install kibana
````
***Then enable and start the Kibana service***

```
sudo systemctl enable kibana
````
```
sudo systemctl start kibana
````

To check Kibana Status

```
sudo systemctl status kibana
````

***Configure Kibana and ElasticSearch***

To configure Elasticsearch to Kibana go to the below mentioned path to change ```kibana.yml``` file

```
sudo nano /etc/kibana/kibana.yml
````

Here uncomment the below mentioned lines to change configurations

```server.port: 5601```

```server.host: '0.0.0.0'```

```server.maxPayload: 1048576```

```elasticsearch.hosts: ['http://127.0.0.1:9200']```

```kibana.index: '.kibana'```



