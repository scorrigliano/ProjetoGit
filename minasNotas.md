# Comandos básicos do git

Comandos extraídos do [vídeo 02](https://www.youtube.com/watch?v=UBAX-13g8OM) da Rafaella Ballerine sobre git e github.<br>
O [vídeo 01](https://www.youtube.com/watch?v=DqTITcMq68k) também é muito interessante.

## A extensão .md
.md = mark down - arquivo de marcação, instruções<br>
Readme.md = leia-me - instruções do projeto que não fazem parte do código

## Configurando um novo repositório
* `git --version` apresenta a versão do git
Como o git direto na pasta que será sincronizada:
* `git init` inicializa um repositório vazio para a pasta
Os "commits" são as versões que subimos do nosso arquivo
* `git add arquivo` deixa pronto para "subir" o arquivo 
* `git status` apresenta o ponto que o git está
* `git commit -m "mensagem"` faz o sincronismo do(s) arquivos(s) chamado(s) no comando add no repositório local
* `git branch -M "main"` troca o nome da branch para "main", que é o nome utilizado atualmente (não é mais "master")
* `git remote add origin "link do repositório - ssh"` origin é o nome ou apelido dado para o link do repositório no github ***usar o link ssh
* `git push -u origin main` sobe o(s) arquivo(s) da branch "main" para o link do "commit"

## Após alterações ou novos arquivos
* `git add .` coloca todos arquivos da pasta em stage
* `git push origin main` sobe o(s) arquivo(s) da branch "main" para o link do "commit" (não precisa do "-u")
* `git checkout -b novo-recurso` desloga da branch atual e já cria uma nova branch (que pode ser usada para testes por exemplo)
* `git checkout main` volta para a branch main
* `git merge novo-botao` junta das alterações

## Clonando repositórios e atualizando repositórios
* `git clone link` clona um repositório do git
* `git pull` (dentro da pasta do projeto) atualiza do repositório local

## Outras infos
É possível puxar um repositório git público para o seu repositório diretamente no git através da função "fork"<br>
E se ainda quiser sugerir alterações através de Contribute/Open pull request


No nosso github, a aba "Pull requests" apresenta alterações sugeridas por terceiros aos seus projetos.

## Outros comandos
Comandos extraídos de [https://www.youtube.com/watch?v=kB5e-gTAl_s&t=60s](https://www.youtube.com/watch?v=kB5e-gTAl_s&t=60s)<br>

* `git config --global user.email "email"` configura o email em uso
* `git config --global user.name "nome"` configura o nome do usuário
* `git reflog` apresenta a lista de alterações com o ID necessário para 
* `git reset --hard ID` baixa a versão indicada pelo ID
* `touch .githignore` cria um arquivo que deve ser editado com os nomes das pastas e aquivos que devem ser ignorados pelo controle de vesão

[https://www.youtube.com/watch?v=6OokP-NE49k](https://www.youtube.com/watch?v=6OokP-NE49k)
* `git commit -m "mensagem --amend"` corrige a mensagem do commit
* `git log` mostra o log de commits
* `git reset -- NOME_DO_ARQUIVO` tira do stage
* `git reset --` desfaz a última alteração no stage
* `git reset` desfaz o último commit (se o push não tiver sido feito ainda
* `git revert HEAD~2` para reverter os 2 últimos commits

