.md = mark down - arquivo de marcação, instruções
Readme.md = leia-me - instruções do projeto que não fazem parte do código

Configurando um novo repositório
*git --version* apresenta a versão do git
Como o git dirento na pasta que será sincronizada
*git init* inicializa um repositório vazio para a pasta
Os "commits" são as versões que subimos do nosso arquivo
*git add arquivo* deixa pronto para "subir" o arquivo 
*git status* apresenta o ponto que o git está
*git commit -m "mensagem"* faz o sincronismo do(s) arquivos(s) chamado(s) no comando add no repositório local
*git branch -M "main"* troca o nome da branch para "main", que é o nome utilizado atualmente (não é mais "master")
*git remote add origin "link do repositório - ssh"* origin é o nome ou apelido dado para o link do repositório no github ***usar o link ssh
*git push -u origin main* sobe o(s) arquivo(s) da branch "main" para o link do "commit"

Após alterações ou novos arquivos
*git add .* coloca todos arquivos da pasta em stage
*git push origin main* sobe o(s) arquivo(s) da branch "main" para o link do "commit" (não precisa do "-u")
*git checkout -b novo-recurso* desloga da branch atual e já cria uma nova branch (que pode ser usada para testes por exemplo)
*git checkout main* volta para a branch main
*git merge novo-botao* junta das alterações

Clonando repositórios e atualizando repositórios
*git clone link* clona um repositório do git
*git pull* (dentro da pasta do projeto) atualiza do repositório local
 
É possível puxar um repositório git público para o seu repositório diretamente no git através da função "fork"
E se ainda quiser sugerir alterações através de Contribute/Open pull request

No nosso github, a aba "Pull requests" apresenta alterações sugeridas por terceiros aos seus projetos.