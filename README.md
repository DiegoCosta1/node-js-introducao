# node-js-introducao

comandos utilizados:
```
PS> npm init
PS> npm install express
PS> node app.js
PS> npm install nodemon
PS> nodemon app.js
```

Problema ao tentar executar nodemon:
`nodemon : O termo 'nodemon' não é reconhecido como nome de cmdlet, função, arquivo de script ou programa operável. Verifique a grafia do nome ou, se um caminho tiver      
sido incluído, veja se o caminho está correto e tente novamente.`

Solução: adicionar propriedades `scripts.dev = nodemon` no arquivo de `package.json` e rodar o nodemon atráves do comando:
```
PS> npm run dev
```

comandos utilizados (parte 2):

comandos utilizados:
```
PS> npm install ejs
```

# Transformando app NodeJS em um arquivo .exe
```
PS> npm i -g pkg
PS> pkg -v
5.8.0
PS> pkg -t node16-win-x64 app.js
```
Erro: 
`pkg : O arquivo C:\Users\dg_co\AppData\Roaming\npm\pkg.ps1 não pode ser carregado porque a execução de scripts foi desabilitada neste sistema. Para obter mais informações, consulte about_Execution_Policies em https://go.microsoft.com/fwlink/?LinkID=135170.`
Solução, alterar política do power shell:
```
PS> Get-ExecutionPolicy
Restricted
PS admin> Set-ExecutionPolicy RemoteSigned
PS> Get-ExecutionPolicy
RemoteSigned
```