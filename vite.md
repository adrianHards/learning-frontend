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
  
## Setting up ESLint and Prettier

### Step 1: Installation

Run the following commands:

```
pnpm install eslint eslint-config-prettier eslint-plugin-prettier --save-dev
pnpm run eslint --init
```

**Preferred Options**:

- **How would you like to use ESLint?** 
  - `check syntax, find problems`
- **What type of modules does your project use?** 
  - `JavaScript modules (import/export)`
- **Which framework does your project use?** 
  - `Vue.js`
- **Does your project use TypeScript?** 
  - `Yes`
- **Where does your code run?** 
  - `Browser`
- **Which format do you want your config file to be in?** 
  - `JSON`
- **Plugins**: 
  - Install `eslint-plugin-vue@latest`, `@typescript-eslint/eslint-plugin@latest`, and `@typescript-eslint/parser@latest`

### Step 2: ESLint Configuration

Update your .eslintrc.json with:

```
{
  "extends": ["plugin:prettier/recommended"],
  "plugins": ["prettier"]
}
```

### Step 3: Prettier Configuration

Run the command to create and populate your Prettier configuration:

```
echo '{n"trailingComma": "none",n"tabWidth": 2,n"semi": true,n"singleQuote": truen}' > .prettierrc.json
```

Your .prettierrc.json should look like:

```
{
  "trailingComma": "none",
  "tabWidth": 2,
  "semi": true,
  "singleQuote": true
}
```

### Step 4: Ignore certain files

Run these commands to create and populate .prettierignore and .eslintignore:

```
echo "node_modulesnpackage.lock.json\nbuild" > .prettierignore
echo "node_modules\npackage.lock.json\nbuild" > .eslintignore
```

### Step 5: Add Run Scripts

Update the scripts section of your package.json to:

```
"scripts": {
  "lint": "eslint .",
  "format": "prettier --write ."
}
```

**Execution**:

- To check for ESLint errors:

```
pnpm run lint
```
  
- To format with Prettier:

```
pnpm run format
```


  <br>
  
</details>


### Recommended IDE setup:

VS Code + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur) + [TypeScript Vue Plugin](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin).

### GitHub

1. `git init`
2. `gh repo create --private --source=.`
