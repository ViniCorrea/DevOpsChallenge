| Build | Release QA | Release Production | 
| :-----: | :-----: | :-----: |
| ![Build Status](https://viniciuscorrea.visualstudio.com/DevOpsChallenge/_apis/build/status/DevOpsChallenge?branchName=master)  | ![Relase QA](https://viniciuscorrea.vsrm.visualstudio.com/_apis/public/Release/badge/deeb99ad-f4ab-4d04-915b-f8739ba18a4f/1/1) | ![Relase PROD](https://viniciuscorrea.vsrm.visualstudio.com/_apis/public/Release/badge/deeb99ad-f4ab-4d04-915b-f8739ba18a4f/1/3) |

# Passo a Passo

1 - Garantir que o projeto estava em pleno funcionamento.
* Foi necessário a correção de alguns testes unitário.

2 - Criação do endpoint para Health Check

3 - Dockerization para publicação - Feito no arquivo Dockerfile

4 - Criação de um Azure Registry para armazenamento privado de containers

5 - Criação do pipeline de publicação para Azure DevOps atráves do arquivo azure-pipelines.yml

6 - Criação de um "Azure WebApp for container Linux" em um novo Resource Group

7 - Criação de um novo Slot chamado "staging"

8 - Criação do pipeline de Release no Azure DevOps
* Preferir criar um pipeline de Release por ter uma rastreabilidade melhor
* Coloquei imagens no que fiz na pastas "/Imagens Release"

9 - Criação de um application insights com um "ping test" configurado para a url https://nibodevopschallenge.azurewebsites.net/healthcheck
* Imagem da configuração em /availability.png

# URLs

Aplicação: https://nibodevopschallenge.azurewebsites.net
Test: https://nibodevopschallenge-staging.azurewebsites.net
Health Check: https://nibodevopschallenge.azurewebsites.net/healthcheck

