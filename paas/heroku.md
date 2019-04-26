# Heroku

O Heroku é uma plataforma como serviço na nuvem que suporta várias linguagens de programação.  

*Obs: A versão gratuita não é indicada para produção, é indicado a versão paga para a produção.*

## Documentação e Acesso ao Serviço

Clique [aqui](https://www.heroku.com) para ver a documentação e acessar o serviço.

## Criar um app

Para criar um app no Heroku siga os seguintes procedimentos:

- Acesse o site do Heroku

- Crie uma conta

- No `Dashboard`, clique em `New` e `Create new app`

- Dê um nome e crie o app

- Na aba `Deploy`:

  - Em `Deployment method`, selecione o `GitHub` e faça o login

  - Em `App connected to GitHub`, digite o repositório para procurar e conecte nele

  - Em `Automatic deploys`, é possível alterar a branch para o deploy

- Na aba `Settings`:

  - Em `Config Vars`, clique em `Reveal Config Vars`

  - Configure as variáveis de ambiente passando chave e valor. Ex: Mongodb, e-mail e outros

  - Configure também a variável de chave `PORT` e valor `80`

- Na aba `Deploy`:

  - Em `Manual deploy`, clique em `Deploy Branch`

  - Depois de terminar a build, clique no botão `View` que aparecerá e copie a url

  - Em `Automatic deploys`, clique em `Enable Automatic Deploys` (este botão realiza somente o deploy, não realiza a integração contínua).

É possível substituir o nome estranho da url por um domínio próprio, mas tem que ter o plano pago do Heroku, caso tenha, siga os seguintes procedimentos:

- Na aba `Settings`, em `Domains and certificates`, clique em `Add domain`

- Digite o nome do domínio e clique em `Save changes`.