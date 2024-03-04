O GitHub é uma plataforma baseada em git, uma das mais utilizadas hoje em dia.
Fornece um serviço de publicação de sites estáticos.

Na aula é ensinado a criar uma conta no GitHub.

Precisamos criar um projeto no GitHub para armazenar nosso projeto local.

A sua página inicial do GitHub é editável, pesquisar sobre depois caso queira personalizar ele.

## Criação de repositórios

Repositórios > New

Principais informações:
*Nome do projeto*
*Public / Private*
*Add README file*
*Add .gitinore*
*License*

Após criar o repositório, o próprio GitHub irá falar o que fazer em seguida.
Ele irá te passar os comandos.
Como já temos um projeto, precisamos fazer um push do nosso projeto para o GitHub.

Dentro de nosso projeto temos o diretório .git, que é o diretório que armazena todas as configurações e versionamento de nosso projeto.

Para visualizar o conteúdo de configuração:

(Dentro do projeto)
$ cat .git/config

Comandos para o push estão no GitHub, mas seguida uma palinha. Dentro do projeto no terminal, executar os seguintes comandos:

$ git remote add origin https://github.com/gbardini/bootstrap-first-project.git

Você pode verificar a configuração do repositório dentro de:
$ cat .git/config

Para enviarmos nosso projeto e modificações ao repositório, usamos o git push.

$ git push origin master

Se atente ao usar o nome da branch.

## GitHub Pages

Na documentação do GitHub https://docs.github.com/pt
É disponibilizado uma infinadade de ferramentas.
Dentre elas há o GitHub Pages, que permite a hospedagem de um site no servidor deles de forma gratuita.
(Usar sites estáticos, que são sites sem o backend {html, css e javascript}).

Para a publicação do seu projeto no GitHub Pages você precisa acessar as configurações dentro do seu projeto no site do GitHub.

Dentro das configurações, acessar a opção "Pages".
É solicitado qual ferramenta utilizar para publicação (Actions ou Branchs).
Vamos utilizar a opção de publicar a partir de uma branch (definir sua branch master).

Temos a opção de inserir um domínio customizável.

Após salvar ele irá informar que seu site está ao vivo.
Normalmente o link é 
https://usuario.github.io/nome-projeto

Nesse caso:
https://gbardini.github.io/bootstrap-first-project

[[14 - LEITURA GITHUB PAGES]]