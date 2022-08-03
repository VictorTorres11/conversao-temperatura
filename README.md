Criando imagem
cd ./src

docker build -t vtmolina011/conversao-temperatura:v1 .

Criando container
docker container run -d --name api -p 8080:8080 kubedev/api-conversao-temperatura:v1

Criando K8S
cd ./src/k8s
kubectl create -f deployment.yaml
