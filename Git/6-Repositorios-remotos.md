<div align="center"><h2>Repositórios remotos </h2></div>



Repositórios remotos são cópias do seu repositório git local hospedados em algum lugar da internet como por exemplo no GitHub. Essas cópias permitem aos outros desenvolvedores ter acesso ao projeto e colaborar com o trabalho.



Para começar a contribuir com repositórios remotos , nós precisaremos passar para o Git a url que representa o endereço de onde está o repositório remoto juntamente com o comando `git remote`.



`git remote add <apelido-repo> <url>`

**Exemplo**

```
$ git remote add origin https://github.com/Dev-allanSantos/BlogGitHub.git
```



a palavra **origin** é como o git apelida a url do repositório remoto. Origin é a palavra padrão, mas você pode digitar qualquer palavra





Agora que o repositório local esta conectado ao repositório remoto é possível realizar pelo menos essas duas ações:

- **push :** enviar o repositório local para o repositório remoto

`git push <apelido-repo> <branch>`

```
git push origin master // enviei minhas alterações para a branch principal
```



- **pull :** resgatar as alterações feitas no repositório remoto para o repositório local.

`git pull <apelido-repo> <branch>`

```
git pull origin master
```





#### A diferença entre o comado fetch e o pull 

esses dois comandos recuperam o estado do projeto hospedado no repositório remoto, no entanto fazem isso de diferentes formas. O comando `git fetch` não altera seu repositório local com as mudanças que ele baixou do repositório remoto. Para que o projeto local absorva essas alterações é necessário fazer um merge após o comando `git fetch`.

O comando git pull recupera as mudanças do repositório remoto e já as integra no diretório local. Essa é a principal diferença entre esses dois comandos.



#### Renomear e apagar repositórios remotos

Para renomear a referência de um repositório remoto , use `git remote rename`:

```
$ git remote rename pb paul //renomeia de pb para paul
```



Para apagar a referência a um repositório remoto, use :

```

$ git remote remove paul // apaga a referência ao repositório paul
```

