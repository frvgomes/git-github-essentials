Git / GitHub Enssentials

Config - Logal onde ficam armazenadas as suas credenciais:
$ git config --global user.name "Francisco Rosemberg"
$ git config --global user.email "frvgomes@gmail.com" 

Para ler todas as credenciais:
$ git config --list3

Init - Comando para inicializar o controle de versão na pasta atual.
$ git init

Ciclo de vida do status dos arquivos
untracked - arquivo não controlado pelo git
unmodified - arquivo controlado pelo git mas não foi modificado.
modified - arquivo controlado que foi modificado.
staged - arquivo pronto/adicionado para o commit.

Status - Comando para informar o status atual do git. Ele mosra branch atual, commits, arquivos 
untracked, arquivos em stage
$ git status
 
Add = Comando para adicionar arquivos no stage. 
$ git add <nome-do-arquivo> ou git add . ( para adicionar todos os arquivos )

dica: caso apareça um warnning referente ao git tentar trocar a forma de como cada linha é terminada nos arquivos do projeto, pasta usar o comando abaixo:
$ git config --global core.autocrlf false
