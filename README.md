# Propriedade Grid do CSS

## Sumário
- [Descrição](#descrição)
- [Funcionalidades Principais](#funcionalidades-principais)
- [Exemplo de Uso Básico](#exemplo-de-uso-básico)
- [Recursos Adicionais](#recursos-adicionais)
- [Compatibilidade do Navegador](#compatibilidade-do-navegador)
- [Conclusão](#conclusão)

## Descrição

A propriedade `grid` do CSS é uma poderosa ferramenta para criar layouts complexos e responsivos em páginas da web. Ela permite organizar elementos em linhas e colunas, facilitando o design de interfaces flexíveis e adaptáveis a diferentes tamanhos de tela e dispositivos.

## Funcionalidades Principais

- **Grid Container**: Define um contexto de grid para os elementos filhos.
- **Grid Items**: Elementos filho dentro do grid container que são organizados em linhas e colunas.
- **Linhas e Colunas**: A propriedade `grid` permite definir o número e a largura das linhas e colunas do grid.
- **Espaçamento**: Controle preciso sobre o espaçamento entre as linhas e colunas do grid.
- **Alinhamento**: Possibilidade de alinhar os itens dentro das células do grid, tanto vertical quanto horizontalmente.
- **Responsividade**: O grid se adapta automaticamente a diferentes tamanhos de tela, tornando o layout responsivo.

## Recursos Adicionais

- **Grid Template Areas**:  Permite definir áreas nomeadas dentro do grid para um controle mais intuitivo do layout.
- **Grid Template Rows e Columns**: Fornece uma maneira flexível de definir o tamanho e o comportamento das linhas e colunas.
- **Grid Implícito**: Elementos que não são explicitamente colocados em uma célula do grid podem ser posicionados automaticamente com base em regras de layout predefinidas.
- **Alinhamento de Conteúdo**: Além do alinhamento dos itens dentro das células, é possível alinhar o conteúdo do grid container dentro de seu espaço.

## Compatibilidade do Navegador

A propriedade grid é amplamente suportada pelos navegadores modernos, mas é importante verificar a compatibilidade com versões mais antigas, especialmente se o suporte para navegadores mais antigos for necessário.

## Exemplo de Uso Básico

```css
HTML->
<div class="container">
  <div class="item cabecalho">Cabeçalho</div>
  <div class="item menu-lateral">Menu Lateral</div>
  <div class="item principal">Conteúdo Principal</div>
  <div class="item rodape">Rodapé</div>
</div>

CSS->
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

body {
  background-color: #01080e;
  color: #dadde0;
  padding: 50px 50px 0 50px;
  font-size: 2rem;
}

.container {
  display: grid;
  grid-template-columns: 1fr 3fr;
  grid-template-rows: 200px 500px 200px;
  grid-template-areas:
    "cabecalho cabecalho cabecalho"
    "menu-lateral principal principal"
    "rodape rodape rodape";
}

.cabecalho {
  grid-area: cabecalho;
}

.menu-lateral {
  grid-area: menu-lateral;
}

.principal {
  grid-area: principal;
}

.rodape {
  grid-area: rodape;
}

.item {
  border: 1px solid #00f4bf;
  text-align: center;
  font-size: 1.25em;
  font-weight: normal;
}
```
## Conclusão

A propriedade grid do CSS oferece uma abordagem flexível e poderosa para criar layouts complexos e responsivos em páginas da web. Com recursos avançados de controle de posicionamento, alinhamento e espaçamento, o grid se tornou uma ferramenta essencial para desenvolvedores front-end na criação de interfaces web modernas e adaptáveis.



