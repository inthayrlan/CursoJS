# Tratamento de dados

### Manipulação de dados:

Guardando, `window.propt('What is your name?')`

A primeira tela exibe uma janela com `window.prompt` o valor e mostrado atraves de concatenação:

 `('Nice to meet you' + nome '!')`

    var nome = window.prompt('What is your name?')
    window.alert('Nice to meet you,' + nome '!')

### Tipos de dados numéricos:

Números inteiros: (ex: 5):

    Number.parseInt(n)

Numeros reais (ex: 1,5):

    Number.parseFloat(n)

Aceita os dois tipos de dados numericos:

    Number(n)

### Convertendo de número para string:

Para converte de número para String utilizamos `String(n)` ou `n.toString()` 

Exemplo a seguir:

        var n1 = Number.parseInt(window.prompt('Input fist number: '))
        var n2 = Number.parseInt(window.prompt('Input second number: '))
        var n3 = Number(window.prompt('Input fist number: '))
        
        var s = n1 + n2 + n3
        
        window.alert('Soma dos valores é: ' + String(s))

### Formatando Strings

Declaração das variaveis:

    nome = 'Thayrlan'
    idade = 41
    nota = 5.5

Exemplo com **concatenação**:

    ' O aluno ' + nome + ' com '+ idade + ' anos tirou a nota ' + nota

Exemplo utilizando **template strings**:

    `O aluno ${nome} com ${idade} anos tirou a nota ${nota}`

Outros exemplos de como formatar strings:

`s.length` - Quantos caracteres a string tem

`s.toUpperCase()` - Tudo para 'MAIÚSCULA'

`s.toLowerCase()` - Tudo para 'minúsculas'

O exemplo abaixo exibe o nome socilitado na `window.prompt` em `toUpperCase` (Maiuscula) e `toLowerCase` (minusculas).

    
          var name = window.prompt("What is your name? ");
    	
    	      document.write(
    	        `Hey ${name}! your name has <strong>${name.length}</strong> letters `
    	      );
    	      document.write(
    	        `,your name in <strong>uppercase</strong> is ${name.toUpperCase()} `
    	      );
    	      document.write(
    	        ` ,and your name in <strong>lowercase</strong> is ${name.toLowerCase()} `
    	      );
      

### Formando números

Exemplos a seguir:

        //Declarando valores.
        > var n1 = 1545.5
        undefined
        
        //Chamando valor no terminal do node.js.
        > n1
        1545.5
        
        //Adicionando duas casa depois da virgula.
        > n1.toFixed(2)
        '1545.50'
        
        //Alterando sinal de '.' para ','.
        > n1.toFixed(2).replace('.',',')
        '1545,50'
        >
    

Exemplos de conversão para valores monetários:

        > n1.toLocaleString('pt-BR', {style: 'currency', currency: 'BRL'})
        'R$ 1,545.50'
        
        > n1.toLocaleString('pt-BR', {style: 'currency', currency: 'USD'})
        'US$ 1,545.50'
        
        > n1.toLocaleString('pt-BR', {style: 'currency', currency: 'EUR'})
        '€ 1,545.50'