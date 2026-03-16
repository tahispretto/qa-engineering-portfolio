## Exemplos de registro de bugs

Nesta seção apresento exemplos de como os bugs são documentados durante o processo de testes. Um bom bug report deve ser claro, objetivo e conter informações suficientes para que o time de desenvolvimento consiga reproduzir e corrigir o problema.

As informações normalmente incluem:

- Título do bug
- Descrição
- Massa de teste utilizada
- Passos para reprodução
- Resultado esperado
- Resultado atual
- Prioridade
- Ambiente de teste


## Exemplo de Bug Report 1

**Título:** Erro ao realizar login com credenciais válidas

**Descrição:**  
Ao tentar realizar login com um usuário válido, o sistema retorna uma mensagem de erro e não permite o acesso.

**Passos para reprodução:**

1. Acessar a página de login  
2. Informar usuário válido  
3. Informar senha válida  
4. Clicar no botão "Entrar"

**Resultado esperado:**  
O usuário deve acessar o sistema com sucesso.

**Resultado atual:**  
O sistema exibe uma mensagem de erro informando que as credenciais são inválidas.

**Prioridade:** Alta  
**Ambiente:** UAT

---

## Exemplo de Bug Report 2

**Título:** Mensagem de validação não exibida ao deixar campo obrigatório vazio

**Descrição:**  
Ao tentar enviar um formulário sem preencher o campo e-mail, que é um campo obrigatório, o sistema não exibe a mensagem de validação esperada.

**Passos para reprodução:**

1. Acessar a página de cadastro  
2. Deixar o campo "Email" vazio  
3. Preencher os demais campos  
4. Clicar em "Cadastrar"

**Resultado esperado:**  
O sistema deve exibir uma mensagem informando que o campo "E-mail" é obrigatório.

**Resultado atual:**  
O formulário é enviado sem exibir a mensagem de validação.

**Prioridade:** Média  
**Ambiente:** UAT