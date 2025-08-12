# karpenter-daemonset-priority-class

Simple demo repository to deploy a Helm Chart with a Priority class

## Install locally

It is possible to install this Helm chart locally by running:

```shell
helm install karpenter-daemonset-priorityclass .
```

## Multiple Deployments

This chart supports multiple deployments by automatically prefixing the PriorityClass name with the Helm release name. Each deployment will create a unique PriorityClass resource, preventing conflicts when deploying the same chart multiple times with different release names.
