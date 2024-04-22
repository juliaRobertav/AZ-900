# Armazenamento

### Contas de Armazenamento

As Contas de Armazenamento do Azure são um serviço fundamental para armazenar e acessar dados na nuvem. Elas fornecem uma solução escalável, durável e segura para armazenar uma variedade de tipos de dados, como arquivos, blobs, tabelas e filas. Aqui estão alguns pontos-chave sobre as Contas de Armazenamento do Azure:

1. Tipos de Contas de Armazenamento: Existem quatro tipos de contas de armazenamento no Azure: Contas de Armazenamento de Uso Geral v2 (GPv2), Contas de Armazenamento de Uso Geral v1 (GPv1), Contas de Armazenamento de Blobs e Contas de Armazenamento de Arquivos. Cada tipo é otimizado para diferentes cenários de armazenamento.
2. Durabilidade e Redundância: As Contas de Armazenamento do Azure oferecem alta durabilidade e redundância para proteger seus dados. Elas replicam automaticamente os dados em várias cópias dentro de uma região do Azure e também podem ser configuradas para replicação geográfica para maior resiliência.
3. Escalabilidade: As Contas de Armazenamento do Azure são altamente escaláveis, permitindo que você aumente ou diminua a capacidade de armazenamento conforme necessário. Elas podem lidar com grandes volumes de dados e suportam cargas de trabalho intensivas em leitura e gravação.
4. Acesso aos dados: As Contas de Armazenamento do Azure fornecem várias opções de acesso aos dados, incluindo APIs RESTful, SDKs, ferramentas de linha de comando e interfaces de usuário baseadas na web. Isso permite que você acesse e gerencie seus dados de forma flexível e conveniente.
5. Segurança: As Contas de Armazenamento do Azure oferecem recursos de segurança robustos, como criptografia de dados em repouso e em trânsito, controle de acesso baseado em função (RBAC), autenticação multifator e integração com serviços de segurança do Azure, como Azure Active Directory e Azure Private Link.
6. Integração com outros serviços: As Contas de Armazenamento do Azure podem ser facilmente integradas a outros serviços do Azure, como Máquinas Virtuais, Serviços de Aplicativo, Azure Functions e muito mais. Isso permite que você crie soluções completas e escaláveis que atendam às suas necessidades de armazenamento e processamento de dados.

Em resumo, as Contas de Armazenamento do Azure são uma solução versátil e confiável para armazenar e acessar dados na nuvem. Elas oferecem escalabilidade, durabilidade, segurança e integração com outros serviços do Azure, permitindo que você crie soluções de armazenamento flexíveis e eficientes.



### Redundância de Armazenamento

A redundância de armazenamento é um conceito importante para garantir a disponibilidade e a durabilidade dos dados armazenados na nuvem. No Azure, existem várias opções de redundância de armazenamento disponíveis:

1. Redundância Local: Com a redundância local, os dados são replicados de forma síncrona em várias unidades de armazenamento dentro de um data center específico. Isso oferece alta disponibilidade dos dados, mas não protege contra falhas de data center.
2. Redundância de Armazenamento Zonal: A redundância de armazenamento zonal replica os dados de forma síncrona em várias zonas de disponibilidade dentro de uma região do Azure. Isso garante a disponibilidade dos dados mesmo em caso de falha em uma zona específica.
3. Redundância Geográfica: A redundância geográfica replica os dados de forma assíncrona em uma região secundária, geralmente em uma localização geograficamente distante. Isso oferece proteção adicional contra falhas de região inteira, permitindo a recuperação de desastres.
4. Redundância de Armazenamento em Nível de Conta: A redundância de armazenamento em nível de conta é uma opção disponível para contas de armazenamento de uso geral v2 (GPv2). Ela replica automaticamente os dados em várias unidades de armazenamento dentro de uma região do Azure, garantindo alta disponibilidade e durabilidade.

É importante considerar os requisitos de disponibilidade, durabilidade e custo ao escolher a opção de redundância de armazenamento adequada para seus dados. O Azure oferece flexibilidade para selecionar a opção mais adequada com base nas necessidades específicas do seu aplicativo ou serviço.

<figure><img src="../.gitbook/assets/image (1) (1).png" alt="" width="563"><figcaption></figcaption></figure>



### Serviços de Armazenamento

O Azure oferece uma variedade de serviços de armazenamento para atender às diferentes necessidades de armazenamento de dados na nuvem. Aqui estão alguns dos principais serviços de armazenamento do Azure:

1. Azure Blob Storage: O Azure Blob Storage é um serviço de armazenamento de objetos escalável e durável, projetado para armazenar grandes quantidades de dados não estruturados, como imagens, vídeos, arquivos de backup e logs. Ele oferece opções de acesso público ou privado aos dados armazenados.
2. Azure File Storage: O Azure File Storage é um serviço de armazenamento de arquivos totalmente gerenciado, que permite compartilhar arquivos entre várias máquinas virtuais e serviços na nuvem. Ele oferece suporte ao protocolo SMB (Server Message Block) e pode ser acessado como um compartilhamento de rede tradicional.
3. Azure Queue Storage: O Azure Queue Storage é um serviço de armazenamento de mensagens que permite a comunicação assíncrona entre componentes de aplicativos distribuídos. Ele é útil para a criação de filas de mensagens para processamento em segundo plano, balanceamento de carga e comunicação entre aplicativos.
4. Azure Table Storage: O Azure Table Storage é um serviço de armazenamento de dados NoSQL, que permite armazenar grandes quantidades de dados estruturados de forma escalável. Ele é adequado para aplicativos que exigem acesso rápido a dados não relacionais, como dados de sensores, logs e perfis de usuário.
5. Azure Disk Storage: O Azure Disk Storage fornece discos virtuais persistentes para uso com máquinas virtuais do Azure. Ele oferece opções de discos gerenciados e não gerenciados, permitindo armazenar e acessar dados como se fossem discos rígidos físicos.
6. Azure Data Lake Storage: O Azure Data Lake Storage é um serviço de armazenamento otimizado para big data, projetado para armazenar, processar e analisar grandes volumes de dados estruturados e não estruturados. Ele oferece integração com ferramentas de análise de big data, como Azure Databricks e Azure HDInsight.

Esses são apenas alguns dos serviços de armazenamento do Azure disponíveis. Cada serviço tem suas próprias características e casos de uso específicos, permitindo que você escolha a opção mais adequada para suas necessidades de armazenamento de dados na nuvem.

<figure><img src="../.gitbook/assets/image (17).png" alt="" width="563"><figcaption></figcaption></figure>

### Pontos de Extremidade

Os serviços de armazenamento do Azure possuem pontos de extremidade públicos que permitem o acesso aos dados armazenados por meio da Internet. Aqui estão alguns pontos de extremidade públicos comuns para os serviços de armazenamento do Azure:

1. Blob Storage: O ponto de extremidade público para o Azure Blob Storage segue o formato `https://<nome_da_conta>.blob.core.windows.net`. Por exemplo, se sua conta de armazenamento for "meuarmazenamento", o ponto de extremidade será `https://meuarmazenamento.blob.core.windows.net`.
2. File Storage: O ponto de extremidade público para o Azure File Storage segue o formato `https://<nome_da_conta>.file.core.windows.net`. Usando o mesmo exemplo anterior, o ponto de extremidade seria `https://meuarmazenamento.file.core.windows.net`.
3. Queue Storage: O ponto de extremidade público para o Azure Queue Storage segue o formato `https://<nome_da_conta>.queue.core.windows.net`. No exemplo anterior, o ponto de extremidade seria `https://meuarmazenamento.queue.core.windows.net`.
4. Table Storage: O ponto de extremidade público para o Azure Table Storage segue o formato `https://<nome_da_conta>.table.core.windows.net`. Usando o exemplo anterior, o ponto de extremidade seria `https://meuarmazenamento.table.core.windows.net`.

É importante lembrar que esses pontos de extremidade públicos são acessíveis pela Internet e, portanto, devem ser protegidos adequadamente com medidas de segurança, como autenticação e controle de acesso. Além disso, você pode configurar regras de firewall e acesso virtual para restringir o acesso aos pontos de extremidade públicos apenas a IPs específicos ou redes virtuais do Azure.

<figure><img src="../.gitbook/assets/image (18).png" alt="" width="563"><figcaption></figcaption></figure>



### Camadas de Acesso de Armazenamento

O Azure Storage oferece diferentes camadas de acesso para atender às necessidades de desempenho e custo dos aplicativos. Aqui estão as principais camadas de acesso de armazenamento do Azure:

1. Hot Access Tier: A camada Hot é otimizada para acesso frequente e rápido aos dados. É ideal para dados que são acessados com frequência e exigem baixa latência. Os dados na camada Hot têm um custo de armazenamento mais alto, mas as taxas de acesso são mais baixas.
2. Cool Access Tier: A camada Cool é projetada para dados que são acessados com menos frequência, mas ainda exigem acesso rápido quando necessário. É mais econômica em termos de custo de armazenamento, mas as taxas de acesso são um pouco mais altas em comparação com a camada Hot.
3. Archive Access Tier: A camada Archive é destinada a dados que são acessados com pouca frequência e podem tolerar tempos de recuperação mais longos. É a camada mais econômica em termos de custo de armazenamento, mas as taxas de acesso são significativamente mais altas e o tempo de recuperação pode levar horas.

A escolha da camada de acesso depende dos requisitos de desempenho e custo do seu aplicativo. Você pode definir a camada de acesso durante a criação ou a modificação de um contêiner de blob ou uma conta de armazenamento.

É importante notar que a camada de acesso pode ser definida em nível de objeto para o Azure Blob Storage, permitindo que você escolha a camada apropriada para cada objeto individualmente, com base em seus padrões de acesso.

<figure><img src="../.gitbook/assets/image (19).png" alt="" width="563"><figcaption></figcaption></figure>



### Migrações para Azure

A migração para o Azure envolve a transferência de aplicativos, dados e infraestrutura existentes para a plataforma de nuvem da Microsoft. Aqui estão algumas opções comuns para migrações para o Azure:

1. Lift and Shift: Essa abordagem envolve mover aplicativos e infraestrutura existentes para o Azure sem fazer alterações significativas no código ou na arquitetura. Isso pode ser feito usando máquinas virtuais do Azure para replicar a infraestrutura local no ambiente de nuvem.
2. Replatforming: Nessa abordagem, os aplicativos são otimizados para aproveitar os serviços gerenciados do Azure. Isso pode envolver a reescrita de partes do código para aproveitar os recursos nativos do Azure, como bancos de dados gerenciados, serviços de análise de dados ou serviços de inteligência artificial.
3. Refactoring: Essa abordagem envolve a reescrita significativa do aplicativo para aproveitar ao máximo os recursos nativos da nuvem. Isso pode incluir a adoção de arquiteturas de microsserviços, o uso de contêineres e a implementação de práticas de DevOps.
4. Rebuilding: Nessa abordagem, o aplicativo é reconstruído do zero usando serviços nativos da nuvem do Azure. Isso pode ser apropriado para aplicativos legados que precisam ser modernizados ou para criar aplicativos totalmente novos.

Além disso, o Azure oferece ferramentas e serviços para facilitar a migração, como o Azure Migrate, que ajuda a avaliar a infraestrutura existente e planejar a migração, e o Azure Site Recovery, que permite a replicação e recuperação de desastres de máquinas virtuais.

É importante planejar cuidadosamente a migração, considerando fatores como segurança, desempenho, custo e compatibilidade com os serviços do Azure. É recomendável buscar orientação especializada ou trabalhar com um parceiro certificado do Azure para garantir uma migração bem-sucedida.



### Azure Data Box

\-> Facilita a migração dos dados

Azure Data Box é um serviço oferecido pela Microsoft Azure que permite a transferência rápida e segura de grandes volumes de dados para a nuvem. Ele é especialmente útil quando a transferência de dados pela internet é lenta ou impraticável devido ao tamanho dos dados ou à largura de banda limitada.

O Azure Data Box é um dispositivo físico robusto e seguro que pode ser enviado para o local do cliente. Ele possui capacidade de armazenamento de até 80 TB (terabytes) e é equipado com recursos de criptografia para garantir a segurança dos dados durante o transporte.

O processo de uso do Azure Data Box é relativamente simples. Primeiro, o cliente solicita o dispositivo Data Box por meio do portal do Azure. Em seguida, os dados são copiados para o dispositivo usando ferramentas de transferência de dados, como o robocopy ou o AzCopy. Depois que os dados são transferidos para o Data Box, ele é enviado de volta para a Microsoft, onde os dados são carregados na conta do Azure do cliente.

O Azure Data Box é uma solução eficiente para migração de dados em larga escala, backup e recuperação de desastres, transferência de dados offline e outras situações em que a transferência pela internet não é viável. Ele acelera o processo de transferência de dados para a nuvem, economizando tempo e recursos para as organizações.

<figure><img src="../.gitbook/assets/image (1).png" alt="" width="375"><figcaption></figcaption></figure>



### Opções de Gerenciamento de Arquivos

<figure><img src="../.gitbook/assets/image (2).png" alt="" width="563"><figcaption></figcaption></figure>

Existem várias opções de gerenciamento de arquivos disponíveis no Azure, cada uma adequada para diferentes necessidades e casos de uso. Aqui estão algumas das principais opções:

1. Azure Blob Storage: O Azure Blob Storage é um serviço de armazenamento de objetos escalável e econômico. Ele é ideal para armazenar e gerenciar grandes volumes de dados não estruturados, como imagens, vídeos, arquivos de log e backups. Os blobs podem ser acessados por meio de URLs únicos e têm suporte para acesso quente, frio e de arquivo.
2. Azure Files: O Azure Files é um serviço de armazenamento de arquivos totalmente gerenciado que permite compartilhar arquivos entre várias máquinas virtuais e serviços do Azure. Ele oferece suporte ao protocolo SMB (Server Message Block) e pode ser montado como uma unidade de rede em sistemas operacionais Windows, Linux e macOS.
3. Azure Data Lake Storage: O Azure Data Lake Storage é um serviço de armazenamento escalável e seguro projetado para análise de big data. Ele permite armazenar e analisar grandes volumes de dados não estruturados, semiestruturados e estruturados. O Data Lake Storage é integrado ao ecossistema do Azure, incluindo serviços de análise, como o Azure Databricks e o Azure Data Factory.
4. Azure Disk Storage: O Azure Disk Storage oferece armazenamento persistente e de alto desempenho para máquinas virtuais do Azure. Ele fornece discos virtuais que podem ser anexados a máquinas virtuais para armazenar dados de aplicativos e sistemas operacionais. Os discos podem ser HDD (Hard Disk Drive) ou SSD (Solid State Drive) e têm suporte para diferentes níveis de desempenho.
5. Azure Backup: O Azure Backup é um serviço de backup e recuperação de desastres baseado em nuvem. Ele permite fazer backup de máquinas virtuais, servidores físicos, bancos de dados e outros recursos do Azure. O Azure Backup oferece recursos de recuperação granular e recuperação de desastres para proteger os dados contra perda ou corrupção.

Essas são apenas algumas das opções de gerenciamento de arquivos disponíveis no Azure. Cada serviço tem suas próprias características e benefícios, e a escolha depende dos requisitos específicos do seu aplicativo ou caso de uso.

