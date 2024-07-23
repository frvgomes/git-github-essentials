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
	
Reset - Comando para desfazer um commit que realizado de forma errada.
	Atenção: a hash enviada no comando deve ser a do commit anterior ao que vc deseja afetar.
	Opções:
	 -- soft Retorna os arquivos para o stage.
	 -- mixed Retorna os arquivos para modified
	 -- hard Retorna os arquivos para versão inicial antes de qualquer alteração.
$ git reset --soft 767c54afb14c58ea64a8d3e8f05c8145c3af442b

Branch - Comando para manipular branchs
	Opções:
	-b Criar uma nova branch ( $ git checkout -n nova-branch )
	branch lista as branchs ( $ git branch )
	checkout Navegar entre branchs ( $ git checkout branch-pra-onde-vou )
	-D Deletar uma branch ( $ git branch -D branch-pra-deletar )
