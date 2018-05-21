# blazemeter-demo
Simple App to Test BlazeMeter Jenkins Integration

# For Kubernetes
To build and run in minikube:

1. minikube start
2. eval $(minikube docker-env)
3. docker build . -t blazemeter-demo 
4. kubectl apply -f k8s
5. minikube service blazemeter-demo

