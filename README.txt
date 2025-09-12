Conceitos Fundamentais
Git: Um sistema de controle de versão distribuído que rastreia as alterações no código-fonte durante o desenvolvimento de software. Ele funciona por meio de comandos no terminal.
GitHub: Uma plataforma de hospedagem de código para controle de versão e colaboração, que usa o Git.
Shell: É um interpretador de comandos que atua como a interface entre o usuário e o sistema operacional. Exemplos incluem Bash, Zsh e PowerShell.
Bash: Um tipo de Shell comum em sistemas operacionais baseados em Unix, como Linux e macOS.
Terminal: É o programa ou janela que permite acessar e usar o Shell, onde os comandos são digitados.
Linha de Comando (CLI - Command Line Interface): A interface textual do computador, onde você digita comandos em vez de usar um mouse para clicar em botões. É o oposto da GUI (Graphical User Interface).
Repositório (Repo): O local onde o Git armazena todas as informações do projeto, incluindo os arquivos e o histórico de alterações.

Comandos Git Essenciais
git init	Cria um novo repositório Git no diretório atual.
git clone <link>	Clona um repositório existente para o seu computador.
git status	Exibe o estado do repositório, mostrando quais arquivos foram modificados, adicionados ou excluídos.
git add .	Adiciona todas as alterações feitas no diretório de trabalho para a "área de staging" (preparação).
git add <nome-do-arquivo>	Adiciona apenas um arquivo específico para a "área de staging".
git commit -m "mensagem"	Salva as alterações da "área de staging" no repositório com uma mensagem descritiva.
git commit -a -m "mensagem"	Adiciona e salva as alterações de arquivos já rastreados em um único comando.
git push	Envia os commits locais para o repositório remoto.
git pull	Baixa e mescla as alterações do repositório remoto para o seu repositório local.
git log	Exibe o histórico de commits do repositório.
git rm <arquivo>	Remove um arquivo do repositório e do sistema de arquivos.
git diff	Exibe as diferenças entre o diretório de trabalho e a "área de staging".
git checkout -- <arquivo>	Descarta as alterações feitas em um arquivo específico, retornando-o ao estado do último commit.
git reset --hard origin/main	Reseta o repositório local para o estado do branch main remoto, descartando todas as alterações locais não comitadas.
git revert <commit-hash>	Cria um novo commit que desfaz as alterações de um commit anterior. É uma forma segura de desfazer mudanças.
git reset <commit-hash>	Desfaz commits, mas mantém as alterações no diretório de trabalho. Útil para reverter um commit sem perder o código.
.gitignore	Um arquivo de texto que lista arquivos e pastas que o Git deve ignorar (não rastrear). Coloque /* para ignorar todo o conteúdo de uma pasta.

Comandos para Branches
git branch	Lista todos os branches locais no repositório.
git branch <nome-do-branch>	Cria um novo branch.
git checkout <nome-do-branch>	Muda para o branch especificado.
git checkout -b <nome-do-branch>	Cria e muda para um novo branch em um único comando.
git merge <nome-do-branch>	Mescla o branch especificado com o branch atual.
git branch -d <nome-do-branch>	Exclui o branch especificado.
git diff <branch1>..<branch2>	Exibe as diferenças entre dois branches.
git merge --abort	Aborta um processo de merge que resultou em conflitos.

Gerenciamento de Histórico e Remoto
git remote add origin <link>	Adiciona um repositório remoto ao seu repositório local.
git remote -v	Lista os repositórios remotos configurados no projeto.
git remote remove <nome>	Remove um repositório remoto.
git fetch	Baixa as alterações do repositório remoto, mas não as mescla com o branch local.
git pull --rebase	Recebe as alterações do repositório remoto e aplica os seus commits locais sobre eles.
git stash	Salva temporariamente as alterações não comitadas. Útil para mudar de branch sem perder o progresso.
git stash list	Exibe a lista de stashes salvas.
git stash apply <stash@{n}>	Aplica as alterações de um stash específico (n é o número do stash na lista).
git stash drop <stash@{n}>	Exclui um stash específico da lista.
git stash clear	Exclui todos os stashes.
git tag -a <nome> -m "mensagem"	Cria uma tag (um "rótulo" para um commit específico) com uma mensagem.
git show <nome-do-branch-ou-tag>	Exibe detalhes sobre um commit, branch ou tag.
git push origin <nome-da-tag>	Envia uma tag específica para o repositório remoto.
git push origin --tags	Envia todas as tags para o repositório remoto.
git submodule add <link> <diretorio>	Adiciona um repositório Git como um submódulo em outro repositório.

git shortlog | log resumido do REPO do projeto, quem está mexendo no código, nome dos autores nque deram os commit
git clean | vai verificar e limpar arquivos não estão sendo trackeados
git gc | liverar memoria sendo utilizada desnecessariamente, faz uma manutenção no REPO
git fsck | Comando de rotina para verificar se existe corrupções em arquivos
git reflog | mapeia todos os passos que demos no REPO, até uma mudança de branch é inserida no log
git archive --formate zip --output main_files.zip main | transforma o REPO em um arquivo compactado
