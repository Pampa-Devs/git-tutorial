# **6.** Comparando e Desfazendo Modificações

## Adicionando nova modificação

Abra o seu arquivo **README.md** novamente e adicione um novo texto:
```
Meu nome é Felipe Almeida

Eu gosto de desenvolver utilizando C#
```

<br>

Mais uma vez, execute o comando **git status** para ver as alterações:
```
$ git status
On branch master
Changes not staged for commit:
    (use "git add <file>..." to update what will be committed)
    (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
```
Podemos ver que nosso arquivo esta com marcado como **modified** após a alteração.

## Comparando modificações

Sabemos que o arquivo **README.md** foi modificado, mas como sabemos exatamente o que foi modificado?


Entrando com o comando **git diff** podemos verificar exatamente o que foi alterado.
```
$ git diff
diff --git a/README.md b/README.md
index 74ca211..06ce193 100644
--- a/README.md
+++ b/README.md
@@ -1 +1,3 @@
-Meu nome é Felipe Almeida
\ No newline at end of file
+Meu nome é Felipe Almeida
+
+Eu gosto de desenvolver utilizando C#
\ No newline at end of file
```
Olhando o resultado do comando git diff, vemos que ele está mostrando tanto a versão do **README.md** anterior ao nosso **commit** quanto a alteração que acabamos de fazer.

## Voltando para o último Commit

Agora, vamos supor que essa nova linha que adicionamos sejá desnecessária. Como voltar para o nosso **último commit**?

<br>

Simplesmente digite **git reset --hard**. Este comando irá desfazer todas as modificações que você fez depois do último commit.
```
$ git reset --hard
HEAD is now at e037bf8 Adicionando arquivos em stage no repositório
```
Se você checar o seu arquivo **README.md** poderá observar que o texto dele agora está exatamente como estáva no inicio deste capítulo. Ou seja, conseguimos "voltar no tempo" com sucesso :)
```
Meu nome é Felipe Almeida
```

[**7.** Criando um Repositório Remoto &rarr;](https://github.com/Pampa-Devs/Git/blob/master/Tutorial/7-create-remote-repository.md)