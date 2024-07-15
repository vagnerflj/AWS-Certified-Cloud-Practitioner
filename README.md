## Resumo - IAM
O **AWS Identity and Access Management (IAM)** é um serviço da AWS que ajuda a controlar quem está autenticado (assinado) e autorizado (tem permissões) para usar os recursos da AWS.

Aqui estão os principais pontos sobre o IAM:



**Controle Granular de Acesso a AWS:** Com o IAM, você pode criar usuários, grupos, papéis e políticas de permissão para controlar o acesso aos serviços e recursos da AWS de uma maneira granular. Por exemplo, você pode permitir que um usuário tenha acesso somente leitura ao Amazon S3 e acesso total ao EC2.

**Compartilhamento Seguro de Acesso:** O IAM permite compartilhar o acesso à sua conta AWS de maneira segura. Em vez de compartilhar suas credenciais de root, você pode criar vários usuários IAM, cada um com suas próprias credenciais e permissões.

**Identidade Federada:** Com o IAM, você também pode permitir usuários que já tenham senhas em outros lugares, como na sua rede corporativa ou em um provedor de identidade baseado em SAML, a obter acesso temporário à sua conta AWS.

**Compatível com Multi-Fator Authentication (MFA):** O IAM é compatível com a autenticação de vários fatores para fornecer uma camada adicional de proteção de segurança ao gerenciar o acesso aos serviços e recursos da AWS.

**Integrado com AWS Services:** O IAM está integrado com todos os serviços da AWS, o que significa que você pode definir permissões para qualquer serviço que desejar.

**Auditoria com AWS CloudTrail:** Com o AWS CloudTrail, você pode registrar todas as ações de usuários e APIs IAM para fins de auditoria.

**Gratuito:** O IAM é um recurso gratuito da AWS; você só paga pelos outros recursos da AWS que seus usuários acessam.

Em suma, o AWS IAM é um serviço de segurança crítico que ajuda a proteger o acesso aos recursos da AWS, permitindo que você controle quem pode fazer o quê em sua conta AWS.

## Resumo - MFA
**A Autenticação Multifator (MFA)** é um método de controle de acesso que exige que um usuário verifique sua identidade usando duas ou mais evidências (fatores) antes que o acesso seja concedido. Estes fatores podem ser algo que o usuário sabe (como uma senha), algo que o usuário tem (como um telefone celular ou um token de hardware) e algo que o usuário é (como uma impressão digital ou reconhecimento facial).

Aqui estão alguns pontos-chave sobre MFA:



**Segurança Aprimorada:** O principal benefício da MFA é que ela aumenta significativamente a segurança, tornando muito mais difícil para os invasores ganharem acesso não autorizado a um sistema. Mesmo que um fator de autenticação seja comprometido (por exemplo, se uma senha for roubada), os outros fatores ainda protegem o sistema.

**Diversos Métodos de Autenticação:** A MFA pode usar uma variedade de métodos de autenticação, como códigos de verificação por SMS, aplicativos de autenticação, tokens de hardware, impressões digitais, reconhecimento facial e muito mais.

**Compatibilidade:** A MFA é compatível com muitos sistemas e serviços, incluindo a maioria das plataformas de nuvem (como AWS, Google Cloud e Azure), serviços de email, redes sociais, plataformas de pagamento online, entre outros.

**AWS MFA:** A AWS suporta MFA e recomenda que os usuários a utilizem para proteger suas contas. Com a MFA ativada, quando um usuário se conecta à AWS, ele é solicitado a inserir seu nome de usuário e senha (primeiro fator) e um código de autenticação de um dispositivo MFA (segundo fator).

Resumindo, a Autenticação Multifator é uma medida de segurança essencial que protege os sistemas de acesso não autorizado, exigindo que os usuários verifiquem sua identidade com vários fatores de autenticação.


## Resumo - Organizações
O AWS Organizations é um serviço da AWS que permite a você centralizar e gerenciar de forma unificada várias contas AWS. Com o AWS Organizations, você pode criar uma organização para administrar suas contas da AWS a partir de um único local.

Aqui estão algumas características principais do AWS Organizations:



**Gerenciamento Centralizado de Contas:** O AWS Organizations permite agrupar e gerenciar todas as suas contas AWS de um único local centralizado. Isso facilita o gerenciamento de contas e recursos em uma organização.

**Controle de Acesso Hierárquico:** Com o AWS Organizations, você pode criar uma estrutura hierárquica de Unidades Organizacionais (OUs) para agrupar suas contas. Isso ajuda a organizar suas contas em uma estrutura que melhor se alinhe com o uso dos recursos em sua organização.

**Políticas de Controle de Serviço:** O AWS Organizations oferece políticas de controle de serviço (SCPs) que permitem que você controle as permissões para as contas em sua organização. Isso permite que você aplique regras de acesso uniformes em todas as suas contas.

**Consolidação de Cobrança:** O AWS Organizations também oferece a capacidade de consolidar sua cobrança em todas as suas contas AWS, o que pode simplificar a gestão de custos e permitir um melhor rastreamento e controle dos gastos da AWS.

**Automação:** Com o AWS Organizations, você pode automatizar a criação e o gerenciamento de contas por meio de APIs e integrações com outras ferramentas da AWS, como o AWS CloudFormation.

Em suma, o AWS Organizations é uma ferramenta poderosa para empresas e equipes que gerenciam várias contas da AWS, permitindo o gerenciamento centralizado de contas, a aplicação de políticas em todas as contas, a consolidação de cobranças e a automação de tarefas de gerenciamento de contas.

## Resumo - Infra Global
A infraestrutura global da AWS é a base sobre a qual os serviços da AWS são construídos. Ela consiste em uma série de Regiões e Zonas de Disponibilidade espalhadas pelo mundo, projetadas para fornecer um serviço seguro, confiável e escalável.

Regiões: Uma região da AWS é uma área geográfica que contém pelo menos duas Zonas de Disponibilidade. Cada região é completamente independente das outras regiões, o que ajuda a isolar falhas e evitar a propagação de problemas de uma região para outra. Em setembro de 2021, a AWS tinha 25 regiões geográficas ao redor do mundo.

**Zonas de Disponibilidade (AZs):** Cada região da AWS é dividida em Zonas de Disponibilidade. Cada AZ é um centro de dados separado dentro de uma região, mas todas as AZs dentro de uma região estão conectadas através de redes de alta velocidade, de baixa latência e totalmente redundantes. As AZs fornecem uma maneira de construir aplicativos altamente disponíveis e tolerantes a falhas.

**Zonas Locais:** As zonas locais da AWS aproximam a computação, o armazenamento, o banco de dados e outros produtos da AWS selecionados dos usuários finais. Com as zonas locais da AWS, você pode executar facilmente aplicativos altamente exigentes que exigem latências em milissegundos de um dígito para seus usuários finais, como criação de conteúdo de mídia e entretenimento, jogos em tempo real, simulações de reservatórios, automação de projetos eletrônicos e machine learning.

**Wavelenght:** O AWS Wavelength permite que os desenvolvedores criem aplicações com latências de um dígito para dispositivos móveis e usuários finais. Os desenvolvedores da AWS podem implantar seus aplicativos nas Zonas do Wavelength, implantações de infraestrutura da AWS que incorporam serviços de computação e armazenamento da AWS aos datacenters dos provedores de telecomunicações na borda das redes 5G e acessam facilmente a variedade de serviços da AWS na região. Isso permite que os desenvolvedores forneçam aplicativos que exigem latências inferiores a 10 milissegundos, como streaming de jogos e vídeos ao vivo, inferência de machine learning na borda e realidade aumentada e virtual (AR/VR).

**OutPosts:** O AWS Outposts leva produtos, infraestrutura e modelos operacionais nativos da AWS a praticamente qualquer datacenter, espaço de colocalização ou instalações on-premises. Você pode usar as mesmas APIs, ferramentas e infraestrutura da AWS no local e na Nuvem AWS para oferecer uma experiência híbrida verdadeiramente consistente. O AWS Outposts foi projetado para ambientes conectados e pode ser usado para oferecer suporte a workloads que precisam permanecer on-premises devido à baixa latência ou às necessidades de processamento de dados locais.

A infraestrutura global da AWS permite que os usuários implantem seus aplicativos e serviços de maneira flexível, resiliente e eficiente em termos de latência, onde quer que seus clientes estejam localizados no mundo. Isso significa que, como usuário da AWS, você pode oferecer uma experiência de usuário mais rápida e melhor para seus clientes, independentemente de sua localização geográfica.

## Resumo - Share Model
O Modelo de Responsabilidade Compartilhada da AWS é uma estrutura de governança que delineia a divisão de responsabilidades de segurança entre a Amazon Web Services (AWS) e o usuário (cliente). Essa divisão de responsabilidades permite que a AWS se concentre na segurança da infraestrutura de computação em nuvem, enquanto o usuário se concentra na segurança dos dados e recursos que colocam na nuvem.

Aqui está uma visão geral das responsabilidades compartilhadas:



**Segurança "da" nuvem:** A AWS é responsável pela proteção da infraestrutura que executa todos os serviços oferecidos na AWS Cloud. Isso inclui hardware, software, redes e instalações que sustentam os serviços AWS Cloud.

**Segurança "na" nuvem:** O cliente é responsável pela segurança de qualquer coisa que coloque "na" nuvem ou conecte "à" nuvem. Isso pode incluir a configuração correta de controles de segurança e conformidade em serviços da AWS, gerenciamento de dados (incluindo criptografia e backups), classificação de ativos e outras várias tarefas de segurança de TI.

Serviços de Infraestrutura, Contêiner e Abstração: Dependendo do tipo de serviço da AWS que está sendo usado (por exemplo, uma instância EC2 versus um banco de dados RDS), a AWS e o cliente compartilharão diferentes partes da responsabilidade de segurança. Por exemplo, para um serviço de infraestrutura como o EC2, a AWS fornece a segurança física, a do hypervisor e a da rede, enquanto o cliente é responsável pelo sistema operacional e pelas aplicações. Para um serviço de contêiner como o RDS, a AWS também é responsável pela segurança do sistema operacional e do serviço de banco de dados, enquanto o cliente ainda é responsável pelas aplicações e dados.

A compreensão e a aplicação adequada do Modelo de Responsabilidade Compartilhada da AWS são fundamentais para garantir a segurança e a conformidade ao usar a AWS. Isso requer que os clientes estejam cientes de suas responsabilidades de segurança e implementem práticas de segurança robustas ao usar serviços da AWS.


## Resumo - EC2
O Amazon Elastic Compute Cloud (EC2) é um componente central da plataforma de computação em nuvem da Amazon. O EC2 permite aos usuários alugar máquinas virtuais usando a infraestrutura da Amazon. Ele foi projetado para tornar a computação em escala na web mais acessível para os desenvolvedores.

Aqui estão alguns pontos-chave sobre o Amazon EC2:



**Máquinas Virtuais:** EC2 fornece instâncias, que são máquinas virtuais executando os sistemas operacionais que você escolher.

**Escalabilidade:** Você pode dimensionar a capacidade de computação facilmente, criando e lançando novas instâncias conforme necessário, o que é útil para lidar com picos de demanda e escala.

**Controle Completo:** Os usuários têm controle total sobre as instâncias do EC2. Eles têm acesso de root, e podem interagir com elas como fariam com qualquer máquina.

**Várias Regiões e Zonas de Disponibilidade:** As instâncias do EC2 podem ser implantadas em várias regiões geográficas e zonas de disponibilidade. Isso ajuda a reduzir latência, aumentar a tolerância a falhas e cumprir os requisitos de residência de dados.

**Modelos de Instância:** O EC2 fornece uma variedade de tipos de instâncias otimizadas para diferentes casos de uso, garantindo que você tenha os recursos de que precisa para o aplicativo que está executando.

**Preços Flexíveis:** O EC2 oferece várias opções de preços, incluindo On-Demand (pague pelo que usar), Reservado (reserve uma instância por um período e obtenha um desconto) e Spot (licitação por capacidade não utilizada a preços mais baixos).

**Armazenamento Integrado:** As instâncias do EC2 podem ser integradas com outros serviços da AWS para fornecer armazenamento (por exemplo, Amazon EBS), bancos de dados (por exemplo, Amazon RDS), e redes (por exemplo, Amazon VPC).

**Segurança:** O EC2 trabalha com o Amazon VPC para fornecer segurança e robustez por meio de grupos de segurança e redes isoladas.

Em resumo, o Amazon EC2 é um serviço poderoso e flexível que forma a espinha dorsal da computação na plataforma AWS, permitindo que as empresas executem e dimensionem aplicativos na nuvem de forma eficiente e segura.


## Resumo - Tipos de EC2
O Amazon EC2 oferece uma variedade de tipos de instâncias otimizados para atender diferentes casos de uso. Os tipos de instâncias compreendem combinações variadas de capacidade de CPU, memória, armazenamento e rede e proporcionam a flexibilidade para escolher a combinação apropriada de recursos para seus aplicativos. Os principais tipos de instâncias do Amazon EC2 incluem:



**Instâncias de Uso Geral (A, T, M):** Essas instâncias proporcionam um bom equilíbrio de computação, memória e rede e são uma boa escolha para muitas cargas de trabalho que não requerem especificações de hardware específicas.

**Instâncias Otimizadas para Computação (C):** Essas instâncias são otimizadas para cargas de trabalho que exigem alta performance de CPU, como computação científica, modelagem e análise financeira, e renderização de mídia.

**Instâncias Otimizadas para Memória (R, X, Z):** Essas instâncias são projetadas para cargas de trabalho que processam grandes conjuntos de dados na memória, como bancos de dados em memória, caches distribuídos, análise em memória e aplicações de big data.

**Instâncias Otimizadas para Armazenamento (D, I, H):** Essas instâncias são projetadas para cargas de trabalho que requerem alto desempenho de armazenamento local, como bancos de dados escalonáveis, processamento de dados em escala de petabytes e aplicações de data warehousing.

**Instâncias Otimizadas para GPU (P, G, F, Inf):** Essas instâncias são projetadas para cargas de trabalho de computação gráfica, como aprendizado de máquina, mineração de criptomoedas, renderização 3D, e aplicações de streaming de jogos.

**Instâncias Arm (A1, M6g, C6g, R6g):** Essas instâncias são baseadas na arquitetura Arm e são uma opção de baixo custo para cargas de trabalho que requerem um bom desempenho de CPU e suportam a arquitetura Arm.

Os tipos de instâncias do Amazon EC2 são constantemente atualizados e ampliados para suportar uma gama cada vez maior de casos de uso. É importante verificar a documentação mais recente da AWS para obter as informações mais atualizadas.


## Resumo - Security Groups
Os Security Groups atuam como um firewall virtual para as suas instâncias Amazon EC2 para controlar o tráfego de entrada e saída. Eles operam ao nível da instância, o que significa que você pode associar diferentes security groups a diferentes instâncias, o que é útil para configurar a segurança a um nível granular.

Aqui estão algumas características principais dos Security Groups na AWS:



**Regras de entrada e saída:** Cada security group consiste em um conjunto de regras de entrada e saída. As regras de entrada controlam o tráfego que é permitido chegar à instância associada ao security group, enquanto as regras de saída controlam o tráfego permitido para sair da instância.

**Estado de conexão:** Os security groups são "stateful", o que significa que se você enviar uma solicitação de uma instância, a resposta é permitida automaticamente, independentemente das regras de saída.

**Permissões por protocolo:** As regras em um security group permitem especificar protocolos permitidos, portas e origem (para tráfego de entrada) ou destino (para tráfego de saída). Isso permite que você restrinja o tráfego para um protocolo ou porta específicos e controle de onde o tráfego é originado ou para onde ele é direcionado.

**Flexibilidade e controle:** Você pode associar diferentes security groups a diferentes instâncias e também pode modificar as regras de um security group a qualquer momento. As novas regras são aplicadas automaticamente a todas as instâncias associadas ao security group.

**Isolamento de instâncias:** Os security groups ajudam a isolar suas instâncias de outras instâncias na mesma rede, uma vez que as regras são aplicadas por instância e não por sub-rede.

Em resumo, os Security Groups são uma ferramenta crucial para gerenciar a segurança na AWS, permitindo que você controle e restrinja o tráfego de entrada e saída para suas instâncias do EC2 de uma maneira muito granular e específica.


## Resumo - EBS
O Amazon Elastic Block Store (EBS) é um serviço de armazenamento de alto desempenho oferecido pela AWS para uso com Amazon Elastic Compute Cloud (EC2). Ele foi projetado para aplicativos que exigem armazenamento de baixa latência para ler e escrever dados em blocos.

Aqui estão algumas características principais do EBS:



**Desempenho de Armazenamento:** EBS fornece armazenamento em bloco de alto desempenho que pode ser anexado a uma instância EC2. Os volumes EBS são otimizados para cargas de trabalho que exigem operações de E/S de baixa latência, como bancos de dados e aplicativos que exigem muita E/S.

**Durabilidade:** O EBS é projetado para durabilidade. Os volumes EBS são automaticamente replicados em sua zona de disponibilidade para proteger contra falhas de componentes, proporcionando alta disponibilidade e durabilidade.

**Tipos de Volume:** EBS oferece vários tipos de volume para atender às necessidades de armazenamento e desempenho. Isso inclui os volumes SSD-backed para cargas de trabalho transacionais de uso geral (gp2 e gp3) e de alto desempenho (io1 e io2), e os volumes HDD-backed para cargas de trabalho throughput intensivas (st1 e sc1).

**Backup com Snapshots:** O EBS oferece a capacidade de criar snapshots (cópias) dos seus volumes, que são armazenados no Amazon S3 para durabilidade. Esses snapshots podem ser usados para criar novos volumes EBS ou para aumentar o tamanho do volume.

**Criptografia:** O EBS oferece a opção de criar volumes criptografados e controlar as chaves de criptografia usando o AWS Key Management Service (KMS). Isso ajuda a atender aos requisitos de conformidade e segurança.

**Integração com a AWS:** EBS é profundamente integrado com outros serviços da AWS, como Amazon CloudWatch para monitoramento, AWS Identity and Access Management (IAM) para controle de acesso, e AWS Snapshot Scheduler para automação de backup.

Em resumo, o Amazon EBS é uma solução de armazenamento em bloco de alto desempenho que é fundamental para muitas aplicações em execução na AWS devido à sua durabilidade, flexibilidade e integração com a AWS.

Resumo - EFS
O Amazon Elastic File System (EFS) é um serviço de armazenamento de arquivos totalmente gerenciado que facilita a configuração e o dimensionamento de sistemas de arquivos em nuvem na AWS. O EFS foi projetado para ser altamente disponível, durável e seguro, e pode ser usado com uma ampla gama de serviços da AWS e aplicações on-premise.



Aqui estão alguns pontos-chave sobre o Amazon EFS:



**Escalabilidade:** O EFS é projetado para escalar automaticamente para acomodar o crescimento dos dados, de alguns gigabytes a petabytes, sem a necessidade de provisionar o armazenamento.

**Alta Disponibilidade e Durabilidade:** O EFS armazena automaticamente os arquivos em vários dispositivos dentro e entre várias zonas de disponibilidade para garantir a disponibilidade e durabilidade dos dados.

**Compartilhamento de Arquivos:** O EFS suporta o compartilhamento de arquivos entre várias instâncias do Amazon EC2, permitindo que múltiplos servidores acessem um sistema de arquivos simultaneamente.

**Integração com AWS:** O EFS pode ser integrado a outros serviços da AWS, como o AWS Backup para backups automatizados e o AWS IAM para controle de acesso.

**Tipos de armazenamento:** O EFS oferece várias classes de armazenamento, incluindo Standard e Infrequent Access (IA), permitindo que você otimize os custos com base em seus padrões de acesso aos arquivos.

**Segurança:** O EFS inclui suporte para criptografia de dados em repouso e em trânsito, bem como integração com o AWS Key Management Service (KMS) para gerenciamento de chaves de criptografia.

Resumindo, o Amazon EFS é uma solução de armazenamento de arquivos escalável, de alta disponibilidade e segura, que facilita o compartilhamento de arquivos entre instâncias EC2 e outros serviços AWS.

Resumo - FSx
O Amazon FSx é um serviço de armazenamento de arquivos totalmente gerenciado da AWS que facilita o lançamento e a execução de sistemas de arquivos de terceiros. O FSx fornece o rico conjunto de recursos e a rápida performance que esses tipos de aplicativos precisam, e atualmente suporta dois sistemas de arquivos: Windows File Server para aplicações baseadas em Windows, e Lustre para cargas de trabalho de computação intensiva.

Aqui estão alguns pontos chave sobre o Amazon FSx:



**FSx para Windows File Server:** Ele fornece um sistema de arquivos nativamente compatível com o Windows, permitindo que você mova com facilidade as aplicações baseadas em Windows que exigem o sistema de arquivos do Windows para a AWS. É construído sobre o Windows Server e oferece suporte a recursos como deduplicação de dados, criptografia de dados em repouso, e acesso via SMB (Server Message Block) e NFS (Network File System).

**FSx para Lustre:** O Lustre é um sistema de arquivos popular para cargas de trabalho de computação intensiva, como análise de big data, modelagem de machine learning e processamento de mídia. O FSx para Lustre é totalmente gerenciado pela AWS, simplificando o processo de criação e execução de um sistema de arquivos Lustre.

**Desempenho:** O Amazon FSx foi projetado para oferecer o desempenho rápido necessário para suportar aplicações exigentes. Ele fornece baixa latência e altas taxas de transferência de dados.

**Compatibilidade e Integração:** O Amazon FSx é totalmente compatível com os sistemas de arquivos que suporta, o que significa que você pode usar suas ferramentas e aplicações existentes sem modificação. Além disso, o FSx se integra com uma série de outros serviços AWS para coisas como backup, monitoramento e acesso seguro a arquivos.

**Segurança:** O Amazon FSx oferece várias funcionalidades de segurança, como a capacidade de armazenar dados em redes virtuais privadas da Amazon (VPCs), suporte a redes de acesso (ACLs) para o Windows File Server, criptografia de dados em repouso e em trânsito, e integração com AWS Key Management Service (KMS) para gerenciamento de chaves de criptografia.

Em resumo, o Amazon FSx é um serviço poderoso e flexível que torna mais fácil do que nunca para você executar sistemas de arquivos totalmente gerenciados na AWS. Ele suporta sistemas de arquivos Windows e Lustre, oferecendo um alto nível de desempenho, segurança e integração com outros serviços AWS.


## Resumo - AutoScaling
O Amazon Auto Scaling é um serviço da AWS que permite o dimensionamento automático de recursos para manter a performance e a disponibilidade de suas aplicações. Ele funciona monitorando continuamente suas aplicações e ajustando a capacidade para manter a performance estável e previsível ao menor custo possível.

Aqui estão algumas características principais do Amazon Auto Scaling:



**Dimensionamento Automático:** O Auto Scaling permite que você defina políticas de dimensionamento que ajustam automaticamente a capacidade de recursos com base nas condições definidas. Por exemplo, você pode dimensionar automaticamente o número de instâncias do Amazon EC2 para atender à demanda de tráfego.

**Otimização de Custo e Performance:** Ao ajustar continuamente a capacidade, o Auto Scaling ajuda a melhorar a disponibilidade e minimizar os custos. Quando a demanda aumenta, o Auto Scaling adiciona automaticamente mais recursos. Quando a demanda diminui, ele remove os recursos desnecessários para economizar dinheiro.

**Balanceamento de Carga:** O Auto Scaling pode ser usado junto com o Elastic Load Balancing (ELB) para distribuir o tráfego de aplicações entre várias instâncias EC2 para melhorar a disponibilidade e a tolerância a falhas.

**Saúde da Aplicação:** O Auto Scaling realiza verificações de saúde em suas instâncias EC2 e substitui automaticamente as instâncias que não estão saudáveis.

**Integração AWS:** O Auto Scaling está integrado com uma série de serviços da AWS, incluindo Amazon CloudWatch, Amazon SNS, AWS CloudFormation, entre outros.

**Flexibilidade:** O Auto Scaling permite dimensionar vários recursos, não se limitando apenas às instâncias EC2. Você também pode dimensionar serviços como Amazon DynamoDB, Amazon Aurora, Amazon ECS, e Amazon RDS.

Em resumo, o Amazon Auto Scaling é um serviço eficaz e essencial para otimizar a performance e a disponibilidade de suas aplicações na AWS, garantindo que você tenha o número certo de recursos da AWS quando precisar.


## Resumo - ELB
O Elastic Load Balancing (ELB) é um serviço da Amazon Web Services (AWS) que distribui automaticamente o tráfego de entrada de aplicações em várias instâncias EC2, contêineres, endereços IP e funções Lambda para garantir que as aplicações tenham alta disponibilidade e desempenho.

Aqui estão algumas características principais do ELB:



**Tipos de Balanceador de Carga:** O ELB oferece três tipos de balanceadores de carga que se adequam a diferentes necessidades de aplicação - o Balanceador de Carga de Aplicação (ALB) para tráfego HTTP e HTTPS, o Balanceador de Carga de Rede (NLB) para tráfego TCP, UDP e TLS, e o Classic Load Balancer para tráfego HTTP, HTTPS, TCP e SSL.

**Alta disponibilidade:** O ELB distribui automaticamente o tráfego em várias instâncias em várias zonas de disponibilidade para garantir a continuidade do serviço, mesmo se uma ou mais instâncias falharem.

**Escalabilidade:** O ELB escala automaticamente a sua capacidade de balanceamento de carga em resposta ao tráfego de entrada.

**Integração com o Auto Scaling:** O ELB trabalha em conjunto com o Auto Scaling da AWS para garantir que há capacidade suficiente para atender ao tráfego de entrada e para substituir as instâncias que falham.

**Segurança:** O ELB oferece recursos de segurança como a integração com o AWS Certificate Manager para SSL/TLS, e a integração com o AWS Identity Access Management (IAM) para controle de acesso.

**Monitoramento e Auditoria:** O ELB integra-se com o Amazon CloudWatch e o AWS CloudTrail para monitorar o desempenho de suas aplicações e registrar as ações realizadas no seu balanceador de carga.

Resumindo, o Elastic Load Balancing é uma ferramenta essencial para a distribuição eficiente de tráfego, melhorando a disponibilidade e a tolerância a falhas das suas aplicações na AWS.

## Tipos de volumes **EBS**

**gp3** & **gp2** SSD Com capacidade de 1GB - 16TB.

**io2 Block Express** SSD com capacidade de 4GB - 64TB.
Leitura Complementar - O que é AWS Artifact
O QUE É O AWS ARTIFACT?

O AWS Artifact, disponível no console, é um portal de autoatendimento para recuperação de artefatos de auditoria que oferece aos clientes acesso sob demanda à documentação de conformidade e aos acordos da AWS.

Você pode usar os relatórios do AWS Artifact para fazer download de documentos de segurança e conformidade, como os relatórios de certificações ISO, Payment Card Industry (PCI – Setor de cartões de pagamento) e Organization Control (SOC – Controles de sistema e organização).

Você pode usar o AWS Artifact Agreements para examinar, aceitar e acompanhar o status de acordos da AWS como o Business Associate Addendum (BAA – Adendo de associado comercial).



QUEM TEM ACESSO AO AWS ARTIFACT?

Todas as contas da AWS têm acesso ao AWS Artifact. Os usuários raiz e do IAM com permissões de administrador podem fazer o download de todos os artefatos de auditoria disponíveis na conta concordando com os termos e condições associados.

Será necessário conceder aos usuários do IAM permissões de acesso não administrativas para o AWS Artifact usando as permissões do IAM. Com isso, você poderá conceder a um usuário o acesso ao AWS Artifact e restringir o acesso a outros serviços e recursos da conta da AWS. Para obter informações sobre como conceder acesso usando o IAM, consulte esse tópico de ajuda na documentação do AWS Artifact.



COMO PERMITO QUE OUTROS USUÁRIOS ACESSEM O AWS ARTIFACT AGREEMENTS?

Sua conta administrativa tem todas as permissões necessárias para usar o AWS Artifact. No entanto, documentos e acordos diferentes podem exigir a delegação de permissões distintas para diversos usuários. Você pode delegar permissões usando as políticas do IAM.



O QUE É UM ARTEFATO DE AUDITORIA?

Um artefato de auditoria é um elemento de evidência que demonstra que uma organização segue um processo documentado ou cumpre um requisito específico. Os artefatos de auditoria são coletados e arquivados ao longo do ciclo de vida de desenvolvimento de um sistema e servem como evidência em auditorias e avaliações internas e/ou externas.

No momento, o AWS Artifact oferece aos clientes relatórios e acordos que podem ser usados como artefatos de auditoria.



COMO FAÇO PARA COMPARTILHAR ARTEFATOS DE AUDITORIA COM OS AUDITORES?

Muitas vezes, será necessário que os auditores tenham acesso aos relatórios de conformidade da AWS. Você pode fazer isso facilmente criando credenciais de usuário do IAM específicas para cada auditor, configurando-as para limitar o acesso aos relatórios relevantes para a auditoria conduzida pelo auditor. Para obter mais informações, veja este tópico de ajuda na documentação do AWS Artifact.





COMO POSSO USAR ESSES ARTEFATOS PARA CUMPRIR REQUISITOS DE AUDITORIA?

Você pode fornecer os artefatos de auditoria da AWS aos auditores ou reguladores como evidência dos controles de segurança da AWS.

Além disso, é possível usar a orientação sobre responsabilidades fornecida por alguns artefatos de auditoria da AWS para projetar a arquitetura de nuvem. Essa orientação ajuda a determinar os controles de segurança adicionais que devem ser implantados para apoiar casos de uso específicos do sistema.



EXISTE UM LIMITE PARA O NÚMERO DE ARTEFATOS QUE POSSO OBTER POR DOWNLOAD?

Não. Você pode acessar e fazer o download de todos os artefatos a qualquer momento, tantas vezes quanto precisar.

Sobre AWS CloudFront
O Amazon CloudFront é um serviço de rede de entrega de conteúdo (CDN) rápido e altamente seguro oferecido pela Amazon Web Services (AWS). Ele distribui dados, vídeos, aplicativos e APIs para os espectadores dos usuários com baixa latência e altas velocidades de transferência.

Aqui estão algumas características notáveis e benefícios do Amazon CloudFront:



Desempenho melhorado: O CloudFront melhora o desempenho dos aplicativos, acelerando a entrega de conteúdo para os usuários finais. Isso é feito através do uso de uma rede global de pontos de presença (PoPs) que roteiam o conteúdo para o usuário a partir do local mais próximo.

Segurança robusta: O CloudFront oferece uma segurança robusta com integração ao AWS Shield, AWS Web Application Firewall (WAF) e Route 53 para ajudar a proteger seu aplicativo contra vários tipos de ataques. Ele também suporta a entrega segura de conteúdo através de HTTPS e integra-se ao AWS Certificate Manager para facilitar o gerenciamento de certificados SSL/TLS.

Escalabilidade: Como parte da AWS, o CloudFront pode escalar automaticamente para lidar com tráfego alto sem necessidade de intervenção manual.

Personalização: Com o CloudFront, você pode personalizar e otimizar o desempenho da entrega de conteúdo com base nas necessidades específicas do seu aplicativo.

Integração com a AWS: O CloudFront está profundamente integrado com outros serviços da AWS, como o S3, EC2, Elastic Load Balancer (ELB) e Route 53, o que facilita a entrega de conteúdo de várias fontes.

Custo Efetivo: O CloudFront usa um modelo de preços pay-as-you-go, onde você paga apenas pelo que usa. Além disso, há opções para economizar dinheiro ao se comprometer com um determinado nível de uso.

Em resumo, o Amazon CloudFront é uma solução de CDN segura, escalável e de alto desempenho que melhora a experiência do usuário, acelerando a entrega de conteúdo, enquanto protege seus aplicativos contra ameaças.
S3 Transfer Acceleration
O Amazon S3 Transfer Acceleration é um recurso do Amazon S3 que permite a transferência rápida e segura de arquivos por longas distâncias entre o cliente e um bucket do S3. Este serviço utiliza a rede global da Amazon CloudFront para acelerar as transferências de upload e download para o S3.

Aqui estão algumas características importantes e benefícios do S3 Transfer Acceleration:



Velocidade aprimorada: Este serviço é especialmente útil quando se precisa transferir grandes quantidades de dados de forma rápida e eficiente de um lugar distante para um bucket do S3.

Facilidade de uso: Ativar a Transfer Acceleration é tão simples quanto marcar uma caixa na configuração do bucket do S3. Não é necessário alterar o código da aplicação.

Utiliza a Rede da Amazon CloudFront: O serviço usa a infraestrutura de borda otimizada para latência da Amazon CloudFront, que tem pontos de presença (PoPs) em todo o mundo para rotear dados pela rede da AWS.

Custo Eficiente: Com a Transfer Acceleration, você paga apenas pelo que usa. No entanto, é importante notar que este serviço é cobrado além das taxas padrão de solicitação e armazenamento do S3.

Segurança: Assim como o S3, a Transfer Acceleration suporta a transferência de dados por HTTPS, oferecendo o mesmo nível de segurança dos dados em trânsito.

Em resumo, o S3 Transfer Acceleration é uma solução eficiente quando se precisa transferir grandes volumes de dados por longas distâncias. Ele maximiza a velocidade de transferência de dados, melhorando o desempenho e a eficiência das operações de negócios que envolvem o S3.

AWS Global Accelerator
O AWS Global Accelerator é um serviço que melhora a disponibilidade e o desempenho de suas aplicações para usuários em todo o mundo. Ele faz isso usando a rede global altamente disponível da AWS e redirecionando o tráfego de usuários para a aplicação mais próxima em termos de latência. Isso resulta em uma melhoria significativa na experiência do usuário.

Aqui estão algumas características notáveis e benefícios do AWS Global Accelerator:



Desempenho aprimorado: O Global Accelerator melhora a velocidade de conexão e a latência para as aplicações da AWS, tornando-as mais rápidas e responsivas para os usuários, não importa onde eles estejam localizados.

Alta Disponibilidade: Utilizando a rede global da AWS, o Global Accelerator oferece uma alta disponibilidade, direcionando os usuários para a instância mais saudável da aplicação.

Fácil de configurar: Basta escolher os recursos da AWS que deseja acelerar, e o AWS Global Accelerator cuida do restante.

Segurança aprimorada: Com o Global Accelerator, você cria um único ponto de entrada para as suas aplicações, o que pode ser útil para configurações de segurança e firewall.

Escalabilidade: O serviço se adapta automaticamente às mudanças no tráfego de aplicação, o que o torna útil para cenários de alto tráfego ou para aplicações com padrões de tráfego imprevisíveis.

Em resumo, o AWS Global Accelerator é uma solução útil para melhorar a velocidade, a disponibilidade e a segurança de aplicações na AWS, proporcionando uma experiência de usuário mais suave e agradável.


Amazon Elastic Container Service (Amazon ECS)
O Amazon Elastic Container Service (ECS) é um serviço de gerenciamento de contêineres altamente escalável e de alto desempenho que suporta contêineres Docker e permite que você execute e gerencie facilmente aplicações em contêiner na Amazon Web Services (AWS).

Aqui estão algumas das principais características e funcionalidades do Amazon ECS:



Integração com a AWS: O ECS se integra perfeitamente com outros serviços da AWS, como o Amazon RDS, o Amazon DynamoDB, o AWS Lambda, o Amazon API Gateway, entre outros, facilitando a criação de aplicações com arquiteturas complexas.

Gerenciamento de Contêineres: O Amazon ECS gerencia o ciclo de vida dos contêineres, incluindo provisionamento, implantação, monitoramento de saúde, escala e desprovisionamento.

Escalabilidade: Com o Amazon ECS, você pode dimensionar suas aplicações de forma rápida e fácil para lidar com demandas de trabalho variáveis.

Segurança: As tarefas do ECS podem usar as funções do IAM para obter um controle de acesso fino aos recursos da AWS. Além disso, você pode executar suas tarefas em uma Amazon Virtual Private Cloud (VPC) para isolar suas aplicações.

Serviço Gerenciado: Como um serviço gerenciado, o Amazon ECS elimina a necessidade de instalar, operar e dimensionar a própria infraestrutura de gerenciamento de contêineres.

Monitoramento e Logs: O ECS oferece integração nativa com o Amazon CloudWatch e o Amazon CloudTrail, permitindo que você visualize métricas de utilização de recursos, acompanhe as chamadas de API e obtenha informações detalhadas sobre a saúde de suas aplicações.

Orquestração de Contêineres: O Amazon ECS permite a orquestração de contêineres complexos através de serviços e tarefas. Você pode especificar o número de contêineres para cada tarefa e definir regras para como eles devem ser posicionados em um cluster.

Em resumo, o Amazon ECS é uma ferramenta poderosa e escalável para a execução de aplicações em contêineres, oferecendo integração com a AWS e a flexibilidade de usar vários modelos de programação.




Amazon Elastic Kubernetes Service (Amazon EKS)
O Amazon Elastic Kubernetes Service (EKS) é um serviço de gerenciamento de contêineres que facilita a execução, escalabilidade e monitoramento de aplicações baseadas em contêineres usando o Kubernetes, um sistema de orquestração de contêineres de código aberto, na plataforma AWS.

Aqui estão algumas das principais características e funcionalidades do Amazon EKS:



Gerenciamento de Kubernetes: O EKS remove a complexidade de configurar e operar um ambiente de Kubernetes, permitindo que você se concentre na construção de aplicações.

Compatibilidade com Kubernetes: O EKS é totalmente compatível com aplicações que rodam em qualquer ambiente padrão do Kubernetes, o que significa que você pode migrar qualquer aplicação padrão Kubernetes para o EKS sem precisar de qualquer modificação.

Integração com a AWS: O Amazon EKS é profundamente integrado com serviços da AWS, como Amazon RDS, AWS Lambda, Amazon S3 e Elastic Load Balancers, fornecendo uma experiência de usuário consistente em todo o ecossistema AWS.

Segurança: O EKS executa automaticamente várias tarefas de segurança, como a rotação periódica das chaves de criptografia usadas para proteger os dados armazenados em seus clusters.

Escalabilidade: Com o EKS, você pode escalonar suas aplicações para lidar com demandas de tráfego pico e para baixo, dependendo das necessidades da aplicação.

Monitoramento e Diagnóstico: O EKS se integra com o AWS CloudTrail e Amazon CloudWatch, fornecendo monitoramento detalhado, log de eventos e diagnóstico de suas aplicações e clusters de Kubernetes.

Serviço Gerenciado: O Amazon EKS elimina a necessidade de instalar, operar e dimensionar a infraestrutura de gerenciamento do Kubernetes, simplificando a operação e manutenção de clusters de Kubernetes.

Em resumo, o Amazon EKS oferece uma maneira poderosa, segura e escalável de executar aplicações baseadas em contêineres na AWS, enquanto aproveita as vantagens do Kubernetes como um padrão de facto para a orquestração de contêineres.


