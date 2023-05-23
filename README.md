# Git-Curso
Curso de Git e Versionamento oferecido pela Ada Tech em parceria com o Santander



## O QUE É VERSIONAMENTO?

- Registro de mudanças em arquivos, que possibilita recuperação ou acesso a versoes anteriores;
- Desenvolvimento de código em colaboração com outros integrantes.
<br>

O versionamento é o registro e controle das mudanças feitas em arquivos. Isso permite 
recuperar versões anteriores e colaborar com outras pessoas durante o desenvolvimento de código.

## O que é GIT?
GIT É um sistema de versionamento de código, que guarda os registros
de versão como snapshots (fotos) do estado do projeto, alem da refência/caminho para essa foto.

<br>

## O Git é um sistema de controle de versão de código-fonte.
* Permite registrar e controlar as alterações feitas nos arquivos ao longo do tempo.
* Facilita a colaboração entre desenvolvedores em projetos de software.
* Mantém um histórico completo das alterações feitas nos arquivos.
* Permite reverter para versões anteriores dos arquivos.
* Ajuda a mesclar as alterações feitas por diferentes desenvolvedores de forma controlada.
* Permite trabalhar em paralelo em diferentes partes do projeto.
* Contribui para o gerenciamento eficiente de projetos de software.

<br>

## O que é github?

O GitHub é uma plataforma de hospedagem e colaboração de desenvolvimento de software baseada em controle de versão Git. É um serviço web que permite aos desenvolvedores hospedar, gerenciar e colaborar em projetos de código aberto e privados

## Git e suas Operações locais

A maioria das operações do GIT são locais e por isso boa parte das operações são praticamente
instantâneas devido a facilidade de acessar arquivos e mseu prop´rio computador.


## Comandos Git

*verificando a versão do GIT instalado em seu computador*
- git --version

Esses comandos são usados para configurar o nome de usuário e o email associados às suas atividades no Git.


*configurando user;*
- git config --global user.name "fernandosilvajesus"

*configurando e-mail;*
- git config --global user.email

*Clonando um resositórios;*
- git clone  https://github.com/fernandosilvajesus/Git-Curso.git



<br><br>
*Git status;* <br>

O comando git status é usado para exibir o estado atual do seu repositório Git. 

## Raiz atual:
Ele mostra a raiz no qual você está trabalhando no momento.

## Mudanças não comprometidas (unstaged changes):

 Mostra os arquivos que foram modificados, mas ainda não foram preparados para o commit. O Git lista os nomes dos arquivos modificados e as alterações específicas feitas em cada arquivo.

## Mudanças preparadas (staged changes): 
Mostra os arquivos que foram adicionados ao stage (área de preparação) para serem incluídos no próximo commit. O Git também lista os nomes dos arquivos nessa seção.
<p>

## Arquivos não monitorados (untracked files): 

Exibe os arquivos que foram adicionados ao diretório de trabalho, mas ainda não foram adicionados ao Git. Esses arquivos não estão sendo rastreados pelo Git.

</p>

*Git diff;* <br>
- git diff
- git diff --staged

## git diff
 é usado para visualizar as diferenças entre o estado atual do seu repositório Git e um estado anterior. Ele mostra as alterações feitas nos arquivos desde o último commit.
<br>

## git diff --staged
 mostra as diferenças entre os arquivos que estão no stage (área de preparação) e o último commit. 

 *git log*
 - git log

  usado para exibir um histórico dos últimos commits feitos no repositório Git. Ele mostra informações detalhadas sobre os commits, como o autor, a data, a mensagem de commit e um identificador único (hash) para cada commit.

  

*git restore*
- git restore nome_arquivo
- git restore  --staged nome_arquivo

## Git restore
**git restore nome_arquivo**, o comando descarta as alterações feitas no arquivo especificado, revertendo-o para a versão mais recente confirmada no último commit. Isso significa que as modificações feitas após o último commit serão descartadas e o arquivo será restaurado para o estado registrado no último commit.

## Git restore --staged

**git restore --staged nome_arquivo** é usado para remover arquivos do stage (área de preparação) e retorná-los ao estado de modificações não preparadas (unstaged changes). Isso significa que as alterações feitas nesses arquivos não serão incluídas no próximo commit, a menos que você as adicione novamente ao stage.

*git push*
- git push origin nome_da_branch

## git push
é usado para enviar suas alterações locais para um repositório remoto. Quando você executa "git push", você está basicamente enviando as confirmações (commits) que você fez no seu repositório local para um repositório remoto específico.

 Isso permite que outras pessoas acessem e vejam suas alterações, bem como contribuam com suas próprias modificações. É comum usar o comando "**git push**" após fazer uma série de commits locais para sincronizar seu repositório local com o repositório remoto.



*git pull*
- git pull origin nome_da_branch

 ## git pull
  é usado para obter as alterações feitas por outros colaboradores em um repositório remoto e incorporá-las ao seu repositório local. Quando você executa "**git pull**", o Git busca as alterações mais recentes no repositório remoto e as mescla automaticamente com o seu repositório local. 
  
  Isso garante que você tenha as versões mais atualizadas dos arquivos e possa continuar trabalhando com as modificações mais recentes feitas por outros colaboradores.