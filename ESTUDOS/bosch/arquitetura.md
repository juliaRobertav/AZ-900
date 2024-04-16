---
description: Arquitetura Azure
---

# Arquitetura

Esse site explica melhor sobre os conceitos de arquitetura azure:

{% embed url="https://learn.microsoft.com/pt-br/azure/architecture/guide/" %}

#### Zonas de disponibilidade

\-> zonas dentro de uma mesma região, mas separadas fisicamente para maior confiabilidade, ou seja, se alguma zona falhar, poderá usar outra

#### Pares de região

\-> alguns serviços são replicados em pares de regiões mais distantes uma da outra, em caso de desastres

#### Regiões Soberanas

\-> EUA segue as questões legais de la e tem serviços do azure governamental que são instancias separadas para controle das questões legais que são acessadas somente por pesssoas do governo e são em instancias separadas, redes diferentes para maior segurança

Também há uma nuvem da China, não tão fechada qanto dos EUA, nela pode acessar os serviços mas não os dados

#### Recursos da Azure

<figure><img src="../.gitbook/assets/image (11).png" alt="" width="563"><figcaption></figcaption></figure>

É possível conectar máquinas virtuais a máquina físicas

#### Grupo de Recursos

<figure><img src="../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

Esses grupos não precisam necessariamente estar em uma mesma região e desde que tenha permissão, é possível usar vários grupos de recursos

{% embed url="https://medium.com/@rodrigocameloMCT/o-que-%C3%A9-grupo-de-recursos-do-azure-a03ef0059ad8" %}

#### Assinatura

Limite de cobrança

Para cada fatura criada é uma conta diferente, separa as faturas para um controle maior

Limita quais funções a assinatura pode usar

#### Grupos de Gerenciamento

<figure><img src="../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

{% embed url="https://learn.microsoft.com/pt-br/azure/governance/management-groups/overview" %}

#### Soluções em computação azure



Fornece opções de computação como discos, processadores...

#### Grupos de Gerenciamento

* Grupos de gerenciamento são contêineres que o ajudarão a gerenciar o acesso, a política e a conformidade entre várias assinaturas

{% embed url="https://learn.microsoft.com/pt-br/azure/governance/management-groups/overview" %}

{% embed url="https://learn.microsoft.com/pt-br/azure/governance/management-groups/overview" %}

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
