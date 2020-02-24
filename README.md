# docker elastic

![https://travis-ci.com/alvisisme/docker-elastic](https://img.shields.io/travis/com/alvisisme/docker-elastic)

同步[elastic官方镜像](https://www.docker.elastic.co/#) 至阿里云，加速国内下载。

## 镜像同步规则

镜像同步对应关系如下所述：

完整的镜像名规则为 **REGISTRY/REPO/NAME:TAG**

例如原始镜像名 **docker.elastic.co/elasticsearch/elasticsearch:7.6.0**

**REGISTRY** 为 **docker.elastic.co**

**REPO** 为 **elasticsearch**

**NAME** 为 **elasticsearch**

**TAG** 为 **7.6.0**

对应会同步至阿里云 **registry.cn-hangzhou.aliyuncs.com/alvisisme/elasticsearch:7.6.0**

即

**REGISTRY** 替换为 **registry.cn-hangzhou.aliyuncs.com**，**REPO** 替换为 **alvisisme**，而 **NAME** 和 **TAG** 不变。


## 阿里云镜像

```bash
#Elasticsearch
docker pull registry.cn-hangzhou.aliyuncs.com/alvisisme/elasticsearch:7.6.0
#Kibana
docker pull registry.cn-hangzhou.aliyuncs.com/alvisisme/kibana:7.6.0
#Beats
docker pull registry.cn-hangzhou.aliyuncs.com/alvisisme/auditbeat:7.6.0
docker pull registry.cn-hangzhou.aliyuncs.com/alvisisme/filebeat:7.6.0
docker pull registry.cn-hangzhou.aliyuncs.com/alvisisme/heartbeat:7.6.0
docker pull registry.cn-hangzhou.aliyuncs.com/alvisisme/journalbeat:7.6.0
docker pull registry.cn-hangzhou.aliyuncs.com/alvisisme/metricbeat:7.6.0
docker pull registry.cn-hangzhou.aliyuncs.com/alvisisme/packetbeat:7.6.0
#Logstash
docker pull registry.cn-hangzhou.aliyuncs.com/alvisisme/logstash:7.6.0
#APM Server
docker pull registry.cn-hangzhou.aliyuncs.com/alvisisme/apm-server:7.6.0
#App Search
docker pull registry.cn-hangzhou.aliyuncs.com/alvisisme/app-search:7.6.0
```
