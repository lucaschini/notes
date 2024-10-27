Função “malloc”:
• Recebe como parâmetro o número de bytes que se
deseja alocar
• Retorna um ponteiro genérico para o endereço
inicial da área de
• A memória alocada, se houver espaço livre:
![[Pasted image 20241027121350.png]]

Toda variável alocada dinamicamente ==tem que ser liberada==
• Comando free
• No nosso Exemplo: Alocação dinâmica de um vetor de
inteiros com 10 elementos
```
	int *v;
	v = (int *) malloc(10*sizeof(int));
	¦
	free(v);
```

==NOTA:==
- Quando usar estrutura e alocar dinamicamente a memória
Substituímos o ==. (ponto) pela -> (seta)==.
