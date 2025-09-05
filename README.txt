O que é o GIT?
É um sistema de controle de versão, que funciona por meio de comando digitados no terminal.
Controla versões de projetos em qualquer linguagem: Python, C#, Java, até documentos de texto, imagens, jogos, etc.

O que é Shell?
É uma tela de comando.
É um interpretador de comandos que serve como ponto entre o usuário e o sistema operacional. Exemplo: Bash, Zsh, PowerShell.

O que é Bash?
É uma tela de comando para Linux e Mac.

O que é Terminal?
Janela para você digitar os comandos.
É o programa que abre o Shell.

O que é Linha de Comando (CLI - Command Line Interface)?
Quando você usa o computador escrevendo comando, em vez de clicar em botões.
CLI é a interface textual do computador, oposta ao GUI (Grphical User Interface). 

git init        | Criar um repositório
cd              | Change directory
git status      | Verificar o status do git
git add .       | Adicionar arquivos ao projeto
git commit -a   | 
-m              | Enviar uma mensagem após o commit
git push        | Enviar código ao REPO remoto
git pull        | Receber alteração do REPO
git clone       | Clonar REPO (Quando já estão criados) . PARA SER NO DIRETÓRIO ATUAL

git rm          | removendo arquivos do REPO
git log         | modificações feitas no projeto
git checkout    | arquivo modificado pode ser retornado ao estado original
Criar um arquivo com nome .gitignore você pode por nome dos arquivos antes de criar nele para ser ignoradas de enviar ao REPO, e se colocar /* é todo os arquivos dentro da pasta
git reset --hard origin/main | resseta mudanças feitas
git branch | 
git branch -d | 
git checkout <nome> | muda de branch
git checkout -b <nome> | Cria um novo branch e também muda já pra ele
git merge <nome>  | merge com o branch atual e o citado.