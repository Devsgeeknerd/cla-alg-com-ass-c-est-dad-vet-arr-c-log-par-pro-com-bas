<!-- Título -->
# Algoritmos e Complexidade Assintótica em C

***Conteúdo da Aula:***

Em uma das vídeo-aulas a seguir, você ouvirá falar sobre o termo **“complexidade assintótica”**...

Mas, o que será que vem a ser esta complexidade?

De maneira bem generalista, nós chamamos de complexidade assintótica a medição do custo computacional para execução de um algoritmo.

Esse custo pode ser verificado nas seguintes vertentes:

* `Temporal`:
  * Vertente que leva em consideração o tempo de execução de um algoritmo.
  * Quanto mais demorada a execução, maior em teoria é a complexidade assintótica temporal do algoritmo;
* `Espacial`:
  * Vertente que leva em consideração os recursos da máquina (processador, memória, acesso a disco rígido) para execução do algoritmo.
  * Quanto mais estes recursos são utilizados, maior é a complexidade assintótica espacial do algoritmo.

Dessa maneira, é importante que consigamos criar algoritmos com complexidade assintótica menor possível, tanto na vertente temporal quanto na vertente espacial.

Uma das formas de se explicitar a notação assintótica de um algoritmo é através de uma notação conhecida como **“Big-O”**.

Nessa notação, pegamos o pior caso de execução de um algoritmo, analisamos a complexidade assintótica dele e a definimos através da notação de uma função chamada `O` (daí vem o nome **Big-O**).

Esta letra `O` maiúscula é, na verdade, a representação da letra **“omicrôn”**.

A maneira de calcularmos a complexidade assintótica de um algoritmo de maneira geral pode se mostrar um processo matemático complexo.

Porém, existem alguns exemplos onde podemos notar facilmente esta complexidade.

Vamos ver os exemplos abaixo:

```c
int numero = 0;
```

Na linha acima, temos um comando de atribuição de valor para uma variável.

O esforço computacional para execução desta linha é o mesmo tanto do ponto de vista temporal quanto do ponto de vista espacial, pois esta linha poderá ser executada `n` vezes que o computador gastará a mesma quantidade de processador e memória, assim como também demorará o mesmo tempo.

Neste caso, nós podemos falar que a complexidade deste algoritmo é `O`(1), ou seja, possui uma complexidade assintótica constante.

```c
int i = 0;
for (int i = 0; i < 5; i++) {
    printf("%d\n", i);
}
```

Este algoritmo já não possui uma complexidade constante.

Na verdade, o tempo de execução dele vai variar de acordo com o tamanho do laço que ele irá executar.

Se o laço for até 1, ele terá complexidade **O(1)**; se for até 2, ele terá complexidade **O(2)**; se ele for até 3, ele terá complexidade **O(3)**; se ele for até `n`, ele terá complexidade **O(n)**.

```c
int i, j = 0;
for (int i = 0; i < 5; i++) {
    for (int j = 0; j < 5; j++) {
        printf("%d\n", i * j);
    }
}
```

Este algoritmo já possui uma complexidade maior que o anterior.

Ele possui dois laços aninhados.

Dessa maneira, ele terá complexidade relacionada à quantidade de laços do primeiro nível multiplicado pela quantidade de laços do segundo nível.

Neste caso, costumamos afirmar que a complexidade assintótica do algoritmo é **O(n2)**.

É importante termos em mente que nossos algoritmos devem ter a complexidade mais próxima de `O(1)` ou `O(n)`, mesmo que não será possível construirmos algoritmos com estas complexidades em todos os trechos.

Também tenha em mente que mensurar a complexidade assintótica de um algoritmo pode não se revelar tão simples como descrito aqui, pois aqui temos apenas uma pequena introdução para que você possa compreender alguns termos utilizados em algumas vídeo-aulas deste ponto em diante.

Porém, recomendamos que você, quando possível, dê uma olhadinha nesse assunto.

Grandes players, como *Microsoft*, *Google*, *Apple* e *Amazon* costumam incluir questões relacionadas à complexidade assintótica de algoritmos em seus processos seletivos.

<!-- Informações -->
## &#8505; Informações

![Visitors](https://api.visitorbadge.io/api/visitors?path=Devsgeeknerd%2Fcla-alg-com-ass-c-est-dad-vet-arr-c-log-par-pro-com-bas&label=Visitantes&labelColor=%23700070&labelStyle=none&countColor=%23000fff&style=plastic&color=%23ffffff "Total de Visitantes")
&nbsp;
![Followers](https://img.shields.io/github/followers/Devsgeeknerd?style=p&label=Seguidores&labelColor=800080&color=000fff "Total de Seguidores")
&nbsp;
![Watchers](https://img.shields.io/github/watchers/Devsgeeknerd/cla-alg-com-ass-c-est-dad-vet-arr-c-log-par-pro-com-bas?style=p&label=Observadores&labelColor=800080&color=000fff "Total de Observadores")
&nbsp;
![Stars](https://img.shields.io/github/stars/Devsgeeknerd/cla-alg-com-ass-c-est-dad-vet-arr-c-log-par-pro-com-bas?style=p&label=Estrelas&labelColor=800080&color=000fff "Total de Estrelas")
&nbsp;
![Forks](https://img.shields.io/github/forks/Devsgeeknerd/cla-alg-com-ass-c-est-dad-vet-arr-c-log-par-pro-com-bas?style=p&label=Bifurcações&labelColor=800080&color=000fff "Total de Bifurcações")
&nbsp;
![Repo Size](https://img.shields.io/github/repo-size/Devsgeeknerd/cla-alg-com-ass-c-est-dad-vet-arr-c-log-par-pro-com-bas?style=p&label=Tamanho&labelColor=800080&color=000fff "Tamanho do Repositório")
&nbsp;
![License](https://img.shields.io/github/license/Devsgeeknerd/cla-alg-com-ass-c-est-dad-vet-arr-c-log-par-pro-com-bas?style=p&label=Licença&labelColor=800080&color=000fff "Licença do Repositório")
