## Cenário 05: Gerenciamento de candidatos no módulo de Recrutamento.

### Caso de Teste 01: Adicionar um novo candidato com dados válidos.

| ID       | Descrição                                                              |
| :------- | :---------------------------------------------------------------------- |
| C05-CT01 | O sistema deve permitir adicionar um novo candidato com informações válidas. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado e ter acesso ao módulo "Recruitment". |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"Recruitment\"             |
| **E** clica em \"Add\"                                           |
| **E** preenche os campos obrigatórios (nome, vaga, e-mail)       |
| **QUANDO** clicar em \"Save\"                                    |
| **ENTÃO** o candidato deve ser adicionado à lista de candidatos  |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O candidato deve ser exibido corretamente na lista após o cadastro. |

|                **Evidência(s)**               |
| :-------------------------------------------: |
| [Vídeo](https://jam.dev/c/c7c4307e-d76d-4a90-b4c7-bea0fd6da1e8) |
---

### Caso de Teste 02: Tentar adicionar candidato sem preencher campos obrigatórios.

| ID       | Descrição                                                                     |
| :------- | :------------------------------------------------------------------------------ |
| C05-CT02 | O sistema deve exibir mensagens de erro ao tentar cadastrar um candidato sem preencher os campos obrigatórios. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado no sistema.                       |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"Recruitment\"             |
| **E** clica em \"Add\"                                           |
| **E** não preenche os campos obrigatórios                       |
| **QUANDO** clicar em \"Save\"                                    |
| **ENTÃO** mensagens de erro devem ser exibidas em cada campo obrigatório |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| Os campos obrigatórios devem ser validados com mensagens de erro. |

|                **Evidência(s)**               |
| :-------------------------------------------: |
| [Vídeo](https://jam.dev/c/90eb96fd-881c-4c50-9f96-001f3157f94c) |
---

### Caso de Teste 03: Buscar candidato cadastrado pelo nome.

| ID       | Descrição                                                        |
| :------- | :---------------------------------------------------------------- |
| C05-CT03 | O sistema deve retornar corretamente um candidato pesquisado pelo nome. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O candidato deve estar cadastrado no sistema.                 |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"Recruitment\"             |
| **E** digita o nome do candidato no campo de busca              |
| **QUANDO** clicar no botão \"Search\"                           |
| **ENTÃO** o sistema deve listar corretamente o candidato correspondente |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O candidato pesquisado deve ser exibido na lista de resultados. |

|                **Evidência(s)**               |
| :-------------------------------------------: |
| [Vídeo](https://jam.dev/c/62da1d78-81fc-4c29-bab9-394062e4eb0e) |

### Caso de Teste 04: Buscar candidato não cadastrado pelo nome.

| ID       | Descrição                                                        |
| :------- | :---------------------------------------------------------------- |
| C05-CT04 | O sistema deve exibir erro se um candidato pesquisado pelo nome não existir. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
|           |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"Recruitment\"             |
| **E** digita o nome do candidato inexistente no campo de busca              |
| **QUANDO** clicar no botão \"Search\"                           |
| **ENTÃO** o sistema deve exibir erro de campo inválido |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| A pesquisa não deve ser realizada. |

|                **Evidência(s)**               |
| :-------------------------------------------: |
| [Vídeo](https://jam.dev/c/7e11f0d6-589a-4d4a-bbbc-5a3a624effc5) |