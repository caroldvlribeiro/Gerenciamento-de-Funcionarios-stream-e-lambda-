# 👥 Gerenciador de Funcionários Java

<div align="center">

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square\&logo=openjdk\&logoColor=white)
![Stream API](https://img.shields.io/badge/Stream%20API-6C63FF?style=flat-square)
![Lambdas](https://img.shields.io/badge/Lambdas-2196F3?style=flat-square)
![POO](https://img.shields.io/badge/POO-FF9800?style=flat-square)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square)

**Sistema de gerenciamento e análise de dados de funcionários com Java Stream API**

[Sobre](#-sobre) • [Funcionalidades](#-funcionalidades) • [Estrutura](#-estrutura-do-projeto) • [Como Usar](#-como-usar) • [Tecnologias](#-tecnologias) • [Exemplos](#-exemplos-de-uso)

</div>

---

## 📖 Sobre

O Gerenciador de Funcionários é uma aplicação desenvolvida em Java para organizar e processar informações de colaboradores de diferentes departamentos de uma empresa.

O sistema utiliza a **Stream API** e Expressões Lambda para realizar consultas, aplicar reajustes salariais, ordenar funcionários e gerar informações sobre a folha de pagamento. A partir de uma lista de funcionários, é possível analisar salários, tempo de serviço e médias salariais por departamento.

A aplicação explora conceitos de Programação Orientada a Objetos e manipulação de coleções, com foco em operações funcionais aplicadas a objetos Java.

---

## ✨ Funcionalidades

* Cadastro e organização de funcionários em uma lista.
* Consulta de funcionários com salário superior a R$ 3.000.
* Aplicação de aumento de 5% para funcionários com mais de 10 anos de serviço.
* Ordenação dos funcionários pelo nome em ordem alfabética.
* Cálculo do total gasto com salários.
* Agrupamento de funcionários por departamento.
* Cálculo da média salarial de cada departamento.

---

## 📂 Estrutura do Projeto

```text
GerenciamentoDeFuncionario/
│
├── 📄 README.md
├── 📄 .gitignore
│
└── 📁 src/
    └── 📁 br/edu/fatecpg/gerenciamentodefuncionario/
        │
        ├── 📁 model/
        │   └── 🔹 Funcionario.java
        │
        └── 📁 controller/
            └── 🔹 ControllerFuncionario.java
```

### 📋 Descrição dos Componentes

#### **model/**

* **Funcionario.java** - Classe que representa os funcionários do sistema.

  * Atributos: `nome`, `departamento`, `salario` e `anosDeServico`.
  * Getters para acesso aos dados.
  * Método `toString()` para exibição dos objetos.

#### **controller/**

* **ControllerFuncionario.java** - Classe responsável pelo gerenciamento e processamento da lista de funcionários.

  * População da lista com colaboradores de diferentes departamentos.
  * Filtragem por salário utilizando `filter`.
  * Aplicação de aumento salarial com `map`.
  * Ordenação alfabética com `sorted`.
  * Cálculo de totais com `reduce`.
  * Agrupamento e cálculo de médias com `groupingBy` e `averagingDouble`.

---

## 🚀 Como Usar

### 1️⃣ Pré-requisitos

* Java JDK 11 ou superior.
* IntelliJ IDEA, Eclipse ou outra IDE compatível.
* Git (opcional, para clonar o repositório).

### 2️⃣ Clonar o repositório

```bash
git clone https://github.com/caroldvlribeiro/GerenciamentoDeFuncionario.git
```

### 3️⃣ Executar o projeto

1. Abra o projeto na IDE.
2. Localize a classe principal `Main.java`.
3. Execute o método `main()` para iniciar a aplicação.
4. Acompanhe os resultados das operações no console.

---

## 📋 Exemplos de Uso

### Funcionários cadastrados

```text
Funcionario{nome='Ana', departamento='TI', salario=4500.0, anosDeServico=12}
Funcionario{nome='Carlos', departamento='RH', salario=2800.0, anosDeServico=5}
Funcionario{nome='Beatriz', departamento='Financeiro', salario=3500.0, anosDeServico=15}
```

### Filtragem por salário

Seleciona os funcionários que possuem salário superior a R$ 3.000.

### Aplicação de aumento salarial

Os funcionários com mais de 10 anos de serviço recebem um aumento de 5% no salário, considerando a abordagem implementada no sistema.

### Ordenação por nome

Os funcionários são organizados em ordem alfabética utilizando `sorted()` e `Comparator.comparing()`.

### Cálculo do total de salários

A operação `reduce()` soma os salários dos funcionários cadastrados, apresentando o total da folha de pagamento.

### Média salarial por departamento

O agrupamento permite analisar o salário médio dos funcionários de cada departamento.

```text
MÉDIA SALARIAL POR DEPARTAMENTO

TI: R$ 4.500,00
RH: R$ 2.800,00
Financeiro: R$ 3.500,00
```

*Os valores apresentados são ilustrativos.*

---

## 🛠 Tecnologias

| Tecnologia                          | Descrição                         |
| ----------------------------------- | --------------------------------- |
| **Java**                            | Linguagem de programação          |
| **Stream API**                      | Processamento de coleções         |
| **Expressões Lambda**               | Operações funcionais              |
| **ArrayList**                       | Armazenamento dos funcionários    |
| **Collections**                     | Manipulação de listas             |
| **Programação Orientada a Objetos** | Organização das classes e objetos |

---

## 🔧 Operações da Stream API

| Operação            | Aplicação no projeto                      |
| ------------------- | ----------------------------------------- |
| `filter()`          | Seleciona funcionários por salário        |
| `map()`             | Aplica aumento de 5% aos salários         |
| `sorted()`          | Ordena funcionários pelo nome             |
| `reduce()`          | Calcula o total dos salários              |
| `groupingBy()`      | Agrupa funcionários por departamento      |
| `averagingDouble()` | Calcula a média salarial por departamento |
| `forEach()`         | Exibe os resultados no console            |

---

## 💡 Conceitos Aplicados

✅ Manipulação de listas de objetos
✅ Filtragem e transformação de dados
✅ Ordenação de funcionários
✅ Operações de redução
✅ Agrupamento por departamento
✅ Cálculo de médias salariais
✅ Expressões Lambda
✅ Programação Orientada a Objetos
✅ Uso da Stream API em Java

---

## 👩‍💻 Autor

**Carolina Ribeiro**

* 🔗 GitHub: [@caroldvlribeiro](https://github.com/caroldvlribeiro)
* 💼 FATEC Praia Grande - DSM

---

<div align="center">

**Desenvolvido com ☕ Java e ❤️ para FATEC Praia Grande**

*DSM - Desenvolvimento de Software Multiplataforma*

</div>
