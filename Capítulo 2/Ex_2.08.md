### *Exercise 2.8:* 

**Exercise 2.8: UCB Spikes In Figure 2.4 the UCB algorithm shows a distinct spike in performance on the 11th step. Why is this? Note that for your answer to be fully satisfactory it must explain both why the reward increases on the 11th step and why it decreases on the subsequent steps. Hint: If c = 1, then the spike is less prominent.**

---
Resposta 1:

Após 10 time steps o algoritmo UCB explorou todas as 10 ações, pois, até serem selecionadas, seu limite superior de confiança é infinito (como Nt (a) = 0), garantindo assim que serão selecionadas uma vez nas primeiras 10 ações. Neste ponto o agente dispõe de uma amostra para avaliar o valor esperado de cada braço e a mesma confiança/incerteza em cada ação. Com c = 2 é provável que escolha a ação com maior retorno da primeira amostra, o que provavelmente lhe dará uma recompensa igualmente grande, criando o pico. Agora, o limite superior de confiança para aquela ação diminuirá e o agente selecionará outra ação menos valiosa, causando a diminuição do desempenho no próximo passo de tempo.
