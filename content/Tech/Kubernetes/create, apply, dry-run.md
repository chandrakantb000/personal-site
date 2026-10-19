#kubernetes #differences #awesome-commands 
#### Differences
While working with kubernetes the most basic commands in kubernetes are
`kubectl create -f file-name.yaml` and `kubectl apply -f file-name.yaml`.
Here comes the concept of imperative and declarative.



#### Awesome command
Just came across this command or more preferably I can say an argument called --dry-run
```
kubectl run nginx-pod --image=nginx --dry-run=client -o yaml > nginx-pod.yaml
```

So what does it do?
Let's break it down

Generally we use the command 
`kubectl run nginx-pod --image=nginx` (this creates and pod named nginx-pod using the image nginx)

`--dry-run=client -o yaml` (without making any changes to kubernetes cluster we test it using --dry-run=client and client means to does it locally without connecting to kube-api-server and then prints the output in yaml format)

`> nginx-pod.yaml` (redirects the output to nginx-pod.yaml file)

How cool is that, it saves a lot of time using this method.

In dry run there are different types like client, server.
I will explore more about server side dry run( in short it sends a request to kubernetes api server so we can verify using multiple checks).