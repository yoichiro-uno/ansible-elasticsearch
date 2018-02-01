
need_local_volume: "yes"
localvolumes:
  - /data/elasticsearch/data
  - /data/elasticsearch/env
  - /data/elasticsearch/conf
  - /data/elasticsearch/log
containersettings:
 - {"container_name": "esmaster01", "container_image": "centos", "container_ports": [ "9200:9200", "9300:9300", "9201:9201"], "container_volumes": [ "/data/elasticsearch/conf:/etc/elasticsearch", "/data/elasticsearch/env:/etc/sysconfig/elasticsearch", "/data/elasticsearch/data:/var/lib/elasticsearch", "/data/elasticsearch/log:/var/log/elasticsearch"]}
 
 
 
