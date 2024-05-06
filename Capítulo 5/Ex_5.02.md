### *Exercise 5.2:*

**Suppose every-visit MC was used instead of first-visit MC on the blackjack task. Would you expect the results to be very dierent? Why or why not?**

---
Resposta 1:

```
Não, pois o estado do blackjack segue uma trajetória monotonamente crescente e sem memória, ou seja, é amostrado com substituição a cada carta recebida. Isso significa que, uma vez visitado um estado durante um episódio, ele nunca será revisado. Nesse cenário, aplicar o método de Monte Carlo a cada visita não teria impacto na função de valor.
```
