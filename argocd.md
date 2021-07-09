#Title: Installation steps for ArgoCD following Lesson 5.10 demo exercise

#Contributors: Chromilo

1. Install ArgoCD by following kubectl commands from  https://argoproj.github.io/argo-cd/getting_started/#1-install-argo-cd

kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

2. Add nodeport service. Start with yaml file for arocd-server service and edit the yaml file to match below after running below command: 
kubectl get svc -n argocd argocd-server -o yaml > argocd-server-nodeport.yaml 

---contents of updated argocd-server-nodeport.yaml ---
apiVersion: v1
kind: Service
metadata:
  annotations:
  labels:
    app.kubernetes.io/component: server
    app.kubernetes.io/name: argocd-server
    app.kubernetes.io/part-of: argocd
  name: argocd-server-nodeport
  namespace: argocd
spec:
  ports:
  - name: http
    port: 80
    protocol: TCP
    targetPort: 8080
    nodePort: 30007
  - name: https
    port: 443
    protocol: TCP
    targetPort: 8080
    nodePort: 30008
  selector:
    app.kubernetes.io/name: argocd-server
  sessionAffinity: None
  type: NodePort
  ---end contents of updated argocd-server-nodeport.yaml---
  
  3. Grab the "admin" password for the containerized ArgoCD application by following https://argoproj.github.io/argo-cd/getting_started/#4-login-using-the-cli. The result of below is the password for your ArcoCD instance.
  
  kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d
  
  4. Login via https://<vagrant IP>:30008 or http://<vagrant IP>:3000