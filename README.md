# Implementação de WAF em Webserver

# Descrição

A implementação de um Web Application Firewall (WAF) em um servidor web é uma prática de segurança projetada para proteger aplicativos web contra uma variedade de ameaças e ataques cibernéticos. Um WAF atua como uma camada de segurança entre o tráfego da Internet e o servidor web, filtrando e monitorando as solicitações HTTP para identificar e bloquear atividades maliciosas.

# Tabela de conteúdos

* [Diagrama](#)

* [Instalação](#)

* [Características](#)

* [Utilização](#)

* [Testes](#)

* [Dúvidas](#)

# Diagrama

<img src="WAF.drawio (1).png">

# Instalação

Na AWS, a criação do WAF só é possível sendo integrado aos serviços de:
  -  CloudFront Distribuição da Amazon
  -  API REST do Amazon API Gateway
  -  Application Load Balancer
  -  AWS AppSyncAPI do GraphQL
  -  Conjunto de usuários do Amazon Cognito
  -  Serviço da AWS App Runner
  -  AWS Instância de acesso verificado

As seguintes dependências necessárias devem ser instaladas para executar o serviço corretamente:
- Criação da Instância
- Criação do Application Load Balancer
- Criação do Target Group
 
# Características

## 1. Filtragem de Tráfego:

- **Inspeção de Solicitações e Respostas:** O WAF inspeciona todas as solicitações HTTP que chegam ao servidor web, bem como as respostas retornadas ao cliente.
- **Filtragem Baseada em Regras:** As regras definidas anteriormente são aplicadas para identificar e bloquear tráfego malicioso. Isso pode incluir ataques como injeção SQL, cross-site scripting (XSS), cross-site request forgery (CSRF), entre outros.

## 2. Prevenção de Ataques:

- **Deteção de Anomalias:** Além das regras específicas, o WAF pode usar técnicas de detecção de anomalias para identificar comportamentos incomuns que podem indicar um ataque em andamento.
- **Mitigação de Ataques:** Quando um ataque é detectado, o WAF pode agir automaticamente para mitigar o impacto, como bloquear o tráfego ofensivo ou alertar os administradores.

## 3. Proteção contra Ameaças Conhecidas e Desconhecidas:

- **Atualizações de Assinaturas:** O WAF é frequentemente atualizado com novas assinaturas e regras para proteger contra ameaças emergentes. Isso inclui a atualização constante das definições de ataques conhecidos.

## 4. Monitoramento e Logging:

- **Registros Detalhados:** O WAF gera registros detalhados de todas as atividades, incluindo tentativas de ataques e tráfego bloqueado. Esses logs são essenciais para análise de segurança e conformidade.


# Utilização

Este serviço é utilizado para incrementar a segurança de serviços provisionados em nuvem.

# Testes

To run tests, you need to run the following command: 

# Duvidas

Em caso de dúvidas relacionadas a este repo, entre em contato comigo pelo linkedin ou email.
