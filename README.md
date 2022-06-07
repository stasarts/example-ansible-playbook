# Что делает playbook

`Playbook` установит три приложения:
* jdk
* elasticsearch
* kibana

Дистрибутив JDK в `.tar.gz` нужно предварительно [скачать](https://www.oracle.com/ru/java/technologies/javase/jdk11-archive-downloads.html) и поместить в каталог `/files`.

# Какие у него есть параметры 

[group_vars/all:](group_vars/all/vars.yml)
* java_jdk_version - версия Java .
* java_oracle_jdk_package - дистрибутив JDK в каталоге `/files`.

[group_vars/elasticsearch:](group_vars/elasticsearch/vars.yml)
* elastic_version - версия Elasticsearch и Kibana. 
* elastic_home/kibana_home - директории установки Elasticsearch и Kibana.

# Какие у него есть теги

* java
* elastic
* kibana
