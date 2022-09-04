# Quick opening k8s dashboard via bash (written for mac)

For quickly access to the script just copy it to `/usr/local/bin/` directory.

Examples of working with script:

```shell
kd -n=kube-system -s=kubernetes-dashboard
kd -k
```

Command line arguments:
```
-n=, --namespace=<namespace name>        - name of namespace where kubernetes dashboard is deployed
-s=, --service=<service name>            - name of service of kubernetes dashboard
     --secret=<secret name>              - name of secret with service account token (Default grep by service name)
     --secret-namespace=<namespace name> - name of namespace where secret with service account token is placed (Default kube-system)
-k, --kill                               - killing the background process named kdsh
-h, --help                               - print this help
```

