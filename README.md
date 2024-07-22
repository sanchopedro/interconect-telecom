# Projeto Interconect Telecom - Análise e Previsão de Churn de Clientes

![Telecom image](./image/telecom.png)

## Índice

1. [Como usar](#1-como-usar)
2. [Sobre o projeto](#2-sobre-o-projeto)
    - [Serviços da Interconnect](#serviços-da-interconnect)
    - [Descrição dos Dados](#descrição-dos-dados)
    - [Esclarecimentos para conclusão do projeto final](#esclarecimentos-para-conclusão-do-projeto-final)
3. [Etapas do Projeto](#etapas-do-projeto)

## 1. Como usar

1. Instale todas as dependências do projeto rodando no terminal o comando:

    ```bash
    pip install -r requirements.txt
    ```

2. Consulte o arquivo [Planejamento.md](Planejamento.md) para ver os passos utilizados na conclusão do projeto Interconect Telecom.
3. O arquivo [interconnect-telecom.ipynb](interconnect-telecom.ipynb) contém os códigos utilizados para a conclusão do projeto.
4. Os datasets do projeto podem ser encontrados na pasta [datasets](./datasets/).

## 2. Sobre o projeto

A operadora de comunicações Interconnect deseja prever a rotatividade de seus clientes. Identificar clientes que planejam trocar de operadora permitirá oferecer-lhes códigos promocionais e planos especiais para retê-los. A equipe de marketing coletou dados pessoais, informações de planos e contratos dos clientes.

### Serviços da Interconnect

A Interconnect oferece principalmente dois tipos de serviços:

1. **Telefonia fixa:** O telefone pode ser conectado a várias linhas ao mesmo tempo.
2. **Internet:** A rede pode ser estabelecida através de DSL (*digital subscriber line*) ou cabo de fibra óptica.

Outros serviços incluem:

- **Segurança na Internet:** Software de antivírus (*DeviceProtection*) e bloqueador de sites maliciosos (*OnlineSecurity*).
- **Suporte técnico:** Linha dedicada de suporte técnico (*TechSupport*).
- **Armazenamento na nuvem:** Armazenamento de arquivos e backup de dados (*OnlineBackup*).
- **Streaming:** Streaming de TV (*StreamingTV*) e filmes (*StreamingMovies*).

Os clientes podem optar por pagamento mensal ou contrato de 1 ou 2 anos, com vários métodos de pagamento e fatura eletrônica.

### Descrição dos Dados

Os dados consistem de arquivos de diferentes fontes:

- `contract.csv` — informação contratual;
- `personal.csv` — dados pessoais do cliente;
- `internet.csv` — informação sobre serviços de Internet;
- `phone.csv` — informação sobre serviços de telefonia.

Em cada arquivo, a coluna `customerID` contém um código único para cada cliente. A informação contratual é válida a partir de 1 de fevereiro de 2020.

Os dados estão localizados na pasta `/datasets/final_provider/`.

### Esclarecimentos para conclusão do projeto final

**Característica objetivo:** a coluna `'EndDate'` é igual a `'No'`.

**Métrica primária:** AUC-ROC.

**Métrica adicional:** Acurácia.

**Critérios de avaliação:**

- AUC-ROC < 0.75 — 0 PPE
- 0.75 ≤ AUC-ROC < 0.81 — 4 PPE
- 0.81 ≤ AUC-ROC < 0.85 — 4.5 PPE
- 0.85 ≤ AUC-ROC < 0.87 — 5 PPE
- 0.87 ≤ AUC-ROC < 0.88 — 5.5 PPE
- AUC-ROC ≥ 0.88 — 6 PPE

## Etapas do Projeto

1. **Elaborar um plano de trabalho**
2. **Investigar a tarefa**
3. **Desenvolver um modelo**
4. **Preparar o relatório**

Este projeto visa criar um modelo preditivo eficaz para identificar a rotatividade de clientes, ajudando a Interconnect a implementar estratégias de retenção de clientes de forma proativa.
