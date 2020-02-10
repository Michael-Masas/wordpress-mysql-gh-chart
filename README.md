# wordpress-mysql-gh-chart
Helm Chart - Github Pages is a Repo for this chart - Link Below :

To add and install the repo and chart:

- helm repo add wpmHelm https://michael-masas.github.io/wordpress-mysql-gh-chart/
- helm repo update
- helm install wordpress-mysql wpmHelm/wpm

if everything is in order you should see :
NAME: wordpress-mysql
LAST DEPLOYED: Mon Feb 10 20:48:40 2020
NAMESPACE: default
STATUS: deployed
REVISION: 1
NOTES:
1. Get the application URL by running these commands:
  export POD_NAME=$(kubectl get pods --namespace default -l "app.kubernetes.io/name=wpm,app.kubernetes.io/instance=wordpress-mysql" -o jsonpath="{.items[0].metadata.name}")
  echo "Visit http://127.0.0.1:8080 to use your application"
  kubectl --namespace default port-forward $POD_NAME 8080:80

