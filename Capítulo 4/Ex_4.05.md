### *Exercise 4.4:*

**How would policy iteration be defined for action values? Give a complete algorithm for computing q, analogous to that on page 80 for computing v. Please pay special attention to this exercise, because the ideas involved will be used throughout the rest of the book.**

---
Resposta 1:

```
1. Initialization
    V(s) ∈ ℝ and π(s) ∈ A(s) arbitrarily for all s ∈ S

2. Policy Evaluation
    
    Loop for each s ∈ S, a ∈ A:
        q <- Q(s,a)
        Q(s,a) <- Σp(s', r | s, a)[r + γΣπ(a'|s')Q(s'|a')]
        Δ <- max(Δ, |q - Q(s,a)|)

3. Policy Improvement 
    policy-stable <- true
    For each s ∈ S, a ∈ A:
        old-action <- π(s)
        π(s) <- argmax a Σp(s', r | s, a)[r + γΣπ(a'|s')q(s'|a')]
        If old-action ≠ π(s), then policy-stable <- false
    If policy-stable, then stop and return Q ≅ q* and π ≅ π*; else go to 2 
```
