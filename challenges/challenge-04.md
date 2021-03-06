# Desafio da semana #4

### Declare uma variável chamada `isTruthy`, e atribua a ela uma função que recebe um único parâmetro como argumento. Essa função deve retornar `true` se o equivalente booleano para o valor passado no argumento for `true`, ou `false` para o contrário.
```js
var isTruthy = arg => !!arg ? true : false;
```

### Invoque a função criada acima, passando todos os tipos de valores `falsy`.
```js
isTruthy('') // false
```

### Invoque a função criada acima passando como parâmetro 10 valores `truthy`.
```js
isTruthy(1) // true 
```

### Declare uma variável chamada `carro`, atribuindo à ela um objeto com as seguintes propriedades (os valores devem ser do tipo mostrado abaixo):
- `marca` - String
- `modelo` - String
- `placa` - String
- `ano` - Number
- `cor` - String
- `quantasPortas` - Number
- `assentos` - Number - cinco por padrão
- `quantidadePessoas` - Number - zero por padrão
```js
var carro = {
  marca: 'Tesla',
  modelo: 'Model S',
  placa: 'HEX-7777',
  ano: 2018,
  cor: 'preto',
  quantasPortas: 4,
  assentos: 5,
  quantidadePessoas: 0
}
```

### Crie um método chamado `mudarCor` que mude a cor do carro conforme a cor passado por parâmetro.
```js
carro.mudarCor = cor => carro.cor = cor;
```

### Crie um método chamado `obterCor`, que retorne a cor do carro.
```js
carro.obterCor = () => carro.cor;
```

### Crie um método chamado `obterModelo` que retorne o modelo do carro.
```js
carro.obterModelo = () => carro.modelo;
```

### Crie um método chamado `obterMarca` que retorne a marca do carro.
```js
carro.obterMarca = () => carro.marca;
```

### Crie um método chamado `obterMarcaModelo`, que retorne:
`"Esse carro é um [MARCA] [MODELO]"` 
Para retornar os valores de marca e modelo, utilize os métodos criados.
```js
carro.obterMarcaModelo = () => `Esse carro é um ${carro.obterMarca()} ${carro.obterModelo()}`
```

### Crie um método que irá adicionar pessoas no carro. Esse método terá as seguintes características:
- Ele deverá receber por parâmetro o número de pessoas entrarão no carro. Esse número não precisa encher o carro, você poderá acrescentar as pessoas aos poucos.
- O método deve retornar a frase: "Já temos [X] pessoas no carro!"
- Se o carro já estiver cheio, com todos os assentos já preenchidos, o método
deve retornar a frase: "O carro já está lotado!"
- Se ainda houverem lugares no carro, mas a quantidade de pessoas passadas por parâmetro for ultrapassar o limite de assentos do carro, então você deve
mostrar quantos assentos ainda podem ser ocupados, com a frase:
"Só cabem mais [QUANTIDADE_DE_PESSOAS_QUE_CABEM] pessoas!"
- Se couber somente mais uma pessoa, mostrar a palavra "pessoa" no retorno
citado acima, no lugar de "pessoas".
```js
carro.adicionarPessoas = qtd => {
  var totalDePessoas = carro.quantidadePessoas + qtd
  var sobra = carro.assentos - carro.quantidadePessoas;
  if (carro.quantidadePessoas === carro.assentos && totalDePessoas >= carro.assentos) {
    return 'O carro já está lotado'
  }
  else if (qtd > sobra) {
    var plural = sobra === 1 ? 'pessoa' : 'pessoas';
    return `Só cabem mais ${sobra} ${plural}!`
  }
  carro.quantidadePessoas += qtd
  return `Já temos ${carro.quantidadePessoas} pessoas no carro!`
}
```

### Agora vamos verificar algumas informações do carro. Para as respostas abaixo, utilize sempre o formato de invocação do método (ou chamada da propriedade), adicionando comentários _inline_ ao lado com o valor retornado, se o método retornar algum valor.

### Qual a cor atual do carro?
```js
carro.obterCor(); // 'preto'
```

### Mude a cor do carro para vermelho.
```js
carro.mudarCor('vermelho');
```

### E agora, qual a cor do carro?
```js
carro.obterCor(); // 'vermelho'
```

### Mude a cor do carro para verde musgo.
```js
carro.mudarCor('verde musgo');
```

### E agora, qual a cor do carro?
```js
carro.obterCor(); // 'verde musgo'
```

### Qual a marca e modelo do carro?
```js
carro.obterMarcaModelo(); // 'Esse carro é um Tesla Model S'
```

### Adicione 2 pessoas no carro.
```js
carro.adicionarPessoas(2); // 'Já temos 2 pessoas no carro!'
```

### Adicione mais 4 pessoas no carro.
```js
carro.adicionarPessoas(4); // 'Só cabem mais 3 pessoas!'
```

### Faça o carro encher.
```js
carro.adicionarPessoas(3); // 'O carro já está lotado'
```

### Tire 4 pessoas do carro.
```js
carro.adicionarPessoas(-4); // 'Já temos 1 pessoas no carro!'
```

### Adicione 10 pessoas no carro.
```js
carro.adicionarPessoas(10); // 'Só cabem mais 4 pessoas!'
```

### Quantas pessoas temos no carro?
```js
carro.quantidadePessoas; // 1
```
