# TASK-5 DAY-5
# Task-5: Deploy Custom App to Kubernetes using Minikube
## Tools Used
- Minikube
- kubectl
- Docker
- YAML files (Deployment & Service)
---

##  Kubernetes YAML Files
# deployment.yaml
![Screenshot 2025-04-14 154845](https://github.com/user-attachments/assets/c7109097-66ff-403d-96f8-d841816e4025)

# service.yaml
![Screenshot 2025-04-14 154825](https://github.com/user-attachments/assets/f44d0922-d45f-4061-8c3a-f72b2aac01e9)

## STEPS TO DEPLOY

```bash
minukube start
```
![Screenshot 2025-04-14 150845](https://github.com/user-attachments/assets/74c11866-d3be-4e84-b71b-cc3adfb8233f)

```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```
![Screenshot 2025-04-14 153629](https://github.com/user-attachments/assets/d43d7f24-9ffb-4f10-9401-50e19ac44e29)

```bash
kubectl get pods
kubectl get svc
kubectl get deployments
```
![Screenshot 2025-04-14 153728](https://github.com/user-attachments/assets/b16cee2f-3f1e-421f-a574-b68d66ed171d)
![Screenshot 2025-04-14 154100](https://github.com/user-attachments/assets/8d18adf2-43b6-48cc-8f3f-179fc573e5c8)

## Scale the Deployment
```bash
kubectl scale deployment nginx-deployment --replicas=4
```
![Screenshot 2025-04-14 154250](https://github.com/user-attachments/assets/a2014df8-a1b6-4ca5-9e33-ac4dff63ac8a)

## Use kubectl describe and Logs
```bash
kubectl describe pod <pod-name>
kubectl logs <pod-name>
```
![Screenshot 2025-04-14 154358](https://github.com/user-attachments/assets/9a6c977e-837b-4401-9f7d-e72d4b9c3fa1)
![Screenshot 2025-04-14 154541](https://github.com/user-attachments/assets/fb7216ef-2465-4589-a9b1-a633a258823d)
# no logs are there.



