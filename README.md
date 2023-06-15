# numaresources-operator-must-gather

[`numaresources-operator`](https://github.com/openshift-kni/numaresources-operator) is an openshift operator for k8s to allow to expose per-NUMA-zone compute resources.
[`openshift-must-gather`](https://github.com/openshift/must-gather) is a tool for collecting cluster data.

`numaresources-operator-must-gather` will create a "must-gather-like" image to collect numaresources-operator related data from openshift clusters.


## How to run 
You can run `numaresources-operator-must-gather` on a cluster with

```shell
oc adm must-gather --image=<image_name>
```

Where `<image_name>` is the name of the curretn image

For more information please refer to must-gather doc page [here](https://docs.openshift.com/container-platform/4.13/support/gathering-cluster-data.html)