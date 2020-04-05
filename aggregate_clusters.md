# Aggregate Clusters in Envoy

Aggregate clusters are a new addition to envoy (included in 1.13). The idea behind aggregate clusters is the need to have the ability to do
failover within a cluster. Prior to aggregate clusters there was no way to failover if there were no healthy hosts in a cluster. With aggregate
cluster we can now define a primary, secondary cluster and envoy will try to find a host within these clusters based on a computed linearized
priority list of hosts.

You can follow along my example here [https://github.com/rkbalgi/appmesh-microsrvc#notes-for-running-aggregate-cluster-demo-on-envoyproxy](https://github.com/rkbalgi/appmesh-microsrvc#notes-for-running-aggregate-cluster-demo-on-envoyproxy)




## Links
 - [https://github.com/envoyproxy/envoy/issues/7454](https://github.com/envoyproxy/envoy/issues/7454)
 - [https://www.envoyproxy.io/docs/envoy/latest/intro/arch_overview/upstream/aggregate_cluster](https://www.envoyproxy.io/docs/envoy/latest/intro/arch_overview/upstream/aggregate_cluster)
 