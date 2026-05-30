# Avaliação P2 - Linguagem de Programação - Prof. Bruno Zolotareff

## Nomes
- Raul Rodrigues Cnao
- Maria Eduarda Snatana de Souza

---

# Máquina de Café com POO

## Resposta da Pergunta

O software desenvolvido consiste em uma simulação de uma Máquina de Café com seis opções de bebidas, utilizando a linguagem Java e os conceitos da Programação Orientada a Objetos (POO). O sistema apresenta ao usuário um menu com diferentes sabores de café e, após a escolha, exibe a bebida selecionada e seu respectivo valor.

Para o desenvolvimento da aplicação foram utilizadas uma classe abstrata chamada **Drink**, uma classe concreta chamada **Cafe** e uma classe principal responsável pela execução do programa.

## Aplicação da Abstração

A abstração foi aplicada através da classe abstrata **Drink**. Essa classe representa uma bebida de forma genérica, contendo apenas as características essenciais que qualquer bebida deve possuir, como o sabor e o valor.

A utilização de uma classe abstrata permite criar um modelo base para futuras bebidas, evitando repetição de código e tornando o sistema mais organizado. Dessa forma, a classe Drink funciona como uma representação conceitual de uma bebida, sem a necessidade de ser instanciada diretamente.

## Aplicação do Encapsulamento

O encapsulamento foi utilizado para proteger os atributos da classe Drink. Os atributos **sabor** e **valor** foram declarados como privados, impedindo que sejam acessados diretamente por outras classes.

Para permitir o acesso controlado a esses dados, foram utilizados os métodos getters e setters. Dessa forma, os atributos ficam protegidos e somente podem ser modificados através dos métodos apropriados, garantindo maior segurança e organização do código.

Essa prática evita alterações indevidas nos dados e segue um dos princípios fundamentais da Programação Orientada a Objetos.

## Aplicação da Herança

A herança foi aplicada através da classe **Cafe**, que herda as características da classe abstrata **Drink**.

Ao utilizar a herança, a classe Cafe passa a possuir automaticamente os atributos e métodos definidos em Drink, podendo utilizá-los sem a necessidade de recriá-los.

Isso proporciona reutilização de código, facilita a manutenção do sistema e torna a aplicação mais organizada, uma vez que características comuns ficam concentradas na classe pai.

## Como Seria Aplicado o Polimorfismo

O polimorfismo não foi implementado diretamente no projeto atual, porém poderia ser utilizado caso fossem criadas novas classes de bebidas derivadas da classe Drink.

Por exemplo, poderiam existir as classes:

- Cafe
- Cappuccino
- ChocolateQuente
- CafeLatte

Todas herdando da classe Drink.

Nesse cenário, uma variável do tipo Drink poderia armazenar objetos de diferentes tipos de bebidas:

```java
Drink bebida = new Cappuccino();
```

ou

```java
Drink bebida = new CafeLatte();
```

Embora a variável seja do tipo Drink, o comportamento executado dependeria da classe concreta associada ao objeto.

O polimorfismo permite que diferentes objetos sejam tratados de maneira uniforme através da classe pai, aumentando a flexibilidade, a reutilização de código e facilitando futuras expansões do sistema.

## Conclusão

O projeto da Máquina de Café permitiu aplicar os principais conceitos da Programação Orientada a Objetos. A abstração foi utilizada através da classe abstrata Drink, o encapsulamento através da proteção dos atributos com getters e setters, e a herança através da classe Cafe que estende Drink.

Além disso, foi possível compreender como o polimorfismo poderia ser implementado futuramente para permitir a inclusão de novos tipos de bebidas sem a necessidade de alterar significativamente a estrutura do sistema, tornando a aplicação mais flexível e escalável.
---
**Disciplina:** Linguagem de Programação  
**Professor:** Bruno Zolotareff
