# Instalando EFK stack en Kubernetes

Minikube tiene instalado EFK

Para habilitarlo deben hacer lo siguiente


    minikube start
    minikube addons list
    minikube addons enable ingress
    minikube addons enable efk
    
Luego de estos pasos pueden levantar el dashboard de kibana con esta instruccion:

    minikube service kibana-logging --namespace=kube-system
