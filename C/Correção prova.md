```
terceira questão (sem ser minha prova)

void Tres(int a[], int *m){
	int pos, i, menor;
	pos = -1; menor = 9999;
	for(i=0;i<30;i++){
		if((a[i] % 6 == 0) && (a[i]<menor)){
			pos = i;
			menor = a[i];
		}
	}

	*m=pos;
}
```
