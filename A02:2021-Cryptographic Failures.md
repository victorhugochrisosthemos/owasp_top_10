# A02:2021-Cryptographic Failures
## O que é
- Essa vulnerabilidade trata de falhas no uso de criptografias<br>
- Pode estar relacionado a criptografias fracas como MD5 e SHA-1, exposição a chaves de permissão, não colocar criptografia onde devia ou não utilizar corretamente o protocolo TLS<br>
- O protocolo TLS substitui o SSL, o protocolo SSL já tem um tipo de ataque para quebrá-lo (POODLE)<br>
## Como é explorada?
- Se um banco de dados conter uma coluna de senhas com criptografia MD5, se alguém tiver acesso a esse dado criptografado pode usar uma ferramenta de quebra de criptografia MD5 para saber a real senha de um usuário<br>
### Exemplo
- O hash MD5 "698dc19d489c4e4db73e28a713eab07b" pode ser facilmente quebrado pela ferramenta de criptografia do site https://10015.io/tools/md5-encrypt-decrypt<br>
## Como evitar?
- Criptografia forte (criptografia AES e RSA são as mais atualizadas no momento)<br>
- Atualizações gerais constantes no sistema de segurança da aplicação<br>
- Uso correto de HTTPS e TLS<br>
