This environment has a `launch.sh`{{execute}}

You can get with `kubectl get nodes`{{execute}}

Now generate the kubeconfig:

`kubectl config set-context ~/.kube/kubeconfig.yml`{{execute}}

Copy the kubeconfig to the node01:

`scp ~/.kube/config node01:/root/.kube/`{{execute}}


