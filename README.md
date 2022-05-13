# -desafiosjs
concluído os desafios do bootcamp

### Desafio
Você recebeu desafio de desenvolver um programa que calcule o quociente e o resto da divisão de dois números inteiros. Não se esqueça que o quociente e o resto da divisão de um inteiro a por um inteiro não-nulo b são respectivamente os únicos inteiros q e r tais que:

0 ≤ r < |b|

Se r < 0: r = r - |b|

a = b × q + r

q = ( a - r ) / b

Caso você não saiba, o teorema que garante a existência e a unicidade dos inteiros q e r é conhecido como ‘Teorema da Divisão Euclidiana’ ou ‘Algoritmo da Divisão’.

** |b| (Módulo / Valor absoluto): É o valor representado de forma positiva;

## Entrada
A entrada é composta por dois números inteiros a e b (-1.000 ≤ a, b < 1.000).

## Saída
Imprima o quociente q seguido pelo resto r da divisão de a por b, considerando as regras apresentadas a cima.

Exemplos de Entrada	Exemplos de Saída
7 3	2 1
7 -3	-2 1
-7 -3	3 2
Resposta:

let line = gets().split(" "); const a = parseInt(line[0]); const b = parseInt(line[1]);

q = parseInt(a / b);

r = a - b * q;

if (r < 0) { r += Math.abs(b);

q = [(a-r)/b] ; //escreva sua lógica aqui }

print(q + " " + r);

2 / 3 - Quadrado e ao Cubo

Todas as entradas e saída dos algoritmos são utilizados o STDIN e STDOUT de cada linguagem, abaixo tem algumas dicas de como utilizar cada STDIN e STDOUT de cada linguagem.

### JavaScript

Em JavaScript as funções de STDIN e STDOUT respectivamente sãogets e console.log, a função gets é implementada internamente para auxiliar a entrada dos dados.

Exemplo:

let line = gets(); // Retorna a próxima linha de entrada
console.log(line); // Imprime o dado
Java

Em Java existe várias formas de implementar o STDIN e STDOUT recomendamos utilizar BufferedReader para o STDIN e o System.out.println para o STDOUT.

Exemplo:

BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
StringTokenizer st = new StringTokenizer(br.readLine()); // Lê a linha de entrada
int a = Integer.parseInt(st.nextToken());
System.out.println(a); // Imprime o dado
Python

Em Python existe várias formas de implementar o STDIN e STDOUT recomendamos utilizar sys.stdin.readline para o STDIN e o print para o STDOUT.

Exemplo:

import sys
a = int(sys.stdin.readline()) // Lê a linha de entrada
print(a); // Imprime o dado
let limit = parseInt(gets());

for (let i = 1; i <= limit; i++) { let X = (i2); let Y = (i3);

print(i, X, Y);

}

Desafio
Você terá o desafio de ler um valor inteiro correspondente à idade de uma pessoa em dias e informe-a em anos, meses e dias

Obs.: apenas para facilitar o cálculo, considere todo ano com 365 dias e todo mês com 30 dias. Nos casos de teste nunca haverá uma situação que permite 12 meses e alguns dias, como 360, 363 ou 364.

Entrada
O arquivo de entrada contém um valor inteiro.

Saída
Imprima a saída conforme exemplo fornecido.

Exemplo de Entrada	Exemplo de Saída
400	1 ano(s) 1 mes(es) 5 dia(s)
800	2 ano(s) 2 mes(es) 10 dia(s)
30	0 ano(s) 1 mes(es) 0 dia(s)
let totalDeDias = parseInt(gets());

let qtdAnos, qtdMeses;

qtdAnos = parseInt( totalDeDias / 365); totalDeDias= parseInt( totalDeDias % 365);

qtdMeses= parseInt( totalDeDias / 30); totalDeDias= parseInt((totalDeDias%365)) %30 ;

let resultado = (qtdAnos + " ano(s) " + '\n' + qtdMeses +" mes(es)" + '\n' + totalDeDias + " dia(s)");

print(resultado);
