# Comandos básicos em git

Esse documento tratasse de uma anotação, sobre os comandos básicos do git, para um maior entendimento sobre o assunto acesse o link a seguir que contem o conteúdo usado nesse documento.[Curso de GIT gratuito] (https://www.youtube.com/watch?v=OuOb1_qADBQ&t=6534s).

### Configurações do git

##### Usado para definir o nome do usuário.

```
git config --global user.name "isac"
```

##### Usado para definir o e-mail do usuário.

```
git config --global user.email "isacdossantossilva@gmail.com"
```

##### Usado para definir o editor(IDE)  sub(é o editor sublime).

```
git config --global core.editor sub 
```

 

### Ler as configurações

##### Comando usado para verificar a versão do git.

```
git --version
```

##### Pesquisar o nome do usuário logado no momento.

```
git config user.name
```

##### Pesquisar o e-mail do usuário logado no momento.

```
git config user.email
```

##### Vai listar todas as configurações salvas, como por exemplo o nome do usuário, e-mail e a IDE usada.

```
git config --list
```



### Comandos Git

##### Iniciar um repositório.

```
git init 
```

##### Adicionar as alterações feitas.

```
git commit
```

##### Verifica o estado dos arquivos e repositórios( vai verificar o que foi adicionado, removido, alterado e etc.).

```
git status 
```

##### Coloca o arquivo ou diretório em questão de forma monitorada.

```
git add nome_do_arquivo
```

##### Coloca todos os arquivos novos de forma monitorada.

```
git add -A
```

##### Adicionar as alterações feitas.

```
git commit -m "Entre as (" ") vem um comentário sobre o commit"
```

##### Ver a lista de todos os commits feitos no branch.

```
git log
```

##### Coloca todos os arquivos novos de forma monitorada e adicionar as alterações feitas.

```
git commit -am "Entre as (" ") vem um comentário sobre o commit"
```

##### Lista os branch existentes no repositório. 

branch -> são as versões do seu do seu sistema

```
git branch 
```

##### Volta o arquivo a um estagio desejado, sem apagar os arquivos a frente. Ele apenas não estarão comitados.

```
git reset --soft Id_do_commit 
```

##### Funciona como o soft mais os arquivos a diante não estarão monitorados.

```
git reset --mixed Id_do_commit 
```

##### Os arquivos a frente do momento em que você desejou voltar serão apagados.

```
git reset --hard Id_do_commit 
```

##### Cria um novo branch, da um ctrl + c e ctrl + v (copia todos os arquivos e repositórios do branch atual para o novo branch criado(nome_branch)).

```
git branch nome_branch 
```

##### Munda para o branch informado.

```
git checkout nome_brach
```

##### Mostra o que você modificou dentro de um arquivo (usar antes de um commit para verificar o que foi feito).

```
git diff 
```

##### Mostra o nome do arquivo onde ocorreu a alteração recente.

```
git diff --name-only
```

##### Usado para saber o que foi alterado dentro de um arquivo especifico.

```
git diff nome_do_arquivo 
```

##### Vai desfazer as modificações feitas no arquivo selecionado( o comando altera o arquivo do branch atual).

```
git checkout HEAD -- nome_arquivo 
```

##### Adiciona um repositório remoto ao repositório local. 

```
git remote add nome_repositório link-do-repositório
```

Obs. nome_repositório é o nome que você da para, representar determinado repositório remoto, você pode escolher qualquer nome mais geralmente o mais comum é nomear como origin.

##### Mais detalhes.

```
git remote -v 
```



* fetch -> Pega as alterações do arquivo remoto (github) para o repositório local(git).

* push -> upar os arquivos/repositórios da maquina(git) para o repositório remoto (github).

  

##### Enviar os arquivos branch nome_brach para o destino nome_do_repositório_remoto.

```
git push -u nome_do_repositório_remoto nome_branch
```

##### Vai enviar o branch nome_do_branch para o servido remoto nome_do_repositório_remoto.

```
git push nome_do_repositório_remoto nome_do_branch 
```

##### Vai reverte o commit dentro no próprio pronpt de comando.

```
it revert --no- edit d138...
```

##### Deleta do repositório nome_do_repositório_remoto do branch nome_do_branch.

```
git push nome_do_repositório_remoto : nome_do_branch
```

##### Apaga o branch nome_do_branch do repositório local.

```
git branch -D nome_do_branch
```

##### Puxar os arquivos do repositório nome_do_repositório_remoto e atualizar no repositório locar no branch nome_do_branch.

```
git pull nome_do_repositório_remoto nome_do_branch
```

##### Clonar um repositório git na sua maquina.

```
git clone url_do_repositorio
```

##### Verificar o nome do repositório remoto. 

```
git remote -v 
```


