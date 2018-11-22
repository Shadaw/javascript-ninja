### Vamos falar um pouco sobre "Futebol". Escolha um campeonato estadual qualquer para começar o desafio. Declare uma variável chamada `championship` que receberá o nome do campeonato, e imprima o nome desse campeonato no console.
```js
var championship = 'Brasileirão';

console.log(championship); // Brasileirão
```

### Declare uma variável chamada `teams`, que receberá um array com 5 elementos. Os elementos serão nomes de times do campeonato escolhido, e os nomes devem estar na ordem em que eles aparecem na tabela no momento da solução desse desafio.
```js
var teams = ['Palmeiras', 'Flamengo', 'Internacional', 'Gremio', 'São Paulo']
```

### Crie uma função chamada `showTeamPosition` com as seguintes características:
    - A função deve receber um número por parâmetro;
    - A função deve retornar a frase:
    "O time que está em [POSIÇÃO]º lugar é o [NOME DO TIME].";
    - Onde [POSIÇÃO] é o valor passado por parâmetro e [NOME DO TIME] é o time
    que está nessa posição no array criado acima com os nomes dos times.
    --------------
    Dica: lembre-se que arrays começam no índice zero, então a posição passada
    deve ser sempre um número a mais que o índice do array ;)
    --------------
    - A função só deve retornar a frase acima somente se o time estiver entre os 5 primeiros.
    - Se não houver time para a posição passada, deve retornar a mensagem:
    "Não temos a informação do time que está nessa posição."
```js
function showTeamPosition(num) {
  if (num <= 0 || num > 5) {
    return "Nao temos a informação do time que está nessa posição";
  }
  return `O time que está em ${num}º lugar é o ${teams[num - 1]}`;
}
```

### Escolha 4 times do campeonato selecionado e mostre a posição dele, usando a função acima. Entre esses 4, adicione 1 que não esteja entre os 5 primeiros.
```js
showTeamPosition(1); // 'O time que está em 1º lugar é o Palmeiras'
showTeamPosition(3); // 'O time que está em 3º lugar é o Internacional'
showTeamPosition(5); // 'O time que está em 5º lugar é o São Paulo'
showTeamPosition(7); // 'Nao temos a informação do time que está nessa posição'
```

### Mostre os números de 20 a 30 no console (inclusive o 30), usando a estrutura de repetição "while".
```js
var count = 20;
while(count <= 30) {
  console.log(count++)
}
```

### Crie uma função chamada `convertToHex`, com as seguintes características:
    - A função recebe uma cor por parâmetro, do tipo string. Exemplo: "red";
    - Escolha 5 cores que serão convertidas do nome da cor para o seu
    equivalente hexadecimal (pode ser qualquer tom);
    - Usando a estrutura switch, verifique se a cor passada por parâmetro é
    algum hexa escolhido. Se for, retorne a frase:
    "O hexadecimal para a cor [COR] é [HEXADECIMAL].";
    - Se a cor passada por parâmetro não estiver entre as selecionadas, mostre
    a frase:
    "Não temos o equivalente hexadecimal para [COR]."
```js
function convertToHex(cor) {
  switch(cor) {
    case 'red':
      console.log(`O hexadecimal para a ${cor} é #FF0000`);
      break;
    case 'black':
      console.log(`O hexadecimal para a ${cor} é #000000`);
      break;
    case 'green':
      console.log(`O hexadecimal para a ${cor} é #008000`);
      break;
    case 'blue':
      console.log(`O hexadecimal para a ${cor} é #0000FF`);
      break;
    case 'white':
      console.log(`O hexadecimal para a ${cor} é #FFFFFF`);
      break;
    default:
      console.log(`Nao temos o equivalente hexadecimal para ${cor}`)
  }
}
```

### Tente mostrar o hexadecimal de 8 cores diferentes usando a função criada acima.
```js
convertToHex('red');    // O hexadecimal para a red é #FF0000
convertToHex('black');  // O hexadecimal para a black é #000000
convertToHex('green');  // O hexadecimal para a green é #008000
convertToHex('blue');   // O hexadecimal para a blue é #0000FF
convertToHex('white');  // O hexadecimal para a white é #FFFFFF
convertToHex('orange'); // Nao temos o equivalente hexadecimal para orange
convertToHex('yellow'); // Nao temos o equivalente hexadecimal para yellow
convertToHex('pink');   // Nao temos o equivalente hexadecimal para pink
```'