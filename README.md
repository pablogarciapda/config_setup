# config_setup
Archivos de configuraciones
vue3-eslint-starter

https://mattgosden.medium.com/quick-vscode-setup-for-vue-js-with-prettier-and-eslint-4b97fc71c587
borrar todo lo realacionado con eslint en el archivo package.json
instalar lo siguiente en la linea de comandos
npm install -D eslint prettier babel-eslint eslint-config-airbnb-base eslint-plugin-import eslint-config-prettier eslint-plugin-prettier eslint-plugin-vue

Create a .eslintrc.js file at your project's root

module.exports = {
  root: true,
  env: {
    browser: true,
  },
  parserOptions: {
    parser: 'babel-eslint',
    sourceType: 'module',
  },
  extends: [
    'airbnb-base',
    'plugin:vue/vue3-essential',
    'prettier/vue',
    'plugin:prettier/recommended'
  ],
  rules: {
    'comma-dangle': 'off',
    'class-methods-use-this': 'off',
    'import/no-unresolved': 'off',
    'import/extensions': 'off',
    'implicit-arrow-linebreak': 'off',
    'import/prefer-default-export': 'off',
    "vue/component-name-in-template-casing": ["error", "kebab-case", {
      "ignores": []
    }],
    'prettier/prettier': ['error', { 'singleQuote': true, 'endOfLine': 'auto' }]
  },
};



*A continuación, cree un .prettierrc     archivo en la raíz de su proyecto.

{
  "semi": true,
  "singleQuote": true,
  "tabWidth": 2,
  "useTabs": false
}
