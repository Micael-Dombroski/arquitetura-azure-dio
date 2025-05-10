# Componenetes de Arquitetura do Azure
## Regiões
  Locais onde há datacenters do Azure. Sempre que você cria um recurso no Azure você deve informar a região em que o recurso ficará, devendo escolher a mais próxima de onde o recurso será acessado para melhorar a velocidade de acesso. Fornecem flexibilidade e escala para reduzir a latência do cliente.<br>
  Nem todo recursos está dispónível para todas as regiões, porém esse indisponibilidade é mais comum em recursos em teste ou que saíram recentemente para acesso global. <br>
  O Microsoft Azure oferece mais regiões globais que qualquer outro provedor de nuvem, com mais de 60 regiões representando mais de 140 países. <br>
  Cada região é composta por um ou mais datacenters muito próximos, cada datacenter representa uma zona de disponibilidade, possuindo uma cópia de todos os dados da região, assim, mesmo que um fique fora do ar os serviços da região seguem funcionando.<br>
  Caso todos os datacenters da região fiquem indisponíveis existe o serviço de disaster recovery, que consiste em manter cópia dos recursos essenciais em outra região e ativar esses recursos quando a região principal esteja fora do ar.

## Zona de disponibilidade
  Fornece proteção contra tempo de inatividade indevido a falha do datacenter. Separa fisicamente os datacenters da mesma região. Cada datacenter possui sistema de alimentação, resfriamento e rede independentes e são conectados por meio de redes privadas de fibra óptica.

## Pares de Região
  Cada região possui uma região par que abriga o serviço de disaster recovery da região, a região par replica automaticamente alguns serviços. <br>
  Deve haver pelo menos 300 milhas (cerca de 483 km) de distância entre os pares de região. <br>
  A recuperação da região afetada é priorizada em caso de interrupção. As atualizações são distribuídas sequencialmente para minimizar o tempo de inatividade.

## Regiões Soberanas
### Serviços Governamentais dos EUA / Azure Governamental
Atende às necessidades de segurança e conformidade das agências federais, governos estaduais e locais dos EUA e seus provedores de soluções. <br>
É uma instância separada do Azure, fisicamente isolada de implantações que não sejam do governo dos EUA e seu acesso é permitido apenas para pessoal verificado e autorizado.

### Azure China
A Microsoft é o primeiro provedor estrangeiro de serviços de nuvem pública da China. Atua em conformidade com as regulamentações governamentais. <br>
Fisicamente separada dos serviços de nuvem do Azure e operado pela 21Vianet. Todos os dados ficam dentro da China para garantir a conformidade.

## Recursos do Azure
  Entre os recursos disponíveis na Azure temos: máquinas virtuais, redes virtuais, serviços de aplitivos, contas de armazenamento, funções e banco de dados SQL.

### Grupo de Recursos
Uma forma de organizar os recursos, podendo abrangir recursos de regiões diferentes, o recurso só pode estar presente em um grupo por vez. <br>
Os recursos podem ser movidos para outros grupos mas não é possível alterar o nome do grupo de recursos. Os aplicativos podem usar vários grupos de recursos.

## Assinaturas do Azure
Uma conta do Microsoft Azure pode ter várias assinaturas, como a de desenvolvimento, a de teste e a de produção, mas cada assinatura só pode ser vinculada a uma conta. <br>
Cada assinatura gera uma cobrança diferente, com isso a empresa pode medir o valor cada em assinaturas em cada projeto, por exemplo.

### Limite de Cobrança
  Gerar relatórios de cobrança e faturas separados para cada assinatura.

### Limite do Controle de Acesso
  Gerenciar e controlar o acesso aos recursos que os usuários podem provisionar com assinaturas específicas.

## Grupos de Gerenciamento
  Os grupos de gerencimantos podem incluir várias assinaturas do Azure, fazendo-as herdar as condições aplicadas no grupo.

## Microsfot Datacenters
Por meio do link "https://datacenters.microsoft.com/globe/explore" podemos visualizar o globo terreste em 3D mostrando todas as regiões implantadas, as regiões que estão sendo desenvolvidas e os projetos de sustentabilidade espalhados pelo mundo, além disso também podemos pela opção "Take a tour" ver  como são esses datacenters da Microsoft.
