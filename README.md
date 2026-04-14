# Oracle-Database-OCI
Implementação de Oracle Database em Cloud Projeto

Implementação de ambiente de banco de dados Oracle em nuvem utilizando Oracle Cloud Infrastructure, incluindo provisionamento de infraestrutura, configuração do sistema operacional, instalação do banco e acesso remoto para administração.

Arquitetura da Solução

Infraestrutura implantada:

Internet   
Security List (Firewall OCI)   
Virtual Cloud Network (VCN)   
Compute Instance   
  Oracle Linux
  Oracle Database 19C
  Oracle Net Listener (1521)
  SSH Access (22)
   
   Tecnologias utilizadas:

Oracle Cloud Infrastructure
Oracle Linux
Oracle Database
Oracle SQL Developer
OpenSSH

Implementação Técnica
Provisionamento da Infraestrutura
Criação de Virtual Cloud Network (VCN)
Configuração de Security Lists
Criação de Compute Instance

Sistema operacional utilizado:
Oracle Linux 8

Configuração de Acesso Remoto

Conexão segura via SSH Key Authentication

Exemplo:

ssh opc@public-ip

Configuração utilizando OpenSSH.
Instalação do Oracle Database

Instalação manual do banco Oracle Database no ambiente Linux.

Configurações realizadas:

parâmetros de kernel
limites de usuário
variáveis de ambiente
ORACLE_HOME
ORACLE_BASE
ORACLE_SID
Criação do banco com DBCA.

Configuração de Rede

Configuração do listener Oracle Net.

Porta utilizada:

1521

Validação:

lsnrctl status

Configuração de Firewall

Regras criadas na VCN:

Porta	Uso
22	acesso SSH
1521	conexão Oracle

Conectividade com Ferramenta Cliente

Conexão realizada com Oracle SQL Developer.

Parâmetros:

Host: Public IP
Porta: 1521
Service Name: ORCL

Resultados do Projeto

Ambiente funcional com:

✔ Oracle Database acessível remotamente
✔ administração via SQL Developer
✔ segurança de acesso via SSH
✔ listener configurado
✔ firewall configurado na OCI




