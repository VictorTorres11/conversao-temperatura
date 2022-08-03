<h3>Criando imagem<br></h3>
cd ./src<br>
docker build -t vtmolina011/conversao-temperatura:v1 .<br>

<h3>Criando container<br></h3>
docker container run -d --name api -p 8080:8080 kubedev/api-conversao-temperatura:v1<br>

<h3>vvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvCriando K8S<br></h3>
cd ./src/k8s<br>
kubectl create -f deployment.yaml
