# Instalando EFK stack en Kubernetes

Minikube tiene instalado EFK

Para habilitarlo deben hacer lo siguiente:

1. Iniciar Minikube con memoria suficiente para correr este tutorial


    minikube start --memory 5120
    
2. Verificamos la lista de addons (buscamos ingress y efk)    

    minikube addons list
    
3. Habilitamos ingress:
   
    minikube addons enable ingress
    
4. Habilitamos efk:
    
    minikube addons enable efk
    
Luego de estos pasos pueden levantar el dashboard de kibana con esta instruccion:

    minikube service kibana-logging --namespace=kube-system
