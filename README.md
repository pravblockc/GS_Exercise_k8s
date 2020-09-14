# GS_Exercise_k8s hello_world

Below are the steps to Install and run the application.

- Install latest verions of helm(v3.3.1) and kubectl(v1.19.1)
- git clone https://github.com/pravblockc/GS_Exercise_k8s.git

# To run the chart
- Naviagte to the folder containig charts.yaml($PROJECT_ROOT/charts)
- `helm install k8s-hello-world-proxy . --dry-run`

# List all pods, services, deployments, and replica sets
kubectl get all
# List running k8s services
kubectl get services
# Use minikube to tunnel into service for local debugging purposes
minikube service <SERVICE_NAME> --url