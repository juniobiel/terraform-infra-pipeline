# terraform-infra-pipeline
Repositório de estudo para criação de CI com Terraform e Github Actions

# Tópicos importantes

## Configuração do lock
Cria-se uma instância de Lock que é uma tabela do dynamoDB para poder ter todas as alterações da pipeline _lockadas_ e armazenadas.

A chave de partição precisa ser `LockID` e está é a única configuração necessária.

## Configuração do statefile
Um _statefile_ é gerado à cada novo deploy da infraestrutura, independentemente do ambiente.

Aqui, é feito a configuração de um S3 bucket com a finalidade de persistir esses arquivos.


## Créditos
Video do canal: [Build and Run](https://www.youtube.com/watch?v=1TNAUW7_bC0)