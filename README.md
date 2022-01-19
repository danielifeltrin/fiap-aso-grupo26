# fiap-aso-grupo26

## TODOS OS ARQUIVOS ESTÃO CONFIGURADOS PARA UTILIZAR O NAMESPACE mbaaso-grupo26
PARA CRIAR O PROJETO EXECUTAR O COMANDO ABAIXO:

oc new-project mbaaso-grupo26

### COMANDOS PARA SUBIR O BD, APLICAÇÃO E TODAS AS DEPENDÊNCIAS:

- ImageStream para salvar a imagem que será gerada:

oc create -f imagestream.yml


- BuildConfig para gerar a imagem a partir do git:

oc create -f buildconfig.yml

- Secret para armazenar os dados de acesso ao BD:

oc create -f secret.yml

- DeploymentConfig e Service do BD: 

oc create -f db-deploymentconfig.yml

oc create -f db-service.yml

- DeploymentConfig, HPA, Service e Route da aplicação: 

oc create -f deploymentconfig.yml

oc create -f hpa.yml

oc create -f service.yml

oc create -f route.yml

------------------------
### O arquivo full.yml contem todos os componentes



