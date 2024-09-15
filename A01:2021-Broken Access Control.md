# A01:2021-Broken Access Control
- Quebra do controle de acesso de algum aplicativo
- Muitos sistemas não validam como é feito o controle de acesso
- Uma aplicação geralmente tem um login e senha, um token de sessão, um cookie, um id de usuário na sessão, data storage
- Mas esse controle de acesso não é bem implementado

## Como é explorada?
- Se é gerado um id de usuário, ao jogar em outro navegador funciona, mas o correto seria esse id ser válido somente para o browser inicial, para um IP ou um cliente somente

### Exemplo
-> Um usuário acessa uma página da aplicação dessa maneira:
    https://curso_online.com/nota_processo_seletivo/usuario123
-> Então faz um teste em trocar um parâmetro da URL:
    https://curso_online.com/nota_processo_seletivo/usuario456
-> O risco no exemplo é conseguir acessar os dados, ou seja, há quebra de controle de acesso, vendo informações que não deveria sobre outros usuários

## Como evitar?
- Todo recurso que não é público precisa enviar informações de validação desse usuário como id de usuário ativo por parâmetro na url, no body ou na requisição e validar se é autenticado e autorizado
  -> Autenticação é validar a identidade do usuário
  -> Autorização é verificar se o usuário tem permissão para acessar o requerimento requerido
- Token JWT
  -> JSON Web Token
  -> É um padrão seguro de troca de informações, realizando autenticação e autorização
- Rastrear o comportamento do usuário e se sair do padrão fazer um alerta para o time de monitoramento
  -> Exemplo: acesso, hora e browser fora do padrão de comportamento do usuário
