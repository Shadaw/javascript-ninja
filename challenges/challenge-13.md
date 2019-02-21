### Crie um array e mostre no console a representação em String desse array, usando o método visto na aula 13.
```js
let arr = ['g', 'u', 's', 't', 'a', 'v', 'o'];
console.log( 'O array em formato de string é:' );
console.log(arr.toString());
// g,u,s,t,a,v,o
```

### Crie 2 arrays `sul` e `sudeste`, que serão as regiões do Brasil. Cada array deve conter os estados dessa região.
```js
let sul = [ 'Paraná', 'Santa Catarina', 'Rio Grande do Sul' ];
let sudeste = ['Espirito Santo', 'Minas Gerais', 'Rio de Janeiro', 'São Paulo'];
```

### Crie uma variável chamada `brasil`, que irá receber as duas regiões concatenadas. Mostre o `brasil` no console.
```js
let brasil = sul.concat(sudeste);
console.log( '\nAlguns Estados do Brasil:' );
console.log(brasil);
// Alguns Estados do Brasil:
// [ 'Paraná',
//   'Santa Catarina',
//   'Rio Grande do Sul',
//   'Espirito Santo',
//   'Minas Gerais',
//   'Rio de Janeiro',
//   'São Paulo' ]
```

### Adicione 3 novos estados da região Norte no início do array e mostre no console.
```js
console.log( '\nMais estados adicionados:' );
// ?
```

### Remova o primeiro estado do array `brasil` e mostre-o no console.
```js
console.log( '\nEstado removido:' );
// ?
```

### Crie um novo array chamado `newSul`, que receba somente os estados do sul, pegando do array `brasil`. Não remova esses itens de `brasil`.
```js
// ?
```

### Mostre no console os estados que estão em `newSul`.
```js
console.log( '\nEstados do Sul do Brasil:' );
// ?
```

### Mostre no console todos os estados que estão em `brasil`.
```js
console.log( '\nAlguns Estados do Brasil:' );
// ?
```

### Crie um novo array chamado `nordeste`, que tenha os estados do nordeste.
```js
// ?
```

### Mostre no console os estados do nordeste.
```js
console.log( '\nEstados do Nordeste:' );
// ?
```

### Remova de `brasil` os estados do `sudeste`, colocando-os em uma variável chamada `newSudeste`.
```js
// ?
```

### Adicione os estados do `nordeste` ao array `brasil`. Esses estados devem ficar no mesmo nível que os estados já existentes, não em um array separado.
```js
// ?
```

### Mostre no console os estados em `newSudeste`.
```js
console.log( '\nEstados em newSudeste:' );
// ?
```

### Mostre no console os estados do `brasil`.
```js
console.log( '\nAlguns estados do Brasil:' );
// ?
```

### usando forEach, percorra o array `brasil` e gere um novo array chamado `newBrasil`. Esse array deve ter cada item como um objeto, com as propriedades:
- `id`: que será o índice do array `brasil`,
- `estado`: que será o estado do array `brasil`.
```js
// ?
```

### Mostre o array `newBrasil` no console
```js
console.log( '\nnewBrasil:' );
// ?
```

### Percorra o array `brasil` e verifique se os estados tem mais de 7 letras cada, atribuindo o resultado à uma variável. Se tiver, mostre no console a frase: 
- "Sim, todos os estados tem mais de 7 letras!"
### Senão, mostre no console:
- "Nem todos os estados tem mais de 7 letras!"
```js
console.log( '\nTodos os estados de `brasil` tem mais de 7 letras?' );
// ?
```

### Percorra o array `brasil` e verifique se o Ceará está incluído, atribuindo o resultado à uma variável. Se esse estado existir no array, mostrar a frase no console:
- "Ceará está incluído!"
### Senão, mostrar a frase:
- "Ceará não foi incluído :("
```js
console.log( '\nCeará está incluído em `brasil`?' );
// ?
```

### Percorra o array `newBrasil` e crie um novo array que some 1 no ID de cada objeto desse array, e adicione a frase abaixo na propriedade `estado`:
- `"[ESTADO] pertence ao Brasil."`
Atribua o novo array a uma variável chamada `map`.
```js
// ?
```

### Mostre no console o array criado acima:
```js
console.log( '\nnewBrasil agora com mais informações:' );
// ?
```

### Filtre o array criado acima, retornando somente os estados que tiverem ID par. Atribua o valor à uma variável chamada `filter`.
```js
// ?
```

### Mostre o array filtrado acima no console.
```js
console.log( '\nEstados com ID par:' );
// ?
```
