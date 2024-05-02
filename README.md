
# Kubernetes 📝  
Este repositório é para subir uma aplicação em Kubernetes utilizando o Google Kubernetes Engine (GKE) 


## Aplicação
Este projeto foi criado especialmente para ser utilizado no Github Action do projeto [tc-2023](https://github.com/devair/tc-2023), logo para rodar localmente é necessário conhecimento prévio em Docker, Kubernetes e seguir a documentação do Minikube para esta finalidade.
      

## Deployment no GKE  

Para realizar o deploy desta aplicação é necessário que tenha uma infraestrutura com os seguintes recursos:

- Google Kubernetes Engine (GKE)
- Instância de Postgres criada no Google Cloud SQL 

a) Estar autorizad a utilizar o gcloud localmente
```bash
  gcloud init
```

```bash
  gcloud auth login
```

b) Acessar o cluster GKE do projeto
```bash
  gcloud container clusters get-credentials <CLUSTER_NAME> --zone <REGION> --project <PROJECT_ID>
```

c) Implantar a aplicação
```bash
  kubectl apply -f .
```

## Deployment localmente
Para rodar localmente é necessário realizar algumas alterações nos arquivos .yaml.

### Requistos
1. Docker Engine instalado com o Kubernetes ativado
2. Minikube instalado
3. Ter uma instância do Postgres em execução

Considerando que os recursos necessário estão instalados localmente, execute o comando abaixo para implantar a aplicação
```bash
  kubectl apply -f .
```
## Documentação de referência  
- [Autorizar a CLI gcloud](https://cloud.google.com/sdk/docs/authorizing?hl=pt-br)
- [Learn Kubernetes Basics](https://kubernetes.io/docs/tutorials/kubernetes-basics)
- [Install Docker Engine](https://docs.docker.com/engine/install/)
- [Minikube start](https://minikube.sigs.k8s.io/docs/start/)

