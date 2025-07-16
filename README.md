## Global Settings 🔥

**Open File:** `Ctrl`+`,` > `Open Settings (JSON)` > `settings.json`

<br />

```
{
  // Viewport width অনুযায়ী লাইন ব্রেক হবে
  "editor.wordWrap": "on",

  // ফাইল সেভ করলেই অটো ফরম্যাট হবে
  "editor.formatOnSave": true,

  // Default formatter হিসেবে Prettier ব্যবহার করবে
  "editor.defaultFormatter": "esbenp.prettier-vscode",

  // শুধুমাত্র React JS (JSX/TSX) ফাইলের জন্য Prettier ফরম্যাটার
  "[javascriptreact]": {
    "editor.formatOnSave": true,
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },

  // Liquid ফাইলের জন্য Shopify এর formatter
  "[liquid]": {
    "editor.defaultFormatter": "Shopify.theme-check-vscode"
  },

  // Minimap বন্ধ রাখা হয়েছে (কোডের সাইড প্যানেল)
  "editor.minimap.enabled": false,

  // Bracket গুলোর কালার হাইলাইট ও গাইড লাইন চালু
  "editor.bracketPairColorization.enabled": true,
  "editor.guides.bracketPairs": "active",

  // ফন্ট সাইজ
  "editor.fontSize": 15,

  // Lint error সেভের সময় ঠিক করে দিবে
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true,
    "source.fixAll.tslint": true
  },

  // Emmet এর Tab shortcut চালু
  "emmet.triggerExpansionOnTab": true,

  // Emmet কে JSX ফাইলে কাজ করার অনুমতি
  "emmet.includeLanguages": {
    "javascript": "javascriptreact"
  },

  // ফাইল move করলে import গুলো auto update হবে
  "javascript.updateImportsOnFileMove.enabled": "always",
  "typescript.updateImportsOnFileMove.enabled": "always",

  // ফোকাস হারালেই ফাইল সেভ হবে
  "files.autoSave": "onWindowChange",

  // Material icon theme ব্যবহার করা হচ্ছে
  "workbench.iconTheme": "material-icon-theme",

  // Default terminal হিসেবে Git Bash ব্যবহার
  "terminal.integrated.defaultProfile.windows": "Git Bash",

  // Untrusted ফাইল সরাসরি open করবে, warning দিবে না
  "security.workspace.trust.untrustedFiles": "open",

  // GitHub Copilot Suggestion বন্ধ রাখা হয়েছে
  "editor.inlineSuggest.enabled": false,
  "github.copilot.enable": {
    "*": false,
    "plaintext": false,
    "markdown": false,
    "javascript": false
  },

  // Code Runner extension টারমিনালে রান করবে (আলাদা output panel নয়)
  "code-runner.runInTerminal": true,

  // Tailwind CSS support বিভিন্ন ফাইলে যুক্ত করা হয়েছে
  "tailwindCSS.includeLanguages": {
    "html": "html",
    "liquid": "html",
    "javascript": "javascript",
    "css": "css"
  },

  // String এর মধ্যে suggestion চালু রাখা হয়েছে
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
