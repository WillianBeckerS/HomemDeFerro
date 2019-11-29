# Homem de Ferro

![GitHub Logo](/img1.bmp)
Format: ![Alt Text](url)

<br /><br />
Erika Burei Alves<br />
Guilherme Aristides Marcos<br />
Willian Becker de Souza<br /><br /><br />


Trabalho de Representação de Conhecimento em Lógica de Predicados.<br />
Disciplina: Introdução a Lógica para a Computação (CSD20).<br />
Professor: Adolfo Gustavo Serra Seca Neto<br />
(DAINF - UTFPR Curitiba).<br /><br /><br />

## 1.  Tema, Descrição do Tema e Integrantes da Equipe

<br />
O trabalho foi produzido pelos discentes Erika Burei Alves, Guilherme Aristides Marcos e Willian Becker de Souza a respeito dos três dos filmes produzidos pela Marvel que retratam como foco a história de Tony Stark, o Homem de Ferro. Logo, o trabalho tem como objetivo abordar características dos personagens e do filme em si, observando-as e analisando-as no quesito da Lógica de Predicados.

<br />

## 2.  Frases e Fórmulas

### 2.1 Propriedades de “objetos”
<br />

Frase | Monge de Ferro é um vilão.
------------ | -------------
Fórmula | Vilão (“Monge de Ferro”)
Definições de predicados/funções | Vilão (X): X é vilão.

<br />

Frase | Tony é um gênio.
------------ | -------------
Fórmula | Gênio (“Tony”)
Definições de predicados/funções | Gênio (X): X é um gênio.

<br />

Frase | Homem de Ferro é um herói.
------------ | -------------
Fórmula | Herói (“Homem de Ferro”)
Definições de predicados/funções | Herói (X): X é herói.

<br />
<br />

### 2.2 Relações entre “objetos”
<br />

Frase | Monge de Ferro e Homem de Ferro são inimigos.
------------ | -------------
Fórmula | Inimigos (“Monge de Ferro”, “Homem de Ferro”)
Definições de predicados/funções | Inimigos (X, Y): X e Y são inimigos.

<br />

Frase | Pepper é namorada do Homem de Ferro.
------------ | -------------
Fórmula | Namora (X, Y): X e Y namoram
Definições de predicados/funções | Namora (“Pepper”, “Homem de Ferro”).

<br />

Frase | Máquina de Combate e Homem de Ferro são amigos.
------------ | -------------
Fórmula | Amigos (“Máquina de Combate”, “Homem de Ferro”)
Definições de predicados/funções | Amigos (X, Y): X e Y são amigos.

<br />
<br />

### 2.3 Negações
<br />

Frase | Rhodes não é um gênio e não é mais inteligente que Tony Stark.
------------ | -------------
Fórmula |  ¬Gênio(“Rhodes”)Λ¬(Inteligente("Tony Stark", "Rhodes")="Rhodes")
Definições de predicados/funções | Inteligente(X, Y): retorna o mais inteligente entre x e y.

<br />

Frase | Monge de Ferro e Homem de Ferro não são amigos.
------------ | -------------
Fórmula | ¬Amigos (“Monge de Ferro”, Homem de Ferro”)
Definições de predicados/funções |

<br />
<br />

### 2.4 Conjunções
<br />

Frase | Tony é um gênio e construiu uma armadura.
------------ | -------------
Fórmula |  Gênio (“Tony”) Λ Construiu (“Tony”, “Armadura”)
Definições de predicados/funções | Construiu (X, Y): X construiu Y.

<br />

Frase | Pepper não é uma heroína e conhece Homem de Ferro.
------------ | -------------
Fórmula | ¬Herói (“Pepper”) Λ Conhece (“Pepper”, “Homem de Ferro”)
Definições de predicados/funções | Conhece (X, Y): X conhece Y

<br />
<br />

### 2.5 Disjunções
<br />

Frase | Tony é mais novo ou mais velho que Pepper.
------------ | -------------
Fórmula | Idade (“Tony”) < Idade (“Pepper”) ∨ Idade (“Tony”) > Idade (“Pepper”)
Definições de predicados/funções | Idade (X): Retorna idade de X

<br />

Frase | Homem de Ferro é mais poderoso do que o Monge de Ferro ou é mais poderoso que o Máquina de combate.
------------ | -------------
Fórmula | Poder (“Homem de Ferro”) > Poder (“Monge de Ferro”) ∨ Poder (“Homem de Ferro”) > Poder (“Máquina de Combate”)
Definições de predicados/funções | Poder (X): Retorna a nível de poder de X.

<br />
<br />

### 2.6 Implicações
<br />

Frase | Se o Tony Stark é um herói, então Tony não é o vilão.
------------ | -------------
Fórmula |  Herói (“Tony”) → ¬Vilão (“Tony”)
Definições de predicados/funções |

<br />

Frase | Se o Homem de Ferro vencer o Monge de Ferro, então o Monge de Ferro perde.
------------ | -------------
Fórmula | Vence (“Homem de Ferro”) → ¬Vence (“Monge de Ferro”)
Definições de predicados/funções | Vence (X): X vence a batalha.

<br />
<br />

### 2.7 Generalizações Universais

<br />

Frase | Todo herói salva e ajuda alguém.
------------ | -------------
Fórmula |  ∃y Ɐx ((Herói (x) → Salva (x, y) ) Λ (Ajuda (x, y))
Definições de predicados/funções | Salva (X, Y): X salva Y. <br /> Ajuda(X, Y): X ajuda Y.

<br />

Frase | Todas as armaduras construidas por tony stark são muito tecnologicas e possuem armas.
------------ | -------------
Fórmula | Ɐx(Construiu (“Tony Stark”, x) → (Tecnologica(x) Λ Possui(x, "armas"))
Definições de predicados/funções | Tecnologica(x): x é muito tecnologica <br /> Possui(X, Y): x possui y

<br />

Frase | Todas as armas do homem de ferro são mais poderosas do que armas comuns.
------------ | -------------
Fórmula | ⱯxⱯz((Arma(x, "Homem de Ferro")->(poder(x)>poder(z)))
Definições de predicados/funções | Arma(x, y): x é arma de y

<br />

Frase | Todas as armaduras construidas por Tony Stark são muito tecnologicas e possuem armas.
------------ | -------------
Fórmula | Ɐx(Construiu (“Tony Stark”, x) → (Tecnologica(x) Λ Possui(x, "armas"))
Definições de predicados/funções | Tecnologica(x): x é muito tecnologica <br /> Possui(X, Y): x possui y

<br />

Frase | Todos as armaduras do homem de ferro são mais caras do que qualquer carro popular
------------ | -------------
Fórmula | ⱯyⱯx(Armadura(x)→(Preço(Armadura(x)) > Preço(CarroPopular(y)))
Definições de predicados/funções | Preço(X): retorna o preço de X <br /> CarroPopular(X): X é um carro popular <br /> Armadura(X): X é uma armadura do homem de ferro

<br />
<br />
	
### 2.8 Generalizações Existenciais

<br />

Frase | Há pelo menos alguém que foi derrotado pelo Homem de Ferro e isto em menos de 30 segundos.
------------ | -------------
Fórmula |  ∃x((Derrotado(X) = "Homem de Ferro") Λ TempoDerrota(X) < 30)
Definições de predicados/funções | Derrotado (X): Retorna quem derrotou X.<br /> TempoDerrota(X): Retorna em quantos segundos X foi derrotado.

<br />

Frase | Há pelo menos alguém que não é amigo do Homem de Ferro e conhece o Homem de Ferro.
------------ | -------------
Fórmula | ∃X (¬Amigo(“Homem de Ferro”, X) Λ Conhece(X, “Homem de Ferro”))
Definições de predicados/funções |

<br />

Frase | Há pelo menos alguém que batalhou ou ajudou o Homem de Ferro e é menos poderoso que ele.
------------ | -------------
Fórmula | ∃X (Batalhou (X, “Homem de Ferro”) ∨ Ajuda (X, “Homem de Ferro”) Λ Poder (X) < Poder (“Homem de Ferro”)
Definições de predicados/funções | Batalhou (X, Y): X batalhou com Y.

<br />

## 3. Assinatura

∑=[R1, R2, R3, C, F1, F2, V]
R1={Herói, Gênio, Vilão, Vence, Tecnológica, CarroPopular, Armadura}
R2={Inimigos, Namora, Amigos, Conhece, Construiu, Salva, Ajuda, Possui, Batalhou, Arma}
C={“Homem de Ferro”,  “Pepper”,  “Tony Stark”,  “Maquina de Combate”,  “Monge de Ferro”,  “Rhodes”,  “Armadura”,  “Armas”}
F1={Idade, Poder, Preço, TempoDerrota, Derrotado}
F2={Inteligente}
V={x, y, z}

<br />

## 4. Modelos
### 4.1 Exemplo de modelo que satisfaz todas as fórmulas(M1)

1 . Universo de Valores Concretos

A={vc1, vc2, vc3, vc4, vc5, vc6, vc7, vc8, vc9, vc10, vc11, vc12, vc13}

2. Constantes
“Homem de Ferro”M1 = vc1
29M1 = vc2
“Pepper”M1 = vc3
31M1 = vc4
“Tony Stark”M1 = vc5
8000M1 = vc6
“Maquina de Combate”M1 = vc7
“Monge de Ferro”M1 = vc8
“Armadura”M1 = vc9
“Rhodes”M1 = vc10
“Armas”M1 = vc11

<br />

3. Funções
IdadeM1 (vc5) = vc2
IdadeM1 (vc3) = vc1
IdadeM1 (...) = vc1
PoderM1 (vc1) = vc6 
PoderM1 (vc8) = vc2
PoderM1 (vc7) = vc4
PoderM1 (...) = vc2
PoderM1(...) = vc2
PreçoM1 (vc9) = vc6

PreçoM1 (...) = vc2    carropop

TempoDerrotaM1 (vc) = vc1
TempoDerrotaM1 (vc2) = vc6
GostarM1 (vc6) = vc2
GostarM1 (...) = vc12
PropriedadeM1 (vc1, vc2) = vc5
PropriedadeM1 (...,...) = v

### 4.2 Exemplo de modelo que não satisfaz alguma das fórmulas(M2)
