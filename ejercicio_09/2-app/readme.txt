El formato de la url de postres es:
postgres://YourUserName:YourPassword@YourHostname:5432/YourDatabaseName

ej: postgres://tico:ticopostgres@$(minikube ip):31001/db1

Para configurar el secret:
echo -n "postgres://tico:ticopostgres@$(minikube ip):31001/db1" | base64

El puerto se puede tomar con: 
kubectl get service postgres -o jsonpath='{.spec.ports[0].nodePort}'
Pero hay que tener en cuenta que si no seteamos uno, el tipo NodePort nos va a dar un puerto random



Luego de aplicar el service, se puede probar la app en la url:
http://$(minikube ip):31002