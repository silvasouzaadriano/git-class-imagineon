## Básico

1. git init 
   1. Inicializa o repositório .git (NUNCA apague essa pasta)
2. git status
   1. Mostra os arquivos alterados e/ou criados
3. git add . or git add <nome do arquivo> <nome do arquivo>
   1. Adiciona os arquivos alterados e/ou criados na stagging area (para serem commitados)
4. git commit -m "<descrição do commit>"
   1. Commita os arquivos, gerando uma nova versão
5. git log
   1. Mostra todos os commits realizados
6. git show <id commit>
   1. Mostra o conteúdo de um commit


## Configurações do git

1. git config 
   1. --local (relacionado ao projeto)
   2. --global (qualquer projeto do meu usuário)
   3. --system (todos os projetos e todos os usuário da máquina)

  git config --edit (abre com VI ou VIM)
  git config --global core.editor code (abre no VSCODE)

## Atalhos

1.[alias]
  1. c = !git add --all && git commit -m
  2. s = !git status -s
  3. l = !git log --pretty=format:'%C(blue)%h%C(red)%d %C(white)%s -%C(cyan) %cn,%C(green) %cr'

## Criando repo com remote

1. gh repo create <nome do projeto> --public --source=. --remote=origin
   1. Exemplo: gh repo create git-class-imagineon --public --source=. --remote=origin