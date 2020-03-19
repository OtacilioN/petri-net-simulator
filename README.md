Authors
======================================

Hugo de Albuquerque Fonseca <hugoalbuquerque0@gmail.com> <br />
Otacilio Saraiva Maia Neto <otacilio.n97@gmail.com>

Objective
======================================

This exercise aims to simulate a Petri net with parallelism and print it using the graphic library Allegro.

Text input
======================================

To simulate the Petri Net using this code, it is necessary to feed it with an input file. The file must not contain any text, and must be formatted _exactly_ as proposed in the table below:

Linha          | Descricao
-------------- | --------------------------------------------
1              | Quantidade de Lugares
2              | Quantidade de Transicoes
3              | Quantidade de Lugares com pelo menos um Token
4              | Quantidade de Arcos Lugar -> Transicao
5              | Quantidade de Arcos Transicao -> Lugar
6,...,x        | Descricao Lugar/Token
x+1,...,y      | Descricao do arco Lugar/Quantidade/Transicao
y+1,...,z      | Descricao do arco Transicao/Quantidade/Lugar

Exemplo de input:
~~~~~~~~~~~~~{.py}
2
2
1
2
2
0 4
0 1 0
1 2 1
0 1 1
1 1 0
~~~~~~~~~~~~~
Isso gera uma Rede de Petri com o seguinte formato:

Inicio da simulacao:
![Exemplo](http://puu.sh/lXP18/8eb140cc09.png "Exemplo - Rede de Petri")

Fim da simulacao:
![Exemplo](http://puu.sh/lXOLq/b90e25f895.png "Exemplo - Rede de Petri")
