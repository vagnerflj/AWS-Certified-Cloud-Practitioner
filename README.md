Resumo - IAM
O AWS Identity and Access Management (IAM) é um serviço da AWS que ajuda a controlar quem está autenticado (assinado) e autorizado (tem permissões) para usar os recursos da AWS.

Aqui estão os principais pontos sobre o IAM:



Controle Granular de Acesso a AWS: Com o IAM, você pode criar usuários, grupos, papéis e políticas de permissão para controlar o acesso aos serviços e recursos da AWS de uma maneira granular. Por exemplo, você pode permitir que um usuário tenha acesso somente leitura ao Amazon S3 e acesso total ao EC2.

Compartilhamento Seguro de Acesso: O IAM permite compartilhar o acesso à sua conta AWS de maneira segura. Em vez de compartilhar suas credenciais de root, você pode criar vários usuários IAM, cada um com suas próprias credenciais e permissões.

Identidade Federada: Com o IAM, você também pode permitir usuários que já tenham senhas em outros lugares, como na sua rede corporativa ou em um provedor de identidade baseado em SAML, a obter acesso temporário à sua conta AWS.

Compatível com Multi-Fator Authentication (MFA): O IAM é compatível com a autenticação de vários fatores para fornecer uma camada adicional de proteção de segurança ao gerenciar o acesso aos serviços e recursos da AWS.

Integrado com AWS Services: O IAM está integrado com todos os serviços da AWS, o que significa que você pode definir permissões para qualquer serviço que desejar.

Auditoria com AWS CloudTrail: Com o AWS CloudTrail, você pode registrar todas as ações de usuários e APIs IAM para fins de auditoria.

Gratuito: O IAM é um recurso gratuito da AWS; você só paga pelos outros recursos da AWS que seus usuários acessam.

Em suma, o AWS IAM é um serviço de segurança crítico que ajuda a proteger o acesso aos recursos da AWS, permitindo que você controle quem pode fazer o quê em sua conta AWS.

Resumo - MFA
A Autenticação Multifator (MFA) é um método de controle de acesso que exige que um usuário verifique sua identidade usando duas ou mais evidências (fatores) antes que o acesso seja concedido. Estes fatores podem ser algo que o usuário sabe (como uma senha), algo que o usuário tem (como um telefone celular ou um token de hardware) e algo que o usuário é (como uma impressão digital ou reconhecimento facial).

Aqui estão alguns pontos-chave sobre MFA:



Segurança Aprimorada: O principal benefício da MFA é que ela aumenta significativamente a segurança, tornando muito mais difícil para os invasores ganharem acesso não autorizado a um sistema. Mesmo que um fator de autenticação seja comprometido (por exemplo, se uma senha for roubada), os outros fatores ainda protegem o sistema.

Diversos Métodos de Autenticação: A MFA pode usar uma variedade de métodos de autenticação, como códigos de verificação por SMS, aplicativos de autenticação, tokens de hardware, impressões digitais, reconhecimento facial e muito mais.

Compatibilidade: A MFA é compatível com muitos sistemas e serviços, incluindo a maioria das plataformas de nuvem (como AWS, Google Cloud e Azure), serviços de email, redes sociais, plataformas de pagamento online, entre outros.

AWS MFA: A AWS suporta MFA e recomenda que os usuários a utilizem para proteger suas contas. Com a MFA ativada, quando um usuário se conecta à AWS, ele é solicitado a inserir seu nome de usuário e senha (primeiro fator) e um código de autenticação de um dispositivo MFA (segundo fator).

Resumindo, a Autenticação Multifator é uma medida de segurança essencial que protege os sistemas de acesso não autorizado, exigindo que os usuários verifiquem sua identidade com vários fatores de autenticação.
