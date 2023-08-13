# aws-script
Exemplo simplificado de um script AWS que gera uma infraestrutura básica para a plataforma de Compartilhamento de Veículos Elétricos na AWS.

## Resources

A seção "Resources" contém as definições dos recursos que serão criados na AWS.

### EC2Instance

Define uma instância EC2 uma VM ou container. Propriedades incluem tipo de instância, imagem do sistema operacional e grupo de segurança.

### EC2SecurityGroup

Cria um grupo de segurança para a instância EC2. Restringe o acesso à porta 80 (HTTP) a partir de qualquer endereço IP.

### AuroraDBCluster

Cria um cluster de banco de dados escalável usando o Amazon RDS (Aurora), versão e credenciais de acesso.

### DataStorageBucket

Cria um bucket Amazon S3 para armazenamento de dados estáticos.

### LoadBalancer

Cria um balanceador de carga Elastic Load Balancing para distribuir o tráfego entre as instâncias. Pode ser acessado na porta 80. 

### LoadBalancerSecurityGroup

Cria um grupo de segurança para o balanceador de carga. Restringe o acesso à porta 80 (HTTP) a partir de qualquer endereço IP.

### ECSCluster

Define um cluster do Amazon Elastic Container Service (ECS) para gerenciamento de contêineres.

### ECSService

Define um serviço do Amazon ECS para executar os microsserviços. Depende do balanceador de carga. Configura o tipo de lançamento (EC2), a definição de tarefa e o balanceamento de carga.

## Alunos
Leandro Negrão Ribeiro de Souza,
Jeferson Shimoda,
João Paulo Carnellossi dos Santos,
Gal Levy.
