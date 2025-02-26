# Diagramas E/R

## Algumas definições

- **Entidade**: "coisa" ou objeto.
- **Conjunto de entidades**: coleção de entidades semelhantes.
- **Atributo**: propriedade ou característica de um conjunto de entidades.
- **Geralmente**, todas as entidades de um conjunto tem as mesmas propriedades.

## Tipos de atributos

- Atributo são valores **simples**.
- Atributo **simples** ou **atômico** é indivisível.
- Atributo **composto** é um atributo que pode ser dividido em partes com significados diferentes.
- Atributo **derivado** é um atributo que pode ser obtido de outros atributos. Por isso não precisa ser armazenado. Idade não precisa ser armazenado, é apenas subtrari da data atual a data de nascimento.

## Relacionamentos

O bar vende cerveja. Uma forma de apresenta essas informações é:

|Bar             |Cerveja        |
|---             |---            |
|Bar do Zé       |Cerveja Skol   |
|Bar do Pequeno  |Cerveja Brahma |
|Bar do Joãozinho|Cerveja Devassa|

#### Relacionamento de muitos para muitos

Por exemplo, **muitos** bares vendem **muitas** cervejas. Bar do Zé vende cerveja Skol, Bardo Pequeno vende Brahma, Bar do Joãozinho vende Devassa...

#### Relacionamentos muitos pra um

**Muitos** bares tem **um** endereço.

#### Relacionamentos um pra um

**Uma** pessoa tem **um** CPF.

> Os relacionamentos **SEMPRE** são verbos. E ás vezes pode ser útil anexar um atributo a um relacionamento.

## Chaves

Uma chave é um conjunto de atributos para um conjunto de entidades, de modo que não há duas entidades neste conjunto que concordem com todos os atributos da chave.

- É permitido que duas entidades concorde com alguns, mas não todos, dos atributos-chave

> Em contexto de projeto, o atributo que se pretende utilizar como chave é denominada "candidato"

## Chaves multiatributo em diagramas E/R

Não se pode ter conjuntos de dados (chave multiatributo) iguais para uma entidade. Por exemplo:

- Um curso tem departamento, número, horário e sala. **Departamento** e **número** são chaves multi atributo.

|Departamento|Número |Horário|Sala|
|---         |---    |---    |--- |
|Sociais     |001    |16h    |B01 |
|Sociais     |002    |16h    |B02 |
|Exatas      |001    |14h    |A05 |
|~~Sociais~~ |~~001~~|13h    |A03 |

> O ultimo elemento está errado, pois repetiu o conjunto **departamento** e **número** (primeiro elemento).

## Técnicas de projeto

> **Faça sempre a pergunta**: esse atributo deveria estar nessa entidade?

- Evitar redundância: Dizer a mesma coisa de duas maneiras diferentes.
- Um conjunto de entidades deve ter pelo menos um atributo não-chave.
- Seja descritivo:
  - **Não** use siglas como noEmp, utilize nomeEmpresa.

## Exercícios
- [Exercício 1](https://excalidraw.com/#json=e59Zd6QwU6qyhiQlfqWnE,mwaIlnyyJKLR2QioPmpsLA)
- [Exercício 2](https://excalidraw.com/#json=GYujwRb-unNy-JCNoq8Ya,6igQw0b2g-khlZrDk4HwdA)