### *Exercise 3.12:*

**Give an equation for vπ in terms of qπ and π.**

---
Resposta 1:

```
vπ(s) = Eπ[Gt | St = s] = Σ[π(a|s) * qπ(s, a)], para todo a ∈ A(s)
```

---
Resposta 2:

```
A função de valor do estado vπ é igual ao retorno cumulativo esperado desse estado, dada uma distribuição de ações. A função de valor de ação de estado qπ é o valor de estar em um estado e realizar uma ação determinística. Portanto, a função valor do estado é a soma ponderada da função valor da ação do estado P, com os pesos iguais às probabilidades de seleção de cada ação:
vπ(s) = Eπ[Gt | St = s] = Σ[π(a|s) * qπ(s, a)]
```