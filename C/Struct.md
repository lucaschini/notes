O que são?
São utilizadas para agrupar ==informações relacionadas== de tipos diferentes de dados.

Cria-se um ==NOVO TIPO== de dados constituído por diferentes tipos básicos de dados.

- A sintaxe para a criação de uma estrutura é:
```
struct nome da estrutura  
{  
tipo campo 1;  
tipo campo 2;  
....  
tipo campo n;  
} ;
```

Exemplo: 
Uma estrutura para controlar os seguintes  
dados relacionados ao estoque de um pequeno  
estabelecimento comercial:  

• Código;  
• nome do produto;  
• quantidade estocada;  
• valor de compra;  
• valor a ser vendido;  

Seria:

```
struct produto
{
int codigo;
char nome[50];
int quantidade;
float valor_compra;
float valor venda;
};
```

Como declarar variáveis do tipo de uma estrutura criada?
-> `struct NOME_DA_ESTRUTURA NOME_DA_VARIÁVEL;`
Exemplo:
`struct produto item;`

Acessando os campos de uma estrutura:
`NOME_DA_VARIAVEL.CAMPO`

![[Pasted image 20241014113051.png]]
![[Pasted image 20241014113102.png]]
Ver mais: [[fflush()]] [[gets()]]
![[Pasted image 20241014113343.png]]

Exemplo de código 1:
Elabore um programa que leia os seguintes dados de  
30 alunos:  
• RA  
• Altura  
• Peso  
• O programa deverá imprimir o RA do aluno:  
• Com maior altura,  
• Menor peso,  
• Maior e menor IMC – “INDICE DE MASSA CORPOREA”.
