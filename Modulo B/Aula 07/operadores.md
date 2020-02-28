### Operadores de precedência

![https://i.imgur.com/QTRnKrD.png](https://i.imgur.com/QTRnKrD.png)

### Ordem de precedência

 `()`  Parênteses.

 `**`  Exponenciação.

 `/`   `%`   `*`  Divisão, Resto da divisão e Multiplicação.

 `+`   `-`  Soma é subtração.

### Ex.: 01. Atribuição | Considerando ordem de precedência.

    //Remover parentese para o script executar usando ordem de precedencia, como no 'Ex.: 02'
    
    var a = 5 + 3
    var b = a % 5
    var c = 5 * (b ** 2)
    var d = 10 - (a / 2)
    var e = (6 * 2) / d
    var f = (b % e) + (4 / e)

### Ex.: 02. Atribuição

    var a = 5 + 3
    var b = a % 5
    var c = 5 * b ** 2
    var d = 10 - a / 2
    var e = 6 * 2 / d
    var f = b % e + 4 / e

## Exemplo de script

---

    <!DOCTYPE html>
    <html lang="en">
      <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Cursos JS : Exemplo</title>
      </head>
    
      <style>
        body {
          margin: 25px;
          font-family: Arial, Helvetica, sans-serif;
          font-size: 27px;
          color: yellow;
          background-color: #1b1b1b;
        }
      </style>
    
      <body>
        <script>
          var name = String(window.prompt("Qual é seu nome?"))
          var n1 = Number(window.prompt("Coloque um número: "));
          var n2 = Number(window.prompt("Agora coloque outro: "));
    
            var s = n1 + n2;
            var sb = n1 - n2;
            var mt = n1 * n2;
            var dv = n1 / n2;
            var s5 = n1 ** n2;
    
              document.write(`A adição entre ${n1} e ${n2} é de: ${s}<br>`);
              document.write(`A subtração entre ${n1} e ${n2} é de: ${sb}<br>`);
              document.write(`A multiplicação entre ${n1} e ${n2} é de: ${mt}<br>`);
              document.write(`A divisão entre ${n1} e ${n2} é de: ${dv}<br>`);
              document.write(`A sua potencialização ${n1} entre ${n2} é de: ${s5}<br>`);
              document.write("<br>");
              document.write("😋 Obrigado pela preferência, " +name+ " volte sempre!"); 
        </script>
      </body>
    </html>