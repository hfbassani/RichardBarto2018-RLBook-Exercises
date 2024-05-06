### *Exercise 3.16:*

**Now consider adding a constant c to all the rewards in an episodic task, such as maze running. Would this have any e↵ect, or would it leave the task unchanged as in the continuing task above? Why or why not? Give an example.**

---
Resposta 1:

```
Na tarefa episódica, adicionar uma constante a todas as recompensas afeta o agente. Como a recompensa cumulativa agora depende da duração do episódio, os intervalos de tempo que geram recompensas positivas agem para prolongar o episódio e vice-versa. No exemplo da corrida no labirinto, podemos ter optado por dar ao agente -1 recompensa em cada passo de tempo para garantir que ele conclua a tarefa rapidamente. Se adicionarmos c = 2 a cada recompensa, de modo que a recompensa em cada intervalo de tempo agora seja positiva, o agente será incentivado a não encontrar a saída e a continuar coletando recompensas intermediárias indefinidamente.
```
