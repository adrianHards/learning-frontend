🚧 work in progress 🚧

<div align="center">

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/95/Vue.js_Logo_2.svg/2367px-Vue.js_Logo_2.svg.png" alt="Vue.js Logo" width="200" height="200">

</div>

# Vue
- [Setup](#setup)

## Setup: 

### Official Docs:
- [Introduction](https://vuejs.org/guide/introduction.html)
- [Interactive Tutorial](https://vuejs.org/tutorial/#step-1)
- [API reference](https://vuejs.org/api/)
- [Vite: Getting Started](https://vitejs.dev/guide/)

### 3rd Party:
- [MDN: Getting Started with Vue](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Client-side_JavaScript_frameworks/Vue_getting_started)
- [Scrimba: Vue](https://scrimba.com/learn/learnvue)
- [Scrimba: TypeScript](https://scrimba.com/learn/typescript)

### Updates
```bash
brew update
brew doctor
brew upgrade node

# either
brew upgrade pnpm
brew install pnpm
```

### Installation with [Vite](https://vitejs.dev/guide/)

Alternatively, you can use [create-vue](https://vuejs.org/guide/quick-start.html#creating-a-vue-application).

```bash
pnpm create vite app-name --template vue-ts

cd vue-practice
pnpm install
pnpm run dev
```
- `vue-ts` specifies we want to use the typescript [template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-vue-ts).

<details>
  <summary>Setting up ESLint and Prettier</summary>
  
  <br>
  
  ### Step 1
  ```bash
  pnpm install eslint eslint-config-prettier eslint-plugin-prettier --save-dev
  pnpm eslint --init
  ```
  
  #### Preferred Options:
  1. How would you like to use ESLint? `check syntax, find problems`
  2. What type of modules does your project use? `JavaScript modules (import/export)`
  3. Which framework does your project use? `Vue.js`
  4. Does your project use TypeScript? `Yes`
  5. Where does your code run? `Browser`
  6. Which format do you want your config file to be in? `JSON`
  7. Choose to install `eslint-plugin-vue@latest @typescript-eslint/eslint-plugin@latest @typescript-eslint/parser@latest`
  
  
  ### Step 2
  Tell ESLint to enforce Prettier rules alongside ESLint rules
  ```
  # .eslintrc.json
  "extends": ["plugin:prettier/recommended"],
  "plugins": ["prettier"],
  ```
  
  ### Step 3
  ### Customise Prettier
   `echo {}> .prettierrc.json`
  
  ```bash
  # .prettierrc.json
  {
  "trailingComma": "none",
  "tabWidth": 2,
  "semi": true,
  "singleQuote": true
  } 
  ```
  
  #### Ignore certain files
  `touch .prettierignore .eslintignore` and copy paste the following into both files:
  
  ```bash
  node_modules
  package.lock.json
  build
  ```
  
  #### Run scripts
  ```bash
  # package.json
  "scripts": {
  "lint": "eslint .",
  "format": "prettier --write ."
  }
  ```
  
  You can now run the following:
  - `pnpm run lint` check for ESLint errors
  - `pnpm run format` format with Prettier

  <br>
  
</details>


### Recommended IDE setup:

VS Code + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur) + [TypeScript Vue Plugin](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin).

### GitHub

1. `git init`
2. `gh repo create --private --source=.`
