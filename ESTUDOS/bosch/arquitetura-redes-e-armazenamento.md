---
description: Arquitetura Azure
---

# Arquitetura

Esse site explica melhor sobre os conceitos de arquitetura azure:

{% embed url="https://learn.microsoft.com/pt-br/training/paths/azure-fundamentals-describe-azure-architecture-services/" %}

{% embed url="https://learn.microsoft.com/pt-br/azure/architecture/guide/" %}

### Regiões

As regiões do Azure são locais geográficos onde os data centers do Azure estão localizados. Cada região é composta por um ou mais data centers que estão fisicamente próximos um do outro, mas suficientemente distantes para garantir a resiliência e a redundância dos serviços.

O Azure possui uma ampla variedade de regiões distribuídas em todo o mundo, abrangendo todos os continentes principais. Alguns exemplos de regiões do Azure incluem:

1. Região Leste dos EUA: localizada na costa leste dos Estados Unidos, incluindo data centers em cidades como Virgínia e Carolina do Norte.
2. Região Oeste da Europa: localizada na Europa Ocidental, com data centers em cidades como Amsterdã e Paris.
3. Região Leste da Ásia: localizada no leste da Ásia, com data centers em cidades como Hong Kong e Cingapura.
4. Região Sul do Brasil: localizada no sul do Brasil, com data centers em cidades como São Paulo e Rio de Janeiro.
5. Região Oeste da Austrália: localizada na Austrália Ocidental, com data centers em cidades como Perth.

Cada região do Azure é independente e opera como uma unidade isolada, com sua própria infraestrutura de data center, energia, rede e serviços. Isso permite que os clientes implantem e executem aplicativos e serviços em uma região específica, garantindo baixa latência, alta disponibilidade e conformidade regulatória.

Além disso, o Azure oferece pares de região, que são duas regiões geograficamente separadas dentro de uma mesma área geográfica. Esses pares de região são projetados para fornecer resiliência e recuperação de desastres, permitindo a replicação de dados e a continuidade do serviço em caso de falhas em uma região.

Em resumo, as regiões do Azure são locais geográficos onde os data centers do Azure estão localizados. Cada região é independente e oferece serviços e recursos do Azure, permitindo que os clientes implantem e executem aplicativos e serviços em uma área geográfica específica.

### Zonas de Disponibilidade

\-> zonas dentro de uma mesma região, mas separadas fisicamente para maior confiabilidade, ou seja, se alguma zona falhar, poderá usar outra

As zonas de disponibilidade no Azure são localizações físicas dentro de uma região do Azure que são projetadas para serem independentes e isoladas entre si. Cada zona de disponibilidade consiste em um ou mais data centers equipados com energia, refrigeração e redes redundantes.

O principal objetivo das zonas de disponibilidade é fornecer alta disponibilidade e resiliência para aplicativos e serviços que são executados no Azure. Ao distribuir os recursos de forma equitativa em diferentes zonas de disponibilidade, o risco de interrupções devido a falhas em um data center ou em uma zona específica é minimizado.

Ao implantar um aplicativo ou serviço no Azure, é recomendável distribuir os recursos em diferentes zonas de disponibilidade para garantir a continuidade do serviço em caso de falhas. Isso é alcançado por meio da replicação de dados e configuração do aplicativo para que possa alternar automaticamente para uma zona de disponibilidade diferente em caso de interrupção.

O Azure garante que as zonas de disponibilidade dentro de uma região estejam conectadas por meio de uma rede de alta velocidade e baixa latência, permitindo a replicação de dados e a alternância automática entre zonas em caso de falha.

Em resumo, as zonas de disponibilidade no Azure são uma forma de garantir alta disponibilidade e resiliência de aplicativos e serviços ao distribuí-los em diferentes localizações físicas dentro de uma região. Isso ajuda a minimizar o risco de interrupções e garante a continuidade do serviço em caso de falhas.



### Pares de Região

\-> alguns serviços são replicados em pares de regiões mais distantes uma da outra, em caso de desastres

Os pares de região no Azure são uma configuração que permite a replicação de dados e a continuidade do serviço entre duas regiões geograficamente separadas. Cada região em um par de região é considerada uma região primária ou secundária.

A configuração de pares de região é importante para garantir a resiliência e a recuperação de desastres em caso de falhas em uma região. Quando uma região primária enfrenta uma interrupção, a região secundária pode assumir a carga de trabalho e manter a continuidade do serviço.

Ao configurar um par de região, é importante escolher regiões que estejam geograficamente distantes o suficiente para minimizar o risco de serem afetadas por um mesmo evento catastrófico, como um terremoto ou uma tempestade severa.

A replicação de dados entre as regiões primária e secundária é realizada por meio de serviços como a replicação geográfica do Azure SQL Database, a replicação de armazenamento do Azure ou a replicação de máquinas virtuais do Azure.

Além da replicação de dados, é importante também configurar a failover automática para que, em caso de falha na região primária, a carga de trabalho seja automaticamente redirecionada para a região secundária.

Os pares de região no Azure são uma estratégia eficaz para garantir a continuidade do serviço e a recuperação de desastres, permitindo que os aplicativos e serviços sejam executados sem interrupções, mesmo em caso de falhas em uma região específica.



### Regiões Soberanas

\-> EUA segue as questões legais de la e tem serviços do azure governamental que são instancias separadas para controle das questões legais que são acessadas somente por pesssoas do governo e são em instancias separadas, redes diferentes para maior segurança

Também há uma nuvem da China, não tão fechada qanto dos EUA, nela pode acessar os serviços mas não os dados

As regiões soberanas no Azure são regiões específicas que são projetadas para atender aos requisitos de soberania de dados e conformidade regulatória de um país ou região específica. Essas regiões são isoladas e operadas por entidades governamentais ou parceiros confiáveis, em conformidade com as leis e regulamentos locais.

As regiões soberanas são projetadas para atender às necessidades exclusivas de governos, setores governamentais e organizações que lidam com dados sensíveis ou críticos. Elas oferecem recursos e serviços do Azure, como computação, armazenamento, rede e serviços de dados, que são adaptados para atender aos requisitos de segurança e conformidade específicos de cada região.

Ao usar as regiões soberanas do Azure, as organizações podem garantir que seus dados permaneçam dentro das fronteiras do país ou região, em conformidade com as leis e regulamentos locais. Isso é especialmente importante para setores como governo, saúde, finanças e defesa, que têm requisitos rigorosos de soberania de dados e conformidade.

As regiões soberanas do Azure são projetadas para fornecer alta disponibilidade, resiliência e segurança, assim como as outras regiões do Azure. Elas também seguem os mesmos padrões de conformidade, como ISO 27001, GDPR e HIPAA, para garantir a proteção dos dados e a conformidade regulatória.

Em resumo, as regiões soberanas no Azure são regiões específicas que atendem aos requisitos de soberania de dados e conformidade regulatória de um país ou região específica. Elas oferecem recursos e serviços adaptados para atender às necessidades exclusivas de governos e organizações que lidam com dados sensíveis ou críticos, garantindo a conformidade com as leis e regulamentos locais.

### Recursos do Azure

Os recursos do Azure são os serviços e funcionalidades disponíveis na plataforma de nuvem da Microsoft, conhecida como Microsoft Azure. Esses recursos abrangem uma ampla gama de áreas, desde computação e armazenamento até inteligência artificial e análise de dados. Aqui estão alguns exemplos dos principais recursos do Azure:

1. Máquinas Virtuais (VMs): permitem a criação e o gerenciamento de máquinas virtuais baseadas em Windows ou Linux, fornecendo recursos de computação escaláveis e flexíveis.
2. Armazenamento: oferece diferentes tipos de armazenamento, como Armazenamento de Blobs (para armazenamento de objetos), Armazenamento de Arquivos (para compartilhamento de arquivos) e Armazenamento de Tabelas (para armazenamento de dados não estruturados).
3. Banco de Dados: inclui serviços de banco de dados relacionais, como o Azure SQL Database, e serviços de banco de dados NoSQL, como o Azure Cosmos DB, para atender a diferentes necessidades de armazenamento e consulta de dados.
4. Redes: fornece recursos para criar e gerenciar redes virtuais, balanceadores de carga, gateways VPN e outros componentes de rede para conectar e proteger aplicativos e serviços.
5. Serviços de Aplicativos: inclui serviços como o Azure App Service, que permite hospedar e gerenciar aplicativos web, móveis e APIs de forma escalável e segura.
6. Análise de Dados: oferece serviços para processamento e análise de dados, como o Azure Data Lake Analytics e o Azure Databricks, que permitem executar consultas e análises em grande escala.
7. Inteligência Artificial (IA) e Aprendizado de Máquina: inclui serviços como o Azure Machine Learning, que permite criar, treinar e implantar modelos de aprendizado de máquina, e o Azure Cognitive Services, que oferece recursos de IA pré-treinados, como reconhecimento de fala e visão computacional.
8. Internet das Coisas (IoT): fornece serviços e ferramentas para conectar, monitorar e gerenciar dispositivos IoT, como o Azure IoT Hub e o Azure IoT Central.

<figure><img src="../.gitbook/assets/image (11) (1).png" alt="" width="563"><figcaption></figcaption></figure>

É possível conectar máquinas virtuais a máquina físicas



### Grupo de Recursos

Um grupo de recursos no Azure é um contêiner lógico que agrupa recursos relacionados para facilitar o gerenciamento, a implantação e o monitoramento. Ele fornece uma maneira organizada de gerenciar todos os recursos associados a um projeto ou aplicativo específico.

Ao criar um grupo de recursos, você pode agrupar recursos que fazem parte de uma solução específica, como máquinas virtuais, armazenamento, redes, bancos de dados e muito mais. Isso permite que você gerencie e implante esses recursos como uma unidade coesa.

Alguns pontos importantes sobre grupos de recursos no Azure:

1. Escopo: Um grupo de recursos é criado em uma assinatura do Azure e pode conter recursos de várias regiões.
2. Gerenciamento: Ao usar um grupo de recursos, você pode gerenciar todos os recursos relacionados de forma centralizada. Isso inclui a implantação, atualização, monitoramento e exclusão de recursos.
3. Agrupamento lógico: Os recursos em um grupo de recursos podem ser implantados, atualizados ou excluídos juntos. Isso facilita a organização e o gerenciamento de recursos relacionados.
4. Tags: É possível adicionar tags a um grupo de recursos para categorizá-lo e identificá-lo com metadados adicionais. Isso ajuda na organização e no controle de custos.
5. Controle de acesso: É possível definir permissões de acesso granulares para um grupo de recursos, permitindo que diferentes usuários ou equipes tenham acesso e controle específicos sobre os recursos contidos nele.
6. Faturamento: Os custos associados aos recursos em um grupo de recursos são agrupados e faturados juntos, facilitando o acompanhamento e a análise dos custos relacionados a um projeto ou aplicativo específico.

Em resumo, um grupo de recursos no Azure é um contêiner lógico que agrupa recursos relacionados para facilitar o gerenciamento, a implantação e o monitoramento. Ele fornece uma maneira organizada de gerenciar recursos em uma assinatura do Azure e permite que você implante, atualize e exclua recursos de forma coesa.

<figure><img src="../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

Esses grupos não precisam necessariamente estar em uma mesma região e desde que tenha permissão, é possível usar vários grupos de recursos

{% embed url="https://medium.com/@rodrigocameloMCT/o-que-%C3%A9-grupo-de-recursos-do-azure-a03ef0059ad8" %}

### Datacenters

Os data centers do Azure são instalações físicas onde os servidores e infraestrutura de rede do Microsoft Azure estão localizados. Esses data centers são projetados para fornecer serviços de nuvem confiáveis, escaláveis e seguros em todo o mundo.

Os data centers do Azure são distribuídos em várias regiões geográficas em todo o mundo. Cada região do Azure pode ter um ou mais data centers, dependendo da demanda e da capacidade necessária para atender aos clientes naquela região.

Esses data centers são construídos com tecnologias avançadas para garantir a disponibilidade, a segurança e a eficiência energética. Eles possuem sistemas de energia redundantes, resfriamento eficiente, proteção contra incêndio, segurança física e controles de acesso rigorosos para proteger os dados e os recursos dos clientes.

Os data centers do Azure são interconectados por meio de uma rede de alta velocidade e baixa latência, permitindo a replicação de dados e a comunicação eficiente entre as regiões. Isso permite que os clientes implantem aplicativos e serviços em várias regiões para garantir alta disponibilidade, resiliência e recuperação de desastres.

Além disso, os data centers do Azure são projetados para atender a uma variedade de requisitos de conformidade e segurança, como ISO 27001, GDPR, HIPAA e muito mais. Isso garante que os dados dos clientes sejam protegidos e que os serviços do Azure estejam em conformidade com as regulamentações e padrões de segurança aplicáveis.

Em resumo, os data centers do Azure são instalações físicas onde a infraestrutura de nuvem do Microsoft Azure está localizada. Eles são projetados para fornecer serviços de nuvem confiáveis, escaláveis e seguros em todo o mundo, garantindo alta disponibilidade, segurança e conformidade regulatória.

### Assinaturas

Limite de cobrança

Para cada fatura criada é uma conta diferente, separa as faturas para um controle maior

Limita quais funções a assinatura pode usar

As assinaturas do Azure são a forma de acesso e utilização dos serviços e recursos oferecidos pela plataforma de nuvem da Microsoft. Uma assinatura do Azure é uma conta que permite aos usuários criar e gerenciar recursos, como máquinas virtuais, bancos de dados, armazenamento, redes e muito mais.

Cada assinatura do Azure está associada a um contrato de serviço e a um modelo de cobrança. Existem diferentes tipos de assinaturas disponíveis, como assinaturas gratuitas, assinaturas de pagamento por uso e assinaturas de contrato de empresa.

As assinaturas gratuitas do Azure permitem que os usuários experimentem os serviços básicos do Azure por um período limitado, sem custos. Essas assinaturas têm limitações de recursos e podem ser atualizadas para uma assinatura paga, se necessário.

As assinaturas de pagamento por uso permitem que os usuários paguem apenas pelos recursos e serviços que utilizam. Os custos são calculados com base no consumo de recursos, como tempo de execução de máquinas virtuais, armazenamento utilizado e transferência de dados.

As assinaturas de contrato de empresa são destinadas a organizações que desejam ter um acordo de longo prazo com a Microsoft. Essas assinaturas oferecem benefícios adicionais, como descontos por volume, suporte técnico prioritário e opções de personalização.

Ao criar uma assinatura do Azure, os usuários podem gerenciar seus recursos por meio do portal do Azure, da linha de comando, APIs ou ferramentas de automação. Eles também podem controlar o acesso aos recursos, monitorar o uso e gerenciar os custos associados à assinatura.

Em resumo, as assinaturas do Azure são contas que permitem aos usuários acessar e utilizar os serviços e recursos da plataforma de nuvem do Microsoft Azure. Existem diferentes tipos de assinaturas disponíveis, cada uma com seus próprios modelos de cobrança e benefícios.



### Grupos de Gerenciamento

Os Grupos de Gerenciamento no Azure são recursos que permitem organizar e gerenciar recursos relacionados em uma hierarquia lógica. Eles fornecem uma maneira de agrupar recursos em uma única unidade de gerenciamento, independentemente da sua localização geográfica ou assinatura do Azure.

Com os Grupos de Gerenciamento, você pode aplicar políticas, atribuir permissões de acesso, monitorar e controlar recursos de forma centralizada. Isso facilita a administração e o gerenciamento de recursos em grande escala, especialmente em ambientes complexos com várias assinaturas e regiões.

Os Grupos de Gerenciamento podem ser usados para organizar recursos com base em diferentes critérios, como departamento, projeto, ambiente (produção, desenvolvimento, teste) ou qualquer outra estrutura que faça sentido para a sua organização.

Dentro de um Grupo de Gerenciamento, você pode definir políticas de conformidade e governança para garantir que os recursos estejam em conformidade com os requisitos de segurança, conformidade e melhores práticas da sua organização. Essas políticas podem ser aplicadas a todos os recursos dentro do grupo, independentemente da assinatura ou região em que estão localizados.

Além disso, os Grupos de Gerenciamento permitem delegar permissões de acesso granulares, permitindo que você conceda acesso a usuários ou equipes específicas para gerenciar recursos dentro do grupo, sem conceder acesso a toda a assinatura.

Em resumo, os Grupos de Gerenciamento no Azure são recursos que permitem organizar e gerenciar recursos relacionados em uma hierarquia lógica. Eles facilitam o gerenciamento centralizado, a aplicação de políticas e o controle de acesso em ambientes complexos com vários recursos e assinaturas.

<figure><img src="../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

{% embed url="https://learn.microsoft.com/pt-br/azure/governance/management-groups/overview" %}

#### Serviços de computação azure



Fornece opções de computação como discos, processadores...

#### Máquinas Virtuais

Se uma VM falhar, será feito uma réplica e se houver sobrecarga de um domínio, será replicado para outro domínio

#### Área de trabalho Azure

#### Serviços de contêineres Azure

<figure><img src="../.gitbook/assets/image (14).png" alt="" width="563"><figcaption></figcaption></figure>

#### Azure Functions

Função seja de programação ou relacionada a outros recursos

<figure><img src="../.gitbook/assets/image (15).png" alt="" width="375"><figcaption></figcaption></figure>



#### Serviço de Aplicativo

\-> PaaS

* Facilita para implementação, criação e dimensionamento de APIs e serviços WEB

#### Rede Virtual

* Comunicação entre rede local e virtual/rede e nuvem
* Controle dessa rede virtual dentro de uma rede privada
* Se for usar rede pública é mais fácil utilizar a internet
* É possível deixar uma rede privada que possui pontos e serviços que se comunicam com a internet

### Serviços de Rede do Azure

#### Gateway de VPN

O Gateway de VPN do Azure é um serviço que pode ser usado para enviar tráfego criptografado entre uma rede virtual do Azure e locais pela Internet pública. Também é possível usar um Gateway de VPN para enviar tráfego criptografado entre as redes virtuais do Azure pela rede da Microsoft. O Gateway de VPN usa um tipo específico de gateway de rede virtual do Azure chamado gateway de VPN. Várias conexões podem ser criadas com o mesmo gateway de VPN.

{% embed url="https://learn.microsoft.com/pt-br/azure/vpn-gateway/vpn-gateway-about-vpngateways" %}

#### ExpressRoute

estende as redes locais para Azure por meio de uma conexão privada

#### DNS do Azure

Cuida da parte de segurança, controle maior, é um dos protocolos de segurança

### Armazenamento

#### Contas de Armazenamento

<figure><img src="../.gitbook/assets/image (1) (1).png" alt="" width="375"><figcaption></figcaption></figure>

#### Serviços de armazenamento

<figure><img src="../.gitbook/assets/image (17).png" alt="" width="563"><figcaption></figcaption></figure>

URLs para acessar esses serviços:

<figure><img src="../.gitbook/assets/image (18).png" alt="" width="563"><figcaption></figcaption></figure>



#### Camadas de acesso de armazenamento

<figure><img src="../.gitbook/assets/image (19).png" alt="" width="563"><figcaption></figcaption></figure>

Frequente -> mais acesssado e um custo menor por acesso mas acaba sendo maior em questão de armazenamento e de acesso

Arquivo Morto -> maior custo de acesso e menor custo para manter, de acesso

#### Migrações para Azure

* Azure Data Box

<figure><img src="../.gitbook/assets/image (1).png" alt="" width="375"><figcaption></figcaption></figure>

\-> Facilita a migração dos dados

* Opções de gerenciamento de arquivos

<figure><img src="../.gitbook/assets/image (2).png" alt="" width="563"><figcaption></figcaption></figure>
