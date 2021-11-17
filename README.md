## Repositório para hospedagem de aulas e exercícios de **SASS**.

### Instalação escopo global:
```
npm install -g sass

```

### Configurando o VUE JS para o SASS:
```
npm install node-sass sass-loader --save-dev
```

### Comando que assiste o código e compila automaticamente:
```
sass --watch scss/style.scss:css/style.css
```



![img_sass](https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/sass/sass.png)

### O que é SASS ?

Pré-processadores são programas que permitem gerar CSS a partir de determinada sintaxe. Existem diversos pré-processadores, sendo que a maioria deles permite adicionar funções que não são possíveis em CSS puro, como *mixins, nesting, seletores, herança*, etc. É possível usar a própria sintaxe CSS mas também podemos escrever a folha de estilo com algumas particularidades, como não usar chaves e colocar elementos dentro um do outro, criando o *nesting*. Essas funções facilitam a manutenção e aumentam a legibilidade do CSS.

* É necessário ter um pacote instalado para compilar o Sass, como *npm*.

* Os arquivos que usam Sass têm uma extensão diferente do CSS, sendo *.sass* ou *.scss.*

* Usando o Sass, é possível implementar *funções, variáveis e lógica de programação.*
  
* Para criar variáveis usa-se o símbolo *$*, junto dele o nome da variável, e depois dos dois pontos o valor. E para usá-las simplesmente chama-se o seu nome. 

*  Usar o *“.css”* ou o *“.sass”*, vai de acordo com a escolha do desenvolvedor, os dois permitem que usar todas as *funções, variáveis e funcionalidades* que o Sass proporciona, a única diferença é a escrita, tirando as chaves e usando a identação.
  
  ### Conceitos Importantes:
  
- [x] **Nesting:** A tradução literal de Nesting é “aninhamento”, assim, ele permite colocar elementos um dentro do outro, evitando a repetição, facilitando na manutenção e deixando o código CSS mais curto.

- [x] **Parent Selector:** é um seletor *&* que permite referenciar o elemento “pai”. Sendo possível adicionar pseudo-classes como *&:hover*, pseudo_elementos como *&:before*, e também sufixos para as classes. No CSS uma classe que seria: *.component .component__text {}*, no Sass fica: *.component { &__text {} }*.

- [x] **Interpolação:** é usada para injetar valores em expressões como variáveis e funções nos nossos seletores. Isso pode ser muito útil ao se passar parâmetros que podem ser alterados. Exemplo de interpolação: *width: calc(900px - #{$size-img});*
  
- [x] **Placeholder Selector (%) e Extend:** é um tipo especial de seletor que é bem parecido com um seletor convencional, mas com um *%* na frente. Ele também não é exibido no arquivo CSS após ser compilado.
  
- [x] **Mixin:** Mixins permitem definir estilos que podem ser reutilizados, e isso evita o uso de classes repetitivas e não semânticas, e também distribui coleções de estilo para bibliotecas. Da mesma maneira que uma variável ou uma função, os mixins precisam de um nome para ter uma referência e poderem ser chamados quando forem utilizados. Também usa-se os mixins para o Design responsivo, adicionando **Media queries**. Depois de ser criado, para o mixin ser utilizado, ele precisa ser chamado pelo *@include* e pelo nome que foi dado.

- [x]  **Funções no Sass:** As funções no Sass permitem definir operações complexas que podem ser reutilizadas em todo o projeto, facilitando abstração de comportamentos em comum.

- [X] **Importar arquivos no Sass:** Pode-se abstrair o CSS, deixando ele separado para cada uma das páginas. Dessa maneira a manutenção fica mais fácil e, para os CSS abstraídos funcionarem, usa-se o *@import*, que importa os arquivos dentro de um principal.

- [X] **Iterações no Sass:** Como em outras linguagens de programação, é possível fazer iterações no Sass com *for, each ou while* usando os At Rules.
- [X] **Condicionais no Sass com valores (ex: boolean):** Pode-se fazer condicionais no Sass com *@if, @else if e @else*, para atribuir determinado trecho de estilo dependendo de uma condição específica.
- [X] **While no Sass:** O while também funciona com at rule, ficando *@while <expression> { ... }*. Ele valida se a expressão é verdadeira, e enquanto ela for válida, ele irá executar o trecho de código contido entre as chaves.
  

*Anotações feitas no Curso de Sass: O CSS com superpoderes - 11/2021*

















