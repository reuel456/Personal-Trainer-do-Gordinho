# 📘 CSS Flexbox: Documentação & Boas Práticas

Uma documentação técnica dedicada ao estudo e aplicação do **CSS Flexible Box Layout** (Flexbox).

---

## 📐 Módulo CSS Flexbox

O Flexbox é um modelo de layout unidimensional projetado para distribuição de espaço entre elementos e alinhamento avançado de componentes em interfaces web responsivas.

### ⚙️ Habilitação do Contexto Flex

Para iniciar um contexto de formação Flexbox, declare a propriedade `display` no elemento container:

```css
.flex-container {
  display: flex;
}
```

### 🎛️ Propriedades do Elemento Pai (Flex Container)

| Propriedade | Descrição | Valores Principais |
| :--- | :--- | :--- |
| **`flex-direction`** | Define o eixo principal de alinhamento dos itens. | `row` *(padrão)* \| `column` \| `row-reverse` \| `column-reverse` |
| **`justify-content`** | Distribui o espaço extra ao longo do eixo principal. | `flex-start` \| `center` \| `flex-end` \| `space-between` \| `space-around` \| `space-evenly` |
| **`align-items`** | Controla o alinhamento dos itens no eixo cruzado (perpendicular). | `stretch` *(padrão)* \| `flex-start` \| `center` \| `flex-end` \| `baseline` |
| **`flex-wrap`** | Define se os itens devem quebrar linha caso excedam a largura. | `nowrap` *(padrão)* \| `wrap` \| `wrap-reverse` |
| **`gap`** | Define o espaçamento simplificado entre as linhas/colunas. | *Ex:* `16px`, `1.5rem` |

### 🧩 Propriedades dos Elementos Filhos (Flex Items)

- **`flex-grow`**: Define o fator de expansão do item em relação ao espaço sobressalente (*default: `0`*).
- **`flex-shrink`**: Define a capacidade de encolhimento do item quando o espaço é insuficiente (*default: `1`*).
- **`flex-basis`**: Determina o tamanho base inicial do item antes da distribuição do espaço restante (*Ex: `250px`, `auto`*).
- **`align-self`**: Sobrescreve o alinhamento individual definido por `align-items` no container.

---

## 💻 Casos de Uso Comuns

### A. Centralização Bidimensional Absoluta
```css
.hero-container {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
}
```

### B. Barra de Navegação Distribuída
```css
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
}
```
