
✅ Exemplo Prático: Login

| Seção                | Conteúdo                                                                 |
|-----------------------|---------------------------------------------------------------------------|
| **ID da História**    | US-015                                                                   |
| **Título**            | Login com e-mail e senha                                                 |
| **Descrição**         | Como **cliente do portal de serviços** <br> Quero **acessar minha conta utilizando e-mail e senha** <br> Para que **eu consiga visualizar e gerenciar meus serviços contratados** |
| **Contexto / Observações** | - O login deve seguir as políticas de segurança da LGPD. <br> - Senha deve ter no mínimo 8 caracteres, contendo letra maiúscula, número e caractere especial. |
| **Cenários**          | 1. **Login bem-sucedido** <br> Dado que o cliente possui cadastro ativo <br> Quando informar corretamente e-mail e senha <br> Então o sistema deve conceder acesso ao portal e redirecionar para a página inicial. <br><br> 2. **Senha incorreta** <br> Dado que o cliente possui cadastro ativo <br> Quando informar e-mail correto mas senha incorreta <br> Então o sistema deve exibir mensagem "Usuário ou senha inválidos". <br><br> 3. **Conta bloqueada** <br> Dado que o cliente excedeu 5 tentativas de login <br> Quando tentar acessar novamente <br> Então o sistema deve exibir mensagem "Conta bloqueada. Redefina sua senha ou entre em contato com o suporte". |
| **Critérios de Aceitação** | - O sistema deve validar credenciais em tempo real. <br> - Bloquear a conta após 5 tentativas inválidas. <br> - A mensagem de erro não deve revelar se o e-mail é válido ou não. <br> - O login deve ocorrer em menos de 3 segundos após o envio das credenciais. |
| **Critérios Técnicos (opcional)** | - Usar autenticação via OAuth 2.0. <br> - Registrar logs de todas as tentativas de login. <br> - Compatível com dispositivos móveis e navegadores desktop. |
