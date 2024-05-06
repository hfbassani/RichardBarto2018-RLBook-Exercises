### *Exercise 4.6:*

**Suppose you are restricted to considering only policies that are "-soft, meaning that the probability of selecting each action in each state, s, is at least "/|A(s)|. Describe qualitatively the changes that would be required in each of the steps 3, 2, and 1, in that order, of the policy iteration algorithm for v⇤ on page 80.**

---
Resposta 1:

```
Para os passos 1 e 2, nada mudaria. Já para o passo 3, não escolheríamos a ação específica pelo argmax. E sim, permitiriamos uma probabilidade uniforme de e/A-1 para todas as ações
```


---
Resposta 2:

```
Durante a etapa de melhoria da política (3), em vez de o argmax simplesmente selecionar uma ação determinística para um estado, atualizamos a política de forma a atribuir probabilidades às ações. Cada ação 'a' pertencente ao conjunto de Ações 'A' em um estado 's' receberia uma probabilidade de p(a) = e/|A(s)| enquanto a ação máxima receberia uma probabilidade de 1 − e + e/|A(s)|. Isso resulta em uma política de produção estocástica e não determinística. Durante a etapa de avaliação da política (2), em vez de considerar apenas os estados, abordamos todos os pares estado-ação, ponderando o valor de cada par pela probabilidade da ação ser selecionada de acordo com nossa política suavizada. No passo 1, a política é inicializada com uma distribuição arbitrária no espaço de ações em cada estado.
```