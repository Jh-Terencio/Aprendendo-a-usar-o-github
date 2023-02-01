# Guia para Aprender a Usar Comandos do GitHub
## Bem-vindo ao meu repositório, onde nosso objetivo é aprender a usar o GitHub e suas funcionalidades. Aqui, você encontrará instruções, comandos, explicações sobre o que cada comando faz e passo a passo para algumas ações. Além disso, nosso objetivo é também introduzir a linguagem de marcação Markdown. <br><br> [Clicando aqui você irá cair em um artigo ensinando a criar um README](https://www.alura.com.br/artigos/escrever-bom-readme).

### 0° tópico: O que é o github e para que ele serve?
  * GitHub é uma plataforma de hospedagem de código e desenvolvimento de software. É uma comunidade de desenvolvedores onde é possível compartilhar, colaborar e contribuir em projetos de software usando o controle de versão Git. Além disso, ele fornece uma ampla gama de ferramentas e recursos para gerenciar projetos de software, incluindo bug tracking, tarefas e documentação.
  * O GitHub serve como uma plataforma para o desenvolvimento de software colaborativo, onde os desenvolvedores podem compartilhar, colaborar e contribuir em projetos de software de forma eficiente. Além disso, ele fornece uma ampla gama de ferramentas e recursos para gerenciar projetos de software, incluindo versionamento de código, gerenciamento de bugs, tarefas, documentação e muito mais. O GitHub também é amplamente utilizado como um repositório para projetos open-source, permitindo que a comunidade contribua e colabore para melhorá-los.
  
  -------------------------
### 1° tópico: Criação de arquivos pelo github 
 * Criar arquivos e salvá-los no GitHub é importante, pois permite o acesso aos seus arquivos de forma remota, sem precisar estar com sua máquina. Além disso, ao trabalhar em equipe, é necessário ter um local compartilhado para todos da equipe, garantindo assim uma organização mais eficiente.
 * Vamos iniciar então esse tópico, como criamos um arquivo em um repositório diretamente do github:
    * Navegue até o repositório desejado.
    * Clique no botão "Add file".
    * Clique no botão "Create new file".
    * Dê um nome ao arquivo e adicione o conteúdo desejado.
    * Adicione um comentario para informar aos demais colaboradores quais mudanças foram feitas.
    * Clique no botão "Commit new file".
    
    -------------------------
 ### 2° tópico: Para que serve o commit e por que ele é importante?
  * O commit é uma ação no controle de versão Git que permite salvar as alterações realizadas em arquivos em uma determinada versão. Cada commit é identificado por um número único de hash e pode conter uma mensagem descritiva que explica as alterações realizadas. Os commits são agrupados em ramos (branches) e permitem a colaboração em equipe, pois é possível visualizar e comparar as diferenças entre as versões do código. Além disso, os commits também permitem a reversão de alterações indesejadas, a criação de novos ramos para experimentações e a integração de mudanças realizadas por diferentes desenvolvedores.

 -------------------------
 ### 3° tópico: Como passar o repositório para sua máquina
  * É super importante você ter uma cópia do seu repositório no seu computador, serve para ter acesso localmente e poder trabalhar com eles offline. Para fazer isso, você precisa clonar o repositório para sua máquina. Aqui estão os passos para clonar um repositório:

    * Abra o terminal ou o Git Bash na sua máquina.
    * Navegue até a pasta onde você deseja salvar o repositório clonado.
    * Digite o comando git clone seguido pelo URL do repositório. Por exemplo: git clone https://github.com/username/repository.git
    * Pressione enter e aguarde o processo de clonagem ser concluído.
    * Depois de concluído, você poderá navegar até a pasta do repositório clonado e começar a trabalhar com os arquivos localmente.
    * Observe que é importante sincronizar as alterações realizadas localmente com o repositório remoto para evitar conflitos. Para fazer isso, você precisa fazer um push das suas alterações para o repositório remoto no GitHub.
  * Comando: 
    ```
    git clone + link https do seu repositório
    ```
  * Após esse passos basta apenas você entrar na pasta através do terminal digitando cd + o nome do repositório
  * Para verificar se a versão mais atual foi salva é só digitar git pull + link https
  * Comando: 
    ```
    git pull + link https do seu repositório
    ```
    -------------------------
 ### 4° tópico: Salvando localmente as mudanças que você fez e salvando remotamente
   * Ao passar seu repositório do github para seu computador você ficará livre para fazer as mudanças que desejar sem alterar o arquivo remoto. Porém, com forme você for fazendo as mudanças, torna-se necessário salvá-las para não acabar perdendo suas atualizações.
   * Para isso utilizamos no terminal o comando git commit, que fará os salvamento das mundaças, mas temas dois jeitos de fazer esse salvamento:
     * Salvando um arquivo em específico: 
       * git commit + nome do arquivo modificado + -m "texto contendo os comentários das modificações"
       * Comando: 
       ```
       git commit README.md -m "Adicionando mudanças do README"
       ```
     * Salvando todos os arquivos de uma vez:
       * git commit + . + -m "texto contendo os comentários das modificações":
       * Comando:
       ```
       git commit . -m "Adicionando mudanças do README"
       ```
     * #### Observação: Os comentários são opcioanis, então se você não quiser não é necssário utilizar o -m "texto", porém é uma boa prática você fazer um comentário sempre que uma mudança for feita.
   * Após salvar e atualizar seu arquivos, é sempre bom passá-los para a nuvem para se precaver de problemas, nunca se sabe quando um arquivo vá corromper, ne?
   * Para isso utilizaremos o terminal novamente, mas dessa vez usando o comando git push origin + nome da branch, que fará o salvamento das mudanças no github
     * Comando: 
       ```
       git push origin main (branch aleatória)
       ```
 -------------------------
 ### x° tópico: Comandos e o que eles fazem
  * git clone: 
    * O git clone é um comando do Git que permite clonar (copiar) um repositório remoto para o seu computador local. Esse comando cria uma cópia idêntica do repositório remoto, incluindo todos os arquivos, histórico de commits e informações de branch. Ao clonar um repositório, você pode trabalhar offline, fazer alterações e, em seguida, enviar suas alterações para o repositório remoto, mantendo-o atualizado. Além disso, o git clone também permite a colaboração em equipe, pois cada membro da equipe pode clonar o repositório remoto e trabalhar em sua própria cópia.
  * git pull:
    * O git pull é um comando do Git que permite atualizar um repositório local com as alterações presentes no repositório remoto. Esse comando faz o download das alterações presentes no repositório remoto para o seu repositório local, incluindo novos arquivos, modificações em arquivos existentes e histórico de commits. Ao fazer o git pull, você garante que o seu repositório local está sempre atualizado com o repositório remoto. Além disso, o git pull também permite a colaboração em equipe, pois cada membro da equipe pode atualizar sua cópia local com as alterações feitas por outros membros.
  * git commit .:
    * O git commit é um comando do Git que permite salvar as alterações realizadas em um repositório local. Quando você faz um commit, você está criando um ponto de referência no histórico do repositório, o que permite reverter as alterações em um momento posterior se necessário. Ao fazer um commit, você deve fornecer uma mensagem que explique as alterações realizadas, o que ajuda a manter o histórico do repositório organizado e fácil de entender. Além disso, o git commit permite que você trabalhe de forma descentralizada, já que as alterações são salvas localmente antes de serem enviadas para o repositório remoto. Isso permite que você continue a trabalhar mesmo sem conexão com a Internet.
  * git push: 
    * O git push é um comando do Git que permite enviar as alterações salvas localmente em um repositório para o repositório remoto no Github ou outra plataforma de hospedagem de código. Quando você faz um push, as alterações que você fez localmente são enviadas para o repositório remoto, onde podem ser acessadas por outros colaboradores. Além disso, o git push permite que você mantenha o repositório remoto atualizado com as alterações mais recentes. É importante destacar que o push deve ser feito após o commit, já que o git commit salva as alterações localmente, enquanto o git push envia as alterações para o repositório remoto.
  * git log –oneline: 
    * O comando git log é a ferramenta básica do Git para explorar o histórico de um repositório. É usado quando se precisa encontrar uma versão específica de um projeto ou saber quais alterações vão ser implantadas por meio do merge de uma ramificação de recurso.
  * git restore –source: 
    * O git restore é uma nova opção quando estamos trabalhando e precisamos restaurar algum arquivo ou o projeto por completo, e isso o git checkout também faz, porém o git restore é especificamente para trabalhar com essa parte de restauração de arquivos ou projeto ao um ponto anterior que chamamos de fonte de restauração

