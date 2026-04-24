# TechNova - Landing Page

Landing page institucional de uma startup de Inteligência Artificial, desenvolvida com HTML5, CSS3 e Bootstrap 5. Apresenta serviços, missão e formulário de contato com consentimento de dados.

---

## Índice

- [Sobre o Projeto](#-sobre-o-projeto)
- [Páginas e Seções](#-páginas-e-seções)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Destaques Técnicos](#-destaques-técnicos)
- [Como Executar](#-como-executar)

---

## Sobre o Projeto

A **TechNova** é uma startup fictícia especializada em soluções de Inteligência Artificial. Esta landing page foi desenvolvida como projeto prático de front-end, com foco em boas práticas de HTML semântico, responsividade via Bootstrap 5 e experiência de navegação com scroll suave.

O projeto conta com uma página principal de apresentação da empresa e uma página de contato com formulário e política de consentimento de dados (LGPD-friendly).

---

## Páginas e Seções

### `index.html` — Página Principal

| Seção | Descrição |
|---|---|
| **Navbar** | Barra de navegação fixa, escura e responsiva com menu hambúrguer para mobile |
| **Hero** | Banner de destaque com gradiente azul/roxo, título, subtítulo e imagem de capa |
| **Quem Somos** | Descrição da empresa e sua missão com IA |
| **Nossos Serviços** | Cards com os 3 serviços: Análise de Dados, Automação Inteligente e Consultoria em IA |
| **Vídeo** | Player de vídeo incorporado apresentando a missão da empresa |
| **Contato** | CTA (call-to-action) com botão direcionando ao formulário de contato |
| **Rodapé** | Copyright e créditos da empresa |

### `contato.html` — Formulário de Contato

Formulário com validação nativa (`required`) contendo os campos:

- **Nome** (texto)
- **E-mail** (formato de e-mail validado pelo browser)
- **Telefone** (campo `tel`)
- **Consentimento de dados** (checkbox obrigatório, alinhado à LGPD)
- Botão de envio e link de retorno à página inicial

---

## Estrutura do Projeto

```
landing-page-tech-nova/
│
├── index.html       # Página principal da landing page
├── contato.html     # Página de formulário de contato
└── style.css        # Estilos customizados (complementares ao Bootstrap)
```

---

## Tecnologias Utilizadas

| Tecnologia | Versão | Uso |
|---|---|---|
| **HTML5** | — | Estrutura semântica das páginas |
| **CSS3** | — | Estilização customizada: hero gradient, scroll suave, espaçamentos |
| **Bootstrap** | 5.3.3 | Layout responsivo, navbar, cards, formulário e utilitários |

As dependências do Bootstrap (CSS e JS Bundle) são carregadas via **CDN jsDelivr**, sem necessidade de instalação local.

---

## Destaques Técnicos

- **Scroll suave** (`scroll-behavior: smooth`) para navegação entre âncoras
- **Navbar fixa** (`fixed-top`) com colapso automático em telas menores via Bootstrap
- **Hero section** com gradiente CSS (`linear-gradient`) cobrindo a tela inteira (`min-height: 100vh`)
- **`scroll-margin-top`** nas seções para compensar o deslocamento da navbar fixa ao usar âncoras
- **Layout de cards** com `row` e `col-md-4` do Bootstrap para a seção de serviços
- **Formulário com validação nativa** via atributo `required` em todos os campos
- **Responsividade total** — sem media queries manuais, aproveitando o grid e utilitários do Bootstrap

---

## Como Executar

Por ser um projeto estático (HTML/CSS puro + CDN), não requer instalação.

**Opção 1 — Abrir diretamente no navegador:**

1. Clone ou baixe o repositório:
   ```bash
   git clone https://github.com/seu-usuario/landing-page-tech-nova.git
   ```
2. Abra o arquivo `index.html` diretamente no navegador.

**Opção 2 — Live Server (recomendado para desenvolvimento):**

1. Instale a extensão [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) no VS Code.
2. Clique com o botão direito em `index.html` → **"Open with Live Server"**.

> 💡 A conexão com a internet é necessária para carregar o Bootstrap via CDN e a imagem de placeholder do hero.
