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

Commit - Comando para empacotar todos os arquivos em stage e salvá-los na branch atual.
$ git commit -m "Mensagem do commit"
 
Log - Comando para listar os commits realizados na branch atual.
$ git log 
Opções:
	--decorate exibe mais informaóes do log
	--author="parte-do-nome" para buscar pelo author
	shortlog exibe o log resumido por autor ( $ git shortlog )
	


Dica: Caso receba o alerta "in the working copy of 'readme.md', LF will be replaced by CRLF the next time Git touches it
" isso significa que o git vai tentar modificar a forma como os arquivos do projeto terminam em funçao do sistema operacional.
Para ocultar a mensagem use o comando abaixo:
$ git config --global core.autocrlf false
