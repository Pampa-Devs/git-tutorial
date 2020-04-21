<h1 align="center">
  <img src="/Images/git.png" alt="Git" width="220px" />
</h1>

# Git - Iniciando em Controle de Versão
*Este arquivo foi escrito em abril de 2020*


## O que é Controle de Versão?

É uma categoria de ferramentas de software que **ajuda um time de software a gerenciar mudanças no código fonte** ao longo do tempo. O software de controle de versão **controla todas as modificações no código** em um tipo especial de banco de dados. **Se um erro for cometido, os desenvolvedores podem voltar no tempo e comparar versões anteriores do código para ajudar a corrigir o erro** e minimizar a interrupção para todos os membros da equipe.

## O que é Git?

De longe, o **sistema de controle de versão moderno** mais usado no mundo hoje é o Git. O Git é um projeto de [código aberto](https://opensource.org/about), mantido ativamente, originalmente **desenvolvido em 2005 por [Linus Torvalds](https://pt.wikipedia.org/wiki/Linus_Torvalds)**, o famoso **criador do kernel do sistema operacional Linux**.

Tendo uma arquitetura distribuída, **o Git é um exemplo de DVCS** (portanto, Sistema de Controle de Versão Distribuído). **Em vez de ter apenas um único local para o histórico completo da versão do software**, como é comum em sistemas de controle de versão outrora populares como CVS ou Subversion (também conhecido como SVN), no Git, **a cópia de trabalho de todo desenvolvedor do código também é um repositório** que pode conter o histórico completo de todas as alterações.

## Inciando no Git

### 1. Repositório
Um repositório git é a pasta `.git/` dentro de um projeto. Este repositório vai mapear todas as mudanças feitas nos arquivos dos seus projetos, construindo um histórico ao longo do tempo. Isso significa que se você deletar a pasta `.git/`, automaticamente todo o histórico de mudanças de seu projeto será deletado.

Além disso, existem dois tipos de repositório no `git`, o **local** e o **remoto**:
* O **local** é o repositório que fica na sua máquina de trabalho. Ele é criado utilizando o comando `git init` dentro da pasta do projeto.
* O **remoto** fica em um servidor como GitHub, GitLab, BitBucket, entre outros.

<h1 align="center">
  <img src="/Images/git_repository.png" alt="Git" width="420px" />
</h1>

### 2. Branch
A **Branch** é uma **ramificação** do seu projeto. 

Pense no seguinte: você é o desenvolvedor de um site e recebe a tarefa de adicionar uma nova página no mesmo. 

Para não causar problemas no site que as pessoas utilizam, você cria uma ramificação do site **(branch master)** no seu computador **(branch local de desenvolvimento)** para então adicionar as mudanças. Ao terminar o seu trabalho, você simplesmente envia suas mudanças para o site, devolvendo a sua ramificação de volta para sua origem.

<h1 align="center">
  <img src="/Images/git_branch.png" alt="Git" width="620px" />
</h1>

### 3. Stage e Commit
Colocar um arquivo em **stage** significa que ele está  **pronto para ser enviado ao repositório**. Você faz isso utilizando o comando `git add nome_arquivo`.
O Git permite que você entregue somente as partes de sua alterações que estão prontas. Isso se chama colocar um arquivo em `stage`.
<br>
Após colocar os seus arquivos em **stage** está na hora de fazer o **commit**. Ao fazer um `git commit -m "mensagem_do_commit"` você está enviando todas as mudanças que estão em `stage` para o repositório local.

<h1 align="center">
  <img src="/Images/git_stage.png" alt="Git" width="420px" />
</h1>

### 4. Histórico
Utilizando o comando `git log` conseguimos ver todos os **commits** feitos dentro do seu repositório, mostrando a data e o autor do mesmo.

<h1 align="center">
  <img src="/Images/git_history.png" alt="Git" width="500px" />
</h1>

### 4. Pull
Assim como podemos enviar nossas modificações para um **repositório remoto**, podemos atualizar o nosso **repositório local** com a versão mais atual do **repositório remoto**. Conseguimos fazer isso utilizando o comando `git pull`.

### 5. Merge
É o `ato de fundir duas branches` (ramificações). Quando você terminar o seu trabalho, você irá fazer um `git merge` para fundir a sua branch com a branch master.

<h1 align="center">
  <img src="/Images/git_merge.png" alt="Git" width="750px" />
</h1>

# Mão na Massa!

Depois de toda essa aula teórica, imagino que você gostaria de algo mais prático não? 

Pois então, criei alguns pequenos tutoriais abordando todos os conceitos acima:

<br>

1. [Instalando e configurando o **Git**](https://github.com/Go-Horse-Coding/Git/blob/master/Tutorial/1-install-git.md)
2. [Criando um **Repositório Git Local**](https://github.com/Go-Horse-Coding/Git/blob/master/Tutorial/2-create-repository.md)
3. [Fazendo Modificações](https://github.com/Go-Horse-Coding/Git/blob/master/Tutorial/3-make-modifications.md)
4. [Conferindo o **Status** do repositório](https://github.com/Go-Horse-Coding/Git/blob/master/Tutorial/4-check-status.md)
5. [Colocando as Modificações em Stage e Fazendo Commit](https://github.com/Go-Horse-Coding/Git/blob/master/Tutorial/5-adding-to-stage.md)
6. [Comparando e Desfazendo Modificações](https://github.com/Go-Horse-Coding/Git/blob/master/Tutorial/6-undoing-changes.md)
7. [Criando um Repositório Remoto](https://github.com/Go-Horse-Coding/Git/blob/master/Tutorial/7-create-remote-repository.md)
8. [Enviando as Modificações para o Repositório Remoto](https://github.com/Go-Horse-Coding/Git/blob/master/Tutorial/8-pusing-to-remote-repository.md)
9. [Fazendo Modificações Diretamente no Repositório Remoto](https://github.com/Go-Horse-Coding/Git/blob/master/Tutorial/9-make-modifications-remote.md)
10. [Atualizando o Repositório Local](https://github.com/Go-Horse-Coding/Git/blob/master/Tutorial/10-pulling-modifications-remote.md)

# Desafio

Agora está na hora de colocar tudo o que você aprendeu em prática. Criamos um desafio simples, porém irá exigir que você clone um repositório localmente, altere um arquivo, adicione esse arquivo em stage, utilize o commit e por fim o push para enviar as mudanças para o servidor.

<br>

**O objetivo é adicionar o seu nome no seguinte arquivo: [NAMES.md](https://github.com/Go-Horse-Coding/Git/blob/master/NAMES.md).**

<br>

Para fazer isso você vai precisar seguir esses passos:
1. Realize um **Fork** deste projeto clicando no botão **Fork** no parte superior direita desta página.
2. Clique em **Clone or download** e copie a url 
3. Em uma pasta em seu computador, abra o **Git Bash** e digite ´git checkout´ junto da url copiada
```
$ git checkout https://github.com/seu_usuario_git/git-tutorial.git
```
4. Entre na pasta recém criada, **git-tutorial** e adicione o seu úsuario do GitHub no arquivo **NAMES.md**.
5. Envie suas alterações para o seu repósitório **Fork**
```
$ git add .
$ git commit -m "Adicionei o meu usuário github"
$ git push
```
6. Volte para [esta página](https://github.com/Go-Horse-Coding/git-tutorial) e clique em **Pull Requests** na parte superior.
7. Crie um novo **Pull Request** clicando em **New pull request** e onde diz **compare:** selecione o repositório **fork** que você criou.
8. Envie o **Pull Request**. Se tudo estiver correto um moderador irá aprovar e o seu nome irá aparecer no **NAMES.md**


# Autores
* [Felipe Almeida](https://github.com/felipe-allmeida) - Fundador do GoHorse Coding e Engenheiro de Software

# Agradecimentos especiais
Todos nessa lista contribuiram de alguma forma seja revisando, achando sinônimos. Basicamente alguma coisa que tornou o tutorial mais simples de se ler :)
* [usaruki](https://github.com/usaruki) - Por revisar todo o material inúmeras vezes de madrugada
* [gvdamian](https://github.com/gvdamian)
* [mpplayer1](https://github.com/mpplayer1)

# Referências
* https://help.github.com/en/github/getting-started-with-github/quickstart
* https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control
* https://www.atlassian.com/git/tutorials/learn-git-with-bitbucket-cloud
* https://medium.com/@programadriano/git-para-iniciantes-3b38fa5d4ddf
* https://githowto.com/pt-BR
* https://guide.freecodecamp.org/git
