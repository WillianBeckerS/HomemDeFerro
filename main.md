# Homem de Ferro

<br />

![GitHub Logo](/img1.bmp)

<br /> <br />
Erika Burei Alves<br />
Guilherme Aristides Marcos<br />
Willian Becker de Souza<br /><br /><br />

Trabalho de Representação de Conhecimento em Lógica de Predicados.<br />
Disciplina: Introdução a Lógica para a Computação (CSD20).<br />
Professor: Adolfo Gustavo Serra Seca Neto<br />
(DAINF - UTFPR Curitiba).<br /><br />

## 1.  Tema, Descrição do Tema e Integrantes da Equipe

<br />

O trabalho foi produzido pelos discentes Erika Burei Alves, Guilherme Aristides Marcos e Willian Becker de Souza a respeito dos três dos filmes produzidos pela Marvel que retratam a história de Tony Stark, o Homem de Ferro. Logo, o trabalho tem como objetivo abordar características dos personagens e do filme em si, analisando-as na ótica da Lógica de Predicados.

<br />

## 2.  Frases e Fórmulas

### 2.1 Propriedades de “objetos”
<br />

Frase | Monge de Ferro é um vilão.
------------ | -------------
Fórmula | Vilão(“Monge de Ferro”)
Definições de predicados/funções | Vilão(X): X é um vilão.

<br />

Frase | Tony Stark é um gênio.
------------ | -------------
Fórmula | Gênio(“Tony Stark”)
Definições de predicados/funções | Gênio(X): X é um gênio.

<br />

Frase | Homem de Ferro é um herói.
------------ | -------------
Fórmula | Herói(“Homem de Ferro”)
Definições de predicados/funções | Herói(X): X é um herói.

<br />

### 2.2 Relações entre “objetos”
<br />

Frase | Monge de Ferro e Homem de Ferro são inimigos.
------------ | -------------
Fórmula | Inimigos(“Monge de Ferro”, “Homem de Ferro”)
Definições de predicados/funções | Inimigos(X, Y): X e Y são inimigos.

<br />

Frase | Pepper é namorada do Tony Stark.
------------ | -------------
Fórmula | Namora(“Pepper”, “Tony Stark”).
Definições de predicados/funções | Namora(X, Y): X e Y namoram.

<br />

Frase | Máquina de Combate e Homem de Ferro são amigos.
------------ | -------------
Fórmula | Amigos(“Máquina de Combate”, “Homem de Ferro”)
Definições de predicados/funções | Amigos(X, Y): X e Y são amigos.

<br />

### 2.3 Negações
<br />

Frase | Rhodes não é um gênio e não é mais inteligente que Tony Stark.
------------ | -------------
Fórmula |  ¬Gênio(“Rhodes”)Λ¬(Inteligente("Tony Stark", "Rhodes")="Rhodes")
Definições de predicados/funções | Inteligente(X, Y): retorna o mais inteligente entre X e Y.

<br />

Frase | Monge de Ferro e Homem de Ferro não são amigos.
------------ | -------------
Fórmula | ¬Amigos(“Monge de Ferro”, Homem de Ferro”)
Definições de predicados/funções |

<br />

### 2.4 Conjunções
<br />

Frase | Tony Stark é um gênio e construiu uma armadura.
------------ | -------------
Fórmula |  Gênio(“Tony Stark”) Λ Construiu(“Tony”, “Armadura”)
Definições de predicados/funções | Construiu(X, Y): X construiu Y.

<br />

Frase | Pepper não é uma heroína e conhece Homem de Ferro.
------------ | -------------
Fórmula | ¬Herói(“Pepper”) Λ Conhece(“Pepper”, “Homem de Ferro”)
Definições de predicados/funções | Conhece(X, Y): X conhece Y.

<br />

### 2.5 Disjunções
<br />

Frase | Tony Stark é mais novo ou mais velho que Pepper.
------------ | -------------
Fórmula | Idade(“Tony Stark”) < Idade(“Pepper”) ∨ Idade(“Tony Stark”) > Idade(“Pepper”)
Definições de predicados/funções | Idade (X): Retorna a idade de X.

<br />

Frase | Homem de Ferro é mais poderoso do que o Monge de Ferro ou é mais poderoso que o Máquina de combate.
------------ | -------------
Fórmula | (Poder(“Homem de Ferro”) > Poder(“Monge de Ferro”)) ∨ (Poder(“Homem de Ferro”) > Poder(“Máquina de Combate”))
Definições de predicados/funções | Poder(X): Retorna o nível de poder de X.

<br />

### 2.6 Implicações
<br />

Frase | Se o Tony Stark é um herói, então Tony Stark não é o vilão.
------------ | -------------
Fórmula |  Herói(“Tony Stark”) → ¬Vilão(“Tony Stark”)
Definições de predicados/funções |

<br />

Frase | Se o Homem de Ferro vencer, então o Monge de Ferro não vence.
------------ | -------------
Fórmula | Vence(“Homem de Ferro”) → ¬Vence(“Monge de Ferro”)
Definições de predicados/funções | Vence(X): X vence a batalha.

<br />

### 2.7 Generalizações Universais

<br />

Frase | Todo herói salva e ajuda alguém.
------------ | -------------
Fórmula |  ∃yⱯx(Herói(x) → (Salva(x, y) Λ Ajuda(x, y)))
Definições de predicados/funções | Salva (X, Y): X salva Y. <br /> Ajuda(X, Y): X ajuda Y.

<br />

Frase | Todas as armaduras construidas por Tony Stark são muito tecnologicas e possuem armas.
------------ | -------------
Fórmula | Ɐx(Construiu(“Tony Stark”, Armadura(x)) → (Tecnologica(x) Λ Possui(x, "Armas")))
Definições de predicados/funções | Tecnologica(X): X é muito tecnologica <br /> Possui(X, Y): X possui Y. <br /> Armadura(X): X é uma armadura do homem de ferro.

<br />

Frase | Todas as armas do Homem de Ferro são mais poderosas do que armas comuns.
------------ | -------------
Fórmula | Ɐx((ArmaDeAlguem(x, "Homem de Ferro") → (Poder(x) > Poder("Armas Comuns")))
Definições de predicados/funções | ArmaDeAlguem(X, Y): X é arma de Y.

<br />

Frase | Todos as armaduras do Homem de Ferro são mais caras do que qualquer carro popular.
------------ | -------------
Fórmula | ⱯyⱯx((Armadura(x) Λ CarroPopular(y)) → (Preço(x) > Preço(y))
Definições de predicados/funções | Preço(X): retorna o preço de X <br /> CarroPopular(X): X é um carro popular

<br />
	
### 2.8 Generalizações Existenciais

<br />

Frase | Há pelo menos alguém que foi derrotado pelo Homem de Ferro e isto em menos de 30 segundos.
------------ | -------------
Fórmula |  ∃z((Derrotado(z) = "Homem de Ferro") Λ (TempoDerrota(z) < "30"))
Definições de predicados/funções | Derrotado(Z): Retorna quem derrotou Z. <br /> TempoDerrota(Z): Retorna em quantos segundos Z foi derrotado.

<br />

Frase | Há pelo menos alguém que não é amigo do Homem de Ferro e conhece o Homem de Ferro.
------------ | -------------
Fórmula | ∃x(¬Amigo(“Homem de Ferro”, x) Λ Conhece(x, “Homem de Ferro”))
Definições de predicados/funções |

<br />

Frase | Há pelo menos alguém que batalhou ou ajudou o Homem de Ferro e é menos poderoso que ele.
------------ | -------------
Fórmula | ∃x((Batalhou(x, “Homem de Ferro”) ∨ Ajuda(x, “Homem de Ferro”)) Λ (Poder(x) < Poder(“Homem de Ferro”)))
Definições de predicados/funções | Batalhou(X, Y): X batalhou com Y.

<br />

## 3. Assinatura

<br />

∑=[R1, R2, R3, C, F1, F2, V] <br />
R1={Herói, Gênio, Vilão, Vence, Tecnológica, CarroPopular, Armadura} <br />
R2={Inimigos, Namora, Amigos, Conhece, Construiu, Salva, Ajuda, Possui, Batalhou, ArmaDeAlguem} <br />
C={“Homem de Ferro”,  “Pepper”,  “Tony Stark”,  “Maquina de Combate”,  “Monge de Ferro”,  “Rhodes”,  “Armadura”,  “Armas”, "Celta"} <br />
F1={Idade, Poder, Preço, TempoDerrota, Derrotado} <br />
F2={Inteligente} <br />
V={x, y, z} <br />

<br />

## 4. Modelos
### 4.1 Exemplo de modelo que satisfaz todas as fórmulas(M1)

<br />

1 . Universo de Valores Concretos <br />

A = {vc1, vc2, vc3, vc4, vc5, vc6, vc7, vc8, vc9, vc10, vc11, vc12, vc13}

<br />

2 . Constantes <br />

"Homem de Ferro"<sup>M1</sup> = vc1 <br />
"29"<sup>M1</sup> = vc2 <br />
"Pepper"<sup>M1</sup> = vc3 <br />
"31"<sup>M1</sup> = vc4 <br />
"Tony Stark"<sup>M1</sup> = vc5 <br />
"8000"<sup>M1</sup> = vc6 <br />
"Maquina de Combate"<sup>M1</sup> = vc7 <br />
"Monge de Ferro"<sup>M1</sup> = vc8 <br />
"Armadura"<sup>6M1</sup> = vc9 <br />
"Rhodes"<sup>M1</sup> = vc10 <br />
"Armas"<sup>M1</sup> = vc11 <br />
"Armas Comuns"<sup>M1</sup> = vc12 <br />
"Celta"<sup>M1</sup> = vc13 <br />

<br />

3 . Predicados <br />

Herói<sup>M1</sup> = {vc1, vc5} <br />
Gênio<sup>M1</sup> = {vc5} <br />
Vilão<sup>M1</sup> = {vc8} <br />
Vence<sup>M1</sup> = {vc1} <br />
Tecnológica<sup>M1</sup> = {vc9} <br />
Armadura<sup>M1</sup> = {vc9} <br />
CarroPopular<sup>M1</sup> = {vc13} <br />
Inimigos<sup>M1</sup> = {(vc1, vc8)} <br />
Namora<sup>M1</sup> = {(vc3, vc5)} <br />
Amigos<sup>M1</sup> = {(vc1, vc7)} <br />
Salva<sup>M1</sup> = {(vc1, vc3), (vc5, vc3)} <br />
Construiu<sup>M1</sup> = {(vc5, vc9)} <br />
Conhece<sup>M1</sup> = {(vc3, vc1), (vc8, vc1)} <br />
Ajuda<sup>M1</sup>= {(vc1, vc3), (vc5, vc3)} <br />
Possui<sup>M1</sup> = {(vc9, vc11)} <br />
Batalhou<sup>M1</sup> = {(vc1, vc8)} <br />
ArmaDeAlguem<sup>M1</sup> = {(vc11, vc1)} <br />

<br />

4 . Funções <br />

Idade<sup>M1</sup> = A → A <br />
Idade<sup>M1</sup> (vc5) = vc2 <br />
Idade<sup>M1</sup> (vc3) = vc4 <br />
Idade<sup>M1</sup> (...) = vc4 <br />
Poder<sup>M1</sup> = A → A <br />
Poder<sup>M1</sup> (vc1) = vc6 <br />
Poder<sup>M1</sup> (vc8) = vc2 <br />
Poder<sup>M1</sup> (vc7) = vc4 <br />
Poder<sup>M1</sup> (vc12) = vc2 <br />
Poder<sup>M1</sup> (vc9) = vc6 <br />
Poder<sup>M1</sup>(...) = vc2 <br />
Preço<sup>M1</sup> = A → A <br />
Preço<sup>M1</sup> (vc9) = vc6 <br />
Preço<sup>M1</sup> (vc13) = vc2 <br />
Preço<sup>M1</sup> (...) = vc2 <br />
Derrotado<sup>M1</sup> = A → A <br />
Derrotado<sup>M1</sup> (vc8) = vc1 <br />
Derrotado<sup>M1</sup> (...) = vc2 <br />
TempoDerrota<sup>M1</sup> = A → A <br />
TempoDerrota<sup>M1</sup> (vc8) = vc2 <br />
TempoDerrota<sup>M1</sup> (...) = vc6 <br />
Inteligente<sup>M1</sup> = AxA → A <br />
Inteligente<sup>M1</sup> (vc5, vc10) = vc5 <br />
Inteligente<sup>M1</sup> (...,...) = vc5 <br />

<br />

<br />

### 4.2 Exemplo de modelo que não satisfaz alguma das fórmulas(M2)
<br />

1 . Universo de Valores Concretos <br />

A = {vc1, vc2, vc3, vc4, vc5, vc6, vc7, vc8, vc9, vc10, vc11, vc12, vc13}

<br />

2 . Constantes <br />

"Homem de Ferro"<sup>M2</sup> = vc1 <br />
"29"<sup>M2</sup> = vc2 <br />
"Pepper"<sup>M2</sup> = vc3 <br />
"31"<sup>M2</sup> = vc4 <br />
"Tony Stark"<sup>M2</sup> = vc5 <br />
"8000"<sup>M2</sup> = vc6 <br />
"Maquina de Combate"<sup>M2</sup> = vc7 <br />
"Monge de Ferro"<sup>M2</sup> = vc8 <br />
"Armadura"<sup>6M2</sup> = vc9 <br />
"Rhodes"<sup>M2</sup> = vc10 <br />
"Armas"<sup>M2</sup> = vc11 <br />
"Armas Comuns"<sup>M2</sup> = vc12 <br />
"Celta"<sup>M2</sup> = vc13 <br />

<br />

3 . Predicados <br />

Herói<sup>M2</sup> = {vc5} <br />
Gênio<sup>M2</sup> = {} <br />
Vilão<sup>M2</sup> = {vc5} <br />
Vence<sup>M2</sup> = {vc1} <br />
Tecnológica<sup>M2</sup> = {vc9} <br />
Armadura<sup>M2</sup> = {vc9} <br />
CarroPopular<sup>M2</sup> = {vc13} <br />
Inimigos<sup>M2</sup> = {(vc1, vc8)} <br />
Namora<sup>M2</sup> = {(vc3, vc5)} <br />
Amigos<sup>M2</sup> = {(vc1, vc7)} <br />
Salva<sup>M2</sup> = {(vc1, vc3), (vc5, vc3)} <br />
Construiu<sup>M2</sup> = {(vc5, vc9)} <br />
Conhece<sup>M2</sup> = {(vc3, vc1), (vc8, vc1)} <br />
Ajuda<sup>M2</sup>= {(vc1, vc3), (vc5, vc3)} <br />
Possui<sup>M2</sup> = {(vc9, vc11)} <br />
Batalhou<sup>M2</sup> = {(vc1, vc8)} <br />
ArmaDeAlguem<sup>M2</sup> = {(vc11, vc1)} <br />

<br />

4 . Funções <br />
Idade<sup>M2</sup> = A → A <br />
Idade<sup>M2</sup> (vc5) = vc2 <br />
Idade<sup>M2</sup> (vc3) = vc4 <br />
Idade<sup>M2</sup> (...) = vc4 <br />
Poder<sup>M2</sup> = A → A <br />
Poder<sup>M2</sup> (vc1) = vc6 <br />
Poder<sup>M2</sup> (vc8) = vc2 <br />
Poder<sup>M2</sup> (vc7) = vc4 <br />
Poder<sup>M2</sup> (vc12) = vc2 <br />
Poder<sup>M2</sup> (vc9) = vc6 <br />
Poder<sup>M2</sup>(...) = vc2 <br />
Preço<sup>M2</sup> = A → A <br />
Preço<sup>M2</sup> (vc9) = vc6 <br />
Preço<sup>M2</sup> (vc13) = vc2 <br />
Preço<sup>M2</sup> (...) = vc2 <br />
Derrotado<sup>M2</sup> = A → A <br />
Derrotado<sup>M2</sup> (vc8) = vc1 <br />
Derrotado<sup>M2</sup> (...) = vc2 <br />
TempoDerrota<sup>M2</sup> = A → A <br />
TempoDerrota<sup>M2</sup> (vc8) = vc4 <br />
TempoDerrota<sup>M2</sup> (...) = vc6 <br />
Inteligente<sup>M2</sup> = AxA → A <br />
Inteligente<sup>M2</sup> (vc5, vc10) = vc5 <br />
Inteligente<sup>M2</sup> (...,...) = vc5 <br />

<br />

<br />
