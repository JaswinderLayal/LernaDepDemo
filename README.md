# LernaDepDemo


**NPM registry setup for testing**
To test locally, use [Verdaccio](https://github.com/verdaccio/verdaccio) for local NPM registry.

Install Verdaccio globally
```bash
$ yarn global add verdaccio
```

Run the registry

```bash
$ verdaccio
```

Initially, you will need to setup the account.

```
$ npm set registry http://localhost:4873/
$ npm adduser --registry http://localhost:4873
Username: <your username here>
Password: <your password here>
Email: <your email here>
```  
<br>

When you run http://localhost:4873 on your web browser you will see the interface where you can see your published packages

## Instructions

```$ npm i```

```$ npm run bootstrap```

Make some changes to text package and run ```$ npm run commit```
and then run  ```$ npm run publish```

Check http://localhost:4873/ and click on button package and see dependencies tab. Exact version of dependencies is listed in button package.json

Try this and release multiple versions and try to install exact version of button. You will see exact version of text is installed and opposed to new version



