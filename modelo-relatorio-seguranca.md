# RELATÓRIO DE IMPLEMENTAÇÃO DE MEDIDAS DE SEGURANÇA
## Data 26/07/2023
## Empresa: AMC Industrias
## Responsável: A. Morlin

# Introdução

Esse relatório apresenta um processo de implementação de ferramentas na empresa AMC Indústrias, realizado por A. Morlin.

O objetivo do projefo foi elencar 3 medidas de segurança em conjunto dos serviços da AWS, com a finalidade de realizar aumentar a segurança na empresa.

# Descrição do Projeto

O projeto de implementação de ferramentas foi dividido em 3 medidas de segurança. A seguir, serão descritas as etapas da implementação:

## Medida 1:
* **Uso de autenticação multifator (MFA) na AWS / Não utilização do usuário Root**
* Habilitar a autenticação multifator (MFA) para o usuário raiz da conta AWS e todos os usuários da organização com acesso Administrativo na conta, além disso, criar credenciais de uso administrativo para evitar o uso do usuário **Root** da conta, deste modo, o uso do usuário root da conta é destinado somente para tarefas que exigem tal login, como algumas tarefas de gerenciamento de conta e serviços apenas.

## Medida 2:
* **Criar o AWS Organizations**
* Com o **AWS Organizations** é possível gerenciar todo o ambiente criando novas contas AWS sem custo  e alocar recursos para o time de Desenvolvimento e Produção separadamento, dessa forma, é possível alocar recursos e usar políticas de governança nas contas de modo isolado.

## Centralizar os logs do CloudTrail:
* Designar uma conta da AWS específica para resgisto em log (***Log Archive***) e definir permissões específicas em um bucket S3 para imperir as exclusões dos logs e criptografar todos os logs em repouso. Desse modo, é possível utilizar outras ferramentas para programar a visualização e análise dos logs, e centralizar na conta de Log Archive, logs de outras orignes, como CloudWatch Logs e dos balanceadores de carga da AWS.

## Conclusão
* A implementação de ferramentas na empresa AMC Indústrias tem como esperado reduzir as falhas de segurança, o acesso não autorizado e realizar auditorias operacionais e de risco no ambiente, o que aumentará a eficiência e produtividade da empresa. 
É indispensável a continuidade da utilização das ferramentas implementadas e a busca por novas tecnologias afim de melhorar ainda mais os processos da empresa.


## Anexos:
* Tarefas que exigem credenciais de root:
https://docs.aws.amazon.com/accounts/latest/reference/root-user-tasks.html

* AWS Organizations: 
https://aws.amazon.com/pt/organizations/

* AWS CloudTrail:
https://docs.aws.amazon.com/pt_br/awscloudtrail/latest/userguide/cloudtrail-user-guide.html



**Responsável pelo Projeto**
***Alexandre Morlin***