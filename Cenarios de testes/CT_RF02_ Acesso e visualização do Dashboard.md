## Cenário 02: Acesso e visualização do Dashboard.

### Caso de Teste 01: Acesso ao Dashboard após login bem-sucedido.

| ID       | Descrição                                                        |
| :------- | :---------------------------------------------------------------- |
| C02-CT01 | Verificar a exibição correta do Dashboard após login com sucesso. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar autenticado com credenciais válidas.     |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessou o sistema com sucesso              |
| **QUANDO** for redirecionado automaticamente após o login         |
| **ENTÃO** a tela do Dashboard deve ser exibida com os atalhos e widgets principais |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O sistema deve exibir corretamente a interface do Dashboard.     |

|                **Evidência(s)**               |
| :-------------------------------------------: |
| [Vídeo](https://jam.dev/c/47e4af1f-5771-4cae-a261-9ca6ea74fdc6) |
---

### Caso de Teste 02: Verificação da exibição dos widgets do Dashboard.

| ID       | Descrição                                                 |
| :------- | :-------------------------------------------------------- |
| C02-CT02 | Os widgets padrão devem ser exibidos corretamente no Dashboard. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar na tela do Dashboard após login.         |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário está autenticado                          |
| **E** está visualizando o Dashboard                              |
| **QUANDO** a página for carregada                                |
| **ENTÃO** widgets como \"Time at Work\" e \"My Actions\" devem ser exibidos |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| Todos os widgets principais devem ser visíveis e funcionais.     |

|                **Evidência(s)**               |
| :-------------------------------------------: |
| [Vídeo](https://jam.dev/c/0f9d24c8-bd90-4b1d-a22b-5f6aedafa201) |
---

### Caso de Teste 03: Acesso ao Dashboard com sessão expirada.

| ID       | Descrição                                                            |
| :------- | :------------------------------------------------------------------- |
| C02-CT03 | O sistema deve redirecionar o usuário para o login se a sessão estiver expirada. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário estava logado, mas a sessão expirou.                |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessou o sistema anteriormente            |
| **E** permaneceu inativo por um longo período                    |
| **QUANDO** tentar acessar o Dashboard novamente                  |
| **ENTÃO** o sistema deve redirecioná-lo para a página de login    |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| A sessão expirada deve ser tratada corretamente com redirecionamento. |

|                **Evidência(s)**               |
| :-------------------------------------------: |
| [Vídeo](https://jam.dev/c/90df263b-536c-413d-bf1f-c22540230749) |