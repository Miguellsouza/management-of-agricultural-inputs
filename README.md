<div align="center">

<img src="logo_AgroSier-removebg-preview.png" alt="AgroSier" width="260">

# AgroSier — Gestão de Insumos Agrícolas

**Plataforma web para planejar, controlar e distribuir insumos agrícolas, reduzindo custos e aumentando a produtividade da lavoura.**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![Font Awesome](https://img.shields.io/badge/Font%20Awesome-528DD7?logo=fontawesome&logoColor=white)
![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow)

</div>

---

## Sobre o projeto

O **AgroSier** (repositório `management_of_agricultural_inputs`) é uma plataforma de gestão de insumos agrícolas voltada a produtores rurais. A proposta é centralizar as informações da propriedade e acompanhar os insumos desde a aquisição até a utilização, apoiando decisões que melhorem a rentabilidade.

> **Missão:** tornar a gestão de insumos agrícolas mais simples, eficiente e transparente, permitindo que produtores tomem decisões melhores para seus negócios.

Nesta etapa, o projeto contém o **front-end** (telas em HTML e CSS puros): página institucional, login, cadastro do produtor e menu principal do sistema.

## Pilares

| Pilar | Descrição |
| --- | --- |
| **Eficiência** | Redução do desperdício e melhor aproveitamento dos recursos |
| **Organização** | Centralização das informações importantes da propriedade |
| **Controle** | Acompanhamento dos insumos da aquisição até a utilização |
| **Rentabilidade** | Melhor controle dos custos para apoiar a produção |

## Funcionalidades

### Site institucional (`index.html`)

- Navegação fixa no topo com âncoras: **Início**, **Sobre**, **Serviços** e **Contato**
- Seção **Sobre nós** com missão e pilares
- Seção **Nossos serviços**:
  - Gestão de estoque
  - Planejamento de compras
  - Distribuição de insumos
  - Controle de custos
  - Planejamento de insumos
- Formulário de contato (nome, e-mail e mensagem)
- Rodapé com redes sociais e direitos reservados

### Autenticação

- **Login** (`teladelogin.html`): e-mail, senha, "Esqueceu a senha?" e link para criar conta
- **Cadastro do produtor** (`teladecriarconta.html`): nome completo, CNPJ, e-mail, telefone, senha e confirmação de senha

### Menu principal (`menuagro.html`)

Painel com os módulos do sistema: **Financeiro**, **Insumos**, **Safra**, **Operacionais**, **Dados** e **Sistema**.

## Tecnologias

- HTML5
- CSS3 (Flexbox e Grid)
- [Font Awesome 7.3.1](https://fontawesome.com/) via CDN para os ícones

Não há dependências para instalar nem etapa de build.

## Estrutura do projeto

```
management_of_agricultural_inputs/
├── index.html                # Página inicial (institucional)
├── teladelogin.html          # Tela de login
├── teladecriarconta.html     # Tela de cadastro do produtor
├── menuagro.html             # Menu principal do sistema
│
├── estilizacaoagro.css       # Estilos da página inicial
├── estiloteladelogin.css     # Estilos da tela de login
├── estilocriarconta.css      # Estilos da tela de cadastro
├── estilomenu.css            # Estilos do menu principal
│
├── logo_AgroSier-removebg-preview.png   # Logotipo
├── logohead.png                         # Favicon
├── img1.jpg                  # Imagem da seção inicial
├── img2.jpg                  # Imagem da seção de contato
├── imglogin.png              # Imagem lateral da tela de login
└── imagecoffeharvest.jpg     # Plano de fundo do menu principal
```

## Como executar

1. Clone o repositório:

   ```bash
   git clone <url-do-repositorio>
   cd management_of_agricultural_inputs
   ```

2. Abra o `index.html` no navegador (duplo clique) **ou** sirva a pasta localmente:

   ```bash
   # Python
   python -m http.server 8000
   # Acesse: http://localhost:8000
   ```

   Também funciona com a extensão **Live Server** do VS Code.

> Os ícones dependem de conexão com a internet, pois o Font Awesome é carregado por CDN.

## Fluxo de navegação

```
index.html ──► teladelogin.html ◄──► teladecriarconta.html
                                     
menuagro.html  (ainda sem ligação com o login)
```

## Status e próximos passos

O projeto está em fase de prototipação visual. Ainda não implementado:

- [ ] Lógica em JavaScript (validação de formulários, máscara de CNPJ e telefone)
- [ ] Back-end e banco de dados (autenticação, cadastro de produtores e insumos)
- [ ] Ligar o login ao menu principal (`menuagro.html`)
- [ ] Páginas dos módulos do menu: Financeiro, Insumos, Safra, Operacionais, Dados e Sistema
- [ ] Envio real do formulário de contato
- [ ] Layout responsivo para celular e tablet
- [ ] Recuperação de senha

## Licença

Distribuído sob a licença Apache 2.0. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

<div align="center">

**AgroSier** — *Juntos pelo campo, sempre* 🌱

© 2025 AgroSier. Todos os direitos reservados.

</div>
