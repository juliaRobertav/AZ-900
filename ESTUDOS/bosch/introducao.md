---
description: Todas as explicações detalhadas desses assuntos estão nos slides :)
---

# Introdução

### Princípios básicos do Microsoft Azure

### Computação em nuvem

Computação em nuvem é a entrega de serviços de  computação por meio da internet

\-> acessar qualquer serviço pela internet

### Tipos de Nuvem

1. pública

* Nuvem Pública: A nuvem pública da Azure é uma plataforma de computação em nuvem oferecida pela Microsoft para uso geral.
* Nesse modelo, os recursos de computação, armazenamento e rede são fornecidos pela Microsoft e compartilhados entre várias organizações. Os clientes podem acessar esses recursos por meio da Internet, pagando apenas pelos serviços utilizados. A nuvem pública é altamente escalável, flexível e econômica, permitindo que as empresas reduzam custos operacionais e se concentrem em suas principais competências.

\-> Principais características da nuvem pública:

* Recursos compartilhados entre várias organizações.
* Acesso via Internet.
* Escalabilidade e flexibilidade.
* Modelo de pagamento por uso.
* Manutenção e atualizações gerenciadas pela provedora de nuvem.

2. &#x20;privada

* Nuvem Privada: A nuvem privada da Azure é uma infraestrutura de nuvem dedicada a uma única organização.
* Nesse modelo, os recursos de computação, armazenamento e rede são implantados em um ambiente isolado, geralmente dentro do data center da própria organização. A nuvem privada oferece maior controle e segurança, permitindo que as empresas atendam a requisitos regulatórios específicos ou mantenham dados sensíveis dentro de suas próprias instalações. No entanto, a nuvem privada requer investimentos significativos em infraestrutura e manutenção.

\-> Principais características da nuvem privada:

* Recursos dedicados a uma única organização.
* Implantação em data center próprio ou de terceiros.
* Maior controle e segurança.
* Atendimento a requisitos regulatórios específicos.
* Investimentos em infraestrutura e manutenção.

3. hibrida

* Nuvem Híbrida: A nuvem híbrida da Azure combina os recursos da nuvem pública e privada, permitindo que as organizações aproveitem o melhor dos dois mundos.
* Nesse modelo, as empresas podem implantar e gerenciar aplicativos e dados em ambientes de nuvem pública e privada, mantendo a flexibilidade e a escalabilidade da nuvem pública, ao mesmo tempo em que mantêm o controle e a segurança da nuvem privada. A nuvem híbrida é ideal para organizações que desejam migrar gradualmente para a nuvem ou que têm requisitos específicos de segurança e conformidade.

\-> Principais características da nuvem híbrida:

* Combinação de recursos da nuvem pública e privada.
* Flexibilidade e escalabilidade da nuvem pública.
* Controle e segurança da nuvem privada.
* Migração gradual para a nuvem.
* Atendimento a requisitos específicos de segurança e conformidade.

### Tipos de Despesas

Existem três tipos principais de despesas relacionadas à computação em nuvem: despesas de capital (CapEx), despesas operacionais (OpEx) e despesas de consumo.

1. Despesas de Capital (CapEx): As despesas de capital são os investimentos iniciais em infraestrutura, hardware e software necessários para implantar uma solução de nuvem. Esses custos são considerados ativos fixos e geralmente são amortizados ao longo do tempo. No contexto da computação em nuvem, as despesas de capital podem incluir a compra de servidores, equipamentos de rede, licenças de software e outros recursos físicos necessários para construir uma infraestrutura de nuvem privada. As despesas de capital são geralmente mais significativas no início do projeto e podem exigir um investimento inicial substancial.
2. Despesas Operacionais (OpEx): As despesas operacionais são os custos contínuos associados à operação e manutenção de uma solução de nuvem. Esses custos são considerados despesas correntes e são pagos regularmente, geralmente em forma de assinaturas ou taxas mensais. No contexto da computação em nuvem, as despesas operacionais podem incluir custos de energia, refrigeração, manutenção, suporte técnico, licenças de software, atualizações e outros serviços relacionados à operação da infraestrutura de nuvem. As despesas operacionais são mais flexíveis e podem ser ajustadas de acordo com a demanda e o uso real dos recursos.
3. Despesas de Consumo: As despesas de consumo são os custos associados ao uso real dos serviços de nuvem. Esses custos são baseados no consumo de recursos, como poder de processamento, armazenamento, largura de banda de rede e outros serviços específicos oferecidos pela provedora de nuvem. As despesas de consumo são normalmente calculadas com base na quantidade de recursos utilizados e na duração do uso. Os clientes pagam apenas pelos serviços que utilizam, o que permite uma maior flexibilidade e escalabilidade. Esse modelo de pagamento por uso é comum na nuvem pública, onde os clientes são cobrados com base na quantidade de recursos consumidos.

Os diferentes tipos de despesas na computação em nuvem possuem escalabilidades distintas, que podem ser alcançadas por meio do dimensionamento horizontal e vertical:

1. Dimensionamento horizontal (scaling horizontal): Também conhecido como escalabilidade horizontal, envolve adicionar mais instâncias ou réplicas do sistema ou aplicativo. Nesse caso, você distribui a carga de trabalho entre várias máquinas ou servidores. Por exemplo, se você tiver um aplicativo web, poderá adicionar mais servidores para lidar com um aumento no tráfego. O dimensionamento horizontal geralmente é mais fácil de implementar, pois não requer alterações significativas na infraestrutura existente. No entanto, pode exigir mecanismos de balanceamento de carga para distribuir o tráfego entre as instâncias.
2. Dimensionamento vertical (scaling vertical): Também conhecido como escalabilidade vertical, envolve aumentar a capacidade de uma única instância ou servidor, adicionando mais recursos a ele. Isso pode incluir aumentar a quantidade de memória, processadores, armazenamento ou outros recursos do sistema. Por exemplo, você pode atualizar um servidor com mais RAM ou adicionar mais núcleos de processamento. O dimensionamento vertical geralmente requer alterações na infraestrutura existente e pode ter limitações físicas, como a capacidade máxima de recursos em um único servidor.

Para isso a Microsoft fornece uma calculadora de preços

{% embed url="https://azure.microsoft.com/pt-br/pricing/calculator/" %}

### Benefícios da Nuvem

#### Confiabilidade

1. Confiabilidade: A nuvem oferece alta confiabilidade ao fornecer recursos redundantes e infraestrutura resiliente. Os provedores de nuvem, como a Microsoft Azure, possuem data centers distribuídos globalmente, garantindo que os serviços estejam disponíveis mesmo em caso de falhas em um local específico. Além disso, a nuvem oferece recursos de backup e recuperação de dados, permitindo que as organizações protejam seus dados contra perdas e interrupções.

#### Previsibilidade

2. Previsibilidade: A nuvem permite que as organizações tenham previsibilidade em relação aos custos e desempenho dos serviços. Os provedores de nuvem geralmente oferecem modelos de preços flexíveis, como pagamento por uso, permitindo que as organizações paguem apenas pelos recursos que realmente utilizam. Além disso, a nuvem oferece recursos de monitoramento e análise, permitindo que as organizações acompanhem o desempenho dos serviços e tomem decisões informadas para otimizar o uso dos recursos.

#### Segurança

3. Segurança: A segurança é uma preocupação fundamental na computação em nuvem. Os provedores de nuvem implementam medidas de segurança avançadas para proteger os dados e as aplicações dos clientes. Isso inclui criptografia de dados em repouso e em trânsito, autenticação de usuários, controle de acesso baseado em funções, detecção de ameaças e monitoramento contínuo. Além disso, os provedores de nuvem estão sujeitos a auditorias e conformidade com padrões de segurança reconhecidos internacionalmente.

#### Governança

4. Governança: A nuvem oferece recursos de governança que permitem que as organizações estabeleçam políticas, controles e processos para garantir o uso adequado dos recursos de nuvem. Isso inclui a definição de políticas de acesso, conformidade com regulamentações, gerenciamento de identidades e acesso, e monitoramento do uso dos recursos. A nuvem também oferece recursos de automação e gerenciamento de configuração, permitindo que as organizações implementem e apliquem consistentemente suas políticas e controles.

#### Gerenciamento

* Há dois tipos de capacidade de gerenciamento para computação em nuvem:&#x20;
* O gerenciamento <mark style="color:blue;">da</mark> nuvem diz respeito a gerenciar seus recursos de nuvem.&#x20;
* O gerenciamento <mark style="color:blue;">na</mark> nuvem diz respeito à maneira de gerenciar seu ambiente de nuvem e seus recursos.

1. <mark style="color:blue;">Gerenciamento da Nuvem</mark>: O gerenciamento da nuvem refere-se às atividades e processos envolvidos na administração dos recursos de nuvem, independentemente de onde esses recursos estejam localizados. Isso inclui a definição e implementação de políticas, monitoramento de desempenho, provisionamento de recursos, gerenciamento de segurança, backup e recuperação de dados, entre outras tarefas. O gerenciamento da nuvem é responsabilidade do provedor de nuvem, como a Microsoft Azure, que oferece ferramentas e serviços para ajudar as organizações a gerenciar seus recursos de nuvem de forma eficiente e segura. Os provedores de nuvem também são responsáveis por garantir a disponibilidade, confiabilidade e escalabilidade dos serviços de nuvem.
2. <mark style="color:blue;">Gerenciamento na Nuvem</mark>: O gerenciamento na nuvem refere-se às atividades de administração e controle realizadas pelos clientes ou usuários dos serviços de nuvem. Isso inclui a configuração e personalização dos recursos de nuvem, monitoramento do desempenho e uso dos serviços, gerenciamento de identidades e acesso, implementação de políticas de segurança, gerenciamento de custos e otimização de recursos. O gerenciamento na nuvem é responsabilidade das organizações ou indivíduos que utilizam os serviços de nuvem para hospedar suas aplicações, armazenar dados e executar suas operações de negócios. Os clientes podem usar ferramentas e serviços fornecidos pelo provedor de nuvem, como painéis de controle, APIs e automação, para facilitar o gerenciamento na nuvem.

### Tipos de Serviço de nuvem

1. Infraestrutura como Serviço (IaaS): O IaaS fornece recursos de infraestrutura virtualizados, como máquinas virtuais, redes, armazenamento e balanceadores de carga. Com o IaaS da Azure, as organizações podem implantar e gerenciar suas próprias aplicações e sistemas operacionais em uma infraestrutura virtualizada. Isso oferece flexibilidade e controle total sobre a configuração e personalização da infraestrutura, permitindo que as organizações construam e gerenciem seus próprios ambientes de TI na nuvem.

Exemplos de serviços de IaaS da Azure incluem:

* Máquinas Virtuais (Azure Virtual Machines)
* Redes Virtuais (Azure Virtual Networks)
* Armazenamento em Blobs (Azure Blob Storage)
* Balanceadores de Carga (Azure Load Balancer)
* Backup e Recuperação (Azure Backup)
* Contêineres

\-> PaaS (plataforma)

\-> SaaS (software)

<figure><img src="../.gitbook/assets/image (10) (1).png" alt="" width="563"><figcaption></figcaption></figure>

* **Não necessariamente é preciso comprar os recursos da azure (principalmente em SaaS) para usar!!**
