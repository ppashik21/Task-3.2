# Task-3.2

Установить ArgoCD в namespace argocd    
kubectl create namespace argocd    
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml    
kubectl port-forward svc/argocd-server -n argocd 8080:443    

Сделать fork какого нибудь helm chart к себе в гит    

Добавить этот helm chart в приложения, настроить автодеплоймент при изменениях в репозитории    

Добавить пользователя deploy и дать ему права только на это приложение и только на его синхронизацию    


*) Задача повышенной трудности: 
Создать телеграмм канал и бота, настроить в него нотификации от ArgoCD    


Примечания:
Если ресурсы позволяют, можно взять достаточно большое микросервисное приложение, например вот это: https://github.com/microservices-demo/microservices-demo/tree/master/deploy/kubernetes/helm-chart    

Если нет - можно взять наш любимый wordpress - https://github.com/bitnami/charts/tree/master/bitnami/wordpress
