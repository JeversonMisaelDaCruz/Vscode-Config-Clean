
## Documentação da Configuração do VSCode

Esta documentação detalha cada configuração presente no seu arquivo `settings.json` do VSCode.

### Índice

- [Ajustes Gerais](#ajustes-gerais)
- [Editor](#editor)
- [JavaScript e TypeScript](#javascript-e-typescript)
- [Extensões e Linguagens](#extensões-e-linguagens)
- [Terminal Integrado](#terminal-integrado)
- [Interface e Aparência](#interface-e-aparência)
- [Git e Controle de Versão](#git-e-controle-de-versão)
- [Explorador de Arquivos](#explorador-de-arquivos)
- [Outras Configurações](#outras-configurações)

---

### Ajustes Gerais

- **Zoom da Janela**

  ```json
  "window.zoomLevel": -0.5
  ```

  Reduz o nível de zoom da janela do VSCode, diminuindo o tamanho dos elementos da interface, incluindo os números das linhas.

- **Auto Salvamento de Arquivos**

  ```json
  "files.autoSave": "afterDelay"
  ```

  Salva automaticamente os arquivos após um pequeno atraso.

- **Exclusão de Arquivos**

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

  Exclui determinados arquivos e pastas da exibição no explorador.

### Editor

- **Tamanho e Altura da Fonte**

  ```json
  "editor.fontSize": 14,
  "editor.lineHeight": 1.5
  ```

  Define o tamanho da fonte e a altura das linhas no editor.

- **Fonte e Ligaduras**

  ```json
  "editor.fontFamily": "JetBrains Mono",
  "editor.fontLigatures": true
  ```

  Configura a família de fontes e habilita ligaduras.

- **Sugestões e Dicas**

  ```json
  "editor.parameterHints.enabled": true,
  "editor.suggestSelection": "first",
  "editor.quickSuggestions": {
    "other": true,
    "comments": false,
    "strings": false
  }
  ```

  Controla as sugestões de código e dicas de parâmetros.

- **Formatação e Ações ao Salvar**

  ```json
  "editor.formatOnSave": true,
  "editor.codeActionsOnSave": {
    "source.fixAll": "explicit"
  }
  ```

  Formata o código e aplica ações ao salvar o arquivo.

- **Estética do Cursor**

  ```json
  "editor.cursorBlinking": "phase",
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.cursorWidth": 2
  ```

  Personaliza a aparência e o comportamento do cursor.

- **Outras Configurações**

  ```json
  "editor.renderLineHighlight": "none",
  "editor.acceptSuggestionOnCommitCharacter": false,
  "editor.accessibilitySupport": "off",
  "editor.semanticHighlighting.enabled": true,
  "editor.minimap.enabled": false,
  "editor.tabSize": 2,
  "editor.stickyScroll.enabled": false,
  "editor.defaultFormatter": "esbenp.prettier-vscode"
  ```

  Diversas configurações para melhorar a experiência de edição.

### JavaScript e TypeScript

- **Sugestões e Importações Automáticas**

  ```json
  "javascript.suggest.autoImports": true,
  "javascript.updateImportsOnFileMove.enabled": "always",
  "typescript.suggest.autoImports": true,
  "typescript.preferences.preferTypeOnlyAutoImports": true
  ```

  Habilita sugestões e atualizações automáticas de importações.

- **Servidor TypeScript**

  ```json
  "typescript.tsserver.log": "off",
  "typescript.tsdk": "/usr/local/lib/node_modules/typescript/lib"
  ```

  Configura o servidor TypeScript.

- **Formatadores Padrão**

  ```json
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[typescript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[typescriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  }
  ```

  Define o Prettier como formatador padrão para JavaScript e TypeScript.

### Extensões e Linguagens

- **Associações de Arquivos**

  ```json
  "files.associations": {
    ".env.*": "dotenv",
    ".prettierrc": "json",
    "*.css": "css",
    ".dev.vars": "dotenv",
    "*.vue": "vue"
  }
  ```

  Associa extensões de arquivo a linguagens específicas.

- **Emmet**

  ```json
  "emmet.includeLanguages": {
    "javascript": "javascriptreact"
  },
  "emmet.syntaxProfiles": {
    "javascript": "jsx",
    "vue-html": "html"
  }
  ```

  Configura o Emmet para funcionar com JavaScript e Vue.

- **ESLint**

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

  Define quais linguagens o ESLint deve validar.

- **Prisma**

  ```json
  "[prisma]": {
    "editor.formatOnSave": true,
    "editor.defaultFormatter": "Prisma.prisma"
  }
  ```

  Configurações específicas para arquivos Prisma.

- **JSON**

  ```json
  "[jsonc]": {
    "editor.defaultFormatter": "vscode.json-language-features"
  },
  "[json]": {
    "editor.defaultFormatter": "vscode.json-language-features"
  }
  ```

  Define o formatador padrão para arquivos JSON e JSON com comentários.

- **Codeium**

  ```json
  "codeium.enableConfig": {
    "*": true,
    "prisma": true
  },
  "codeium.enableCodeLens": false
  ```

  Configura o comportamento da extensão Codeium.

### Terminal Integrado

- **Fonte e Tamanho**

  ```json
  "terminal.integrated.fontSize": 12,
  "terminal.integrated.fontFamily": "JetBrainsMono mono"
  ```

  Define a fonte e o tamanho do terminal integrado.

- **Aceleração e Ambiente**

  ```json
  "terminal.integrated.gpuAcceleration": "on",
  "terminal.integrated.env.osx": {},
  "terminal.integrated.env.linux": {}
  ```

  Configura a aceleração gráfica e variáveis de ambiente.

- **Alertas**

  ```json
  "terminal.integrated.showExitAlert": false
  ```

  Desabilita alertas ao sair do terminal.

### Interface e Aparência

- **Tema e Ícones**

  ```json
  "workbench.colorTheme": "Ayu Mirage Bordered",
  "workbench.iconTheme": "vscode-icons"
  ```

  Escolhe o tema de cores e ícones do VSCode.

- **Barra Lateral e Layout**

  ```json
  "workbench.sideBar.location": "right",
  "workbench.layoutControl.enabled": false
  ```

  Move a barra lateral para a direita e desabilita o controle de layout.

- **Zoom e Status Bar**

  ```json
  "window.zoomLevel": -0.5,
  "workbench.statusBar.visible": false
  ```

  Ajusta o zoom e oculta a barra de status.

- **Explorador de Arquivos**

  ```json
  "explorer.sortOrder": "foldersNestsFiles",
  "explorer.fileNesting.enabled": true,
  "explorer.fileNesting.patterns": {
    "package.json": ".eslint*, prettier*, tsconfig*, vite*, pnpm-*, bun.lockb, nest*, package-lock*",
    "tailwind.config.*": "tailwind.config*, postcss.config*",
    ".env.local": ".env*",
    ".env": ".env*"
  },
  "explorer.compactFolders": false,
  "explorer.confirmDelete": false,
  "explorer.confirmDragAndDrop": false
  ```

  Configura a visualização e comportamento do explorador de arquivos.

### Git e Controle de Versão

- **Configurações do Git**

  ```json
  "git.enableSmartCommit": true,
  "git.autofetch": true,
  "git.openRepositoryInParentFolders": "always"
  ```

  Otimiza o fluxo de trabalho com Git.

- **GitLens**

  ```json
  "gitlens.codeLens.authors.enabled": false
  ```

  Desabilita o CodeLens de autores no GitLens para melhorar a performance.

### Outras Configurações

- **Atualizações e Segurança**

  ```json
  "update.mode": "default",
  "update.showReleaseNotes": false,
  "security.promptForLocalFileProtocolHandling": false
  ```

  Controla como o VSCode lida com atualizações e segurança.

- **Comandos e Central de Configurações**

  ```json
  "window.commandCenter": false,
  "workbench.settings.applyToAllProfiles": [
    "terminal.integrated.defaultProfile.windows"
  ],
  "settingsSync.ignoredSettings": [
    "terminal.integrated.defaultProfile.windows"
  ]
  ```

  Ajusta preferências relacionadas a comandos e perfis.

- **Outros**

  ```json
  "console-ninja.featureSet": "Community",
  "remote.autoForwardPortsSource": "hybrid",
  "codeium.enableCodeLens": false
  ```

  Configurações adicionais para extensões e funcionalidades remotas.

---

Espero que esta configuração ajustada e a documentação sejam úteis para você. Se gostou deixe uma estela nesse repositorio!
