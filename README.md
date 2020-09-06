## Ferramentas

- minikube
  - status
  - start

- kubectl
  - cluster-info
  - apply -f **/path/to/file.yml** cria o pod conforme arquivo de configuração
  - get
    - pods
    - services
  - set image [tipo-do-objeto]/[nome-do-objeto] [nome-do-container]=[nome-da-imagem]
  - create
    - secret generic [secret-name] --from-literal key=value

## Registry
docker run -d -p 1234:5000 --restart always --name registry registry:2

Visualizar containers do kubernetes no terminal aberto
eval $(minikube docker-env)