# A10:2021-Server-Side Request Forgery (SSRF)

## O que é

## Como funciona?

### Exemplo

## Como evitar?
- Não deixe o usuário ter acesso direto a URL
- Valide e sanitize todo input de users
- Use o firewall para evitar que o servidor web acesse recursos internos
- Valide a autenticidade e a permissão de qualquer requerimento do usuário
- Limite timeout para evitar ataques DoS
- Use bibliotecas seguras de requisições HTTP
