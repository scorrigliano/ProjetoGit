# Comandos básicos do git

Comandos extraídos do [video 02](https://www.youtube.com/watch?v=UBAX-13g8OM) da Rafaella Ballerine sobre git e github.

## e extensão .md
.md = mark down - arquivo de marcação, instruções
Readme.md = leia-me - instruções do projeto que não fazem parte do código

## Configurando um novo repositório
<b>*git --version*</b> apresenta a versão do git
Como o git direto na pasta que será sincronizada:
<b>*git init*</b> inicializa um repositório vazio para a pasta
Os "commits" são as versões que subimos do nosso arquivo
<b>*git add arquivo*</b> deixa pronto para "subir" o arquivo 
<b>*git status*</b> apresenta o ponto que o git está
<b>*git commit -m "mensagem"*</b> faz o sincronismo do(s) arquivos(s) chamado(s) no comando add no repositório local
<b>*git branch -M "main"*</b> troca o nome da branch para "main", que é o nome utilizado atualmente (não é mais "master")
<b>*git remote add origin "link do repositório - ssh"*</b> origin é o nome ou apelido dado para o link do repositório no github ***usar o link ssh
<b>*git push -u origin main*</b> sobe o(s) arquivo(s) da branch "main" para o link do "commit"

## Após alterações ou novos arquivos
<b>*git add .*</b> coloca todos arquivos da pasta em stage
<b>*git push origin main*</b> sobe o(s) arquivo(s) da branch "main" para o link do "commit" (não precisa do "-u")
<b>*git checkout -b novo-recurso*</b> desloga da branch atual e já cria uma nova branch (que pode ser usada para testes por exemplo)
<b>*git checkout main*</b> volta para a branch main
<b>*git merge novo-botao*</b> junta das alterações

## Clonando repositórios e atualizando repositórios
<b>*git clone link*</b> clona um repositório do git
<b>*git pull*</b> (dentro da pasta do projeto) atualiza do repositório local

## Outras infos
É possível puxar um repositório git público para o seu repositório diretamente no git através da função "fork"
E se ainda quiser sugerir alterações através de Contribute/Open pull request

No nosso github, a aba "Pull requests" apresenta alterações sugeridas por terceiros aos seus projetos.
