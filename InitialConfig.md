1. Instalar as seguintes dependências:

* <code>yarn add -D @babel/core @babel/preset-env @babel/preset-react webpack webpack-cli babel-loader webpack-dev-server style-loader css-loader file-loader @babel/plugin-proposal-class-properties</code>

* <code>yarn add react react-dom prop-types</code>

2. Criar e configurar o arquivo <i>babel.config.js</i>(ver no arquivo)

3. Criar e configurar o arquivo <i>webpack.config.js</i> para gerar o bundle. Criar a pasta <i>public</i> na raiz.

4. Criar a pasta <i>src</i> na raiz e dentro dela o arquivo <i>index.js</i>, é o arquivo de entrada da aplicação.

5. Adicionar no <i>package.json</i> o seguinte script:
<code>
  "scripts": {
    "build": "webpack --mode producion",
    "dev": "webpack-dev-server --mode development"
  },
</code>

6. Criar o arquivo <i>index.html</i> na pasta <i>public</i>

7. Configurar o <i>webpack-dev-server</i>:

1.1. Ver código no arquivo.
1.2. Sempre que adicionar um loader via npm, ou yarn, lembre-se de adicionar também nas configuraÇões deste arquivo.