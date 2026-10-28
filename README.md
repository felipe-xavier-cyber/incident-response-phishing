Contexto: Detecção de envio massivo de e-mails (350 destinatários) com anexo PDF malicioso a partir de uma conta corporativa interna (vrodrigues@...). O assunto era "Proposta de RFP".

Análise Técnica (Triagem de IoCs):

Identificação do vetor: Conta legítima comprometida (AuthAs: Internal).

Análise do anexo: PDF sem detecção no VirusTotal, mas contendo um link embutido para uma página de redirecionamento (ibuild-corp.com/...).

Engenharia Social: O link redirecionava para uma página falsa de login da Microsoft para captura de credenciais.

Ações de Contenção e Erradicação (Playbook):

Bloqueio imediato da conta no M365.

Revogação de todos os tokens de sessão ativos (para expulsar o atacante).

Reset de senha e reconfiguração de MFA.

Auditoria e remoção de regras de encaminhamento (Forwarding Rules) maliciosas criadas pelo atacante.

Habilidades demonstradas: Incident Response (IR), Análise de Phishing, Threat Intelligence (VirusTotal), Microsoft 365 Security, IAM (Identity & Access Management).
