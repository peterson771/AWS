
# Tags

 - São pares de chave e valor utilizados para uma indentificação de recursos na AWS.

- Elas ajudam a gerenciar, identificar, organizar, automatizar, pesquisar e filtrar recursos distintos. 

- As TAGS são case sensitive.

- Alguns exemplos de utilização das Tags:
     
    - Organização de recursos
    - Alocação de cursos
    - Automação
    - Controle de acesso
    - Governança

# EBS

- Persistencia de dados mesmo após excluir a instancia. Podemos ter diversos volumes EBS conectados a uma instancia 

- Tem que estar mesma AZ da instancia (região), automaticamente é replicado na AZ

- Os dois tipos de volumes de EBS são: HD e SSD, podemos alterar o tipo do disco e também o tamanho do disco. 

# Snapshots de volumes EBS

- São registros do estado (foto) de um determinado ambiente, sistema ou disco em um determinado momento. O primeiro Snapshots é sempre full e os demais são incrementais.

- Os Snapshots são armazenados dentro de um buckets S3, a cobrança é gerada na quantidade de dados. Podemos configurar uma lixeira para retenção dos dados desse Snapshots.

- Arquivamento do Snapshots é um nível de armazenamento de baixo custo a longo prazo que não precisa de uma recuperação rápida e frequente. Podendo até levar 72 horas para o restore


- Clicando com o botão direito no EBS, temos a opção de criar um Snapshots.
