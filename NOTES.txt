## Deployment of project

**To expose deployment port(8080)**

<br>

`kubectl expose deployment nodejs-app --type=NodePort`

**To port forward**

<br>

`kubectl port-forward svc/nodejs-service 8080:8080 --address 0.0.0.0`

**To access ArgoCD**

<br>

`kubectl port-forward -n argocd svc/argocd-server 9001:80 --address 0.0.0.0`

#To check ingress
curl -L domain.com
