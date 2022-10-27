---
title: karmadactl addons list
---

List karmada addons from Kubernetes

### Synopsis

List Karmada addons from Kubernetes

```
karmadactl addons list
```

### Examples

```
  # List Karmada all addons installed in Kubernetes cluster
  karmadactl addons list
  
  # List Karmada all addons included scheduler estimator of member1 installed in Kubernetes cluster
  karmadactl addons list -C member1
  
  # Specify the host cluster kubeconfig
  karmadactl addons list --kubeconfig /root/.kube/config
  
  # Specify the karmada control plane kubeconfig
  karmadactl addons list --karmada-kubeconfig /etc/karmada/karmada-apiserver.config
  
  # Sepcify the namespace where Karmada components are installed
  karmadactl addons list --namespace karmada-system
```

### Options

```
  -C, --cluster string              Name of the member cluster that enables or disables the scheduler estimator.
      --context string              The name of the kubeconfig context to use.
  -h, --help                        help for list
      --karmada-context string      The name of the karmada control plane kubeconfig context to use.
      --karmada-kubeconfig string   Path to the karmada control plane kubeconfig file. (default "/etc/karmada/karmada-apiserver.config")
  -n, --namespace string            namespace where Karmada components are installed. (default "karmada-system")
```

### Options inherited from parent commands

```
      --add-dir-header                   If true, adds the file directory to the header of the log messages
      --alsologtostderr                  log to standard error as well as files
      --kubeconfig string                Paths to a kubeconfig. Only required if out-of-cluster.
      --log-backtrace-at traceLocation   when logging hits line file:N, emit a stack trace (default :0)
      --log-dir string                   If non-empty, write log files in this directory
      --log-file string                  If non-empty, use this log file
      --log-file-max-size uint           Defines the maximum size a log file can grow to. Unit is megabytes. If the value is 0, the maximum file size is unlimited. (default 1800)
      --logtostderr                      log to standard error instead of files (default true)
      --one-output                       If true, only write logs to their native severity level (vs also writing to each lower severity level)
      --skip-headers                     If true, avoid header prefixes in the log messages
      --skip-log-headers                 If true, avoid headers when opening log files
      --stderrthreshold severity         logs at or above this threshold go to stderr (default 2)
  -v, --v Level                          number for the log level verbosity
      --vmodule moduleSpec               comma-separated list of pattern=N settings for file-filtered logging
```

### SEE ALSO

* [karmadactl addons](karmadactl_addons.md)	 - Enable or disable a Karmada addon

#### Go Back to [Karmadactl Commands](karmadactl_index.md) Homepage.


###### Auto generated by [spf13/cobra script in Karmada](https://github.com/karmada-io/karmada/tree/master/hack/tools/genkarmadactldocs).