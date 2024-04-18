---
description: Todas as explicações detalhadas desses assuntos estão nos slides :)
---

# Introdução

### Computação em nuvem

Computação em nuvem é a entrega de serviços de  computação por meio da internet

\-> acessar qualquer serviço pela internet

* Tipos de nuvem:

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



#### Tipos de despesas



\-> CapEx (Capital)

\-> OpEx (Operacional) - cobrado na hora

* Benefícios:

\-> Alta disponibilidade

\-> Escalabilidade&#x20;

* Horizontal - adiciona mais instâncias
* Vertical -  recursos,aumenta a capacidade de uma única instância



* Dimensionamentos:

1. Dimensionamento horizontal (scaling horizontal): Também conhecido como escalabilidade horizontal, envolve adicionar mais instâncias ou réplicas do sistema ou aplicativo. Nesse caso, você distribui a carga de trabalho entre várias máquinas ou servidores. Por exemplo, se você tiver um aplicativo web, poderá adicionar mais servidores para lidar com um aumento no tráfego. O dimensionamento horizontal geralmente é mais fácil de implementar, pois não requer alterações significativas na infraestrutura existente. No entanto, pode exigir mecanismos de balanceamento de carga para distribuir o tráfego entre as instâncias.
2. Dimensionamento vertical (scaling vertical): Também conhecido como escalabilidade vertical, envolve aumentar a capacidade de uma única instância ou servidor, adicionando mais recursos a ele. Isso pode incluir aumentar a quantidade de memória, processadores, armazenamento ou outros recursos do sistema. Por exemplo, você pode atualizar um servidor com mais RAM ou adicionar mais núcleos de processamento. O dimensionamento vertical geralmente requer alterações na infraestrutura existente e pode ter limitações físicas, como a capacidade máxima de recursos em um único servidor.

Para isso a Microsoft fornece uma calculadora de preços

{% embed url="https://azure.microsoft.com/pt-br/pricing/calculator/" %}

\-> Confiabilidade

\-> Previsibilidade

\-> Segurança (obrigatório a garantia)

\-> Governança

\-> Gerenciamento

* gerenciamento <mark style="color:blue;">**da**</mark> nuvem
* gerenciamento <mark style="color:blue;">**na**</mark> nuvem

### Tipos de Serviço de nuvem

\-> IaaS (infraestrutura)

* Máquina Virtual e Contêiner por exemplo fazem parte da infraestrutura

\-> PaaS (plataforma)

\-> SaaS (software)

<figure><img src="../.gitbook/assets/image (10) (1).png" alt="" width="563"><figcaption></figcaption></figure>

* **Não necessariamente é preciso comprar os recursos da azure (principalmente em SaaS) para usar!!**
