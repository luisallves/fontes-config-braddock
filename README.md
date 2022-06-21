Seja bem vindo, aqui estão todas as fontes necessárias pra deixar seu VS Code no Shape do Braddock!
Separei ainda algumas dicas que vão ser úteis na hora de configurar o VS Code. 

# 1. Clone este repositório e instale as fontes.
Clone esse repositório e mova todas as pastas de fontes para: o dioretório 
```sh
~/fonts
```
# 2. Edite as configurações do seu VS code.
Com seu VS Code aberto, Ultilize o atalho abra as configurações, clicando na engrenagem no canto inferior esquerdo do VS Code,

Depois altere a primeira linha das configurações do Braddock para:
```sh
"editor.fontFamily": "Operator Mono, Fira Code, Menlo, Monaco, 'Courier New', Monospace",
```

Reinicie seu terminal e o seu VS Code se não funcionar me chama no slack "Luís Alves = Turma 22 - Tribo A"

<details>
#<summary><strong> Você pode copiar as configurações autalizadas</strong></summary><br />
  
As configurações devem estar dessa forma:
  
```
{
"editor.fontFamily": "Operator Mono, Fira Code, Menlo, Monaco, 'Courier New', Monospace",
  "editor.fontLigatures": true,
  "editor.tokenColorCustomizations": {
    "textMateRules": [
      {
        "scope": [
          //following will be in italic
          "comment",
          "variables",
          "entity.name.type.class", //class names
          "constant", //String, Number, Boolean…, this, super
          "storage.modifier", //static keyword
          "storage.type.class.js", //class keyword
          "keyword" //import, export, return…
        ],
        "settings": {
          "fontStyle": "italic"
        }
      }
    ]
  },
  "terminal.integrated.fontFamily": "Fira Code",
  "editor.mouseWheelZoom": true,
  "editor.fontSize": 20,
  "editor.tabSize": 2,
  "window.restoreWindows": "none",
  "terminal.integrated.fontSize": 16,
  "editor.minimap.enabled": false,
  "editor.lineHeight": 25,
  "explorer.compactFolders": false,
  "workbench.editor.labelFormat": "short",
  "extensions.ignoreRecommendations": true,
  "editor.suggest.showTypeParameters": true,
  "editor.parameterHints.enabled": true,
  "editor.linkedEditing": true,
  "editor.snippetSuggestions": "top",
  // Muito útil
  "window.openFoldersInNewWindow": "off",
  "editor.guides.bracketPairs": true,
  "editor.formatOnSave": true,
  "editor.formatOnPaste": true,
  // ESLINT
  "eslint.format.enable": true,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
    // "source.organizeImports": true
  },
  "eslint.validate": [
    "javascript",
    "javascriptreact",
    "html",
    "typescriptreact"
  ],
  // Prettier
  "prettier.jsxBracketSameLine": false,
  "prettier.singleQuote": true,
  // REACT SETTINGS
  "emmet.includeLanguages": {
    "javascript": "javascriptreact"
  },
  "emmet.syntaxProfiles": {
    "javascript": "jsx"
  },
  "javascript.preferences.jsxAttributeCompletionStyle": "auto",
  "javascript.suggest.autoImports": true,
  "typescript.updateImportsOnFileMove.enabled": "always",
  // Alterar os ícones para quem tem TOC
  "material-icon-theme.activeIconPack": "react_redux",
  "files.associations": {
    "**/src/**/*.js": "javascriptreact",
    "**/src/**/*.jsx": "javascriptreact"
  },
  "html.format.wrapAttributes": "force",
  "diffEditor.ignoreTrimWhitespace": false,
  "[javascriptreact]": {
    "editor.defaultFormatter": "dbaeumer.vscode-eslint"
  },
  "workbench.colorTheme": "Trybe Theme -  Dark",
  "window.zoomLevel": 1,
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
}
```
  </details>
