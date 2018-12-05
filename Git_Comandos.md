# =======	Comandos úteis	==========

#Lista das insformações do GIT.

``git config --list``


#Comando responsável por inicializar o repositório e ficar enxergando todas as mudanças que houver dentro do projeto.

``git init``

#Informa o status do repositório.

``git status``

#O Git adiciona o arquivo e passa a reconhecê-lo, caso esteja com o status Untracked, no exemplo acima apontamos o arquivo chamado Jenkinsfile.

``git add Jenkinsfile`` 

#O Git  irá adicionar todos os arquivos que estiver dentro do diretório e passa a reconhecê-lo, caso esteja com o status Untracked, no exemplo acima apontamos o arquivo chamado Jenkinsfile.

``git add .``


#Comando para comitar o arquivo e, o -m significa que no ato será escrito um comentário.

``git commit -m "(comentário)"``

#Exibe o log como hash do commit.

``git log``

#Exibe com mais informações. 

``git log --decorate``

#Exibirá todos os commit feito pelo autor inserido.

``git log --author="nome do autor"``

#Exibirá em ordem alfabética de autores, o número de commit feito e quais os nomes de cada.

``git shortlog``

#Exibirá o que foi alterado no commit através da hash.

``git show + (hash)``

#Exibe as alterações feitas no arquivo antes mesmo de ser feito o commit. Comando muito importante para revisar suas alterações antes do COMMIT.

``git diff``

#Exibe todos os arquivos que foram alterados.

``git diff --name-only``

#Comando utilizado para desfazer alguma alteração no arquivo antes de ter feito o reconhecimento do arquivo dentro do repositório (git add).

``git checkout (+ nome do arquivo)``

#Desfaz a alteração do arquivo mesmo após o reconhecimento do arquivo no repositório ( após o git add )

``git reset HEAD (+ nome do arquivo)``

#Desfaz o comit mas...
``git reset --soft (+ hash)``
 
#Desfaz...

``git reset --mixed (+ hash)``

#Deve ser usado apenas se houver certeza, pois ele altera o histórico do commit.

``git reset --hard ( + hash)``

#Comando para adicionar um novo repositório remoto.

``git remote add (+crie um nome)``

#Esse comando é utilizado para fazer o upload dos arquivos alterados para o GitHub

``git push origin (origin é o nome do repositório)  master (master é o nome da branch)``

#Esse comando é utilizado para realizar o Download das alterações quando são feitas através do GitHub.

``git pull origin (origin é o nome do repositório) master (master é o nome da branch)``

#Cria uma nova Branch chamada teste ou se ja existir ele muda para a Branch digitada.

``git checkout -b teste``

#Lista as Branch existentes

``git branch``

#Apaga a Branch chamada teste

``git branch -D teste``

#Criando um arquivo .gitignore é possível bloquear quaisquer arquivos para fazer o upload no GitHub. Esse bloqueio pode ser feito através do nome direto do arquivo ou bloqueando a extensão do mesmo. Exemplo: Supondo que dentro do repositório há diversos arquivos .json e você não quer que o mesmo vá para a área pública, portanto, crie o arquivo dentro do mesmo repositório .gitignore e dentro dele adicione *.json .

``.gitignore``

#Comando utilizado para salvar o seu arquivo alterado mas que ainda não esta pronto para comitar, ou seja, o mesmo esta em WIP (working in progress). 

``git stash``


#Ele aplica as mudanças que você havia inserido e, agora, irá aparecer como arquivo alterado após rodar um git status como por exemplo. Após as devidas alterações o arquivo pode ser comitado.

``git stash apply``

#Limpa as informações que estão no stash.

``git stash clear``

#É possível criar alias dentro do Git, nesse caso, o comando acima configura um alias para o comando git status, o mesmo ficará como git s. git config(seta configuração) --global (modo global) alias.s (determina a letra s) status (comando configurado no alias).

``git config --global alias.s status``


#Comando para criar uma TAG.

``git tag -a 1.0.0 -m "Nova Tag"``

#Comando para fazer o push da tag criada.

``git push origin master --tags``

#Listando as branch's locais e remotas

``git branch -a``


