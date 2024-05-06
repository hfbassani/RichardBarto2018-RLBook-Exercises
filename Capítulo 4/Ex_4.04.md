### *Exercise 4.4:*

**The policy iteration algorithm on page 80 has a subtle bug in that it may never terminate if the policy continually switches between two or more policies that are equally good. This is okay for pedagogy, but not for actual use. Modify the pseudocode so that convergence is guaranteed.**

---
Resposta 1:

```
1. Initialization
    V(s) ∈ ℝ and π(s) ∈ A(s) arbitrarily for all s ∈ S

2. Policy Evaluation
    Loop:
        Δ <- 0
        Loop for each s ∈ S:
            v <- V(s)
            V(s) <- Σp(s', r | s, π(s))[r + γvπ(s')]
            Δ <- max(Δ, |v - V(s)|)
    until Δ < θ (a small number determining the accuracy of estimation)

3. Policy Improvement 
    policy-stable <- true
    For each s ∈ S:
        old-action <- π(s)
        π(s) <- argmax a Σp(s', r | s, a)[r + γvπ(s')]
        If old-action ≠ π(s), then policy-stable <- false
    If policy-stable, then stop and return V ≅ x* and π ≅ π*; else go to 2 
```

---
Resposta 2:

```
A melhoria abaixo segue a mesma ideia de ter as etapas de Policy Evaluation e Policy Improvement, porém há algoritmos mais otimizados, como por exemplo o Value Iteration.

1. Initialization
    V(s) ∈ ℝ and π(s) ∈ A(s) arbitrarily for all s ∈ S

2. Policy Evaluation
    Loop:
        Δ <- 0
        Loop for each s ∈ S:
            v <- V(s)
            V(s) <- Σp(s', r | s, π(s))[r + γvπ(s')]
            Δ <- max(Δ, |v - V(s)|)
    until Δ < θ (a small number determining the accuracy of estimation)

3. Policy Improvement
    Loop:
        Δ <- 0
        old-state-value <- v
        Go to 2
        For each s ∈ S:
            π(s) <- argmax a Σp(s', r | s, a)[r + γvπ(s')]
            Δ <- max(Δ, |old-state-value(s) - V(s)|)
    until Δ < θ (a small number determining the accuracy of estimation)
```


---
Resposta 3:

```
Ao realizar o argmax durante a etapa de melhoria de política do algoritmo, é possível continuar alternando indefinidamente entre duas ações ótimas. No momento, um empate é resolvido selecionando aleatoriamente entre as ações que maximizam o valor. Em vez disso, poderia ser sempre selecionada a primeira ação resultante do argmax, garantindo assim que a mesma ação ótima seja escolhida durante a iteração, definindo o booleano estável-política como verdadeiro e garantindo a convergência.

```