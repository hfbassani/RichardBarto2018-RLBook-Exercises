### *Exercise 2.3:*

**In the comparison shown in Figure 2.2, which method will perform best in the long run in terms of cumupative reward and probability of selecting the best acton? How much better will it be? Express your answer quantitatively.**

---
Resposta 1:

```
O método ε = 0.01 performa melhor ao longo do tempo, mesmo ε = 0.1 convergindo mais rápido, porém conforme o número de tentantivas cresce, ε = 0.01 tem desempenho superior. Isso ocorre porque, ambos convergem para um valor de recompensa ótimo quando o número de tentantivas tende ao infinito. Porém, como ε = 0.01 utiliza ações gulosas (greedy) em cerca de 99% das vezes, enquanto que o outro por 90%, serão escolhidas mais vezes a ação que maximize a recompensa, ou seja, o fator aleatório, será menor para ε = 0.01.

Simulando quantitativamente o q*(a), ou seja, a recompensa ótima para cada ação, temos:

    Para ε = 0.01 --> 0.99 * 1.5 = 1.485
    Para ε = 0.1 --> 0.9 * 1.5 = 1.35

Percebe-se que com ε = 0.01, é esperado uma recomensa maior.

Ps.: Levei em consideração que a recompensa esperada para 1 - ε, ações aleatórias é 0, visto que, são desconhecidas e aleatórias.
```

---
Resposta 2:

```
Quando o "e-greedy" é médio o algoritmo pode escolher uma maquina muito ruim e por azar a recompensa dela for muito alta, dessa forma iria demorar mais para o algoritmo perceber que aquela maquina é de fato ruim. Com "e-greedy" é muito pequeno acontece algo pior pois com o raciocinio de sempre escolher a melhor ação o algoritmo pode achar uma maquina que lhe dar 3 como recompensa enquanto que a maioria das outras lhe dão -1. Porem pode existir uma maquina que lhe der 10 como média. A grande questão é escolher o valor certo da explotação/exploração
```

---
Resposta 3:

```
O método e = 0,1 explorou mais e usualmente encontrou a ação ideal mais cedo, mas nunca selecionou essa ação mais de 91% das vezes. O método e = 0,01 melhorou mais lentamente, mas eventualmente teria um desempenho melhor do que o método e = 0,1 em ambas as medidas de desempenho mostradas na figura.

Simulando quantitativamente o q*(a), ou seja, a recompensa ótima para cada ação, temos:

    Para ε = 0.01 --> 0.99 * 1.5 = 1.485
    Para ε = 0.1 --> 0.9 * 1.5 = 1.35
```