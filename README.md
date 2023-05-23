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

## Ramo atual:
Ele mostra o ramo no qual você está trabalhando no momento.

## Mudanças não comprometidas (unstaged changes):

 Mostra os arquivos que foram modificados, mas ainda não foram preparados para o commit. O Git lista os nomes dos arquivos modificados e as alterações específicas feitas em cada arquivo.

## Mudanças preparadas (staged changes): 
Mostra os arquivos que foram adicionados ao stage (área de preparação) para serem incluídos no próximo commit. O Git também lista os nomes dos arquivos nessa seção.
<p>

## Arquivos não monitorados (untracked files): 

Exibe os arquivos que foram adicionados ao diretório de trabalho, mas ainda não foram adicionados ao Git. Esses arquivos não estão sendo rastreados pelo Git.

</p>