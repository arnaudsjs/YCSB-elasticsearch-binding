# YCSB-elasticsearch-binding
An Elasticsearch database interface for YCSB which allows remote connections to the different Elasticsearch nodes in a cluster.

Installation guide
==================

!!! Install Elasticsearch version: 1.5.1 !!!

* Download the YCSB project as follows: git clone https://github.com/brianfrankcooper/YCSB.git
* Remove the already existing Elasticsearch binding: rm -rf YCSB/elasticsearch
* Include the new YCSB binding within the YCSB directory: git clone https://github.com/arnaudsjs/YCSB-elasticsearch-binding.git elasticsearch
* Compile everything by executing the following command within the YCSB directory: mvn clean package

Manual
======

Parameters to set: 

* es.index.key (default: "es.ycsb")
* cluster.name (default: "es.ycsb.cluster")
* hosts (default: "localhost"): A comma-separated list of Elasticsearch nodes to connect to eg. <host1>,<host2>,...
