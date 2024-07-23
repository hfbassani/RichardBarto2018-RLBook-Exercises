### *Exercise 8.3:*

**How might the tabular Dyna-Q algorithm shown on page 164 be modified
to handle stochastic environments? How might this modification perform poorly on
changing environments such as considered in this section? How could the algorithm be
modified to handle stochastic environments and changing environments?**

---
Resposta 1:

```
Olhando o algoritmo de Dyna-Q, o passo (e) poderia considerar o conjunto de tuplas (R,S'), assim no quarto passo de (f) poderia ser uma amostragem aleatória deste conjunto. Para ambientes dinâmicos, como explicado no exemplo 8.3, o agente pode ficar preso em uma região subótima e demorar mais para atingir o objetivo, ou até mesmo nunca atingi-lo. A modificação para lidar com esta situação pode ser então a mesma mostrada no exemplo 8.3, para garantir uma melhor exploração no ambiente.
```
