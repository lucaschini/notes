Estrutura composta da seguinte maneira:
- informação
- Onde vai estar a próxima informação  
Ref: [[Lista.canvas|Lista]]

Basicamente: 

```
typedef struct no {
 int info;
 int no *prox;
} No;
```

// Esse nó é padrão nas três, [[Lista]] [[Pilha]] [[Fila]]

Inserção de elemento
-> uso do comando [[malloc]]
```
no *novo
novo = (no*)malloc(1*sizeof(no));
novo->info = valor;
novo->prox = null;
```

Função que verifica se um certo valor existe na lista:

```
int busca(lista *aux, int valor){
	while(aux!=NULL){
		if(aux->info == valor){
			return 1;
		}
		aux = aux->prox;
	}
	return 0;
}
```

Função que apaga um elemento (no começo):

```
//chamada
inicio = apagarum(inicio);

lista *apagaum(lista *aux){
	lista *apagar;
	apagar = aux;
	aux = aux->prox;
	free(apagar);
		return aux;
}
```

Função para apagar todos os elementos da lista:

```
//chamada
inicio = libera(inicio);

lista *libera(lista *aux){
	lista *apag;
		while(aux!=NULL){
			apag = aux;
			aux = aux->prox;
			free(apag);
		}
		return aux;
}
```
