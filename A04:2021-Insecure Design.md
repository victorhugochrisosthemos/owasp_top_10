# A04:2021-Insecure Design
## O que é?
- A estrutura de desenvolvimento do projeto não supoorta mecanismos de segurança, debilitando a segurança do sistema
## Como é explorada?
- É necessário que uma aplicação leve em consideração os seguintes cenários:
    - Controle de acesso adequado;
    - Validação e sanitização de inputs users
    - Uso adequdo de criptografia
    - Proteção contra ataques:
        - SQL injection
        - XSS
        - Brute force
### Exemplo
- Ataque de força bruta pode ser usado se o sistema não cuidar dessa questão na tela de cadastro/entrada do usuário
- Manipulação de URLs sem permissão, se não tratado esse processo pode dar acesso de administrador do sistema
## Como evitar?
- Utilizar princípios de segurança nas metodologia de desenvolvimento dos sistemas (DevSecOps)<br>
- Fazer análise de riscos para os projetos, identificando <br>
- Implementar controle de segurança<br>
- Treinamento da equipe de desenvolvimento e revisões do design no quesito segurança<br>
