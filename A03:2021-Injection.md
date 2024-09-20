# A03:2021-Injection

## O que é?
- É uma vulnerabilidade em que o usuário de um sistema insere dados de maneira inadequada, dando acesso a ele a informações sensíveis para a aplicação<br>
- Ao conseguir fazer um injection, pode-se inserir um código que se for interpretado pelo sistema pode retornar informações do banco de dados por exemplo<br>
- Esse problema ocorre quando não é feito uma sanitização dos dados de entrada do usuário<br>
## Como se aplica?
- Existem diversos tipos de injection:<br>
<strong>-> SQL Injection<br></strong>
Injeção de código de banco de dados (SQL)<br>
<strong>-> Command Injection<br></strong>
Injeção de comandos interpretados pelo sistema operacional<br>
<strong>-> Cross-Site Scripting(XSS)<br></strong>
Injeção de scripts de JavaScript<br>
<strong>-> LDAP Injection<br></strong>
Injeção de comandos executados pelo protocolo que mantêm serviços de diretório de uma rede(Lightweight Directory Access Protocol)<br>
<strong>-> XML Injection<br></strong>
Injeção de consultas XML<br>
<strong>-> Code Injection<br></strong>
Injeção de código em PHP, Python ou outra linguagem que possivelmente rode no ambiente do servidor<br>
<strong>-> NoSQL Injection<br></strong>
Injeção de códigos que rodam em bancos de dados NoSQL<br>
<strong>-> XPath Injection<br></strong>
Injeção de comandos de XPath (XML Path Language) que gerencia dados XML<br>
<strong>->Host Header Injection<br></strong>
Pode redirecionar o tráfego ao manipular o host  do cabeçalho HTTP de uma página<br>
<strong>->Email Header Injection<br></strong>
Injeção de comandos de campos de cabeçalhos de emails, enviando emails não autorizados<br>
### Exemplo

## Como prevenir?
