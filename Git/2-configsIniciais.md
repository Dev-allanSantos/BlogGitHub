## Configurações Iniciais



O git armazena as configurações em variáveis e o lugar onde essa variáveis estão armazenadas definem seu escopo. Para saber mais acesse o [capítulo 1.6 do livro Pro Git Book](https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-Configura%C3%A7%C3%A3o-Inicial-do-Git)



### Configurando sua identidade

Ao iniciar no git é importante definir algumas configurações para dizer ao git quem você é e dessa forma o git poderá identificar quem fez as alterações

```
$ git config --global user.name "nomeUsuario" //define o nome
$ git config --global user.email email@email.com // define o email
$ git config --global user.nickname usuarioNickname //define o apelido do usuario
```



### Visualizar as configurações

```
$ git config --list

user.email=allan.gama720@gmail.com
user.nickname=Dev-allanSantos
user.name=Allan dos Santos
email.name=allan.gama720@gmail.com
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
filter.lfs.clean=git-lfs clean -- %f
:
```



Também é possível pesquisar por uma variável específica:

```
$ git config user.name
Allan dos Santos
```

