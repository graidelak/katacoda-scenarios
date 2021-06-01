In this demo we are going to create a pod. We will launch a simple static-web: 

You can create a pod with `kubectl run pod --image=nginx:latest`{{execute}}

or from the manifest, copy and paste this yaml in the terminal:

<pre class="file" data-filename="static-web.yaml" data-target="insert" data-marker="#TODO-insert">
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
EOF
<pre>

Then apply the yaml to create the pod:

`kubectl apply -f static-web.yaml`{{execute}}

To check if the pod is up and running:

`kubectl get pod`{{execute}}

You have created a Pod. Congratulations!



