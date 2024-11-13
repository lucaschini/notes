Para se inverter uma [[Fila]] usa-se [[Pilha]]

```
Fila *inverte(Fila *F){
	Pilha Paux = criaPilha();

	while(vaziaFila(F) == 0){
		push(Paux,retiraFila);
	}
	while(vaziaPilha(Paux) != 1){
		insereFila(F, pop(Paux));
	}
	free(Paux);
	return F;
}
```
