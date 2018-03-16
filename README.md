<<<<<<< HEAD
elasticsearch_host_ip: 172.21.11.147
elasticsearch_host_port: 9200
elasticsearch_type_name: sensordata
elasticsearch_index_name: fluentd
elasticsearch_logstash_prefix: sensordata
elasticsearch_flush_interval: 10s
elasticsearch_url: "http://172.21.11.147:9200"

=======

need_local_volume: "yes"
localvolumes:
  - /data/elasticsearch/data
  - /data/elasticsearch/env
  - /data/elasticsearch/conf
  - /data/elasticsearch/log
containersettings:
 - {"container_name": "esmaster01", "container_image": "centos", "container_ports": [ "9200:9200", "9300:9300", "9201:9201"], "container_volumes": [ "/data/elasticsearch/conf:/etc/elasticsearch", "/data/elasticsearch/env:/etc/sysconfig/elasticsearch", "/data/elasticsearch/data:/var/lib/elasticsearch", "/data/elasticsearch/log:/var/log/elasticsearch"]}
 
 
 
>>>>>>> 33377676bcfafdc28a14258afd33a14589369200
