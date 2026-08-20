# Modelagem de Aplicativo Mobile para E-commerce de Farmácia

## Etapa 1 - Requisitos - Diagrama de Casos de Uso

**Atores:**
* Cliente
* Fornecedor
* Farmacêutico
* Entregador
* Médico
* Administração
* Atendente de suporte

**Requisitos Funcionais:**
* Gestão de Usuários: Cadastro, login (autenticação segura) e recuperação de senha.
* Catálogo de Produtos: Pesquisa de medicamentos e produtos de higiene, visualização de detalhes, preços e disponibilidade.
* Carrinho de Compras: Adicionar, remover e atualizar quantidade de itens.
* Processamento de Pedidos: Finalização da compra, escolha de entrega ou retirada e integração com meios de pagamento.
* Histórico de Pedidos: Acompanhamento do status de entrega e visualização de compras anteriores.
* Validação de Receita: Upload de fotos de receitas médicas para medicamentos controlados.
* Chat de Suporte: Canal direto de comunicação entre o Comprador e o Suporte.
* Dashboard: Página dedicada para geração de relatórios financeiros e de estoque em PDFs e acompanhamento de estoque e geração de métricas.

**Requisitos Não Funcionais:**
* Segurança: Criptografia de dados sensíveis (pagamento e dados pessoais) em conformidade com LGPD.
* Performance: Tempo de carregamento da página de listagem de produtos inferior a 2 segundos.
* Disponibilidade: O sistema deve operar com 99,9% de tempo de atividade.
* Usabilidade: Interface intuitiva e acessível em dispositivos mobile (iOS e Android).
* Escalabilidade: Capacidade de suportar picos de acessos em horários de maior movimento.

## Etapa 2 - Interface

Proposta de interface (telas e navegação) para o futuro sistema:
[Link do Figma](https://www.figma.com/design/nVxPTUu7r737D7mTjQOZDF/eCommerce-App-UI-Kit---Case-Study-Ecommerce-Mobile-App-Ul-kit--Community-?node-id=1-16990&t=WzQJHXpOeicdc2wW-1)

## Etapa 4 - SCRUM

### 1. Definir o Backlog do Sistema (Product Backlog)
No GitHub, cada item abaixo seria criado como uma Issue. O Product Backlog é a lista de todas as funcionalidades que o aplicativo precisa ter, organizadas em grandes grupos (Épicos).

**Épico 1: Autenticação e Segurança**
* Issue #1: Cadastro de usuário (Nome, E-mail, Telefone, Senha).
* Issue #2: Login com E-mail e Senha.
* Issue #3: Verificação de E-mail (código de 6 dígitos).
* Issue #4: Recuperação de senha.

**Épico 2: Navegação e Catálogo**
* Issue #5: Página Inicial (Dashboard do paciente com atalhos e ofertas).
* Issue #6: Busca e visualização do Catálogo de Produtos.
* Issue #7: Filtro de produtos por categoria (Remédios, Higiene, Vitaminas, etc.).

**Épico 3: Compra e Upload de Receita**
* Issue #8: Carrinho de Compras (cálculo de subtotal, taxas e descontos).
* Issue #9: Upload de Receita Médica (obrigatório para medicamentos controlados).
* Issue #10: Finalizar Pedido (Checkout com opções de entrega, endereço e pagamento via Cartão/Pix).

**Épico 4: Gestão do Cliente**
* Issue #11: Meus Pedidos (Histórico e rastreamento de entregas).
* Issue #12: Suporte (Visualizar nota fiscal e contatar atendimento).

**Épico 5: Painel Administrativo**
* Issue #13: Dashboard de Estoque e Vendas (Visão geral de faturamento e alertas de baixo estoque).

### 2. Definir a Primeira Sprint (Sprint Backlog)
A primeira Sprint deve focar em entregar o valor mais básico para o usuário poder usar o app: criar a conta, entrar no sistema e ver a página inicial.

No GitHub, criaríamos um Milestone chamado "Sprint 1 (Duração: 2 semanas)" e adicionaríamos as seguintes Issues a ele. A pontuação (Story Points) reflete a dificuldade de cada tarefa:
* Issue #1: Cadastro de usuário (5 Pontos)
* Issue #3: Verificação de E-mail (3 Pontos)
* Issue #2: Login com E-mail e Senha (3 Pontos)
* Issue #4: Recuperação de senha (2 Pontos)
* Issue #5: Página Inicial - Estrutura e layout (5 Pontos)
**Total da Sprint: 18 Pontos**

### 3. Simular a Execução da Sprint
Utilizando o GitHub Projects (quadro Kanban), as colunas seriam: To Do (A Fazer), In Progress (Em Progresso), Review (Revisão/Testes) e Done (Concluído).

Simulação de uma Sprint de 10 dias úteis:
* **Dias 1 e 2:** A equipe move as Issues #1 (Cadastro) e #3 (Verificação) para In Progress. Desenvolvimento focado na criação do banco de dados e conexão da API de e-mail.
* **Dia 3:** Issue #1 vai para Review. Issue #3 continua em desenvolvimento.
* **Dia 4:** Issue #1 é testada, aprovada e movida para Done.
* **Dia 5:** Issue #3 vai para Done. A equipe puxa a Issue #2 (Login) para In Progress.
* **Dia 6:** Issue #2 é concluída (Done). Issue #4 (Recuperação) vai para In Progress.
* **Dia 7:** Issue #4 é concluída (Done). A equipe puxa a maior tarefa restante, a Issue #5 (Página Inicial).
* **Dias 8 e 9:** Desenvolvimento total focado na interface da Issue #5.
* **Dia 10:** Issue #5 é testada, ajustada e movida para Done. A Sprint é finalizada com 100% de entrega.

### 4. Gerar um Burndown Chart

**Tabela de Acompanhamento (Pontos Restantes ao final do dia)**

| Dia | Pontos Ideais | Pontos Reais (Restantes) | O que foi entregue no dia |
|---|---|---|---|
| 0 | 18 | 18 | Início da Sprint |
| 1 | 16.2 | 18 | Nenhuma tarefa finalizada |
| 2 | 14.4 | 18 | Nenhuma tarefa finalizada |
| 3 | 12.6 | 18 | Nenhuma tarefa finalizada |
| 4 | 10.8 | 13 | Issue #1 concluída (-5 pts) |
| 5 | 9.0 | 10 | Issue #3 concluída (-3 pts) |
| 6 | 7.2 | 7 | Issue #2 concluída (-3 pts) |
| 7 | 5.4 | 5 | Issue #4 concluída (-2 pts) |
| 8 | 3.6 | 5 | Nenhuma tarefa finalizada |
| 9 | 1.8 | 5 | Nenhuma tarefa finalizada |
| 10 | 0 | 0 | Issue #5 concluída (-5 pts) |

**Representação Visual (Gráfico Burndown)**
```text
Pontos Restantes
18 | * (Dia 0)
   |  \
15 |   \
   |    \
13 |     * (Dia 4)
   |      \
10 |       * (Dia 5)
   |        \
 7 |         * (Dia 6)
   |          \
 5 |           *===*===* (Dias 7 a 9)
   |                    \
 0 |_____________________* (Dia 10)
     0 1 2 3 4 5 6 7 8 9 10  Dias da Sprint
```

## Etapa 5 - Teste

|   ID | Funcionalidade   | Cenário de Teste                              | Passos para Execução                                                                                                                   | Resultado Esperado                                                                                               | Status   |
|-----:|:-----------------|:----------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------|:---------|
|    1 | Cadastro         | Criar conta com dados válidos                 | 1. Preencher Nome, E-mail, Telefone e Senha.2. Clicar em "Sign Up".                                                                    | Conta criada com sucesso e usuário direcionado para a tela de verificação de e-mail.                             | False    |
|    2 | Cadastro         | Tentativa de cadastro com e-mail já existente | 1. Preencher os dados usando um e-mail já cadastrado.2. Clicar em "Sign Up".                                                           | O sistema deve exibir a mensagem de erro "E-mail já cadastrado".                                                 | False    |
|    3 | Verificação      | Inserir código correto                        | 1. Acessar a tela de verificação.2. Digitar o código de 6 dígitos recebido.3. Clicar em "Verify Account".                              | Conta verificada e usuário direcionado para a Página Inicial.                                                    | False    |
|    4 | Login            | Acesso com credenciais válidas                | 1. Inserir e-mail e senha corretos.2. Clicar em "Login".                                                                               | Acesso liberado e redirecionamento para a Página Inicial.                                                        | False    |
|    5 | Login            | Acesso com senha incorreta                    | 1. Inserir e-mail correto e senha errada.2. Clicar em "Login".                                                                         | O sistema deve impedir o acesso e exibir "E-mail ou senha incorretos".                                           | False    |
|    6 | Recuperação      | Solicitar link de recuperação                 | 1. Clicar em "Forgot Password".2. Inserir e-mail cadastrado.3. Clicar em "Send Reset Link".                                            | O sistema deve confirmar o envio e o usuário deve receber o link na caixa de entrada.                            | False    |
|    7 | Carrinho         | Adicionar produto ao carrinho                 | 1. Buscar um produto (ex: Amoxicilina).2. Clicar no ícone de adicionar ao carrinho.                                                    | O contador do carrinho no topo da tela deve atualizar para "1".                                                  | False    |
|    8 | Carrinho         | Cálculo de valores                            | 1. Adicionar produtos com preços diferentes.2. Acessar o Carrinho.                                                                     | O subtotal e o valor total devem corresponder à soma exata dos itens, somados ao frete e taxas.                  | False    |
|    9 | Receita          | Upload de receita médica                      | 1. Adicionar um remédio controlado ao carrinho.2. Na tela de Checkout, clicar em "Upload File".3. Selecionar um arquivo PDF ou imagem. | O arquivo deve ser anexado ao pedido com sucesso e o sistema deve permitir seguir para o pagamento.              | False    |
|   10 | Checkout         | Finalizar pedido (Pix)                        | 1. Preencher endereço.2. Selecionar método "Pix".3. Clicar em "Place Order".                                                           | Pedido registrado no sistema. O aplicativo deve gerar o código Pix e redirecionar para a tela de "Meus Pedidos". | False    |
