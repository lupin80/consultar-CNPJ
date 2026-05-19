```markdown
<div align="center">

# 🔥 Consulta Inteligente de CNPJ

**Plataforma corporativa moderna para consulta empresarial completa via CNPJ**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Font Awesome](https://img.shields.io/badge/Font_Awesome-339AF0?style=for-the-badge&logo=fontawesome&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare_CDN-F38020?style=for-the-badge&logo=cloudflare&logoColor=white)

<br/>

[Funcionalidades](#-funcionalidades) •
[Demo](#-demo) •
[Instalação](#-instalação) •
[Tecnologias](#-tecnologias) •
[Estrutura](#-estrutura-do-projeto) •
[API](#-api-utilizada) •
[Licença](#-licença)

<br/>

<img src="https://img.shields.io/badge/status-ativo-00d26a?style=flat-square" alt="Status">
<img src="https://img.shields.io/badge/versão-2.0.0-7b2dff?style=flat-square" alt="Versão">
<img src="https://img.shields.io/badge/licença-MIT-0066ff?style=flat-square" alt="Licença">

</div>

---

## 📋 Índice

- [Sobre o Projeto](#-sobre-o-projeto)
- [Funcionalidades](#-funcionalidades)
- [Demo](#-demo)
- [Instalação](#-instalação)
- [Como Usar](#-como-usar)
- [Tecnologias](#-tecnologias)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [API Utilizada](#-api-utilizada)
- [Paleta de Cores](#-paleta-de-cores)
- [Responsividade](#-responsividade)
- [Impressão / PDF](#-impressão--pdf)
- [Performance](#-performance)
- [Contribuição](#-contribuição)
- [Licença](#-licença)
- [Autor](#-autor)

---

## 📖 Sobre o Projeto

O **Consulta Inteligente de CNPJ** é uma aplicação web **single-page** que permite consultar dados cadastrais completos de empresas brasileiras diretamente pela Receita Federal, utilizando a API pública da **CNPJ WS**.

O projeto foi desenvolvido com foco em:

- 🎨 **Design moderno** com glassmorphism e gradientes vibrantes
- ⚡ **Performance** com zero dependências JavaScript
- 📱 **Responsividade** total (mobile-first)
- 🖨️ **Geração de PDF** via impressão nativa do navegador
- ♿ **Acessibilidade** com atributos ARIA e semântica HTML5

---

## ✨ Funcionalidades

| Funcionalidade | Descrição |
|---|---|
| 🔍 **Consulta por CNPJ** | Busca completa de dados cadastrais via API pública |
| 🎭 **Máscara automática** | Formatação automática do CNPJ durante digitação (`XX.XXX.XXX/XXXX-XX`) |
| 📊 **Painel de Stats** | Barra de resumo rápido com porte, UF, data de abertura e capital social |
| 🏢 **Banner Corporativo** | Exibição destacada da razão social com badges de status |
| 👥 **Quadro Societário** | Lista completa de sócios e qualificações |
| 🏷️ **Badges Inteligentes** | Indicadores visuais de situação cadastral (Ativa/Inativa), UF e porte |
| 📄 **Geração de PDF** | Impressão otimizada com regras `@media print` dedicadas |
| ⌨️ **Atalho Enter** | Consulta disparada ao pressionar Enter no campo de busca |
| 🔄 **Loading animado** | Spinner bicolor com texto em gradiente durante a consulta |
| ⚠️ **Tratamento de erros** | Mensagens amigáveis para CNPJ inválido, não encontrado ou rate-limit |
| 🎞️ **Animações de entrada** | Cards aparecem com efeito `fadeUp` escalonado |

---

## 🖥️ Demo

### Tela Inicial
```
┌──────────────────────────────────────────────┐
│  [CNPJ]  logo animada                        │
│                                              │
│  Consulta Inteligente de Empresas            │
│  Plataforma corporativa moderna...           │
│                                              │
│  🔎 [________________] [CONSULTAR] [PDF]     │
└──────────────────────────────────────────────┘
```

### Resultado da Consulta
```
┌──────────────────────────────────────────────┐
│  🏢 Porte  📍 UF  📅 Abertura  💰 Capital   │  ← Stats Bar
│                                              │
│  ┌────────────────────────────────────────┐  │
│  │  RAZÃO SOCIAL DA EMPRESA               │  │  ← Banner
│  │  Nome Fantasia                          │  │
│  │  [✓ Ativa] [📍 SP] [🏢 ME]            │  │  ← Badges
│  └────────────────────────────────────────┘  │
│                                              │
│  ┌──────────┐ ┌──────────┐ ┌──────────┐     │
│  │ CNPJ     │ │ Situação │ │ Telefone │     │  ← Info Cards
│  └──────────┘ └──────────┘ └──────────┘     │
│  ┌──────────┐ ┌──────────┐ ┌──────────┐     │
│  │ E-mail   │ │ Capital  │ │ Natureza │     │
│  └──────────┘ └──────────┘ └──────────┘     │
│                                              │
│  ┌────────────────────────────────────────┐  │
│  │ Endereço Completo                      │  │  ← Full Width
│  └────────────────────────────────────────┘  │
│  ┌────────────────────────────────────────┐  │
│  │ Quadro Societário                      │  │  ← Full Width
│  │ 👤 Sócio 1 — Qualificação             │  │
│  │ 👤 Sócio 2 — Qualificação             │  │
│  └────────────────────────────────────────┘  │
└──────────────────────────────────────────────┘
```

---

## 🚀 Instalação

### Opção 1 — Abrir diretamente

O projeto é um **arquivo HTML único** (zero build). Basta:

```bash
# Clonar o repositório
git clone https://github.com/seu-usuario/consulta-cnpj.git

# Entrar na pasta
cd consulta-cnpj

# Abrir no navegador
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

### Opção 2 — Servidor local

```bash
# Com Python 3
python -m http.server 8000

# Com Node.js (npx)
npx serve .

# Com PHP
php -S localhost:8000
```

Acesse: `http://localhost:8000`

### Opção 3 — Deploy direto

O projeto funciona em qualquer hospedagem estática:

| Plataforma | Deploy |
|---|---|
| **GitHub Pages** | Faça push e ative nas Settings |
| **Netlify** | Arraste a pasta no painel |
| **Vercel** | `vercel --prod` |
| **Cloudflare Pages** | Conecte o repositório |

---

## 📘 Como Usar

1. **Abra** a página no navegador
2. **Digite** o CNPJ no campo de busca (a máscara formata automaticamente)
3. **Clique** em `Consultar Empresa` ou pressione `Enter`
4. **Visualize** todos os dados da empresa nos cards informativos
5. **Gere o PDF** clicando em `Gerar PDF` (abre o diálogo de impressão)

### Exemplos de CNPJ para teste

| Empresa | CNPJ |
|---|---|
| Banco do Brasil | `00.000.000/0001-91` |
| Petrobras | `33.000.167/0001-01` |
| Vale S.A. | `33.592.510/0001-54` |

> ⚠️ **Nota:** A API pública possui limite de requisições. Caso receba erro 429, aguarde alguns segundos.

---

## 🛠️ Tecnologias

### Core

| Tecnologia | Versão | Uso |
|---|---|---|
| **HTML5** | — | Estrutura semântica |
| **CSS3** | — | Estilização, animações, glassmorphism |
| **JavaScript** | ES2020+ | Lógica, fetch API, manipulação DOM |

### CDN (Cloudflare)

| Recurso | CDN | Uso |
|---|---|---|
| **Font Awesome** | `cdnjs.cloudflare.com` | Ícones vetoriais |
| **Google Fonts (Inter)** | `fonts.googleapis.com` | Tipografia |

### API

| Serviço | Endpoint | Uso |
|---|---|---|
| **CNPJ WS** | `publica.cnpj.ws/cnpj/{cnpj}` | Dados cadastrais da Receita Federal |

### Nenhuma dependência local

```
✅ Zero npm install
✅ Zero node_modules
✅ Zero build step
✅ Zero framework
```

---

## 📁 Estrutura do Projeto

```
consulta-cnpj/
│
├── index.html          # Arquivo único (HTML + CSS + JS)
│
├── README.md           # Documentação do projeto
│
└── assets/             # (opcional) screenshots para o README
    ├── screenshot-home.png
    ├── screenshot-result.png
    └── screenshot-mobile.png
```

### Arquitetura do HTML

```
index.html
│
├── <head>
│   ├── Meta tags (charset, viewport)
│   ├── Google Fonts (Inter)
│   ├── Cloudflare CDN (Font Awesome)
│   └── <style> (CSS completo inline)
│
├── <body>
│   ├── .container
│   │   └── .main-card
│   │       ├── .top (logo, título, busca)
│   │       ├── .loading (spinner)
│   │       ├── .error (mensagens)
│   │       └── .result
│   │           ├── .stats-bar (resumo rápido)
│   │           ├── .company-banner (destaque)
│   │           ├── .info-grid (10 cards)
│   │           └── .footer
│   │
│   └── <script> (JavaScript completo inline)
│
└── Funções JS
    ├── Máscara CNPJ (input listener)
    ├── consultarCNPJ() — fetch + parse
    ├── preencherDados() — DOM manipulation
    ├── showError() / hideError()
    └── imprimirPDF() — window.print()
```

---

## 🌐 API Utilizada

### CNPJ WS (Pública)

| Item | Detalhe |
|---|---|
| **Base URL** | `https://publica.cnpj.ws/cnpj/` |
| **Método** | `GET` |
| **Autenticação** | Nenhuma (pública) |
| **Rate Limit** | ~3 req/min (plano gratuito) |
| **Formato** | JSON |

### Dados Retornados

```json
{
  "razao_social": "EMPRESA LTDA",
  "capital_social": "100000.00",
  "natureza_juridica": { "descricao": "..." },
  "porte": { "descricao": "..." },
  "estabelecimento": {
    "cnpj": "00000000000100",
    "nome_fantasia": "...",
    "situacao_cadastral": "Ativa",
    "data_inicio_atividade": "2020-01-15",
    "telefone1": "1199999999",
    "email": "contato@empresa.com",
    "logradouro": "...",
    "numero": "100",
    "bairro": "...",
    "cep": "01000000",
    "cidade": { "nome": "São Paulo" },
    "estado": { "sigla": "SP" }
  },
  "socios": [
    {
      "nome": "FULANO DA SILVA",
      "qualificacao_socio": { "descricao": "Sócio-Administrador" }
    }
  ]
}
```

### Códigos de Resposta Tratados

| Código | Significado | Ação na App |
|---|---|---|
| `200` | Sucesso | Preenche os dados |
| `404` | CNPJ não encontrado | Exibe mensagem de erro |
| `429` | Rate limit excedido | Exibe aviso para aguardar |
| `5xx` | Erro no servidor | Exibe erro genérico |

---

## 🎨 Paleta de Cores

### Cores Principais

| Cor | Hex | Uso |
|---|---|---|
| 🟠 Amber Flame | `#ff5500` | Botão primário, logo, destaques |
| 🩷 Hot Pink | `#ff2d7b` | Gradientes, loader, hover |
| 🔵 Signal Blue | `#0066ff` | Links, focus, badges UF |
| 🟡 Honey Glow | `#ffb800` | Labels, destaques dourados |
| 🟣 Vivid Purple | `#7b2dff` | Gradiente título, badges porte |

### Cores de Status

| Cor | Hex | Uso |
|---|---|---|
| 🟢 Vivid Green | `#00d26a` | Badge "Ativa", sucesso |
| 🔴 Alert Red | `#ff2d55` | Badge "Inativa", erros |
| 🩵 Cyan | `#00d4ff` | Labels, bordas laterais |
| 🟢 Teal | `#00c9a7` | Labels, bordas laterais |
| 🩷 Magenta | `#d916ff` | Labels, gradientes |

### Cores Neutras

| Cor | Hex | Uso |
|---|---|---|
| ⬛ Ink | `#0a0a14` | Texto principal |
| ◼️ Charcoal | `#1d1d2b` | Valores dos cards |
| ◽ Smoke | `#5a5a65` | Subtítulos |
| ⬜ Snow Gray | `#f2f2f7` | Background geral |

### Gradientes

```css
/* Primário (3 cores) */
linear-gradient(135deg, #ff5500 0%, #ff2d7b 50%, #ffaa00 100%)

/* Banner escuro */
linear-gradient(135deg, #07071a 0%, #141438 35%, #0d2e52 65%, #071422 100%)

/* Título */
linear-gradient(135deg, #0a0a14 0%, #2a2a4a 60%, #7b2dff 100%)
```

---

## 📱 Responsividade

| Breakpoint | Comportamento |
|---|---|
| `> 768px` | Layout completo, grid multi-coluna, botões inline |
| `≤ 768px` | Padding reduzido, título menor, botões full-width, stats empilhados |

### Adaptações Mobile

- Título reduzido de `48px` → `32px`
- Botões ocupam 100% da largura
- Cards em coluna única
- Stats bar empilhada verticalmente
- Banner com padding reduzido
- Company name de `38px` → `24px`

---

## 🖨️ Impressão / PDF

O projeto inclui regras `@media print` dedicadas:

```
✅ Background branco (economia de tinta)
✅ Remoção da barra de busca
✅ Remoção do loading e stats bar
✅ Bordas laterais coloridas forçadas (print-color-adjust)
✅ Box-shadow removido
✅ Banner com cores preservadas
```

Para gerar PDF:
1. Consulte um CNPJ
2. Clique em **Gerar PDF**
3. No diálogo de impressão, selecione **Salvar como PDF**

---

## ⚡ Performance

| Métrica | Valor |
|---|---|
| **Arquivo único** | ~18 KB (gzipped) |
| **Dependências JS** | 0 (zero) |
| **Framework** | Nenhum (vanilla) |
| **Fontes externas** | 2 (Inter + Font Awesome via CDN) |
| **Requisições** | 3 estáticas + 1 API por consulta |
| **First Paint** | < 500ms |

### Otimizações Aplicadas

- `preconnect` para Google Fonts e Cloudflare CDN
- `backdrop-filter` com fallback de opacidade
- CSS inline (zero FOUC)
- JS inline (zero round-trip adicional)
- Animações com `transform` e `opacity` (GPU-accelerated)
- `will-change` implícito via `transition`

---

## 🤝 Contribuição

Contribuições são bem-vindas! Siga os passos:

```bash
# 1. Fork o repositório

# 2. Crie uma branch
git checkout -b feature/minha-feature

# 3. Commit suas mudanças
git commit -m "feat: adiciona funcionalidade X"

# 4. Push para a branch
git push origin feature/minha-feature

# 5. Abra um Pull Request
```

### Padrão de Commits

| Prefixo | Uso |
|---|---|
| `feat:` | Nova funcionalidade |
| `fix:` | Correção de bug |
| `style:` | Mudança visual/CSS |
| `refactor:` | Refatoração de código |
| `docs:` | Documentação |
| `perf:` | Melhoria de performance |

---

## 📄 Licença

Este projeto está sob a licença **MIT**.

```
MIT License

Copyright (c) 2025

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
```

---

## 👤 Autor

Desenvolvido com 🔥 por **[Seu Nome](https://github.com/seu-usuario)**

---

<div align="center">

**⭐ Se este projeto foi útil, considere dar uma estrela!**

<br/>

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JS](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Cloudflare](https://img.shields.io/badge/CDN-Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white)

</div>
```

---

## 📌 Resumo do que o README cobre

| Seção | Conteúdo |
|---|---|
| **Badges** | Status, versão, licença, tecnologias |
| **Sobre** | Descrição e objetivos do projeto |
| **Funcionalidades** | Tabela completa com 11 features |
| **Demo** | Diagramas ASCII da interface |
| **Instalação** | 3 opções (direto, servidor local, deploy) |
| **Como Usar** | Passo a passo + CNPJs de teste |
| **Tecnologias** | Core, CDN, API — tudo detalhado |
| **Estrutura** | Árvore de arquivos + arquitetura HTML |
| **API** | Endpoint, rate limit, resposta JSON, códigos HTTP |
| **Paleta de Cores** | Todas as 15+ cores com hex e uso |
| **Responsividade** | Breakpoints e adaptações mobile |
| **Impressão** | Regras @media print documentadas |
| **Performance** | Métricas e otimizações aplicadas |
| **Contribuição** | Guia + padrão de commits |
| **Licença** | MIT completa |
