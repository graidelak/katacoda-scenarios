In this demo we are going to create a pod. We will launch a simple static-web: 

You can create a pod with `kubectl run nginx --image=nginx:latest`{{execute}}

or from the manifest, copy and paste this yaml in the terminal:
```
apiVersion: v1
kind: Pod
metadata:
  name: static-web
  labels:
    role: myrole
spec:
  containers:
    - name: web
      image: nginx
      ports:
        - name: web
          containerPort: 80
          protocol: TCP
```{{copy}}

Then apply the yaml to create the pod:
`kubectl apply -f static-web.yaml`{{execute}}

To check if the pod is up and running:

`kubectl get pod`{{execute}}

You have created a Pod. Congratulations!



