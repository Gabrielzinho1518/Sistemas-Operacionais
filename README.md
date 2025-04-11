# Sistemas-Operacionais

**Políticas de escalonamento**

1) FIFO OU FCFS ( não preemptivo, escalona o 1º processo que chega na fila de prontos )
   
2) SJF ( escalona o processo de menor cicle de CPU, por 1 º) 
Não - preemptivo
Preemptivo interrompe a execução se chegar um processo menor

3) Prioridade: PCB ou descritor: tem a prioridade do processo

Cenário: Escalonamento por prioridade                             
| Processo | Instante Chegada | Ciclo de CPU | Prioridade | Início Execução | Fim Execução | Tempo de Espera | Tempo de Retorno |
|----------|------------------|--------------|------------|------------------|---------------|------------------|-------------------|
| P1       |        0         |      3       |     4      |        0         |       3       |        0         |         3         |
| P2       |        1         |      4       |     0      |        3         |       7       |        2         |         6         |
| P3       |        2         |      2       |     0      |        7         |       9       |        5         |         7         |
| P4       |        3         |      1       |     1      |        9         |      10       |        6         |         7         |
