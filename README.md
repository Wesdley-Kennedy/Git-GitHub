


# Git & GitHub

Anotações sobre Git e GitHub do curso de versionamento de código [Java com Spring Boot Claro](https://web.dio.me/track/coding-the-future-claro-java-spring-boot) na DIO.

## 📚 Documentação:
- [Documentação Git](https://git-scm.com/docs/git/pt_BR)

- [Documentação GitHub](https://docs.github.com/pt/get-started)

## ✍️ Anotações:

- O que é versionamento de código: O  versionamento é uma maneira organizada de administrar mudanças, criando versões. Seja em um documento de texto ou software, a cada incremento, teremos uma nova versão daquilo que estamos criando, pois estamos inserindo algo que não estava lá anteriormente. Nesse sentido, o versionamento atua criando um histórico das mudanças realizadas, que pode ser acessado e utilizado para recuperar alguma versão específica.

- O que uma Branch: Branch é uma ramificação no git é um ponteiro para as alterações feitas nos arquivos do projeto. É útil em situações nas quais você deseja adicionar um novo recurso ou corrigir um erro, gerando uma nova ramificação garantindo que o código instável não seja mesclado nos arquivos do projeto principal. Depois de concluir a atualização dos códigos da ramificação, você pode mesclar a ramificação com a principal, geralmente chamada de Main.
- O git não reconhece pastas com seu diretório vazio, para que seja reconhecido devemos adicionar algum arquivo dentro da pasta vazia.




## ⌨️ Comandos Essenciais Git:

- git help

Existem inúmeros comandos no Git, muito mais do que os 25 dessa lista, cada um com sua função, parâmetros e características. Felizmente, o próprio Git tem o comando help para trazer ajuda diretamente no terminal.

- git init

Esse é o comando que você irá utilizar para criar um novo projeto de git. O comando irá criar um repositório novo em branco e, a partir daí, será possível armazenar seu código fonte, alterar, salvaguardar alterações etc.

- git clone

Esse comando Git cria uma cópia exata de um repositório já existente.
Então… quando usar git init e quando usar git clone? O git clone é mais avançado, uma vez que ele mesmo executa um comando git init internamente. Além disso, ele verifica todo o conteúdo do projeto.

- git add

Esse comando Git adiciona os arquivos especificados de código ao seu repositório, sejam arquivos novos ou arquivos anteriores que foram alterados. Oferece diferentes possibilidades de sintaxe.

- git commit

É fundamental se estabelecer uma diferença entre git add e git commit:
git add adiciona seus arquivos modificados à fila para serem submetidos a um commit posteriormente. Os arquivos não passaram por um commit.
O git commit executa o commit dos arquivos que foram adicionados e cria uma nova revisão com um log. Por outro lado, se você não adicionar nenhum arquivo, o git não fará o commit de nada.
É possível combinar as duas ações em um único comando: $ git commit -a.
Também é possível adicionar uma mensagem para a execução de um commit. Exemplo:

$ git commit -m “seu comentário”

- git branch

É comum na maior parte do tempo possuir múltiplas variações em seu repositório Git, chamadas de branches (“ramificações”). A grosso modo, um branch é um caminho independente de desenvolvimento, uma alternativa.
A princípio pode parecer fácil se perder em diversos caminhos, mas o comando git branch facilita o gerenciamento de tudo isso. Com diferentes parâmetros, é possível listar, criar ou apagar os branches.
Exemplos:

$ git branch (lista todas as ramificações)
$ git branch <nome_do_branch> (cria um branch com o nome especificado)
$ git branch -d <nome_do_branch> (deleta o branch com o nome especificado)

- git checkout

Ainda sobre branches, esse comando Git pode ser utilizado para trocar de uma ramificação para outra.

- git remote

O comando Git remote estabelece uma conexão entre seu repositório local e um repositório remoto.

- git push

Esse comando serve para subir suas modificações para um repositório remoto conectado anteriormente com git remote.

- git fetch

Quando você precisa baixar as mudanças criadas por outros membros do seu projeto colaborativo, você precisa do comando Git fetch. A partir desse comando, você irá receber todas as informações de commits, para avaliar, antes de aplicar essas alterações na sua versão local do repositório.

- git pull

O comando Git pull baixa o conteúdo (não os metadados) do que foi alterado no repositório remoto para o seu repositório local e imediatamente atualiza seu contreúdo para a última versão.

- git stash

Esse comando Git armazena temporariamente seus arquivos modificados em uma área chamada stash (“esconderijo”), sem interagir com os outros arquivos até ser necessário.

- git show

Quer detalhes específicos sobre um commit que o log não mostra? O comando Git show é a resposta.

- git rm

Para remover arquivos da sua pasta, você pode utilizar o comando Git rm.

- git merge

Esse comando Git integra as mudanças de dois branches diferentes em um único branch. Ele precisa ser iniciado a partir de um branch já selecionado, que será mesclado com outro, com o nome passado por parâmetro.

- git rebase

Git rebase a princípio parece fazer o mesmo que um comando git merge: ele integra dois branches em um branch único. Porém, esse comando refaz o histórico de commits, tornando-o linear. É o mais indicado para consolidar múltiplos branches.

- git pull –rebase

Essa é uma variação do comando pull mostrado anteriormente. A partir dessa instrução, o Git irá fazer um rebase (não um merge) depois de se utilizar um comando pull.

- git cherry-pick

Esse é um comando poderoso que permite selecionar qualquer commit específico de um brach e aplicá-lo a outro branch, sem precisar de uma mescla completa. A operação fica adicionada no histórico.

- git archive

Esse comando Git combina múltiplos arquivos em um único arquivo, como se fosse um arquivo zipado. Esse pacote pode ser aberto depois e os arquivos contidos podem ser extraídos individualmente.

- git blame

O comando “dedo-duro”, blame ajuda a determinar qual usuário realizou qual mudança em um determinado arquivo.

- git tag

Tags são uma boa opção para marcar uma branch e evitar alteração, principalmente em releases públicos.

- git diff

Para comparar dois arquivos gits ou dois branches antes de passarem por um commit ou um push, é importante executar esse comando Git.

- git citool

Esse comando Git oferece uma alternativa gráfica ao commit.

- git whatchanged

Esse comando oferece informações de log, mas em formato raw.
