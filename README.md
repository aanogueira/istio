# Istio Operator

A modified version of the [Istio Operator](https://github.com/istio/istio/tree/master/operator)
where the Kubernetes resources are applied in a a reverse alphabetic order and the Service
is applied a bit later in order for the
[AWS Target Group Binding](https://kubernetes-sigs.github.io/aws-load-balancer-controller/guide/targetgroupbinding/targetgroupbinding/)
to be ready before the Deployment catches the `NLB` changes.

> Currently supported versions can be check in the `releases`/`tags` section of this project.

**Docker images**: [operator](https://hub.docker.com/r/aanogueira/operator)

