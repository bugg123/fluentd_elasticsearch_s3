# Collecting Docker Log Files with Fluentd and Elasticsearch
This directory contains the source files needed to make a Docker image
that collects Docker container log files using [Fluentd][fluentd]
and sends them to an instance of [Elasticsearch][elasticsearch].
This image is designed to be used as part of the [Kubernetes][kubernetes]
cluster bring up process. The image resides at Quay under the name
[quay.io/fluentd_elasticsearch/fluentd][image].

# Credit
This repo is a subset of the kubernetes repo located [here][original].  An image was needed with both elasticsearch and s3 plugins, so this was created to have both.

[fluentd]: http://www.fluentd.org/
[elasticsearch]: https://www.elastic.co/products/elasticsearch
[kubernetes]: https://kubernetes.io
[image]: https://quay.io/repository/fluentd_elasticsearch/fluentd?tab=tags
[original]: https://github.com/kubernetes/kubernetes/tree/master/cluster/addons/fluentd-elasticsearch/fluentd-es-image
