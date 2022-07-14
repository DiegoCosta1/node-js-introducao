# node-js-introducao

comandos utilizados:
```
$ npm init
$ npm install express
$ node app.js
$ npm install nodemon
$ nodemon app.js
```

!Problema ao tentar executar nodemon:
```
nodemon : O termo 'nodemon' não é reconhecido como nome de cmdlet, função, arquivo de script ou programa operável. Verifique a grafia do nome ou, se um caminho tiver      
sido incluído, veja se o caminho está correto e tente novamente.
```

Solução: adicionar propriedades `scripts.dev = nodemon` no arquivo de `package.json` e rodar o nodemon atráves do comando:
```
$ npm run dev
```

comandos utilizados (parte 2):

comandos utilizados:
```
$ npm install ejs
```