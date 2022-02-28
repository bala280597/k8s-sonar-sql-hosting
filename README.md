# k8s-sonar-sql-hosting
1) Clone this repo using git clone command.
2) For SQL, create resource from manifest file using kubectl command.
3) For SQL connection, kubectl exec -it mysql-0 -n sql -- mysql -u root -p
4) For sonar,
    1) helm repo add sonarqube https://SonarSource.github.io/helm-chart-sonarqube
    2) kubectl create namespace sonarqube.
    3) helm repo update.
    4) helm upgrade --install -n sonarqube sonarqube sonarqube/sonarqube
    5) Delete service and create service from sonar repo.

