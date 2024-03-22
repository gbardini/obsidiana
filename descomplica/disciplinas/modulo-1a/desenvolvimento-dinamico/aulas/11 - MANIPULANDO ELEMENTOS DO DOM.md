Toda vez que você abre uma página, é carregado o DOM
![[dom-definition.png]]
![[descomplica/disciplinas/modulo-1a/desenvolvimento-dinamico/img/dom.png]]

Conseguimos manipular os elementos, o mais difícil é encontrar esses elementos na árvore.

![[possibilidades-dom.png]]

Dado a seguinte página html:
![[html-page.png]]
Sua DOM seria:
![[descomplica/disciplinas/modulo-1a/desenvolvimento-dinamico/img/dom.png]]![[dom-parent-childs-siblings.png]]
![[dom-window.png]]

Prática:
![[pratica-um.png]]
![[pratica-dois.png]]

Para trabalharmos com numeros no prompt, temos que usar o:

Number.parseFloat(window.prompt(.....));

## Encontrando elementos do DOM
![[elements-by-tag.png]]
![[tagname.png]]

Ao procurar na DOM pela tag, ele ira trazer os resultados que são compatíveis com a tag selecionada em forma de array.
Então caso você queira interagir com um elemento específico, você teria que usar o índice como acima.

![[javascript-power.png]]

[[11 - LEITURA MANIPULANDO ELEMENTOS DO DOM]]