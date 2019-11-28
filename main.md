#Homem de Ferro

![GitHub Logo](/img1.bmp)
Format: ![Alt Text](url)

First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column


fsdfs<br />fwfwef


Frases e Fórmulas:

->Propriedades de “objetos”

-Frase: Monge de Ferro é um vilão.

-Fórmula: Vilão (“Monge de Ferro”)

- Definições de predicados/funções: Vilão (X): X é vilão.

-Frase: Homem de Ferro é um herói.

-Fórmula: Herói (“Homem de Ferro”)

- Definições de predicados/funções: Herói (X): X é herói.

-Frase: Tony é um gênio.

-Fórmula: Gênio (“Tony”)

- Definições de predicados/funções: Gênio (X): X é um gênio.

->Relações entre “objetos”

-Frase: Monge de Ferro e Homem de Ferro são inimigos.

-Fórmula: Inimigos (“Monge de Ferro”, “Homem de Ferro”)

- Definições de predicados/funções: Inimigos (X, Y): X e Y são inimigos.

-Frase: Pepper é namorada do Homem de Ferro.

-Fórmula: Namora (X, Y): X e Y namoram

- Definições de predicados/funções: Namora (“Pepper”, “Homem de Ferro”).

-Frase: Máquina de Combate e Homem de Ferro são amigos.

-Fórmulas: Amigos (“Máquina de Combate”, “Homem de Ferro”)

- Definições de predicados/funções: Amigos (X, Y): X e Y são amigos.

->Negações

-Frase: Rhodes não é um gênio.

-Fórmula: ¬Gênio (“Rhodes”)

-Frase: Monge de Ferro e Homem de Ferro não são amigos.

-Fórmula: ¬Amigos (“Monge de Ferro”, Homem de Ferro”)

->Conjunções

-Frase: Tony é um gênio e construiu uma armadura.

-Fórmula: Gênio (“Tony”) Λ Construiu (“Tony”, “Armadura”)

- Definições de predicados/funções: Construiu (X, Y): X construiu Y.

-Frase: Pepper não é uma heroína e conhece Homem de Ferro.

-Fórmula: ¬Herói (“Pepper”) Λ Conhece (“Pepper”, “Homem de Ferro”)

- Definições de predicados/funções: Conhece (X, Y): X conhece Y.

->Disjunções

-Frase: Tony é mais novo ou mais velho que Pepper.

-Fórmula: Idade (“Tony”) < Idade (“Pepper”) ∨ Idade (“Tony”) > Idade (“Pepper”)

-Definições de predicados/funções: Idade (X): Retorna idade de X.

-Frase: Homem de Ferro é mais poderoso do que o Monge de Ferro ou é mais poderoso que o Máquina de combate.

-Fórmula: Poder (“Homem de Ferro”) > Poder (“Monge de Ferro”) ∨ Poder (“Homem de Ferro”) > Poder (“Máquina de Combate”)

- Definições de predicados/funções: Poder (X): Retorna a nível de poder de X.

->Implicações

-Frase: Se o Tony Stark é um herói, então Tony não é o vilão.

-Fórmula: Herói (“Tony”) → ¬Vilão (“Tony”)

- Definições de predicados/funções:

-Frase: Se o Homem de Ferro vencer o Monge de Ferro, então o Monge de Ferro perde.

-Fórmula: Vence (“Homem de Ferro”) → ¬Vence (“Monge de Ferro”)

- Definições de predicados/funções: Vence (X): X vence a batalha.

->Generalizações Universais

-Frase: Todo herói salva e ajuda alguém.

-Fórmula: ∃Y Ɐ X ((Herói (X) → Salva (X, Y) ) Λ (Ajuda (X, Y))

- Definições de predicados/funções: Salva (X, Y): X salva Y.

***Pessoa (Y): Y é uma pessoa.

-Frase:

-Fórmula:

- Definições de predicados/funções:

-Frase:

-Fórmula:

- Definições de predicados/funções:

->Generalizações Existenciais

-Frase: Há pelo menos alguém que foi derrotado pelo Homem de Ferro e isto em menos de 30 segundos.

-Fórmula: ∃X (Derrotado (X) = Homem de Ferro) Λ TempoDerrota (X) < 30

- Definições de predicados/funções: Derrotado (X): Retorna quem derrotou X.

Tempo Derrota (X): Retorna em quantos segundos X foi derrotado.

-Frase: Há pelo menos alguém que não é amigo do Homem de Ferro e conhece o Homem de Ferro.

-Fórmula: ∃X (¬Amigo (“Homem de Ferro”, X) Λ Conhece (X, “Homem de Ferro”)

- Definições de predicados/funções:

-Frase: Há pelo menos alguém que batalhou ou ajudou o Homem de Ferro e é menos poderoso que ele.

-Fórmula: ∃X (Batalhou (X, “Homem de Ferro”) ∨ Ajudou (X, “Homem de Ferro”) Λ Poder (X) < Poder (“Homem de Ferro”)

- Definições de predicados/funções: Batalhou (X, Y): X batalhou com Y.

Ajudou (X, Y): X ajudou Y.
