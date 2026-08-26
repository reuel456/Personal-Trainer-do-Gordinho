Markdown# 📦 Guia Completo: Flexbox no CSS & Dicas de GitHub

Este repositório contém um guia completo sobre o uso do **Flexbox** no CSS e instruções práticas de uso do **GitHub**.

---

## 🎨 Guia Prático de CSS Flexbox

O **Flexbox** (Flexible Box Layout) é um modelo unidimensional criado para alinhar, distribuir e organizar elementos em uma página web de forma responsiva.

### ⚙️ Configuração Inicial

Para ativar o Flexbox, defina a propriedade `display` no elemento pai (container):

```css
.container {
  display: flex; /* ativa o flexbox para os filhos diretos */
}
📌 Propriedades do Container (Pai)PropriedadeFunçãoValores Principaisflex-directionDefine a direção do eixo principalrow (padrão), column, row-reverse, column-reversejustify-contentAlinha os itens no eixo principalflex-start, center, flex-end, space-between, space-around, space-evenlyalign-itemsAlinha os itens no eixo cruzadostretch (padrão), flex-start, center, flex-end, baselineflex-wrapDefine se os itens quebram linhanowrap (padrão), wrap, wrap-reversegapEspaçamento entre os itensEx: 16px, 1rem🧩 Propriedades dos Itens (Filhos)flex-grow: Define o quanto o item pode crescer para ocupar o espaço livre (ex: flex-grow: 1;).flex-shrink: Define se o item pode encolher se o espaço for menor (ex: flex-shrink: 0;).flex-basis: Tamanho inicial do item antes da distribuição do espaço (ex: flex-basis: 200px;).align-self: Sobrescreve a regra align-items do container para este item específico.💡 Exemplos PráticosCentralização PerfeitaCSS.centralizado {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}
Menu de Navegação ResponsivoCSS.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
}
