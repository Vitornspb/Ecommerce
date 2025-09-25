# ⚡ VN Tech | Sua Loja de Tecnologia

Uma loja de e-commerce de tecnologia responsiva e moderna, construída com foco em **HTML, CSS e JavaScript Vanilla**. Este projeto simula um catálogo de produtos com funcionalidades básicas de **filtragem por categoria** e **pesquisa por nome**.

## ✨ Funcionalidades

* **Design Responsivo:** Layout adaptável para diferentes tamanhos de tela.
* **Menu de Categorias:** Filtragem de produtos instantânea por categorias (Smartphones, Notebooks, Fones, etc.).
* **Barra de Busca:** Pesquisa dinâmica de produtos pelo nome (ativada ao apertar Enter ou clicar na lupa).
* **Layout Moderno:** Interface visual com tema escuro na navegação e cores de destaque vibrantes.
* **Hero Section:** Destaque para promoções (ex: Black Friday Antecipada).
* **Acessibilidade:** Uso de atributos `aria-label` e `aria-hidden` para elementos de ícones.

---

## 🛠️ Tecnologias Utilizadas

O projeto foi construído utilizando as bases do desenvolvimento web:

* **HTML5:** Estrutura semântica da página.
* **CSS3:** Estilização e layout (arquivo `style.css`).
    * Uso de **variáveis CSS** (`:root`) para cores.
    * Layouts com **Flexbox** e **CSS Grid** (para o container de produtos).
* **JavaScript (Vanilla JS):** Lógica de filtragem, busca e renderização dos cartões de produtos (arquivo `script.js`).
* **Font Awesome:** Biblioteca de ícones (via CDN).

---

## 🚀 Como Executar o Projeto

É muito simples visualizar e testar o projeto:

1.  **Baixe os Arquivos:** Certifique-se de ter os arquivos `index.html`, `style.css` e `script.js` na mesma pasta.
2.  **Abra no Navegador:** Dê um duplo clique no arquivo **`index.html`** para abri-lo em qualquer navegador moderno (Chrome, Firefox, Edge, etc.).

O JavaScript será executado automaticamente, carregando a lista inicial de produtos.

## ⚙️ Uso do JavaScript (`script.js`)

O arquivo `script.js` é o núcleo da aplicação e gerencia todo o catálogo de produtos:

1.  **Dados:** A lista de produtos (`let produtos = [...]`) está definida como um *array* no topo do arquivo.
2.  **Filtragem e Busca:** As funções `trocarCategoria()` e `pesquisar()` trabalham juntas com a função principal `mostrarProdutos()` para filtrar o *array* de produtos em tempo real, verificando o nome e a categoria.
3.  **Performance:** O script inicializa o carregamento dos produtos apenas após o evento `DOMContentLoaded`, garantindo que a página esteja pronta.

---

## 🎨 Personalização

### Cores Principais (via `style.css`)

Você pode alterar rapidamente o esquema de cores modificando as variáveis CSS na seção `:root` do arquivo `style.css`:

```css
:root {
    --primary-color: #FF4111;    /* Cor de destaque principal (Ex: raio, botões ativos) */
    --secondary-color: #2C3E50;  /* Cor de fundo secundária (Ex: barra de categorias, footer) */
    --accent-color: #3498DB;     /* Cor de botões de ação (Ex: "Ver Detalhes") */
    /* ...outras variáveis */
}
