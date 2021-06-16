# Desenvolvendo Software de Verdade

- Curso by Codar.me
- Foco: Desenvolvendo software para a produção, resolver a dor do cliente, criar hipóteses para resolver um problema, implementar as hipóteses e evoluir o projeto com o tempo

## Sumário

- Customer Development
  - Ferramenta
- Levantamento de Requisitos
  - Funcionalidades do app de Planejamento Financeiro
  - Features
- Definindo o MVP
- Configurando o ambiente
  - VS Code Extensions
  - Other extensions
  - Monoespaced Font
  - Zsh, Oh my Zsh, and Spaceship
    - Zinit
  - VS Code Setting in setting.json
  - VS Code Keyboard Shortcuts

## Customer Development

- Objetivo
  - Entender o problema para resolver o problema do cliente
- Perguntas
  - Qual o problema que queremos resolver?
- App que será desenvolvido
  - App de Planejamento Financeiro
- Dor
  - Visibilidade de gastos previstos (luz, aluguel, condomínio, prestações)
  - Gestão de contas a pagar e receber

### Ferramenta

- excalidraw.com : Para anotações / Brainstorm

## Levantamento de Requisitos

Receitas:

- Salário
- Rendimentos de investimentos
- Freelancer

Despesas:

- Fatura do Cartão: Gastos previstos
- Despesas Programadas: Netflix, Spotify, Gympass, lazer
- Gastos do Casal: Aluguel, condomínio, mercado, gasolina

### Funcionalidades do app de Planejamento Financeiro

Despesa / Receitas

- única ou recorrente
  - se recorrente: parcelada ou programada
  - quantidade de vezes
- fixa ou variável
- centro de custo
- ser descontada de uma conta (cc, crédito, carteira)
- categoria
- entrada ou saída
- data de vencimento
- efetivada (paga ou recebida)

Contas

- nome
- crédito ou débito
- saldo inicial (não aplica para crédito)
- limite (só aplica para crédito)
- vencimento fatura (só aplica para crédito)
- data de fechamento da fatura do cartão

Centros de custo (moradia)

- nome

Categorias (luz, água, aluguel)

- nome

Cadastro de usuário

- nome
- email
- senha

### Features

- cadastro de usuário
- login
- recuperação de senha (via email)
- editar perfil (nome e email)
- alterar senha
- CRUD contas
- CRUD centro de custo
- CRUD categorias
- CRUD de lançamentos (despesas e receitas)
- cron de lançamentos recorrentes
- dar como efetivado (pago / recebido)
- dashboard (saldo do mês, saldo geral de cada conta, saldo total)
- mover despesa/receita para mês anterior ou posterior

## Definindo o MVP

- App: PayUfirst (PUF)
- Desenvolvimento de produto
  - Ao desenvolver um produto temos que criar um MVP (Minimal Viable Product)

## Configurando o ambiente

### VS Code Extensions

- lucy (theme)
- eslint
- prettier (code formatter)
- gitlens
- markdown all in one
- markdownlint
- Markdown Preview Enhanced
- vscode-icons
- Bracket Pair Colorizer
- Path Intellisense (auto-complete paths)
- Remote Development / Remote WSL (WSL 2 support for VS Code)
- Settings Sync (save all vscode configurations)

### Other extensions

- mdx (for .md extension - write javascript inside the markdown)
- Live Share (good for pair programming)

### Monoespaced Font

- Fira code: <https://github.com/tonsky/FiraCode>
  - Has programming ligatures
- How to install: <https://github.com/tonsky/FiraCode/wiki>

### Zsh, Oh my Zsh, and Spaceship

- Zsh (Z Shell): <https://zsh.org/>
  - Github: <https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH>
- Oh my Zsh: <https://ohmyz.sh/>
  - It is possible to add plugins to th terminal
- Spaceship: Theme for On My Zsh
- Tutorial to install Zsh, Oh My Zsh and spaceship on Windows: <https://dev.to/erickrock80/pt-br-instalando-oh-my-zsh-no-windows-terminal-3a8l>

#### Zinit

- <https://github.com/zdharma/zinit>
- Plugin for syntax higlight in terminal: <https://github.com/zdharma/fast-syntax-highlighting>

### VS Code Setting in setting.json

- <https://gist.github.com/brunobertolini/8968487cff8ecd93dbd1d6c1787424b9>
- Some examples:

{
"files.trimTrailingWhitespace": true,
"editor.fontFamily": "JetBrains Mono", // Other is "Fira Code"
"javascript.updateImportsOnFileMove.enabled": "always",
"explorer.compactFolders": false,
}

### VS Code Keyboard Shortcuts

- <https://gist.github.com/brunobertolini/b3ee863f7f3912fa0dc1af4461f5528a>
- File -> Preferences -> Keyboard Shortcuts
