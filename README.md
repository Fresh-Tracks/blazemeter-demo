# blazemeter-demo
Simple App to Test BlazeMeter Jenkins Integration

# For Kubernetes
To build and run in minikube:

1. minikube start
2. eval $(minikube docker-env)
3. docker build . -t blazemeter-demo
4. kubectl apply -f k8s
5. minikube service blazemeter-demo

To build and push to GCR/Bowl
1. docker build . -t blazemeter-demo 
2. docker tag blazemeter-demo:latest gcr.io/freshtracks-io/blazemeter-demo:latest
3. docker push gcr.io/freshtracks-io/blazemeter-demo
4. kubectl apply -f k8s

To run the simple jmeter script:

1. brew install jmeter
2. jmeter -t blazemeter-demo.jmx


