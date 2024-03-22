*O que é docker?*
O docker é uma plataforma aberta, para facilitar o desenvolvimento. Tendo o mais próximo um ambiente de produção e testes. Criado para disponibilizar uma aplicação da forma mais rápida e leve possível.

![[dockerxvm.png]]

O Docker utiliza somente o necessário de um sistema operacional para rodar uma aplicação. Na VM é virtualizado um ambiente inteiro.

*Containers*
São ambientes isolados contendo um conjunto de processos a partir de uma image. Eles compartilham do mesmo kernel do SO, mas seu processo é isolado do restante do sistema.

*Images*
As imagens são compostas por sistemas de arquivos de camadas que ficam uma sobre a outra.
EX: Posso pegar uma imagem do ubuntu e com base nessa imagem construir uma aplicação.

*Container x Image*
O Container é iniciado a partir de uma image, ou seja, nunca temos uma image em execução, mas sim um container. A image é a base do container.

## Por que usar docker?
A implantação do aplicativo é mais rápida;
Controle de versão de images;
Reversibilidade;
*Unificação de ambiente de desenvolvimento, QA e produção;*
Não deixa a diferença do ambiente do cliente afetar a usabilidade do aplicativo.

## Configurando o PostgreSQL no docker
Iremos montar um compose para subir o PostgreSQL.