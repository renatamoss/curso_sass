<template>
  <div class="home">
    <div class="banner">
      <h1 class="banner__title">O que é SASS ?</h1>
      <p class="banner__tex">
        Pré-processadores são programas que permitem gerar CSS a partir de
        determinada sintaxe. Existem diversos pré-processadores, sendo que a
        maioria deles permite adicionar funções que não são possíveis em CSS
        puro, como *mixins, nesting, seletores, herança*, etc. É possível usar a
        própria sintaxe CSS mas também podemos escrever a folha de estilo com
        algumas particularidades, como não usar chaves e colocar elementos
        dentro um do outro, criando o *nesting*. Essas funções facilitam a
        manutenção e aumentam a legibilidade do CSS.
      </p>
    </div>

    <div class="topics">
      <ul class="topics__list">
        <li class="topics__item topics__background">
          É necessário ter um pacote instalado para compilar o Sass, como gulp
          ou npm.
        </li>
        <li class="topics__item">
          Os arquivos que usam Sass têm uma extensão diferente do CSS, sendo
          .sass ou .scss.
        </li>
        <li class="topics__item topics__background">
          Usando o Sass, é possível implementar funções, variáveis e lógica de
          programação.
        </li>
        <li class="topics__item">
          Para criar variáveis usa-se o símbolo $, junto dele o nome da
          variável, e depois dos dois pontos o valor. E para usá-las
          simplesmente chama-se o seu nome.
        </li>
        <li class="topics__item topics__background">
          Usar o “.css” ou o “.sass”, vai de acordo com a escolha do
          desenvolvedor, os dois permitem que usar todas as funções, variáveis e
          funcionalidades que o Sass proporciona, a única diferença é a escrita,
          tirando as chaves e usando a identação.
        </li>
        <li class="topics__item">
          O que é Nesting? A tradução literal de Nesting é “aninhamento”, assim,
          ele permite colocarmos elementos um dentro do outro, evitando a
          repetição, facilitando na manutenção e deixando o código CSS mais
          curto.
        </li>

        <li class="topics__item topics__background">
          Como usar o Parent Selector? O Parent Selector é um seletor & que
          permite referenciar o elemento “pai”. Sendo possível adicionar
          pseudo-classes como &:hover, pseudo_elementos como &:before, e também
          sufixos para as classes. No CSS uma classe que seria: .component
          .component__text {}, no Sass fica: .component { &__text {} }.
        </li>

        <li class="topics__item">
          O que é Interpolação e como fazê-lo? Interpolação é usada para injetar
          valores em expressões como variáveis e funções nos nossos seletores.
          Isso pode ser muito útil ao se passar parâmetros que podem ser
          alterados.
        </li>
        <li class="topics__item topics__background">
          O Placeholder Selector é um tipo especial de seletor que é bem
          parecido com um seletor convencional mas com um *%* na frente e ele
          também não é exibido no arquivo CSS após ser compilado.
        </li>

        <li class="topics__item">
          Da mesma maneira que uma variável ou uma função, os mixins precisam de
          um nome para ter uma referência e poderem ser chamados quando forem
          utilizados. Também usa-se os mixins para o Design responsivo,
          adicionando **Media queries**. Depois de ser criado, para o mixin ser
          utilizado ele precisa ser chamado pelo *@include* e pelo nome que foi
          dado.
        </li>

        <li class="topics__item topics__background">
          As funções no Sass permitem definir operações complexas que podem ser
          reutilizadas em todo o projeto, facilitando abstração de
          comportamentos em comum.
        </li>
        <li class="topics__item">
          Pode-se abstrair o CSS, deixando ele separado para cada uma das
          páginas. Dessa maneira a manutenção fica mais fácil e, para os CSS
          abstraídos funcionarem, usa-se o *@import*, que importa os arquivos
          dentro de um principal.
        </li>
      </ul>
    </div>

    <div class="img">
      <img
        class="img__logo"
        src="../../../public/img/logo-sass.svg"
        alt="Logo Sass"
      />
      <img
        class="img__glass"
        src="../../../public/img/glass-sass.svg"
        alt="Glass Sass"
      />
    </div>

    <footer class="footer">
      <p>Curso de Sass - 2021</p>
    </footer>
  </div>
</template>

<script>
export default {
  name: "Home",

};
</script>

<style >

 /* src="./style.scs" lang="scss" */

</style>