This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## ReactJS - `Utilizando React Hooks`

Treinamento BootCamp - Diminuindo a verbosidade excessiva <br>
`React Hooks` é uma API que ajuda a dimninuir a verbosidade na parte de compartilhamento de informações entre componentes, estado e ciclo de vida. 

**Nota: Você pode colocar uma nota qualquer aqui!**


### `Documentação` passo a passo

## Excluir os comentários e o arquivo 
manifest.json

## Excluir esses e zelar para evitar os erros -  remover as referências
App.css <br>
App.test.js <br>
index.css <br>
logo.svg <br>
serviceWorker.js <br>

## Gerando o arquivo `.editorConfig`
Botão direito nos arquivos em uma área livre e escolher 'Generator .editorConfig' <br>
Será gerado o arquivo <br>

## Adicionado `eslint` - versão específica
yarn add eslint@^6.6.0 -D

## Inicializando o `eslint`
yarn eslint --init <br>
Responda as perguntas conforme abaixo: <br>
? How would you like to use ESLint? To check syntax, find problems, and enforce code style <br>
? What type of modules does your project use? JavaScript modules (import/export) <br>
? Which framework does your project use? React <br>
? Does your project use TypeScript? No <br>
? Where does your code run? Browser <br>
? How would you like to define a style for your project? Use a popular style guide <br>
? Which style guide do you want to follow? Airbnb: https://github.com/airbnb/javascript <br>
? What format do you want your config file to be in? JavaScript <br>
Checking peerDependencies of eslint-config-airbnb@latest <br>
Responsa 'Y' para tudo o que for questionado e aguarde a instalação.<br>

## Ajustando o `eslint`
Talvez aqui tenha que ajustar a versão do eslint pois na instalação acima tenha sido feito downgrade <br>
yarn add eslint@^6.6.0 -D

## Instalando `pretier` - deixa o código mais bonito - eslint procura erros (ausência de pontos)
yarn add prettier eslint-config-prettier eslint-plugin-prettier babel-eslint -D

## Certifique que o arquivo `.editorConfig` esteja assim
root = true <br>
[*] <br>
end_of_line = lf <br>
indent_style = space <br>
indent_size = 2 <br>
charset = utf-8 <br>
trim_trailing_whitespace = true <br>
insert_final_newline = true <br>

## Arquivo `eslintrc.js`
extends: [
    'plugin:react/recommended',
    'airbnb',
    'prettier',
    'prettier/react',
  ],
  
  plugins: [
    'react',
    'prettier',
    'react-hooks'
  ],
  
  rules: {
    'prettier/prettier':'error',
    'react/jsx-filename-extension' :[
      'warn',
      { extensions: ['.jsx','.js']}
    ],
    'import/prefer-default-export': 'off',
    'no-param-reassign': 'off',
    'no-console': ['error',{ allow: ['tron']}],
    'react-hooks/rules-of-hooks':'error',
    'react-hooks/exhaustive-deps': 'warn'
  },

## Instalando plugin do `eslint` próprio para usar os hooks
yarn add eslint-plugin-react-hooks -D


## Rodando a aplicação - essa configuração está no `package.json`
yarn react-scripts start

### Site
https://skylab.rocketseat.com.br/node/utilizando-react-hooks/lesson/configurando-estrutura-2

### Local
C:\Temp\Bootcamp2019\bootcamp_modulo08