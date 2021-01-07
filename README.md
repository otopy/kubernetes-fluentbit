# kubernetes-fluentbit

Файлы деплоя для fluentbit в kubernetes

* 01-flb-acc.yaml - ServiceAccount, ClusterRole, ClusterRoleBinding, Secret (access to elasticsearch)
* 02-flb-cm.yaml - ConfigMap. Конфигурационные файлы fluentbit.
* 03-flb-services.yaml - Service и Endpoints для доступа ко внешнему (за пределами кластера k8s) elasticserach.
* 04-flb-ds.yaml - DaemonSet
* 05-flb-ds-service.yaml - Service для доступа к метрикам fluentbit
* 06-flb-sm.yaml - ServiceMonitor для PrometheusOperator.

За основу были использованы файлы из проекта https://github.com/fluent/fluent-bit-kubernetes-logging
