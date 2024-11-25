
# Amazon EC2

 - Amazon elastic compute cloud é um serviço da AWS que fornece capacidade computacional redimensionável.

 - Uma instancia do EC2 é equivalente a uma maquina virtual.

# Tipos de instancias

 - O Amazon EC2 oferece uma ampla seleção de tipos de instancias otimizadas para atender a diferentes caso de uso.

 - Cada categoria tem uma infinidade de configurações de hardware para atender a cada necessidade.

 - https://aws.amazon.com/ec2/instance-types/?gclid=CjwKCAiA3ZC6BhBaEiwAeqfvytinjssYYeyGnrhiVXNcavtKcUOcwPCCuZMS5KIHqdFMXK1lGzfrShoCgZ8QAvD_BwE&trk=a5a8f3c9-c18a-485c-bbdb-52b795178fbe&sc_channel=ps&ef_id=CjwKCAiA3ZC6BhBaEiwAeqfvytinjssYYeyGnrhiVXNcavtKcUOcwPCCuZMS5KIHqdFMXK1lGzfrShoCgZ8QAvD_BwE:G:s&s_kwcid=AL!4422!3!490415521566!e!!g!!ec2!12028491727!115492232145

# Modelos de aquisição.

- Sob demanda -> paga pela utilização do hardware ligada quando estiver ligada, quanto o volume EBS ele é cobrado

- Instancias reservadas -> oferecem um desconto considerável em comparação a definição de preço sob demanda. Não existe a opção de alterar a categoria e hardware desse modelo.


 - Saving Plans -> modelo de preços flexíveis em troca de um compromisso de uso específico por um período de 1 até 3 anos. Para recursos como Fargate, EC2 e Lambda o desconto pode chegar até 66%
 
 - Spot -> permite que a instancia seja execultada até em 6 horas o desligamento é enviado 2 minutos antes e todo conteúdo é excluído.

 # Ciclos de vida de uma instancia EC2

- Pending -> estado após criar a instancia.

- Running -> instancia ligada.

- Stopped -> instancia desligada
 
- Terminated -> não é possivel recuperar esse estado, sendo excluída após um período.


# Recursos para proteger a instancia.

- Instance settings - chage stop protection e change termination protection


# EC2 Key Pairs

- Consiste em uma chave privada usada para acessar uma instancia EC2. Pode ser criado uma key pairs para cada EC2 ou utilizar uma já existente. O formato utilizado no linux é RSA e .pem

- Alterar a permissão da chave para 400.

      - chmod 400 chave01.pem



