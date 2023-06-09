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

*git fetch*
- git fetch 

 ## git fetch
 É usado para buscar (fetch) todas as alterações e referências de um repositório remoto para o seu repositório local. Ao contrário do comando "git pull", o "git fetch" não mescla automaticamente as alterações no seu ramo de trabalho atual. Em vez disso, ele atualiza as referências locais, como as branches remotas e tags, para refletir o estado atual do repositório remoto.


  ## O que são branches em Git e como isso pode nos ajudar

Em Git, uma branch (ramificação) é uma linha independente de desenvolvimento que permite que você trabalhe em diferentes recursos, correções de bugs ou experimentos de forma isolada, sem interferir no código principal do projeto. Cada branch representa uma versão paralela do repositório contendo seus próprios commits (confirmações) e histórico.

Aqui estão alguns pontos-chave sobre branches em Git e como eles podem nos ajudar:

1. Desenvolvimento Isolado: Ao criar uma branch, você pode trabalhar em uma nova funcionalidade ou correção de bug sem afetar o código principal do projeto. Isso permite que você experimente livremente e faça alterações sem preocupação em impactar o trabalho de outros desenvolvedores.

2. Colaboração Paralela: Branches permitem que vários desenvolvedores trabalhem em diferentes partes do projeto simultaneamente. Cada desenvolvedor pode criar sua própria branch para trabalhar em uma tarefa específica, e posteriormente, mesclar suas alterações com a branch principal quando estiverem prontas para serem incorporadas.

3. Controle de Versão e Histórico: Cada branch possui seu próprio histórico de commits, o que facilita a revisão das alterações específicas feitas em uma determinada funcionalidade ou correção de bug. O Git permite alternar entre diferentes branches para visualizar o código e histórico correspondentes.

4. Testes e Experimentos: Branches podem ser usadas para testar e experimentar novas ideias sem afetar o fluxo principal do projeto. Se uma nova funcionalidade não funcionar conforme o esperado, você pode simplesmente descartar a branch sem prejudicar o código principal.

5. Gerenciamento de Releases: Branches também são úteis para o gerenciamento de versões e releases. Por exemplo, você pode criar uma branch específica para uma versão estável do software e continuar desenvolvendo novos recursos em outra branch. Isso permite manter a estabilidade do código em uma versão enquanto trabalha em melhorias futuras.

6. Revisão de Código: Branches facilitam o processo de revisão de código, pois você pode compartilhar uma branch específica com outros desenvolvedores para revisão antes de mesclá-la com a branch principal. Isso ajuda a garantir a qualidade do código e a identificar possíveis problemas antes que eles sejam incorporados ao projeto principal.

Em resumo, as branches em Git permitem o desenvolvimento paralelo, isolado e organizado de diferentes recursos e correções de bugs. Elas ajudam a evitar conflitos de código, permitem colaboração eficiente entre desenvolvedores, facilitam o controle de versão e proporcionam um ambiente seguro para testes e experimentos. O uso adequado de branches pode melhorar a produtividade, a qualidade do código e a organização em projetos de desenvolvimento de software.


## Criando uma nova Branch
usando o comando abaixo<br>
- <code>git branch nome_da_nova_branch</code>

Agora você criou nova branch e pode começar a trabalhar nela. <br>
para selecionar essa nova branch deve usar o comando<br>

- <code>git checkout nome_da_nova_branch</code>

Agora você está na nova branch criada e pode começar a trabalhar nela. Todas as alterações e commits que você fizer serão específicos para essa branch. 

## Utilizando uma sintaxe resumida 
Se você quiser criar uma nova branch e mudar para ela em um único comando, você pode usar o seguinte comando:

- <code>git checkout -b nome_da_nova_branch</code>

## visualizando Branch criadas
- <code>git branch</code>
O comando acima ira retornar todas as Branch 




## Merging branches

É o processo de combinar as alterações feitas em duas ou mais branches diferentes em uma única branch. Ele permite que você leve as alterações feitas em uma branch para outra.

Quando você faz um merge, o Git analisa as alterações feitas nas branches envolvidas e combina essas alterações em um novo commit, criando um estado consolidado que inclui as alterações de ambas as branches.

Isso é útil quando você trabalha em uma branch separada para adicionar um novo recurso ou corrigir um bug e, em seguida, deseja incorporar essas alterações ao código principal do projeto.







## Para realizar um merge no Git, siga estes passos:

1. Use o comando "git branch" para verificar em qual branch você está atualmente. Ele lista todas as branches existentes e marca com um asterisco (*) a branch atual.

2. Certifique-se de estar na sua branch principal. Se não estiver, use o comando "git checkout" seguido do nome da sua branch principal para mudar para ela.

3. Agora você está na sua branch principal e pronto para realizar o merge. Use o comando "git merge" seguido do nome da outra branch que você deseja mesclar com a sua branch principal.


