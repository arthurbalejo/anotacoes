NAO ESQUECER DO SUDO
#### para iniciar o git em uma pasta basta navegar até ela e utilizar o comando: 
- 'git init'
#### para criar arquivos se usa o touch, ex:
- 'touch texto.txt'
#### para ver o estatus dos arquivos no git o comando eh:
- 'git status'
#### para adicionar os arquivos ao estage antes do commit eh:
- 'git add <nome_do_arquivos>'
#### para remover arquivos do estage eh:
- 'git rm --cached <nome_do_arquivos>'
#### para adicionar todos os arquivos ao stage eh:
- 'git add .'
#### para commitar eh:
- 'git commit -m <descricao>'
#### para ver o historico das modificacoes
- 'git log'
- 'git log --oneline' para menos informacao
####  para voltar a uma versão anterior
- git checkout <codigo do commit>
####  para ir ao ultimo ponto
- git checkout <nome do branch>
#### para alterar o historico sem alterar a originalidade
- git revert <codigo do commit>
#### revert eh para voltar no tempo
- git reset <codigo do commit>
- revert eh para voltar no tempo (perigoso) limpa todo historico futuro
- git reset <codigo do commit> --hard
#### gitignore muito importante para ambientes virtuais
- criar arquivo '.gitignore' e escrever o nome do arquivo a ser ignorado
#### branch: como vamos adicionar uma funcionalidade ao nosso programa não adicionamos no arquivo original, para isso existe o branch. criamos uma linha do tempo parela para testarmos a funcionalidade nova. depois de adicionada e testada fundimos o branch com o arquivo principal
- "git branch" mostra todos os branchs
- "git branch <nome branch>" cria um branch novo
- 'git checkout test' entra no branch criado
- 'git branch -D <nome do branch>' para deletar branch
#### merge: entrar no arquivo principal e dar um merge com o branch que será fundido
'git merge <nome_do_branch>'
mesmo depois de ter dado merge da para continuar trabalhando no branch sem interferir no arquivo original.
se alguem alterar o arquivo que tu esta utilizando no branch, na hora do marge vai dar conflito e preicsa ser resolvido manualmente
origin para criar apelido do endereço github
- 'git push origin <endereço_projeto_github>'
#### para ver qual o origin que esta
- 'git remote -v'
#### agora é só colocar
- 'git push origin <nome do branch>'
#### para clonar um projeto
- 'git clone <link do projeto> <nome pasta que sera criada(opcional)>'
#### para apagar uma pasta mesmo contendo arquivos
- 'rm -rf <nome da pasta>'
####quando clonamos ele ja adiona a origin
modo de criar um branch e ja mudar para ele
- 'git checkout -b <nome branch>'
#### equivalente a:
- 'git branch <nome branch>'
- 'git checkout <nome branch>'
#### para adicionar o repositório ao origin
- 'git remote add origin <endereçoSSH_rep>'

