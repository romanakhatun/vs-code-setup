## Global Settings 🔥

**Open File:** `Ctrl`+`,` > `Open Settings (JSON)` > `settings.json`

<br />

```
{
  //Lines will wrap at viewport width //
  "editor.wordWrap": "on",

  // VSCode will automatically run the formatter whenever you save a file //
  "editor.formatOnSave": true,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "[javascriptreact]": {
    "editor.formatOnSave": true,
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[liquid]": {
    "editor.defaultFormatter": "Shopify.theme-check-vscode"
  },

  // A Minimap (code outline) gives a high-level overview of source code //
  "editor.minimap.enabled": false,

  //Allows matching brackets to be identified with colours //
  "editor.bracketPairColorization.enabled": true,
  "editor.guides.bracketPairs": "active",

  "editor.fontSize": 15,

  // Fix all linting errors on save //
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true,
    "source.fixAll.tslint": true
  },

  // Enable expanding Emmet abbreviations with Tab key.
  "emmet.triggerExpansionOnTab": true,
  "emmet.includeLanguages": {
    "javascript": "javascriptreact"
  },

  //Always update path automatically//
  "javascript.updateImportsOnFileMove.enabled": "always",
  "typescript.updateImportsOnFileMove.enabled": "always",

  "files.autoSave": "onWindowChange",
  "workbench.iconTheme": "material-icon-theme",
  "terminal.integrated.defaultProfile.windows": "Git Bash",
  "security.workspace.trust.untrustedFiles": "open",

  // Copilot বন্ধ রাখার জন্য
  "editor.inlineSuggest.enabled": false,
  "github.copilot.enable": {
    "*": false,
    "plaintext": false,
    "markdown": false,
    "javascript": false
  },
  "code-runner.runInTerminal": true,

  //Tailwind css support
  "tailwindCSS.includeLanguages": {
    "html": "html",
    "liquid": "html",
    "javascript": "javascript",
    "css": "css"
  },
  "editor.quickSuggestions": {
    "strings": true
  }
}
```
- [emmet.triggerExpansionOnTab](https://code.visualstudio.com/docs/editor/emmet)

<br/>

## Custom Snippets 🔥

**Open File:** `Ctrl`+`Shift`+`P` > `Preferences: Configure User Snippets` > `javascript.json`

<br />

```
{
  "Print to console": {
    "prefix": "cl",
    "body": ["console.log($1)"],
    "description": "Log output to console"
  },
  "useEffect Hook": {
    "prefix": "customUseEffect",
    "body": ["useEffect(() => {", "   $1", "}, []);"],
    "description": "useEffect Hook"
  },
  "useState Hook": {
    "prefix": "customUseState",
    "body": ["const [$1, set$2] = useState($3);"],
    "description": "useState Hook"
  },
  "Array Method": {
    "prefix": "customArrayMethod",
    "body": [
      "${1:arrayName}.${2|forEach,map,filter,reduce,some|}((${3:item}) => {",
      "    $4",
      "});"
    ],
    "description": "Array Method"
  }
}
```

- [Custom Snippet Generator](https://snippet-generator.app)

<br/>

## Extensions 🔥

**Open File:** `Ctrl`+`Shift`+`X`

1. [Auto Import](https://marketplace.visualstudio.com/items?itemName=steoates.autoimport)
2. [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker)
3. [Code Time](https://marketplace.visualstudio.com/items?itemName=softwaredotcom.swdc-vscode)
4. [ES7+ React/Redux/React-Native snippets](https://marketplace.visualstudio.com/items?itemName=dsznajder.es7-react-js-snippets)
5. [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
6. [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)
7. [npm Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.npm-intellisense)
8. [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
9. [Tailwind CSS IntelliSensePreview](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss)
10. [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
11. [Import Cost](https://marketplace.visualstudio.com/items?itemName=wix.vscode-import-cost)
12. [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
13. [REST Client](https://marketplace.visualstudio.com/items?itemName=humao.rest-client)
14. [Shopify Liquid](https://marketplace.visualstudio.com/items?itemName=Shopify.theme-check-vscode)
