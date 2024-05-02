
# Kubernetes 📝  
Este repositório é para subir uma aplicação em Kubernetes utilizando o Google Kubernetes Engine (GKE) 


## Aplicação
Este projeto foi criado especialmente para ser utilizado no Github Action projeto [tc-2023](https://github.com/devair/tc-2023)

      

## Deployment  

Para realizar o deploy desta aplicação é necessário que tenha uma infraestrutura com os seguintes recursos:

- Google Kubernetes Engine (GKE)
- Instância de Postgres criada no Google Cloud SQL 


```bash
  npm run deploy
```  

## Documentation  
- [Estrutura de Deployment](https://github.com/GoogleCloudPlatform/cloud-sql-proxy/blob/main/examples/k8s-sidecar/no_proxy_private_ip.yaml)  
