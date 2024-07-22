# Projeto: Interconect Telecom

## 1. Como usar

- Primeiramente, instalar todas as dependências do projeto, rodando no terminal o `pip install -r requirements.txt`
- O arquivo [Planejamento.md](Planejamento.md) mostra os passos que foram utilizados para concluir o projeto Interconect Telecom
- O arquivo [interconnect-telecom.ipynb](interconnect-telecom.ipynb) mostra os códigos utilizados para a conclusão do projeto
- Os datasets do projeto podem ser encontrados na pasta [dataset](./datasets/)

## 2. Sobre o projeto

A operadora de comunicações Interconnect gostaria de ser capaz de predizer a rotatividade de seus clientes. Se for descoberto que um usuário está planejando trocar de operadora, a empresa oferecerá-lhe códigos promocionais e opções de plano especiais. A equipe de marketing da Interconnect coletou alguns dados pessoais da sua clientela, incluindo a informação sobre seus planos e contratos.

### Serviços da Interconnect

A Interconnect fornece principalmente dois tipos de serviços:

1. Telefonia fixa. O telefone pode ser conectado a várias linhas ao mesmo tempo.
2. Internet. A rede pode ser estabelecida através de uma linha telefônica (DSL, *digital subscriber line - linha digital de assinante*) ou através de um cabo de fibra óptica.

Alguns outros serviços fornecidos pela empresa incluem:

- Segurança na Internet: software de antivírus (*DeviceProtection* - proteção de dispositivos) e um bloqueador de sites maliciosos (*OnlineSecurity* - segurança online).
- Uma linha dedicada de suporte técnico (*TechSupport*).
- Armazenamento de arquivos na nuvem e backup de dados (*OnlineBackup*).
- Streaming de TV (*StreamingTV*) e um diretório de filmes (*StreamingMovies*).

Os clientes podem escolher entre fazer um pagamento mensal e assinar um contrato de 1 ou 2 anos. Eles podem usar vários métodos de pagamento e receber uma fatura eletrônica após a transação.

### Descrição dos Dados

Os dados consistem de arquivos obtidos de fontes diferentes:

- `contract.csv` — informação contratual;
- `personal.csv` — dados pessoais do cliente;
- `internet.csv` — informação sobre serviços de Internet;
- `phone.csv` — informação sobre serviços de telefonia.

Em cada arquivo, a coluna `customerID` contém um código unívoco atribuído a cada cliente. A informação contratual é válida a partir de 1 de fevereiro de 2020.

### Dados

Os dados também estão localizados na plataforma na pasta `/datasets/final_provider/`.

### Esclarecimentos para conclusão do projeto final

Característica objetivo: a coluna `'EndDate'` é igual a `'No'`.

1. Métrica primária: AUC-ROC.

2. Métrica adicional: Acurácia.

* **Critérios de avaliação:**

    - AUC-ROC < 0.75 — 0 PPE
    - 0.75 ≤ AUC-ROC < 0.81 — 4 PPE
    - 0.81 ≤ AUC-ROC < 0.85 — 4.5 PPE
    - 0.85 ≤ AUC-ROC < 0.87 — 5 PPE
    - 0.87 ≤ AUC-ROC < 0.88 — 5.5 PPE
    - AUC-ROC ≥ 0.88 — 6 PPE

#### Etapas do Projeto:

- Elaborar um plano de trabalho.
- Investigar a tarefa.
- Desenvolver um modelo.
- Preparar o relatório.

