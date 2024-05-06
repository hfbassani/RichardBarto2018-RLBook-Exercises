### *Exercise 6.4*

**The specific results shown in the right graph of the random walk example are dependent on the value of the step-size parameter, α. Do you think the conclusions about which algorithm is better would be affected if a wider range of α values were used? Is there a different, fixed value of α at which either algorithm would have performed significantly better than shown? Why or why not?**

---
Resposta 1:

```

O gráfico sugere que a precisão a longo prazo dos métodos TD é inversamente relacionada ao α escolhido, o que é intuitivo, já que valores de α maiores podem provocar oscilações da função de valor em torno do verdadeiro valor. A principal desvantagem do método Monte Carlo parece ser sua menor quantidade de atualizações de função de valor em comparação com os métodos TD. Para 100 episódios, o método MC não pode realizar mais do que 100 atualizações, enquanto o método TD, com uma duração esperada do episódio de 6, realiza 600 atualizações de função de valor em 100 episódios. Nenhum valor de α parece capaz de compensar essa redução na taxa de amostragem.
```
