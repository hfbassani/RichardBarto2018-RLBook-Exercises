### *Exercise 3.3:*

**Consider the problem of driving. You could define the actions in terms of the accelerator, steering wheel, and brake, that is, where your body meets the machine. Or you could define them farther out—say, where the rubber meets the road, considering your actions to be tire torques. Or you could define them farther in—say, where your brain meets your body, the actions being muscle twitches to control your limbs. Or you could go to a really high level and say that your actions are your choices of where to drive. What is the right level, the right place to draw the line between agent and environment? On what basis is one location of the line to be preferred over another? Is there any fundamental reason for preferring one location over another, or is it a free choice?**

---
Resposta 1:

```
Depende do objetivo que o modelador quer alcançar. Creio que o mais correto nessa situação é entender o problema que o algoritmo vai sanar e escolher os elementos que o agente venha a possuir um maior controle sobre o estado por meio das suas ações realizadas.
```

---
Resposta 2:

```
Há uma compensação entre complexidade do espaço de ação estatal, despesas computacionais e precisão. Se for tradaça uma fronteira, seria criado um espaço de estado-ação dependente do número de neurônios e de sua interação com ações físicas como girar o volante; muito grande para ser armazenado ou computado de forma eficiente. Da mesma forma, se traçarmos o limite ao nível da viagem, perderemos os detalhes necessários para agir a cada segundo nas mudanças de estado na estrada que podem levar a um acidente. O fator limitante fundamental nesta seleção é se o objetivo pode ser alcançado com segurança na camada de abstração escolhida; na verdade, esta parece ser uma das tarefas da engenharia de forma mais ampla.
```