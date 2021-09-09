## Try it

[https://my-json-server.typicode.com/typicode/demo](https://my-json-server.typicode.com/typicode/demo)

## Use your own data

Fork it and change `db.json` values or create a repo with a `db.json` file.

Receive:

container_network_receive_bytes_total
container_network_receive_errors_total
container_network_receive_packets_dropped_total
container_network_receive_packets_total

Transmit:

container_network_transmit_bytes_total
container_network_transmit_errors_total
container_network_transmit_packets_dropped_total
container_network_transmit_packets_total


go_info{}

## Thanos(storage) Prometheus(metrics) Grafana(visual) Umgebung:

NAME                                                      READY   STATUS    RESTARTS   AGE
pod/alertmanager-metrics-kube-prometheus-alertmanager-0   2/2     Running   0          6m21s
pod/metrics-kube-prometheus-operator-7d64586d94-j6z4w     1/1     Running   0          6m35s
pod/metrics-kube-state-metrics-8cf6b7ff-jgxp7             1/1     Running   0          6m35s
pod/metrics-node-exporter-k4pv7                           1/1     Running   0          6m35s
pod/prometheus-metrics-kube-prometheus-prometheus-0       3/3     Running   0          6m21s
pod/storage-thanos-bucketweb-84bcc96b9-hn4vg              1/1     Running   0          5m54s
pod/storage-thanos-compactor-5686c6469b-klg5p             1/1     Running   0          5m54s
pod/storage-thanos-query-79fd85db55-7z2x4                 1/1     Running   0          5m54s
pod/storage-thanos-query-frontend-78fc999b68-qvfgb        1/1     Running   0          5m54s
pod/storage-thanos-ruler-0                                1/1     Running   0          5m53s
pod/storage-thanos-storegateway-0                         1/1     Running   0          5m54s
pod/visual-grafana-6cb7988db9-g8bqv                       1/1     Running   0          5m30s

NAME                                                TYPE           CLUSTER-IP     EXTERNAL-IP     PORT(S)                      AGE
service/alertmanager-operated                       ClusterIP      None           <none>          9093/TCP,9094/TCP,9094/UDP   6m22s
service/metrics-kube-prometheus-alertmanager        ClusterIP      10.0.16.127    <none>          9093/TCP                     6m35s
service/metrics-kube-prometheus-operator            ClusterIP      10.0.157.99    <none>          8080/TCP                     6m35s
service/metrics-kube-prometheus-prometheus          LoadBalancer   10.0.196.216   20.93.253.45    9090:32350/TCP               6m35s
service/metrics-kube-prometheus-prometheus-thanos   ClusterIP      None           <none>          10901/TCP                    6m35s
service/metrics-kube-state-metrics                  ClusterIP      10.0.186.51    <none>          8080/TCP                     6m35s
service/metrics-node-exporter                       ClusterIP      10.0.238.232   <none>          9100/TCP                     6m35s
service/prometheus-operated                         ClusterIP      None           <none>          9090/TCP                     6m21s
service/storage-thanos-bucketweb                    ClusterIP      10.0.244.233   <none>          8080/TCP                     5m54s
service/storage-thanos-compactor                    ClusterIP      10.0.156.135   <none>          9090/TCP                     5m54s
service/storage-thanos-query                        ClusterIP      10.0.245.126   <none>          9090/TCP,10901/TCP           5m54s
service/storage-thanos-query-frontend               LoadBalancer   10.0.74.244    20.93.251.116   9090:30856/TCP               5m54s
service/storage-thanos-ruler                        ClusterIP      10.0.12.230    <none>          9090/TCP,10901/TCP           5m54s
service/storage-thanos-storegateway                 ClusterIP      10.0.17.112    <none>          9090/TCP,10901/TCP           5m54s
service/visual-grafana                              LoadBalancer   10.0.119.34    20.93.251.243   3000:30940/TCP               5m30s

NAME                                   DESIRED   CURRENT   READY   UP-TO-DATE   AVAILABLE   NODE SELECTOR   AGE
daemonset.apps/metrics-node-exporter   1         1         1       1            1           <none>          6m35s

NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/metrics-kube-prometheus-operator   1/1     1            1           6m35s
deployment.apps/metrics-kube-state-metrics         1/1     1            1           6m35s
deployment.apps/storage-thanos-bucketweb           1/1     1            1           5m54s
deployment.apps/storage-thanos-compactor           1/1     1            1           5m54s
deployment.apps/storage-thanos-query               1/1     1            1           5m54s
deployment.apps/storage-thanos-query-frontend      1/1     1            1           5m54s
deployment.apps/visual-grafana                     1/1     1            1           5m30s

NAME                                                          DESIRED   CURRENT   READY   AGE
replicaset.apps/metrics-kube-prometheus-operator-7d64586d94   1         1         1       6m35s
replicaset.apps/metrics-kube-state-metrics-8cf6b7ff           1         1         1       6m35s
replicaset.apps/storage-thanos-bucketweb-84bcc96b9            1         1         1       5m54s
replicaset.apps/storage-thanos-compactor-5686c6469b           1         1         1       5m54s
replicaset.apps/storage-thanos-query-79fd85db55               1         1         1       5m54s
replicaset.apps/storage-thanos-query-frontend-78fc999b68      1         1         1       5m54s
replicaset.apps/visual-grafana-6cb7988db9                     1         1         1       5m30s

NAME                                                                 READY   AGE
statefulset.apps/alertmanager-metrics-kube-prometheus-alertmanager   1/1     6m22s
statefulset.apps/prometheus-metrics-kube-prometheus-prometheus       1/1     6m21s
statefulset.apps/storage-thanos-ruler                                1/1     5m54s
statefulset.apps/storage-thanos-storegateway                         1/1     5m54s


### storage(Thanos):

pod/storage-thanos-bucketweb-84bcc96b9-hn4vg              1/1     Running   0          5m54s
pod/storage-thanos-compactor-5686c6469b-klg5p             1/1     Running   0          5m54s
pod/storage-thanos-query-79fd85db55-7z2x4                 1/1     Running   0          5m54s
pod/storage-thanos-query-frontend-78fc999b68-qvfgb        1/1     Running   0          5m54s
pod/storage-thanos-ruler-0                                1/1     Running   0          5m53s
pod/storage-thanos-storegateway-0                         1/1     Running   0          5m54s

service/storage-thanos-bucketweb                    ClusterIP      10.0.244.233   <none>          8080/TCP                     5m54s
service/storage-thanos-compactor                    ClusterIP      10.0.156.135   <none>          9090/TCP                     5m54s
service/storage-thanos-query                        ClusterIP      10.0.245.126   <none>          9090/TCP,10901/TCP           5m54s
service/storage-thanos-query-frontend               LoadBalancer   10.0.74.244    20.93.251.116   9090:30856/TCP               5m54s
service/storage-thanos-ruler                        ClusterIP      10.0.12.230    <none>          9090/TCP,10901/TCP           5m54s
service/storage-thanos-storegateway                 ClusterIP      10.0.17.112    <none>          9090/TCP,10901/TCP           5m54s

deployment.apps/storage-thanos-bucketweb           1/1     1            1           5m54s
deployment.apps/storage-thanos-compactor           1/1     1            1           5m54s
deployment.apps/storage-thanos-query               1/1     1            1           5m54s
deployment.apps/storage-thanos-query-frontend      1/1     1            1           5m54s

replicaset.apps/storage-thanos-bucketweb-84bcc96b9            1         1         1       5m54s
replicaset.apps/storage-thanos-compactor-5686c6469b           1         1         1       5m54s
replicaset.apps/storage-thanos-query-79fd85db55               1         1         1       5m54s
replicaset.apps/storage-thanos-query-frontend-78fc999b68      1         1         1       5m54s

statefulset.apps/storage-thanos-ruler                                1/1     5m54s
statefulset.apps/storage-thanos-storegateway                         1/1     5m54s


### metrics(Prometheus):

pod/metrics-kube-prometheus-operator-7d64586d94-j6z4w     1/1     Running   0          6m35s
pod/metrics-kube-state-metrics-8cf6b7ff-jgxp7             1/1     Running   0          6m35s
pod/metrics-node-exporter-k4pv7                           1/1     Running   0          6m35s

service/metrics-kube-prometheus-alertmanager        ClusterIP      10.0.16.127    <none>          9093/TCP                     6m35s
service/metrics-kube-prometheus-operator            ClusterIP      10.0.157.99    <none>          8080/TCP                     6m35s
service/metrics-kube-prometheus-prometheus          LoadBalancer   10.0.196.216   20.93.253.45    9090:32350/TCP               6m35s
service/metrics-kube-prometheus-prometheus-thanos   ClusterIP      None           <none>          10901/TCP                    6m35s
service/metrics-kube-state-metrics                  ClusterIP      10.0.186.51    <none>          8080/TCP                     6m35s
service/metrics-node-exporter                       ClusterIP      10.0.238.232   <none>          9100/TCP                     6m35s

daemonset.apps/metrics-node-exporter   1         1         1       1            1           <none>          6m35s

deployment.apps/metrics-kube-prometheus-operator   1/1     1            1           6m35s
deployment.apps/metrics-kube-state-metrics         1/1     1            1           6m35s

replicaset.apps/metrics-kube-prometheus-operator-7d64586d94   1         1         1       6m35s
replicaset.apps/metrics-kube-state-metrics-8cf6b7ff           1         1         1       6m35s


### visual(Grafana):

pod/visual-grafana-6cb7988db9-g8bqv                       1/1     Running   0          5m30s

service/visual-grafana                              LoadBalancer   10.0.119.34    20.93.251.243   3000:30940/TCP               5m30s

deployment.apps/visual-grafana                     1/1     1            1           5m30s

replicaset.apps/visual-grafana-6cb7988db9                     1         1         1       5m30s


### without installation name:

pod/alertmanager-metrics-kube-prometheus-alertmanager-0   2/2     Running   0          6m21s
