# Sistemas-Operacionais

**Políticas de escalonamento**

1) FIFO OU FCFS ( não preemptivo, escalona o 1º processo que chega na fila de prontos )
   
2) SJF ( escalona o processo de menor cicle de CPU, por 1 º) 
Não - preemptivo
Preemptivo interrompe a execução se chegar um processo menor

3) Prioridade: PCB ou descritor: tem a prioridade do processo

4) Round-Robin, Revejamento circula ou fatia de tempo (RR)
|--> somente preemptivo
|--> quantum (q) = fatia de tempo
|--> Fila esta organizada em ordem de chegada 

Cenário: Escalonamento por prioridade                             
| Processo | Instante Chegada | Ciclo de CPU | Prioridade |  Fim Execução | Tempo de Espera | Tempo de Retorno |
|----------|------------------|--------------|------------|---------------|---------------|---------------------|
| P1       |        0         |      3       |     4      |               |       3       |        0            |              
| P2       |        1         |      4       |     0      |               |       7       |        2            |                 
| P3       |        2         |      2       |     0      |               |       9       |        5            |                 
| P4       |        3         |      1       |     1      |               |      10       |        6            |                 
| P5       |        4         |       5      |     3      |               |       15      |                     |                   
| P6       |        5         |       2      |     0      |               |               |                     |                   

Problema: Espera indefinida, stavation  ou postergação indefinida 
Solução: Técnica de envelhecimento ( aging )
