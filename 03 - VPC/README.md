
# VPC

 - Virtual Private Cloud é um recurso AWs que possibilita a criação de redes virtuais privadas definida e gerenciada pelo usuário

 - VPC => Subnets =>  Route Tables => Network connections

- subnets => privadas e publicas = 3 (dentro da zona de disponibilidade diferentes). Zonas de disponibilidades = 3

- Ficar atendo a seleção das zona de disponibilidade quando estiver criando as subnets publicas e privadas. Por padrão a AWS adiciona todas na mesma zona.

![VPC](https://github.com/peterson771/AWS/blob/main/03%20-%20VPC/VPC.png)

![Create VPC](https://github.com/peterson771/AWS/blob/main/03%20-%20VPC/create_vpc.png)
  

# Internet Gateway

- É um recurso da VPC horizontalmente dimensionado, redundante e altamente disponível que permite a comunicação entre a VPC e internet

- E uma espécie de roteador que dá acesso a VPC a internet.

# Nat Gateway

- Nat Gateway - saida para subnet privada (tradução de endereço privado para publico)

- Temos dois padrões publico e privados. Proporciona acesso somente de dentro para fora, não conseguimos acessar o que está dentro da rede

# Diferença entre Nat Gateway e Internet Gateway

- As subnets configuradas no Internet Gateway tem acesso a internet e podem ser acessadas de fora da VPC da AWS.

- As subnets criadas no Nat Gateway podem consumir recursos na internet mais não podem ser acessadas fora da VPC da AWS.

![Funcionamento](https://github.com/peterson771/AWS/blob/main/03%20-%20VPC/funcionamento.png)

# VPC Peering

- Recurso da AWS que permite a comunicação entre VPCs, quando configurado permite o tráfego entre elas.

- Todo o tráfego entre as VPCs é criptografado e utiliza a infraestrutura global da AWS. Não há cobrança para criar o VPC Peering, todo o tráfego dentro da mesma zona de disponibilidade é gratuíto

# AWS Private Link

- É um serviço utilizado para prover segurança entre conexões privadas entre a VPC e outros serviços da AWS ou até mesmo em ambientes on-premisses.

- Utiliza um NLB para conectar diferentes ENI (Elastic Network Interface)

![VPC Peering](https://github.com/peterson771/AWS/blob/main/03%20-%20VPC/vpc_peering.png)

# VPC Endpoints

- São recursos que permitem a comunicação com serviços suportados pela AWS de forma privada através do Private Link
