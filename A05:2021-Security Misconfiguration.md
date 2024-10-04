# A05:2021-Security Misconfiguration

## O que é
- Vulnerabilidade gerada pela configuração incorreta de serviços que estejam rodando em uma aplicação
- Um sistema pode importar diversas funcionalidades de diferentes fontes para seu funcionamento
- Esses serviços podem ser de servidores, BD, APIs, bibliotecas ou o ambiente de execução do sistema
## Como funciona?
- Acesso de diretórios e arquivos sem a devida permissão
- Contas com senhas fracas
- Informações sensíveis expostas em mensagem de erro
- Desatualização da versão desses serviços
- Configurações de segurança desabilitadas
### Exemplo
- Um sistema web é sustentado na internet e as configurações da acessa ao BD continuam com o login e senha admin. Nessa situação, não ter atualizado as configurações de usuários com altas permissões ao mudar o ambiente de desenvolvimento para o de execução permite oum atacante a ganhar acesso total do BD
## Como evitar?
- Atualização contínua do sistema de segurança do sistema
- Desativar funções desnecessárias
- Gerenciamento de patches (atualização dos serviços importado no sistema)
- Políticas de privilégios de usuário rígidas, evitando exposições desnecessárias do sistema
