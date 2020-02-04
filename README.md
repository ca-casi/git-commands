## Comandos git

```
git log
git whatchanged
git whatchanged -p
```

git remote add nomedorepositorio
ou
git remote add origin - Com isso, você está indicando que o repositório Git local se conecta com um repositório remoto através do alias ou atalho origin cujo endereço real é 

***O que faz:*** Envia as alterações locais para o repositório remoto
```
git push
```

Envia as alterações locais para o repositório remoto

Outra alternativa é utilizar, no primeiro push, a opção -u ou --set-upstream. Ela atrela a branch remota à local, fazendo com que não seja mais necessário passar como parâmetros a origem e a branch no comando push, que fica então assim: git push.

git clone 

git commit -m (-m de mensagem)

git branch - lista as branchs
git branch -r - lista as branchs remotas
git branch -t design origin/design - cria a branch local lincada com a remota
git branch nomedabranch - cria um novo branch
git branch nomedabranch - cria um novo branch

git checkout -t origin/design - cria uma branch local chamada design lincada com a branch remota

git push -d origin design - remove a branch remota
git push origin :design - remove a branch remota

git fetch origin - Este comando verifica todas as atualizações que foram realizadas no repositório de atalho origin .

git mergetool --tool-help

git rebase master desenvolvimento - comano utilizado para atualizar a branch desenvolvimento com as alterações da master

git rebase --abort
git rebase --skip
git rebase --continue


git reset HEAD - vou o repositório para o estado mais recente.
git reset 19dc036cc5736fa451d7b13453ed9eaafa8e8549 - git reset + o identificador do commit retorna o repositório para este ponto.

git revert 19dc036cc5736fa451d7b13453ed9eaafa8e8549 - é utilizado para desfazer as alterações que um antigo commit fez. Ele cria um novo commit desfazendo o que foi solicitado.

git stash - guarda as alterações que não foram comitadas em uma pilha.
git stash list - lista as alterações que foram armazenadas.
git stash pop - retorna a última alteração armazenada através do stash
git stash apply - retorna a última alteração que foi feita sem deleta-lá
git stash apply stash@{0} - retorna a alteração armazenada no stash através do seu nome. Para ver o nome do stash armazenado utilizar o comando git stash list.
git stash drop - apaga as alterações que foram armazenadas.

git bisect - comando utilizado para encontrar alterações antigas que podem estar causando algum tipo de problema ... Buscando por bugs em muitos commits

Descarta as alterações do último commit:
git reset --hard HEAD~1



