# **5.** Colocando as modificações em **Stage** e fazendo **Commit**

## Adicionando o README.md em stage

Ao adicionar um arquivo em **stage**, você está dizendo que ele está pronto para ser enviado ao **repositório local**. 
<br>
<br>
Existem duas maneiras para fazer isso:

1. Adicionando um arquivo individualmente:
```
$ git add README.md
```
2. Adicionando todos os arquivos que sofreram modificações:
```
$ git add .
```

Após adicionar o arquivo README.md em **stage**, execute novamente o comando **git status**:
```
$ git status
On branch master

No commits yet

Changes to be commited:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md
```

Agora a mensagem que antes era **Untracked** mudou para **Changes to be committed**. 

## Fazendo Commit dos arquivos em **stage**

Com o nosso arquivo adicionado com sucesso em **stage**, podemos finalmente enviar o mesmo para o repositório  local utilizando o **commit**:
```
$ git commit -m "Adicionando arquivos em stage no repositório"
[master (root-commit) 15f1691] Adicionando arquivos em stage no repositório
1 file changed, 0 insertions(=), 0 deletions(-)
create mode 100644 README.md
```

Ao utilizar o comando **git commit** para enviar o **README.md** ao repositório local, você incluiu a flag **-m** que permite um comentário na linha de comando. 
Ou seja, para cada commit você pode adicionar uma mensagem diferencida explicando qual o objetivo do mesmo.

<br>

Executando o comando **git status** novamente você verá o seguinte:
```
$ git status
On branch master
nothing to commit, working tree clean
```
O diretório de trabalho agora está limpo pois suas alterações foram enviadas ao repositório local!

[6. Criando um Repositório Remoto &rarr;](https://github.com/Go-Horse-Coding/Git/edit/master/Tutorial/6-create-remote-repository.md)
