# :chart_with_upwards_trend:  Big O Notation

> "O quão o código fica devagar, ao longo que os dados crescem"

## O que é?


Big O trata-se de uma notação para descrever o quão eficiente é um algorítimo ao longo que seus dados aumentam. Já uma notação é uma forma concisa e padrão de descrever algo longo.

Com Big O torna-se possível comparar algorítimos e a velocidade e eficiência de cada.

![Big O](https://www.30secondsofcode.org/assets/illustrations/big-o-complexity.png)

Exemplos de operações:

> n = quantidade de dados (Como uma variável x)

 - Constante: O(1) *"Não importa quantos dados são fornecidos. A quantidade de etapas permanece a mesma."*
 - Tempo linear: O(n)
 - Tempo logarítmico: O(n log n) *"Quando os dados são reduzidos a cada etapa."*
 - Tempo quadrático: O(n²)
 - Tempo exponencial: O(2^n)
 - Tempo fatorial: O(n!)
 - Tempo polinomial: 2^{O(log n)}

Por exemplo, em javascript, este código:
  

      function  addUp(n) {
        
        let  sum  =  0;
        for (let  i  =  0; i  <=  n; i++) {
		sum  +=  i;
		}
        return  sum;
        }
Neste programa, caso o usuário forneça, por exemplo, 1000000000 como dado, o programa teria que passar por 1000000000 passos até chegar no resultado *(Nesse caso, ele faria um for loop para cada número até chegar no resultado)*. Logo, sua notação de complexidade tratar-se-ia de **O(n)**, uma vez que o "n" é fornecido pelo usuário.

Já neste código:

    function  addUp(n) {
    
	    let  sum  =  n  * (n  +  1) /  2;
	    return  sum;
    
    }
Não importa o número fornecido pelo usuário, o código sempre dará 3 passos. Fazendo com este código tenha uma complexidade de **O(1)**, porque por mais que sejam 3 passos, eles não são significativos o bastante para serem mais complexos que **O(1)**.