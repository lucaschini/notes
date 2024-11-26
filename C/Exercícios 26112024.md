- Elabore uma função que retorne o maior elemento de uma pilha
```
int maiorPilha(Pilha *P){

	No *aux;
	int maior;
	aux = P->Topo;
	maior = aux->info;
	while(aux != NULL){
		if(aux->info > maior){
			maior = aux->info;
		}
		aux = aux->prox;
	}
	return maior;
}
```

- Elabore uma função que conte quantos nós possui uma árvore binária
```
int qtdNode(NoArv *Pai){
	int cont = 1;

	if(Pai->FD != NULL){
		cont = qtdNode(Pai->FD) + cont;
	}

	if(Pai->FE != NULL){
		cont += qtdNode(Pai->FE);
	}

	return cont;
}

chamada da função: 
int qtd;
Arv A;
.
.
.
qtd = qtdNode(A);
```

- Elabore um procedimento que apague um certo elemento da pilha, se ele existir
```
Pilha *apagaNum(Pilha *P, int N){
	Pilha *aux = criaPilha();
	int num;
	while(P->Topo != NULL){
		num = pop(P);
		if(num != N){
			push(num,aux);
		}
	}

	while(vazia(aux) != 1){
		push(P, pop(aux));;
	}
	return P;
}
```