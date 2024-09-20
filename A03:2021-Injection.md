# A03:2021-Injection

## O que é?
- É uma vulnerabilidade em que o usuário de um sistema insere dados de maneira inadequada, dando acesso a ele a informações sensíveis para a aplicação<br>
- Ao conseguir fazer um injection, pode-se inserir um código que se for interpretado pelo sistema pode retornar informações do banco de dados por exemplo<br>
- Esse problema ocorre quando não é feito uma sanitização dos dados de entrada do usuário<br>
## Como se aplica?
- Existem diversos tipos de injection:<br>
-> SQL Injection<br>
Injeção de código de banco de dados (SQL)<br>
-> Command Injection<br>
Injeção de comandos interpretados pelo sistema operacional<br>
-> Cross-Site Scripting(XSS)<br>
Injeção de scripts de JavaScript<br>
-> LDAP Injection<br>
Injeção de comandos executados pelo protocolo que mantêm serviços de diretório de uma rede(Lightweight Directory Access Protocol)<br>
-> XML Injection<br>
Injeção de consultas XML<br>
-> Code Injection<br>
Injeção de código em PHP, Python ou outra linguagem que possivelmente rode no ambiente do servidor<br>
-> NoSQL Injection<br>
Injeção de códigos que rodam em bancos de dados NoSQL<br>
-> XPath Injection<br>
Injeção de comandos de XPath (XML Path Language) que gerencia dados XML<br>
->Host Header Injection<br>
Pode redirecionar o tráfego ao manipular o host  do cabeçalho HTTP de uma página
->Email Header Injection<br>
Injeção de comandos de campos de cabeçalhos de emails, enviando emails não autorizados<br>
### Exemplo

## Como prevenir?
