# Kubernetes with Docker & Minikube

This project demonstrates how to run two separate pods — one with **Nginx** and another with a **Node.js** application — simultaneously using **Minikube** and **Docker**.

## 🛠️ Tech Stack

- Kubernetes
- Docker
- Minikube
- Node.js
- Nginx
- YAML for pod definitions

---

Deploy Pods
kubectl apply -f nginx-pod.yaml
kubectl apply -f nodejs-pod.yaml



Verify Pods
kubectl get pods



Access the Applications
kubectl port-forward pod/nodejs-pod-name 3000:3000
kubectl port-forward pod/nginx-pod-name 8080:80


when you do  it step by step it use  minikube ip and default assign ip but 
sometime it does not work  so youhave touse this code to forwqrd the ip.
