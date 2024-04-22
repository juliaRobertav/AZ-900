# IAS (Identidade, Acesso e Segurança)

### Resumo

A identidade, acesso e segurança são aspectos fundamentais no Azure para garantir a proteção dos recursos e dados na nuvem. Aqui está uma explicação geral e abrangente sobre esses conceitos no Azure:

1. Identidade: A identidade no Azure refere-se à autenticação e autorização dos usuários e serviços que acessam os recursos. O Azure Active Directory (Azure AD) é o serviço de gerenciamento de identidade e acesso do Azure, que permite criar e gerenciar identidades de usuários, grupos e aplicativos. Ele oferece recursos como autenticação multifator, autenticação única (SSO) e integração com serviços de diretório local.
2. Acesso: O acesso no Azure envolve a concessão de permissões adequadas aos usuários e serviços para acessar os recursos. O Azure RBAC (Role-Based Access Control) é usado para atribuir funções e permissões aos usuários com base em suas responsabilidades. Ele permite definir políticas granulares de acesso para controlar quem pode fazer o quê nos recursos do Azure. Além disso, o Azure AD também oferece recursos de gerenciamento de acesso condicional para aplicar políticas de acesso com base em condições específicas, como localização, dispositivo ou risco.
3. Segurança: A segurança no Azure abrange várias camadas de proteção para garantir a confidencialidade, integridade e disponibilidade dos dados e recursos. O Azure oferece recursos de segurança em várias áreas, como rede, identidade, dados e aplicativos. Isso inclui firewalls de rede, grupos de segurança de rede, monitoramento de segurança, criptografia de dados em repouso e em trânsito, detecção de ameaças, gerenciamento de chaves e muito mais. Além disso, o Azure também está em conformidade com várias certificações e padrões de segurança reconhecidos globalmente.

É importante implementar práticas de segurança recomendadas, como o uso de senhas fortes, monitoramento contínuo, atualizações de segurança, backups regulares e revisões de permissões de acesso. O Azure fornece ferramentas e serviços para ajudar na implementação e gerenciamento da identidade, acesso e segurança, permitindo que as organizações protejam seus recursos e dados na nuvem de maneira eficaz.



### ID do Microsoft Entra

A ID do Microsoft Entra (Microsoft Entra ID) é uma identificação única fornecida pela Microsoft para permitir o acesso a vários serviços e produtos da empresa. Ela é usada para autenticar e autorizar usuários a acessar recursos como o Azure, Office 365, Xbox Live, Windows e outros serviços da Microsoft.

A ID do Microsoft Entra é criada quando um usuário se registra em um serviço da Microsoft, como a criação de uma conta do Outlook.com, uma assinatura do Office 365 ou uma conta do Xbox Live. Essa ID é composta por um endereço de email e uma senha associada a ela.

Ao fazer login com a ID do Microsoft Entra, os usuários podem acessar seus serviços e produtos da Microsoft em diferentes dispositivos, como computadores, smartphones e tablets. A autenticação pode ser feita por meio de métodos como senha, autenticação multifator ou autenticação biométrica, dependendo das configurações de segurança definidas pelo usuário.

A ID do Microsoft Entra também permite que os usuários acessem recursos adicionais, como armazenamento em nuvem no OneDrive, sincronização de configurações entre dispositivos e integração com outros serviços e aplicativos da Microsoft.

É importante manter a ID do Microsoft Entra segura, usando senhas fortes e mantendo as informações de login confidenciais. Além disso, é recomendável habilitar a autenticação multifator sempre que possível para aumentar a segurança da conta.

* gerenciamento de identidades e acesso baseado em nuvem
* autenticação
* quem pode acessar e quais dispositivos podem acessar
* SSO

### Microsoft Entra Domain Services

Microsoft Entra Domain Services (anteriormente conhecido como Azure Active Directory Domain Services) é um serviço do Azure que fornece recursos de diretório ativo gerenciado na nuvem. Ele permite que as organizações estendam seu ambiente do Active Directory local para a nuvem, fornecendo recursos como autenticação, autorização e gerenciamento de identidade.

Com o Microsoft Entra Domain Services, as organizações podem aproveitar os recursos do Active Directory sem a necessidade de implantar e gerenciar controladores de domínio locais. O serviço é totalmente gerenciado pela Microsoft, o que significa que as atualizações de segurança, patches e backups são tratados automaticamente.

Algumas das principais funcionalidades do Microsoft Entra Domain Services incluem:

1. Autenticação de usuário: Os usuários podem fazer login usando suas credenciais do Active Directory, permitindo o acesso a recursos na nuvem e no local.
2. Integração com aplicativos do Azure: O Microsoft Entra Domain Services permite que os aplicativos do Azure se integrem ao ambiente do Active Directory, permitindo a autenticação e autorização baseadas em identidade.
3. Gerenciamento de identidade: O serviço oferece recursos de gerenciamento de identidade, como criação de usuários, grupos e políticas de segurança.
4. Suporte a protocolos de autenticação: O Microsoft Entra Domain Services suporta protocolos de autenticação padrão, como Kerberos e NTLM, permitindo a interoperabilidade com aplicativos e serviços existentes.
5. Integração com redes virtuais do Azure: O serviço pode ser integrado a redes virtuais do Azure, permitindo que as máquinas virtuais se juntem ao domínio e acessem recursos do Active Directory.

O Microsoft Entra Domain Services é uma opção conveniente para organizações que desejam estender seu ambiente do Active Directory para a nuvem sem a necessidade de gerenciar infraestrutura local adicional. Ele simplifica o gerenciamento de identidade e oferece recursos de diretório ativo na nuvem de forma segura e escalável.

* Controlar e gerenciar os domínios (segurança)
* Sincronizado com Microsoft ID Entra
* Executar aplicativos herdados

<figure><img src="../.gitbook/assets/image (5).png" alt="" width="375"><figcaption></figcaption></figure>

### Comparar Autenticação e Autorização

A autenticação e a autorização são dois conceitos fundamentais em segurança da informação e controle de acesso. Embora estejam relacionados, eles têm propósitos diferentes. Aqui está uma comparação entre autenticação e autorização:

Autenticação:

* Definição: A autenticação é o processo de verificar a identidade de um usuário ou entidade que está tentando acessar um sistema ou recurso.
* Objetivo: Garantir que apenas usuários legítimos tenham acesso aos recursos, protegendo contra acesso não autorizado.
* Método: A autenticação geralmente envolve a apresentação de credenciais, como nome de usuário e senha, para verificar a identidade do usuário. Outros métodos de autenticação incluem autenticação multifator, autenticação biométrica (impressão digital, reconhecimento facial) e certificados digitais.
* Exemplo: Digitar um nome de usuário e senha ao fazer login em uma conta de email.

Autorização:

* Definição: A autorização é o processo de conceder ou negar permissões específicas a um usuário ou entidade autenticada para acessar recursos ou executar determinadas ações.
* Objetivo: Controlar o que um usuário autenticado pode fazer dentro de um sistema ou recurso, com base em suas permissões e privilégios.
* Método: A autorização é baseada em regras e políticas definidas pelo sistema. Ela determina quais recursos um usuário pode acessar e quais ações ele pode realizar nesses recursos.
* Exemplo: Um usuário autenticado pode ter permissão para ler, gravar ou excluir arquivos em uma pasta compartilhada, com base nas permissões atribuídas a ele.

Resumindo, a autenticação verifica a identidade de um usuário, enquanto a autorização controla o acesso e as permissões desse usuário aos recursos. A autenticação é o primeiro passo para garantir a segurança, enquanto a autorização define as restrições e os privilégios concedidos aos usuários autenticados. Ambos os conceitos são essenciais para garantir a proteção adequada dos sistemas e dados.

<figure><img src="../.gitbook/assets/image (6).png" alt="" width="375"><figcaption></figcaption></figure>



### Autenticação Multifator

A autenticação multifator (MFA) é um método de autenticação que requer a apresentação de mais de um fator de autenticação para verificar a identidade de um usuário. Em vez de depender apenas de uma senha, a autenticação multifator adiciona camadas extras de segurança, tornando mais difícil para um invasor obter acesso não autorizado.

Os fatores de autenticação geralmente são classificados em três categorias:

1. Algo que você sabe: Isso inclui senhas, códigos PIN ou respostas a perguntas de segurança.
2. Algo que você possui: Isso envolve dispositivos físicos, como smartphones, tokens de segurança ou cartões inteligentes.
3. Algo que você é: Isso se refere a características biométricas únicas, como impressões digitais, reconhecimento facial ou varredura de retina.

Ao usar a autenticação multifator, o usuário precisará fornecer pelo menos dois desses fatores para ser autenticado com sucesso. Por exemplo, ao fazer login em uma conta, o usuário pode inserir sua senha (algo que ele sabe) e, em seguida, receber um código de verificação em seu smartphone (algo que ele possui) para inserir como segundo fator.

A autenticação multifator é altamente recomendada para aumentar a segurança das contas e proteger contra ataques de força bruta, phishing e roubo de identidade. Ao adicionar camadas extras de autenticação, mesmo que um fator seja comprometido, o invasor ainda precisará superar os outros fatores para obter acesso. Isso torna o processo de autenticação mais seguro e confiável.

* Segurança adicional, mais de uma confirmação para autenticação completa

<figure><img src="../.gitbook/assets/image (23).png" alt="" width="563"><figcaption></figcaption></figure>



### B2B do Microsoft Entra External ID

O B2B (Business-to-Business) do Microsoft Azure permite que organizações convidem usuários externos para acessar recursos e colaborar em projetos. O External ID (Identificador Externo) é um atributo usado para identificar e vincular um usuário externo a uma organização específica.

Ao convidar um usuário externo para acessar recursos do Azure, a organização pode fornecer um External ID para esse usuário. Esse ID pode ser um identificador exclusivo gerado pela organização ou pode ser um identificador externo já existente, como um endereço de e-mail ou um identificador de usuário em outro sistema.

O External ID é útil para rastrear e gerenciar usuários externos em uma organização, permitindo que a empresa mantenha o controle sobre quem tem acesso aos recursos do Azure. Ele também pode ser usado para fins de auditoria e relatórios, ajudando a identificar quais usuários externos estão associados a quais organizações.

Ao usar o B2B do Microsoft Azure, as organizações podem estabelecer colaborações seguras com parceiros de negócios, fornecedores ou clientes externos, permitindo que eles acessem recursos específicos do Azure de forma controlada e protegida. O External ID é uma parte importante desse processo, ajudando a garantir a identificação correta dos usuários externos e a manutenção da segurança e conformidade dos dados e recursos compartilhados.

<figure><img src="../.gitbook/assets/image (7).png" alt="" width="375"><figcaption></figcaption></figure>

Acessar sua conta através de outros serviços de autenticação (Entra ID), como gmail, facebook, github por exemplo



### B2C do Identidades Externas do Azure AD

\-> conseguir acessar seus serviços através de outros tipos de contas

O B2C (Business-to-Consumer) do Azure AD (Azure Active Directory) é um serviço que permite que organizações forneçam autenticação e gerenciamento de identidade para usuários externos, como clientes, parceiros ou fornecedores. O recurso de Identidades Externas no Azure AD B2C é usado para permitir que esses usuários externos acessem aplicativos e serviços da organização.

Com o Azure AD B2C, as organizações podem criar políticas de autenticação personalizadas para atender às necessidades específicas de seus usuários externos. Isso inclui a capacidade de oferecer opções de login social, como usar contas do Facebook, Google ou Microsoft, além de permitir o registro de novas contas diretamente no Azure AD B2C.

As Identidades Externas no Azure AD B2C são gerenciadas por meio de políticas de identidade, que definem como os usuários externos podem se autenticar e interagir com os aplicativos. Essas políticas podem ser configuradas para exigir autenticação multifator, verificação de e-mail ou número de telefone, entre outras opções de segurança.

Ao usar o Azure AD B2C, as organizações podem fornecer uma experiência de autenticação e gerenciamento de identidade consistente para seus usuários externos, independentemente do aplicativo ou serviço que estão acessando. Isso simplifica o processo de integração de usuários externos e ajuda a garantir a segurança e a privacidade dos dados compartilhados.

Em resumo, o recurso de Identidades Externas no Azure AD B2C permite que as organizações ofereçam autenticação e gerenciamento de identidade para usuários externos, facilitando o acesso seguro a aplicativos e serviços.

<figure><img src="../.gitbook/assets/image (8).png" alt="" width="375"><figcaption></figcaption></figure>



### Acesso Condicional

\-> IF/ELSE

Se a pessoa tem permissão para acessar

O Acesso Condicional é um recurso do Azure Active Directory (Azure AD) que permite controlar e restringir o acesso a recursos com base em condições específicas. Ele ajuda a proteger os dados e recursos da organização, garantindo que apenas usuários autorizados e dispositivos confiáveis tenham acesso.

Com o Acesso Condicional, é possível definir políticas de acesso que levam em consideração vários fatores, como localização geográfica, horário do dia, tipo de dispositivo, estado de segurança do dispositivo e muito mais. Essas políticas podem ser configuradas para permitir, negar ou solicitar autenticação adicional, dependendo das condições definidas.

Por exemplo, uma política de Acesso Condicional pode ser configurada para permitir que usuários acessem recursos apenas durante o horário comercial e de locais específicos. Ou pode ser configurada para exigir autenticação multifator quando um usuário tenta acessar recursos de um dispositivo não confiável.

O Acesso Condicional também pode ser integrado a outros serviços e recursos do Azure, como o Azure Information Protection, para aplicar políticas de proteção de dados com base em condições de acesso.

Ao usar o Acesso Condicional, as organizações podem fortalecer a segurança e reduzir o risco de acesso não autorizado aos recursos. Ele oferece uma camada adicional de proteção, garantindo que o acesso seja concedido somente quando as condições definidas forem atendidas, ajudando a proteger contra ameaças internas e externas.

Em resumo, o Acesso Condicional no Azure AD permite controlar e restringir o acesso a recursos com base em condições específicas, aumentando a segurança e proteção dos dados e recursos da organização.

<figure><img src="../.gitbook/assets/image (9).png" alt="" width="375"><figcaption></figcaption></figure>



### Controle de Acesso baseado em Função

* Divide as tarefas dentro da equipe e concede somente a quantidade de acesso de que os usuários precisam para trabalhar

O Controle de Acesso Baseado em Função (Role-Based Access Control - RBAC) é um modelo de controle de acesso que permite que as organizações gerenciem e concedam permissões de acesso a recursos com base nas funções e responsabilidades dos usuários dentro da organização.

No RBAC, as permissões são atribuídas a funções específicas, e os usuários são associados a essas funções. Cada função tem um conjunto de permissões predefinidas que determinam quais ações um usuário pode realizar em um recurso específico. Por exemplo, uma função de "Administrador" pode ter permissões para criar, modificar e excluir recursos, enquanto uma função de "Usuário" pode ter permissões apenas para visualizar e acessar recursos existentes.

O RBAC permite que as organizações definam suas próprias funções personalizadas com base nas necessidades específicas. Isso permite um controle granular sobre o acesso aos recursos, garantindo que os usuários tenham apenas as permissões necessárias para realizar suas tarefas.

Além disso, o RBAC no Azure AD permite que as organizações atribuam funções a usuários individuais ou a grupos de usuários. Isso simplifica o gerenciamento de permissões, pois as alterações podem ser feitas em nível de função, em vez de ter que modificar as permissões de cada usuário individualmente.

O RBAC é uma prática recomendada para garantir a segurança e a conformidade dos recursos e dados da organização. Ele ajuda a evitar o acesso não autorizado, minimiza o risco de erros humanos e facilita a auditoria e o monitoramento do acesso aos recursos.

Em resumo, o Controle de Acesso Baseado em Função (RBAC) é um modelo de controle de acesso que permite que as organizações gerenciem e concedam permissões de acesso a recursos com base nas funções e responsabilidades dos usuários, garantindo um acesso seguro e adequado aos recursos.



### Confiança Zero

A Confiança Zero (Zero Trust) é um modelo de segurança que se baseia na premissa de que não se deve confiar automaticamente em nenhum usuário, dispositivo ou rede, mesmo que estejam dentro da rede corporativa. Em vez disso, cada solicitação de acesso deve ser verificada e autenticada, independentemente da origem.

No modelo de Confiança Zero, todas as solicitações de acesso são tratadas como potencialmente não confiáveis e são submetidas a uma série de verificações e autenticações antes de serem autorizadas. Isso inclui a autenticação multifator, a verificação de identidade, a análise de risco, a inspeção de tráfego e outras medidas de segurança.

Em vez de confiar em uma rede interna como um perímetro de segurança, a Confiança Zero adota uma abordagem de "confiar, mas verificar". Isso significa que cada solicitação de acesso é avaliada com base em vários fatores, como a identidade do usuário, o dispositivo usado, a localização, o comportamento de acesso anterior e outros dados relevantes.

A Confiança Zero também promove a segmentação de rede e o princípio do "menor privilégio", onde os usuários têm acesso apenas aos recursos necessários para realizar suas tarefas, reduzindo assim a superfície de ataque.

Esse modelo de segurança é especialmente relevante em um ambiente em nuvem, onde os recursos estão distribuídos em várias redes e dispositivos. A Confiança Zero ajuda a proteger os dados e recursos, independentemente de sua localização, e fornece uma camada adicional de segurança contra ameaças internas e externas.

Em resumo, a Confiança Zero é um modelo de segurança que não confia automaticamente em usuários, dispositivos ou redes, exigindo autenticação e verificação rigorosas para cada solicitação de acesso. Isso ajuda a proteger os recursos e dados contra ameaças, mesmo em um ambiente distribuído e em nuvem.

* "Não confiar em nada"
* Se houver alguma modificação, é preciso outra validação



### Proteção Completa

* abordagem por camadas

<figure><img src="../.gitbook/assets/image (10).png" alt="" width="340"><figcaption></figcaption></figure>

* Perímetro -> Local
* Ataques contra uma camada são isolados das camadas subsequentes

A "Proteção Completa" é um conceito amplo que se refere a uma abordagem abrangente para garantir a segurança e proteção de dados, sistemas e recursos de uma organização. Envolve a implementação de várias camadas de segurança e medidas de proteção para mitigar riscos e minimizar a exposição a ameaças.

A proteção completa abrange diferentes aspectos da segurança, incluindo:

1. Segurança da rede: Implementação de firewalls, detecção e prevenção de intrusões, segmentação de rede e monitoramento de tráfego para proteger a infraestrutura de rede contra ataques e acessos não autorizados.
2. Segurança de dados: Utilização de criptografia para proteger dados em repouso e em trânsito, implementação de políticas de controle de acesso para garantir que apenas usuários autorizados tenham acesso aos dados e implementação de backups e recuperação de desastres para proteger contra perda de dados.
3. Segurança de aplicativos: Implementação de práticas de desenvolvimento seguro, como testes de segurança, correção de vulnerabilidades e monitoramento contínuo de aplicativos para proteger contra ataques de aplicativos e exploração de vulnerabilidades.
4. Segurança de identidade e acesso: Utilização de autenticação multifator, gerenciamento de identidade e acesso baseado em função (RBAC) para garantir que apenas usuários autorizados tenham acesso a recursos e dados.
5. Conscientização e treinamento: Educação dos usuários sobre práticas de segurança, como evitar phishing, uso seguro de senhas e proteção de informações confidenciais.
6. Monitoramento e resposta a incidentes: Implementação de sistemas de monitoramento de segurança em tempo real, detecção de ameaças e resposta a incidentes para identificar e responder rapidamente a atividades suspeitas ou ataques em andamento.

A proteção completa requer uma abordagem em camadas, combinando tecnologias, processos e conscientização para garantir a segurança abrangente de uma organização. É um esforço contínuo que deve ser adaptado e atualizado à medida que as ameaças evoluem e novas vulnerabilidades são descobertas.



### Microsoft Defender para Nuvem

O Microsoft Defender para Nuvem é uma solução de segurança abrangente projetada para proteger ambientes em nuvem, como o Microsoft Azure e o Microsoft 365 (anteriormente conhecido como Office 365). Ele oferece recursos avançados de detecção, prevenção e resposta a ameaças para ajudar a proteger os dados e recursos nessas plataformas.

O Microsoft Defender para Nuvem combina várias soluções de segurança em uma única plataforma unificada, fornecendo proteção em tempo real contra ameaças cibernéticas. Alguns dos recursos e funcionalidades incluídos são:

1. Proteção contra ameaças avançadas: O Microsoft Defender para Nuvem utiliza inteligência artificial e aprendizado de máquina para detectar e bloquear ameaças avançadas, como malware, ransomware e ataques de phishing.
2. Detecção de comportamento suspeito: Ele monitora continuamente as atividades do usuário e do sistema em busca de comportamentos suspeitos, identificando atividades maliciosas e tomando medidas para mitigar os riscos.
3. Gerenciamento de vulnerabilidades: A solução ajuda a identificar e corrigir vulnerabilidades em tempo hábil, garantindo que os sistemas estejam protegidos contra explorações conhecidas.
4. Proteção de identidade e acesso: O Microsoft Defender para Nuvem inclui recursos de autenticação multifator e monitoramento de identidade para proteger contra acesso não autorizado e roubo de credenciais.
5. Análise de segurança avançada: Ele fornece insights detalhados sobre ameaças e atividades maliciosas por meio de painéis de controle e relatórios, permitindo que as equipes de segurança monitorem e respondam a incidentes de forma eficaz.
6. Integração com outras soluções de segurança: O Microsoft Defender para Nuvem pode ser integrado a outras soluções de segurança da Microsoft, como o Microsoft Defender para Endpoint e o Microsoft Cloud App Security, para fornecer uma proteção abrangente em todo o ambiente de nuvem.

Em resumo, o Microsoft Defender para Nuvem é uma solução de segurança abrangente projetada para proteger ambientes em nuvem, oferecendo recursos avançados de detecção, prevenção e resposta a ameaças. Ele ajuda a proteger os dados e recursos em plataformas como o Azure e o Microsoft 365, garantindo uma segurança robusta e em tempo real.

* serviço de monitoramento que fornece proteção contra ameaças nos datacenters do Azure e locais (responsabilidade Azure)
* recomendações de segurança
* detectar e bloquear malware
* possui logs e gráficos

