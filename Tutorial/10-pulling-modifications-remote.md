# **10.** Atualizando o Repositório Local

No capítulo anterior, adicionamos modificações no arquivo **README.md** em nosso repositório remoto. Agora vamos atualizar nosso **repositório local** com essas alterações.

<br>

Para isso, abra a **CLI do GitBash** dentro da pasta do seu projeto **git4noobs** e digite o `git pull` para atualizar o seu repositório local:

```
$ git pull
remote :Enumerating objects: 5, done
remote: Counting objects: 100% (5/5), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 663 bytes | 6.00 KiB/s, done.
From https://github.com/felipe-allmeida/git4noobs
    e037bf8..facc6a7    master      -> origin/master
Updating e037bf8..facc6a7
Fast-forward
    README.md | 4 +++-
    1 file changed, 3 insertions(+), 1 deletion(-)
```

Abra o seu arquivo **README.md** no seu **repositório local** e veja que as alterações que você fez no **repositório remoto** estarão dentro do arquivo.

<br>

Isso quer dizer que agora o seu **repositório local** está igual ao **repositório remoto**. 

<br>

Com isso chegamos ao final de nosso tutorial, espero que você tenha aproveitado!

[&larr; Voltar a página inicial](https://github.com/Go-Horse-Coding/git-tutorial/blob/master/README.md)
