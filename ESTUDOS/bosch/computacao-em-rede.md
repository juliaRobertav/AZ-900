# Computação em Rede



### Serviços de Computação do Azure

O Azure oferece uma ampla gama de serviços de computação para atender às necessidades de diferentes cargas de trabalho e cenários de aplicativos. Alguns dos principais serviços de computação do Azure incluem:

1. Máquinas Virtuais (VMs): Permitem a criação e o gerenciamento de máquinas virtuais baseadas em Windows ou Linux, oferecendo flexibilidade e controle total sobre o ambiente de computação.
2. Azure Functions: É um serviço de computação sem servidor que permite executar código em resposta a eventos, como acionadores de HTTP, eventos de armazenamento ou mensagens em filas.
3. Azure App Service: Oferece uma plataforma gerenciada para hospedar aplicativos web, móveis e APIs. Suporta várias linguagens de programação e integração com outros serviços do Azure.
4. Azure Batch: É um serviço de computação em lote para executar cargas de trabalho em paralelo e de alto desempenho. É útil para processamento em lote, renderização de imagens, simulações e outras tarefas intensivas em computação.
5. Azure Container Instances: Permite executar contêineres sem a necessidade de gerenciar a infraestrutura subjacente. É uma opção rápida e fácil para implantar e executar contêineres isolados.
6. Azure Kubernetes Service (AKS): É um serviço gerenciado que simplifica a implantação, o gerenciamento e a escala de aplicativos em contêiner usando o Kubernetes.
7. Azure Service Fabric: É uma plataforma de sistema distribuído que facilita a construção, implantação e gerenciamento de aplicativos escaláveis e altamente disponíveis.



### Máquinas Virtuais

As máquinas virtuais do Azure (VMs) são emulações de software de computadores físicos.

&#x20;• Inclui processador virtual, memória, armazenamento e rede.&#x20;

• Oferta de IaaS que oferece personalização e controle total.

Os Conjuntos de Dimensionamento de VMs e os Conjuntos de Disponibilidade de VMs são recursos do Azure que visam melhorar a disponibilidade, escalabilidade e gerenciamento de máquinas virtuais (VMs) em um ambiente de nuvem.

* Conjuntos de Dimensionamento de VMs (VM Scale Sets): Permitem criar e gerenciar um conjunto de VMs idênticas que podem ser dimensionadas automaticamente com base na demanda. Isso permite que você aumente ou diminua o número de VMs em resposta ao tráfego do aplicativo, garantindo que a capacidade seja ajustada de acordo com as necessidades. Os Conjuntos de Dimensionamento de VMs são úteis para cargas de trabalho que exigem escalabilidade horizontal, como aplicativos web, serviços de back-end e clusters de processamento.
* Conjuntos de Disponibilidade de VMs (VM Availability Sets): São usados para garantir alta disponibilidade e tolerância a falhas para VMs. Ao criar um Conjunto de Disponibilidade, você distribui as VMs em diferentes domínios de falha e atualização dentro de uma região do Azure. Isso garante que, se um domínio de falha ou atualização for afetado, pelo menos uma VM permanecerá em execução. Os Conjuntos de Disponibilidade são recomendados para cargas de trabalho críticas que exigem alta disponibilidade, como aplicativos empresariais e bancos de dados.

Ambos os recursos podem ser usados em conjunto para obter uma solução mais robusta. Por exemplo, você pode criar um Conjunto de Dimensionamento de VMs dentro de um Conjunto de Disponibilidade para obter escalabilidade e alta disponibilidade ao mesmo tempo.

Em resumo, os Conjuntos de Dimensionamento de VMs permitem dimensionar automaticamente o número de VMs com base na demanda, enquanto os Conjuntos de Disponibilidade garantem alta disponibilidade e tolerância a falhas para VMs. Ambos os recursos são úteis para melhorar a escalabilidade, disponibilidade e gerenciamento de VMs no Azure.



### Área de trabalho virtual do Azure

A Área de Trabalho Virtual do Azure, também conhecida como Windows Virtual Desktop (WVD), é um serviço de virtualização de desktop baseado na nuvem oferecido pelo Azure. Ele permite que você forneça desktops virtuais e aplicativos remotos para seus usuários, permitindo que eles acessem seus ambientes de trabalho a partir de qualquer dispositivo, em qualquer lugar.

Com a Área de Trabalho Virtual do Azure, você pode criar e gerenciar pools de máquinas virtuais do Windows que são usadas para fornecer desktops virtuais. Esses desktops podem ser personalizados com aplicativos e configurações específicas para atender às necessidades dos usuários.

Além disso, a Área de Trabalho Virtual do Azure oferece suporte para a virtualização de aplicativos, permitindo que você publique aplicativos individuais em vez de desktops completos. Isso é útil quando você precisa fornecer acesso a aplicativos específicos para usuários ou grupos de usuários.

A Área de Trabalho Virtual do Azure oferece recursos avançados, como redimensionamento automático de máquinas virtuais com base na demanda, integração com serviços do Azure, como o Azure Active Directory, e suporte para ambientes de trabalho multiusuário.

Esse serviço é particularmente útil para organizações que desejam fornecer acesso remoto a aplicativos e desktops, permitindo que os usuários trabalhem de forma flexível e produtiva, sem a necessidade de manter infraestrutura local complexa.

Em resumo, a Área de Trabalho Virtual do Azure é um serviço de virtualização de desktop baseado na nuvem que permite fornecer desktops virtuais e aplicativos remotos para usuários. Ele oferece flexibilidade, escalabilidade e segurança, permitindo que os usuários acessem seus ambientes de trabalho a partir de qualquer dispositivo, em qualquer lugar.



### Serviços de contêineres do Azure

O Azure oferece uma variedade de serviços de contêineres para ajudar no desenvolvimento, implantação e gerenciamento de aplicativos em contêiner. Alguns dos principais serviços de contêineres do Azure incluem:

1. Azure Container Instances: É um serviço sem servidor que permite executar contêineres isolados sem a necessidade de gerenciar a infraestrutura subjacente. É uma opção rápida e fácil para implantar e executar contêineres individuais.
2. Azure Kubernetes Service (AKS): É um serviço gerenciado que simplifica a implantação, o gerenciamento e a escala de aplicativos em contêiner usando o Kubernetes. O AKS oferece recursos avançados, como balanceamento de carga, escalabilidade automática e monitoramento integrado.
3. Azure Container Registry: É um serviço de registro de contêiner privado que permite armazenar, gerenciar e implantar imagens de contêiner. Ele fornece um local seguro para armazenar e compartilhar imagens de contêiner usadas em seus aplicativos.
4. Azure Container Instances for Web Apps: É uma opção de hospedagem para aplicativos web baseados em contêiner. Ele permite que você implante aplicativos web em contêiner diretamente no Azure sem a necessidade de configurar e gerenciar um cluster Kubernetes.
5. Azure Service Fabric: Embora não seja exclusivamente um serviço de contêineres, o Azure Service Fabric oferece suporte a implantação e gerenciamento de aplicativos em contêiner. Ele fornece recursos para criar aplicativos escaláveis e altamente disponíveis usando contêineres e serviços de microsserviços.

Esses serviços de contêineres do Azure oferecem opções flexíveis para implantar, gerenciar e escalar aplicativos em contêiner, permitindo que você escolha a abordagem mais adequada às suas necessidades. Eles simplificam o processo de implantação e gerenciamento de contêineres, fornecendo recursos avançados para garantir a escalabilidade, a disponibilidade e a segurança dos aplicativos.

<figure><img src="../.gitbook/assets/image (14).png" alt="" width="563"><figcaption></figcaption></figure>



### Azure Functions

O Azure Functions é um serviço de computação sem servidor fornecido pela Microsoft Azure. Ele permite que os desenvolvedores criem e implantem funções pequenas e orientadas a eventos que podem ser acionadas por vários eventos e executem código em um ambiente sem servidor. O Azure Functions suporta várias linguagens de programação, incluindo C#, JavaScript, Python e mais.

As principais características do Azure Functions incluem:

1. Execução orientada a eventos: As funções podem ser acionadas por vários eventos, como solicitações HTTP, temporizadores, filas de mensagens, eventos de armazenamento e mais. Esse modelo orientado a eventos permite que os desenvolvedores criem aplicativos que respondam a eventos ou condições específicas.
2. Arquitetura sem servidor: O Azure Functions abstrai a infraestrutura subjacente, permitindo que os desenvolvedores se concentrem apenas na escrita do código de suas funções. O serviço dimensiona automaticamente o ambiente de execução com base na demanda, garantindo desempenho e eficiência de custos ideais.
3. Preço conforme o uso: Com o Azure Functions, você paga apenas pelo tempo real de execução de suas funções. Não há custos iniciais ou cobranças por tempo ocioso, tornando-o uma solução econômica para cargas de trabalho orientadas a eventos.
4. Integração com outros serviços do Azure: O Azure Functions se integra perfeitamente a outros serviços do Azure, como Azure Storage, Azure Event Hubs, Azure Cosmos DB e mais. Isso permite que os desenvolvedores criem fluxos de trabalho complexos e aproveitem as capacidades de outros serviços do Azure em suas funções.
5. Opções de desenvolvimento e implantação: O Azure Functions oferece várias opções de desenvolvimento e implantação, incluindo portal do Azure, Visual Studio, Azure CLI e Azure DevOps. Essa flexibilidade permite que os desenvolvedores escolham as ferramentas e fluxos de trabalho que melhor atendam às suas necessidades.

O Azure Functions é comumente usado para criar aplicativos sem servidor, microsserviços e arquiteturas orientadas a eventos. Ele oferece uma solução escalável e econômica para executar pequenos trechos de código em resposta a eventos ou acionadores específicos.



### Comparar opções de Computação

O Azure oferece várias opções de computação para atender às diferentes necessidades e cargas de trabalho. Vamos comparar algumas delas:

1. Máquinas Virtuais (VMs): As VMs do Azure fornecem uma infraestrutura virtualizada, permitindo que você execute aplicativos e sistemas operacionais completos em um ambiente flexível. Elas oferecem controle total sobre a configuração e personalização do ambiente de computação, mas exigem gerenciamento e manutenção contínuos.
2. Azure Functions: O Azure Functions é um serviço de computação sem servidor que permite que você execute pequenos trechos de código em resposta a eventos específicos. Ele dimensiona automaticamente com base na demanda e você paga apenas pelo tempo de execução das funções. É ideal para cargas de trabalho orientadas a eventos e oferece uma abordagem mais simplificada, sem a necessidade de gerenciar a infraestrutura subjacente.
3. Serviço de Aplicativo (App Service): O Azure App Service é uma plataforma gerenciada para hospedar aplicativos da web, móveis e APIs. Ele oferece suporte a várias linguagens de programação e frameworks, como .NET, Java, Node.js e PHP. O App Service gerencia a infraestrutura subjacente, permitindo que você se concentre no desenvolvimento de aplicativos.
4. Azure Batch: O Azure Batch é um serviço de computação em lote que permite executar cargas de trabalho de alto desempenho e paralelas em escala. Ele é ideal para processamento em lote, simulações, renderização de imagens e outras tarefas intensivas em computação. O Azure Batch gerencia automaticamente a distribuição de tarefas em várias VMs para otimizar o desempenho.
5. Serviço de Contêiner do Azure (Azure Container Service): O Azure Container Service permite implantar e gerenciar aplicativos em contêiner usando tecnologias como Docker e Kubernetes. Ele fornece uma plataforma escalável e flexível para executar aplicativos em contêiner em várias VMs, simplificando o gerenciamento e a orquestração de contêineres.

Essas são apenas algumas das opções de computação do Azure. A escolha depende das necessidades específicas do seu aplicativo, como controle, escalabilidade, gerenciamento e custo.

<figure><img src="../.gitbook/assets/image (15).png" alt="" width="375"><figcaption></figcaption></figure>



### Serviços de Aplicativo Azure

Facilita para implementação, criação e dimensionamento de APIs e serviços WEB

Os Serviços de Aplicativo do Azure são uma opção popular para hospedar aplicativos da web, móveis e APIs na nuvem. Eles oferecem uma plataforma gerenciada que simplifica o processo de implantação, dimensionamento e gerenciamento de aplicativos.

Aqui estão alguns pontos-chave sobre os Serviços de Aplicativo do Azure:

1. Hospedagem flexível: Os Serviços de Aplicativo suportam várias linguagens de programação, como .NET, Java, Node.js, Python e PHP. Isso permite que você desenvolva aplicativos usando a linguagem de sua escolha.
2. Escalabilidade automática: Os Serviços de Aplicativo do Azure dimensionam automaticamente seus aplicativos com base na demanda. Isso significa que, se houver um aumento repentino no tráfego, o serviço ajustará automaticamente a capacidade para lidar com a carga.
3. Gerenciamento simplificado: O Azure gerencia a infraestrutura subjacente dos Serviços de Aplicativo, incluindo patches de segurança, atualizações e monitoramento. Isso permite que você se concentre no desenvolvimento de aplicativos, em vez de se preocupar com a infraestrutura.
4. Integração com outros serviços do Azure: Os Serviços de Aplicativo podem ser facilmente integrados a outros serviços do Azure, como bancos de dados SQL do Azure, Armazenamento do Azure, Serviços Cognitivos do Azure e muito mais. Isso permite que você crie aplicativos mais poderosos e ricos em recursos.
5. DevOps e CI/CD: Os Serviços de Aplicativo do Azure têm integração nativa com ferramentas de DevOps populares, como o Azure DevOps e o GitHub Actions. Isso facilita a implantação contínua (CI/CD) e a automação do ciclo de vida do aplicativo.

Em resumo, os Serviços de Aplicativo do Azure oferecem uma plataforma gerenciada e flexível para hospedar seus aplicativos na nuvem. Eles simplificam o processo de implantação, dimensionamento e gerenciamento, permitindo que você se concentre no desenvolvimento de aplicativos e na entrega de valor aos usuários finais.



### Serviços de Rede Azure

Os Serviços de Rede do Azure fornecem uma variedade de recursos e serviços para ajudar na criação e gerenciamento de redes na nuvem. Aqui estão alguns dos principais serviços de rede do Azure:

1. Virtual Network (VNet): O Azure Virtual Network permite criar redes isoladas na nuvem, semelhantes a redes locais tradicionais. Ele permite que você defina sub-redes, configure regras de firewall, conecte-se a redes locais por meio de VPNs e controle o tráfego de rede.
2. Azure Load Balancer: O Azure Load Balancer distribui o tráfego de entrada entre várias instâncias de máquinas virtuais ou serviços de back-end para melhorar a disponibilidade e a escalabilidade dos aplicativos. Ele oferece balanceamento de carga baseado em TCP e UDP.
3. Azure Application Gateway: O Azure Application Gateway é um serviço de balanceamento de carga de aplicativos que fornece recursos avançados, como roteamento baseado em URL, balanceamento de carga com base na sessão e terminação SSL. Ele é especialmente útil para aplicativos da web.
4. Azure VPN Gateway: O Azure VPN Gateway permite estabelecer conexões seguras entre redes locais e redes virtuais do Azure por meio de VPNs. Isso permite a extensão de redes locais para a nuvem e a conexão segura entre locais geograficamente distribuídos.
5. Azure ExpressRoute: O Azure ExpressRoute oferece uma conexão dedicada e privada entre sua infraestrutura local e a nuvem do Azure. Ele fornece maior largura de banda, latência reduzida e maior segurança em comparação com conexões públicas pela Internet.
6. Azure DNS: O Azure DNS é um serviço de hospedagem de DNS (Domain Name System) que permite gerenciar e resolver nomes de domínio na nuvem do Azure. Ele fornece resolução rápida e confiável de nomes de domínio para seus aplicativos e serviços.

Esses são apenas alguns dos serviços de rede do Azure disponíveis. Eles oferecem recursos avançados para criar, conectar e proteger redes na nuvem, permitindo que você crie arquiteturas de rede flexíveis e escaláveis para seus aplicativos e serviços.

#### Rede Virtual

* Comunicação entre rede local e virtual/rede e nuvem
* Controle dessa rede virtual dentro de uma rede privada
* Se for usar rede pública é mais fácil utilizar a internet
* É possível deixar uma rede privada que possui pontos e serviços que se comunicam com a internet

#### Gateway de VPN

O Gateway de VPN do Azure é um serviço que pode ser usado para enviar tráfego criptografado entre uma rede virtual do Azure e locais pela Internet pública. Também é possível usar um Gateway de VPN para enviar tráfego criptografado entre as redes virtuais do Azure pela rede da Microsoft. O Gateway de VPN usa um tipo específico de gateway de rede virtual do Azure chamado gateway de VPN. Várias conexões podem ser criadas com o mesmo gateway de VPN.

{% embed url="https://learn.microsoft.com/pt-br/azure/vpn-gateway/vpn-gateway-about-vpngateways" %}

<figure><img src="../.gitbook/assets/image (20).png" alt="" width="563"><figcaption></figcaption></figure>

#### ExpressRoute

estende as redes locais para Azure por meio de uma conexão privada

<figure><img src="../.gitbook/assets/image (22).png" alt="" width="563"><figcaption></figcaption></figure>

#### DNS do Azure

Cuida da parte de segurança, controle maior, é um dos protocolos de segurança.
