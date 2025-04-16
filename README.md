# Kubernetes-Cluster-with-Minikube

Install Minikube on an Amazon EC2 instance using the `none` driver and deploying a simple NGINX app exposed via a `NodePort`.

## Prerequisites

- Amazon Linux EC2 instance (t2.medium or higher recommended)
- Docker installed and running
- Sudo/root access
- kubectl and Minikube binaries
  
## Installation and setup steps

1. Install `kubectl`
2. Install `Minikube` and dependencies
3. Start Minikube with none drive
4. Create `deployment.yaml` and `service.yaml`
5. Apply the configurations
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
6. Deploy `Kubectl`
kubectl get deploy
7. Check pod and service status
kubectl get pods
kubectl get svc nginx-service
8. Add  Security Groups
Ensure the following inbound rules in your EC2 security group:
Port 22 (SSH)
Port 80 (HTTP)
Port 32065 (NodePort)
Optional: Port Range 30000–32767 (for future NodePort services)
9. Access from browser/ ngnix-server
10. Cleanup
minikube delete

![Screenshot (67)](https://github.com/user-attachments/assets/c16204ab-0aa9-4352-88ed-7b4fc5cf9949)


![Screenshot (68)](https://github.com/user-attachments/assets/4d50755e-f0ef-4338-b000-7b985895762c)


![Screenshot (69)](https://github.com/user-attachments/assets/b687e4fe-9983-45cf-85be-2869da5cc836)

![Screenshot (70)](https://github.com/user-attachments/assets/b3d58e61-fa16-4ce7-905f-46250f2d29d4)

![Screenshot (71)](https://github.com/user-attachments/assets/bfd5dfe0-e700-4205-a35f-29a6e8304457)

![Screenshot (72)](https://github.com/user-attachments/assets/39daec3e-cbff-4983-b97c-c32ad20495a3)

![Screenshot (73)](https://github.com/user-attachments/assets/21c8b680-d040-4f97-8283-e5e6ee441f37)


![Screenshot (74)](https://github.com/user-attachments/assets/639fbeaa-2379-40aa-95ae-2bef92021cc0)

![Screenshot (75)](https://github.com/user-attachments/assets/07ef2115-9596-4092-8e75-24f04451148a)

