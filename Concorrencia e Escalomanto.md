# 2-BIM-Exercicios

[2-BIM] - Exercícios - Concorrência
Ana Laura Pedrotti Schwingel

Resolva a lista de exercícios abaixo sobre concorrência. 

1.	O que é concorrência e como este conceito está presente nos sistemas operacionais multiprogramáveis?
Concorrência é um mecanismo dos sistemas operacionais para que mais de um processo seja executado pelo processador ao mesmo tempo, concorrentemente. Está presente através das técnicas de interrupção, exceção, buffering, spooling e reentrância. 

2.	Por que o mecanismo de interrupção é fundamental para a implementação da multiprogramação?
Porque é o mecanismo que torna possível a implementação de concorrência nos computadores que possuem sistemas multiprogramáveis. É com a utilização da interrupção que o sistema operacional sincroniza a execução de todas as rotinas, dos programas e controla os dispositivos. 

3.	Explique o mecanismo de funcionamento das interrupções.
Uma interrupção é sempre gerada por algum evento externo ao programa, e, nesse caso, independe da instrução que está sendo executada. Um exemplo de interrupção ocorre quando um dispositivo de entrada e saída sinaliza ao processador que uma operação de entrada saída está completa. Neste caso, o processador deve interromper o programa que está sendo executado para tratar o término da operação de entrada saída.
Ao final da execução de cada instrução, a unidade de controle verifica a ocorrência de algum tipo de interrupção. Nesse caso, o programa em execução é interrompido e o controle desviado para uma rotina responsável por tratar o evento ocorrido, chamada rotina de tratamento de interrupção. Como existem vários tipos de interrupção, pode haver diferentes rotinas de tratamento de interrupção.

Para que o programa interrompido possa retomar sua execução exatamente do ponto onde foi interrompido, é necessário que, no momento da interrupção, sejam guardadas informações a respeito da execução do programa. Estas informações são basicamente o conteúdo dos registradores que deverão ter seus valores restaurados quando a execução do programa interrompido for reiniciada.


4.	O que são eventos síncronos e assíncronos? Como estes eventos estão relacionados ao mecanismo de interrupção e exceção?
Eventos síncronos são eventos que podem ocorrer um de cada vez, e está relacionado ao mecanismo de execução, devido a execução ser resultante direto de uma instrução do programa. 
Eventos assíncronos são eventos imprevisíveis e podem ocorrer muitas vezes. As interrupções são decorrentes desses eventos e não da instrução do programa. 
5.	Dê exemplos de eventos associados ao mecanismo de exceção.
6.	Qual a vantagem da E/ S controlada por interrupção comparada com a técnica de pooling?
7.	O que é DMA e qual a vantagem desta técnica?
8.	Como a técnica de buffering permite aumentar a concorrência em um sistema computacional?
9.	Explique o mecanismo de spooling de impressão.
10.	Em um sistema multiprogramável, seus usuários utilizam o mesmo editor de textos (200 Kb), compilador (300 Kb), software de correio eletrônico (200 Kb) e uma aplicação corporativa (500 Kb). Caso o sistema não implemente reentrância, qual o espaço de memória principal ocupado pelos programas quando 10 usuários estiverem utilizando todas as aplicações simultaneamente? Qual o espaço liberado quando o sistema implementa reentrância em todas as aplicações?
