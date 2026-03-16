## Testes exploratórios estruturados

Os testes exploratórios permitem explorar o sistema de forma dinâmica, identificando comportamentos inesperados e bugs que podem não estar cobertos por casos de teste formais.  
Para que sejam eficazes, utilizo **charters de exploração**, que definem o objetivo e o foco da sessão de teste, sem limitar a criatividade.

## Estrutura de um charter exploratório

Cada exploratory charter contém:

- **Objetivo:** Qual funcionalidade ou fluxo será explorado  
- **Foco:** Pontos específicos de atenção durante a sessão  
- **Duração:** Tempo estimado para a exploração  
- **Notas / Observações:** Anotações de comportamento, bugs encontrados ou insights  
- **Riscos ou áreas críticas:** Possíveis áreas que merecem atenção especial  


## Exemplos de charters exploratórios

### Charter 1: Login e autenticação
- **Objetivo:** Validar diferentes fluxos de login no sistema  
- **Foco:**  
  - Login com credenciais válidas  
  - Login com credenciais inválidas  
  - Campos obrigatórios vazios  
- **Duração:** 45 minutos  
- **Notas / Observações:**  
  - Verificar mensagens de erro  
  - Testar consistência da interface  
- **Riscos / áreas críticas:**  
  - Integração com API de autenticação  
  - Validação de sessão e cookies  

### Charter 2: Cadastro de usuário
- **Objetivo:** Explorar o fluxo de criação de novos usuários  
- **Foco:**  
  - Validação de campos obrigatórios  
  - Testes de formatação de dados (email, senha)  
  - Interações com mensagens de validação  
- **Duração:** 60 minutos  
- **Notas / Observações:**  
  - Verificar consistência das mensagens de erro  
  - Testar comportamento com dados repetidos  
- **Riscos / áreas críticas:**  
  - Validação de unicidade de email  
  - Integração com banco de dados
