# Sistemas-Operacionais

**Políticas de escalonamento**

1) FIFO OU FCFS ( não preemptivo, escalona o 1º processo que chega na fila de prontos )
   
2) SJF ( escalona o processo de menor cicle de CPU, por 1 º) 
Não - preemptivo
Preemptivo interrompe a execução se chegar um processo menor

3) Prioridade: PCB ou descritor: tem a prioridade do processo

Cenário: Escalonamento por prioridade                             |--------------------|
                                                                  |                    |
Processo	Instante de Chegada	Ciclo de CPU	Prioridade
P1	0	3	4
P2	1	4	0
P3	2	2	0
P4	3	1	1
