In this demo we are going to create a pod. We will launch a simple static-web: 

You can create a pod with `kubectl run pod --image=nginx:latest`{{execute}}

or from the manifest 

`kubectl apply -f pod/static-web.yaml`{{execute}}

To check if the pod is up and running:

`kubectl get pod`{{execute}}

You have created a Pod. Congratulations!



