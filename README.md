```md
# Configurações do VSCode

Esta configuração otimiza o Visual Studio Code para um ambiente de desenvolvimento clean e eficiente. É ideal para desenvolvedores que buscam uma interface minimalista, sugestões automáticas e formatação consistente.

---

## Interface do VSCode

### Arquivo em Branco ao Iniciar

O VSCode inicia com um arquivo em branco, pronto para começar a codificar.

```json
"workbench.startupEditor": "newUntitledFile"
```

### Fonte e Formatação

Configurações de fonte e espaçamento para melhorar a legibilidade do código.

```json
"editor.fontSize": 16,
"editor.lineHeight": 1.8,
"editor.fontFamily": "JetBrains Mono"
```

### Desativar Minimap

Remove o minimapa para uma interface mais limpa.

```json
"editor.minimap.enabled": false
```

### Destaque da Linha de Código Atual

Desativa o destaque da linha ativa para um visual mais neutro.

```json
"editor.renderLineHighlight": "none"
```

---

## Sugestões e Importações

### Importações Automáticas

Facilita a importação de módulos em projetos JavaScript e TypeScript.

```json
"javascript.suggest.autoImports": true,
"typescript.suggest.autoImports": true,
"typescript.updateImportsOnFileMove.enabled": "always"
```

### Sugestão de Códigos

Melhora a experiência de sugestão de código, destacando a primeira opção.

```json
"editor.suggestSelection": "first"
```

---

## Ferramentas e Validações

### Validação com ESLint

Garante a validação de código consistente em diferentes linguagens.

```json
"eslint.validate": [
  "javascript",
  "javascriptreact",
  "typescript",
  "typescriptreact",
  "vue",
  "graphql",
  "json",
  "jsonc",
  "java"
]
```

### Formatação Automática

Aplica formatação automática ao salvar arquivos.

```json
"editor.formatOnSave": true
```

---

## Terminal Integrado

### Fonte e Tamanho do Terminal

Configura uma fonte personalizada e tamanho adequado para o terminal integrado.

```json
"terminal.integrated.fontSize": 14,
"terminal.integrated.fontFamily": "JetBrainsMono mono"
```

### Aceleração de GPU

Habilita a aceleração de GPU para melhor performance do terminal.

```json
"terminal.integrated.gpuAcceleration": "on"
```

---

## Aparência e Personalização

### Tema e Ícones

Define um tema moderno e ícones personalizados.

```json
"workbench.colorTheme": "Ayu Mirage Bordered",
"workbench.iconTheme": "vscode-icons"
```

### Configurações de Exibição

Exibe pastas sem compactação no explorador e oculta a barra de rolagem vertical.

```json
"explorer.compactFolders": false,
"editor.scrollbar.vertical": "hidden"
```

### Ordem de Exibição no Explorador

Organiza o explorador de arquivos para mostrar pastas antes dos arquivos.

```json
"explorer.sortOrder": "foldersNestsFiles"
```

---

## Melhoria de Performance e Limpeza

### Ocultar Arquivos e Pastas Desnecessárias

Esconde arquivos irrelevantes para um projeto, como `node_modules` e `.git`.

```json
"files.exclude": {
  "**/CVS": true,
  "**/.DS_Store": true,
  "**/.hg": true,
  "**/.svn": true,
  "**/.git": true,
  ".vscode": true,
  "node_modules": true
}
```

### Salvamento Automático

Configura o salvamento automático após um pequeno atraso.

```json
"files.autoSave": "afterDelay"
```

---

## Outras Configurações Notáveis

### Configuração de Extensões

Habilita o uso do Codeium para sugestões assistidas por IA.

```json
"codeium.enableConfig": {
  "*": true,
  "prisma": true
}
```

### Desempenho e Experiência do Editor

Ativa a animação suave do cursor e define a largura para uma navegação mais fluida.

```json
"editor.cursorBlinking": "phase",
"editor.cursorSmoothCaretAnimation": "on",
"editor.cursorWidth": 2
```

### Commit Inteligente no Git

Ativa a opção de commit rápido sem confirmação.

```json
"git.enableSmartCommit": true
```

---

Esta configuração proporciona uma experiência de desenvolvimento otimizada e organizada no Visual Studio Code .
```
