Utilizaremos o Git para controle de versionamento de codigo.

Foi criado pela comunidade.

# Primeiros passos

- Iremos adicionar sua identidade do git;
Comandos: 
$ git config --global user.name "Gabriel Godoy"
$ git config --global user.email bardini52@gmail.com

Entramos no repositorio local e iniciamos com o comando:
git init.

Isso ira criar o diretorio .git

Utilizamos o git add para adicionar os arquivos a serem commitados.
A syntaxe do comando é bem simples:

## Para adicionar um arquivo:
$ git add nomearquivo

ou

Para adicionar todos os arquivos (não recomendados pois normalmente alguns arquivos como o vendor não são versionados):
$ git add .

O comando git add adiciona os arquivos no stage área, que é onde os arquivos ficam antes de serem commitados.

## Status Git
O seguinte comando é utilizado para verificar o status do git do repositório atual (mudanças, o que precisa ser commitado, etc):
$ git status

## Stage Area
O Stage Area acompanha e observa as mudanças dos arquivos.

## Commit
Usamos o commit para perssistir as mudanças, e colocamos uma mensagem curta e objetiva do que foi alterado.
$ git commit -m

A partir de então, as alterações serão rastreadas.

## Log
Para verificarmos todos os commits realizados no projeto podemos utilizar o git log:
$ git log
## Verificar diferenças
Com o comando git status conseguimos verificar as alterações, mas não sabemos quais são elas.

Utilizamos o suguinte comando para verificar as alterações dos arquivos com base do que foi alterado no stage area:
$ git diff

Para persistimos essas alterações, seguimos usando o git add para adicionar à stage area a ser commitada. Após usar o git add, o arquivo não aparecerá mais no git diff.

$ git add arquivo-a-ser-alterado.html

## Branchs
Quando formos trabalhar em uma nova melhoria, utilizamos as branchs. As branchs são como se fossem ramificações. As pessoas trabalham naquela branch e ao finalizar é juntado à linha principal.

Iremos criar um ramo para a seção about para modificações.

### Comando para verificar branch atual:
$ git branch

### Comando para criar uma nova branch:
$ git branch nome-nova-branch

### Comando para alterar de branch:
$ git checkout nome-da-branch

De exemplo usaremos a branch sessao-sobre
$ git branch sessao-sobre
$ git checkout sessao-sobre

Modificando arquivos, após:
Verificar status
$ git status 

Verificar diferenças
$ git diff

Persistir as modificações:
$ git add arquivo-modificado.html
$ git commit -m "Atualizado sessao sobre"

Se você voltar para a branch master, você verá que as modificações não estão presentes.
$ git checkout master

Criaremos uma branch para correção de um bug apareceu:
$ git branch bug-fix
$ git checkout bug-fix

(O ramo criando do bug-fix, levou em consideração a branch master, e não a sessao-sobre)

Após arrumar o bug, verificar o git status, git diff.
Logo em seguida:

$ git add arquivo-corrigido.html
$ git status
$ git commit -m "Arrumado bug-fix"
(Atenção, mesmo que você commite dentro da branch os arquivos modificados, ela não subira para a branch master)

$ git checkout master

### Agora faremos o merge das branchs
$ git merge bug-fix

### Após o merge, podemos deletar a branch
$ git branch -d bug-fix

Podemos voltar na branch da sessão sobre que estávamos trabalhando anteriormente.
$ git checkout sessao-sobre

Após finalizarmos nossas alterações nessa branch, adicionarmos ao stage area com o git add e commitarmos com o git commit, voltamos à branch master para fazermos o merge.
$ git checkout master
$ git merge sessao-sobre

Novamente, agora poderemos deletar o ramo que acabamos de fazer o merge.
$ git branch -d sessao-sobre

[[13 - LEITURA VERSIONAMENTO DE CODIGO]]