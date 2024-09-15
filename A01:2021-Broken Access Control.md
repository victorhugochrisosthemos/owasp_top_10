# A01:2021-Broken Access Control
- Quebra do controle de acesso de algum aplicativo<br>
- Muitos sistemas não validam como é feito o controle de acesso<br>
- Uma aplicação geralmente tem um login e senha, um token de sessão, um cookie, um id de usuário na sessão, data storage<br>
- Mas esse controle de acesso não é bem implementado<br>

## Como é explorada?
- Se é gerado um id de usuário, ao jogar em outro navegador funciona, mas o correto seria esse id ser válido somente para o browser inicial, para um IP ou um cliente somente<br>

### Exemplo
-> Um usuário acessa uma página da aplicação dessa maneira:<br>
    https://curso_online.com/nota_processo_seletivo/usuario123<br>
-> Então faz um teste em trocar um parâmetro da URL:<br>
    https://curso_online.com/nota_processo_seletivo/usuario456<br>
-> O risco no exemplo é conseguir acessar os dados, ou seja, há quebra de controle de acesso, vendo informações que não deveria sobre outros usuários<br>

## Como evitar?
- Todo recurso que não é público precisa enviar informações de validação desse usuário como id de usuário ativo por parâmetro na url, no body ou na requisição e validar se é autenticado e autorizado<br>
  -> Autenticação é validar a identidade do usuário<br>
  -> Autorização é verificar se o usuário tem permissão para acessar o requerimento requerido<br>
- Token JWT<br>
  -> JSON Web Token<br>
  -> É um padrão seguro de troca de informações, realizando autenticação e autorização<br>
- Rastrear o comportamento do usuário e se sair do padrão fazer um alerta para o time de monitoramento<br>
  -> Exemplo: acesso, hora e browser fora do padrão de comportamento do usuário<br>
