# aula-git-flow
aula git flow linux tips
https://www.youtube.com/watch?v=dJjVr6Ya7B8&t=1819s

git flow - estabele um fluxo de entrega

branches:
main - pricipal
develop - dev
feature branch
release branch
hotfix

git flow init (inicia a configuração de definição das branches)
git flow feature start <nome_feature> ex: feature/12345 obs: executar dentro da feature main (produção)
git flow feature finish <nome_feature> obs: finaliza entrega para testes
git flow feature publish <nome_feature>  obs: publica para que outros devs possam atuar


