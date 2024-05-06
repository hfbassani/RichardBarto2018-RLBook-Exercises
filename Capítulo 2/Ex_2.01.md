### *Exercise 2.1:*

**In *ε*-greedy action selection, for the case of two actions and *ε* = 0.5, what is the probability that the greedy action is selected?**

---
Resposta 1:

```
A probabilidade de selecionar a ação ótima converge para mais de 1 - ε, logo

1 - 0.5 = 0.5

0.5 é a probabilidade para encontrar a melhor ação
```

---
Resposta 2:

```
A probabilidade da ação greedy ser selecionada é de 0,75

Justificativa: Existe duas formas da melhor ação ser escolhida:

1) O algoritmo escolhe a melhor ação: 1-ε, ou seja 0,5, é a probabilidade dele escolher a melhor ação
2) O algoritmo escolhe uma ação aleatória e essa ação é a melhor ação: ε * 0,5 = 0,5 * 0,5 = 0,25

Somando as duas probabilidades temos 0,75 como sendo a probabilidade da melhor ação ser escolhida.
```

Resposta 3:

```
Ação gananciosa selecionada com p = 0,5.

```