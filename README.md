# Sistema Bancário Simples

Este projeto é um sistema bancário simples em Java utilizando OOP, que permite aos usuários realizar operações básicas, como depósitos, saques e transferências entre contas correntes e contas poupança.

## Funcionalidades

- **Depositar**: Permite depositar um valor especificado em uma conta.
- **Sacar**: Permite sacar um valor especificado de uma conta, desde que haja saldo suficiente.
- **Transferir**: Permite transferir um valor especificado de uma conta para outra, desde que haja saldo suficiente.
- **Ver Saldo**: Permite visualizar o saldo atual de uma conta.

## Estrutura do Projeto

O projeto é composto pelas seguintes classes:

### `Conta`

Classe abstrata que representa uma conta bancária genérica. Contém métodos para:

- `getNumero()`: Retorna o número da conta.
- `getSaldo()`: Retorna o saldo da conta.
- `depositar(double valor)`: Deposita um valor na conta.
- `sacar(double valor)`: Saca um valor da conta.
- `transferir(double valor, Conta destino)`: Transfere um valor para outra conta.

### `ContaCorrente` e `ContaPoupanca`

Classes que estendem `Conta` e representam tipos específicos de contas bancárias:

- `ContaCorrente`: Representa uma conta corrente.
- `ContaPoupanca`: Representa uma conta poupança.

### `Banco`

Classe principal que contém o método `main` e permite a interação do usuário com o sistema bancário via console. As operações disponíveis incluem:

- Depositar na Conta Corrente
- Depositar na Conta Poupança
- Sacar da Conta Corrente
- Sacar da Conta Poupança
- Transferir da Conta Corrente para Conta Poupança
- Transferir da Conta Poupança para Conta Corrente
- Ver Saldo da Conta Corrente
- Ver Saldo da Conta Poupança
- Sair

## Tecnologias Utilizadas

- **Java**: Linguagem de programação principal usada no projeto.

## Requisitos

- JDK 8 ou superior

## Executando o Projeto

1. Abra um terminal e navegue até o diretório do projeto.
2. Compile as classes Java:
    ```sh
    javac Banco.java
    ```
3. Execute a aplicação:
    ```sh
    java Banco
    ```
