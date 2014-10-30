# Research on Git Commit Messages #

----------

## Setup ##

1. Copie o arquivo new-commit.conf para o repositório atual que está trabalhando. Faça as modificações necessárias se for o caso.
2. Coloque a pasta do projeto git-new-commit no path. Digite no console: `PATH=$PATH:<caminho>`. Exemplo: PATH=$PATH:/D/GitHub/git-new-commit
3. Para executar, digite: `git new-commit` 

Setando variáveis de ambiente OSX
http://stackoverflow.com/questions/135688/setting-environment-variables-in-os-x

## Instruções ##

O git-new-commit substitui o comando `git commit -m` oficial do git por um novo processo de construção da mensagem de commit. O processo é o mesmo:

Adicione os arquivos a serem comitados

    git add --all

Insira a mensagem de commit


    git new-commit

Sincronize o repo


    git push

## new-commit.conf ##

**Elementos**:

Adicione ou remova elementos para o processo de construção da mensagem de acordo com suas necessidades. 

    elements = ["Label", "SubProject", "Summary", "Remarks", "Files"]

- Label: Insere uma label pre-definida (ver labels)
- SubProject: Insere uma subpasta baseado em uma regex para demarcar um subproject
- Summary: Insere uma mensagem resumida sobre a ação
- Remarks: Insere comentários adicionais
- Files: Insere arquivos modificados

**Labels**:

    labels = ["BUGFIX", "NEWFEATURE", "REFACTORING", "OPTIMIZATION", "CLEANING", "MISC"]

**Descripts**:

Adiciona descrições para cada label facilitando seu entendimento

    descripts = ["General fix", "Adding new capabilities", "Restructuring code without changing behavior", "Make it  work more efficiently or use fewer resources", "Remove unused code", "Anything else"]

**SubProject**

Adiciona um subprojeto na mensagem. Para ativar, coloque o elemento "SubProject" em elements e modifique o campo do regex de acordo com a pasta do seu projeto 

    subprojectregex = "src/([a-zA-Z]+)/.*"






 
