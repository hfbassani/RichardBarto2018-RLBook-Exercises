### *Exercise 7.3:*

**Why do you think a larger random walk task (19 states instead of 5) was used in the examples of this chapter? Would a smaller walk have shifted the advantage to a different value of n? How about the change in left-side outcome from 0 to 1 made in the larger walk? Do you think that made any difference in the best value of n?**

---
Resposta 1:

```
Considerando que o passeio aleatório de 5 estados tivesse sido utilizado, o valor ideal para n provavelmente seria menor. Conforme apresentado no exemplo, definir n como 3 e observar um episódio começando em C e fazendo a transição C → D → E → "Final" atualizaria C em direção à recompensa de 1, representando uma estimativa incorreta do verdadeiro valor de C. Parece que o provável valor ótimo neste caso seria n = 2 e, portanto, poderia se fazer a suposição geral de que, para espaços de estados menores, valores menores de n são mais apropriados. Se n ≥ 2, então, para episódios mais longos, as atualizações não seriam mais inicializadas em outro valor de estado, mas sim feitas atualizações com base em seus próprios valores. A mudança no valor esquerdo de 0 para -1 poderia redizor o valor ideal de n neste exemplo. Definir o valor esquerdo como -1 localiza efetivamente os estados no lado esquerdo da caminhada mais próximos de uma recompensa, o que significa que as atualizações não precisam ser propagadas retroativamente para fazer boas atualizações no valor desses estados.
```
