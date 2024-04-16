---
description: Arquitetura Azure
---

# Arquitetura

Zonas de disponibiidade -> zonas dentro de uma mesma região, mas separadas fisicamente para maior confiabilidade, ou seja, se alguma zona falhar, poderá usar outra

Pares de região -> alguns serviços são replicados em pares de regiões mais distantes uma da outra, em caso de desastres

Regiões Soberanas -> EUA segue as questões legais de la e tem serviços do azure governamental que são instancias separadas para controle das questões legais que são acessadas somente por pesssoas do governo e são em instancias separadas, redes diferentes para maior segurança

Também há uma nuvem da China, não tão fechada qanto dos EUA, nela pode acessar os serviços mas não os dados



Recursos da Azure

<figure><img src="../.gitbook/assets/image (11).png" alt="" width="563"><figcaption></figcaption></figure>

É possível conectar máquinas virtuais a máquina físicas



Grupo de Recursos

<figure><img src="../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

Esses grupos não precisam necessariamente estar em uma mesma região e desde que tenha permissão, é possível usar vários grupos de recursos

{% embed url="https://medium.com/@rodrigocameloMCT/o-que-%C3%A9-grupo-de-recursos-do-azure-a03ef0059ad8" %}

Assinatura

Limite de cobrança

Para cada fatura criada é uma conta diferente, separa as faturas para um controle maior

Limita quais funções a assinatura pode usar



Grupos de Gerenciamento

<figure><img src="../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

{% embed url="https://learn.microsoft.com/pt-br/azure/governance/management-groups/overview" %}
