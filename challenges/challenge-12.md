### Crie um objeto chamado `person`, com as propriedades:
  - `name`: String
  - `lastname`: String
  - `age`: Number

Preencha cada propriedade com os seus dados pessoais, respeitando o tipo
de valor para cada propriedade.
```js
let person = {
  name: "Gustavo",
  lastname: "Alexandre",
  age: 18
}
```

### Mostre no console, em um array, todas as propriedades do objeto acima. Não use nenhuma estrutura de repetição, nem crie o array manualmente.
```js
console.log( 'Propriedades de "person":' );
console.log(Object.keys(person));
// [ 'name', 'lastname', 'age' ]
```

### Crie um array vazio chamado `books`.
```js
let books = [];
```

### Adicione nesse array 3 objetos, que serão 3 livros. Cada livro deve ter a
seguintes propriedades:
`name`: String
`pages`: Number
```js
books = [
  {
    name: "A Game of Thrones",
    pages: 694
  },
  {
    name: "javascript Eloquente",
    pages: 472
  },
  {
    name: "fight Club",
    pages: 208
  }
]
```

### Mostre no console todos os livros.
```js
console.log( '\nLista de livros:' );
console.log(books)
// [ { name: 'A Game of Thrones', pages: 694 },
//   { name: 'javascript Eloquente', pages: 472 },
//   { name: 'fight Club', pages: 208 } ]
```

### Remova o último livro, e mostre-o no console.
```js
console.log( '\nLivro que está sendo removido:' );
console.log(books.pop())
// { name: 'fight Club', pages: 208 }
```

### Mostre no console os livros restantes.
```js
console.log( '\nAgora sobraram somente os livros:' );
console.log(books);
// [ { name: 'A Game of Thrones', pages: 694 },
//   { name: 'javascript Eloquente', pages: 472 } ]
```

### Converta os objetos que ficaram em `books` para strings.
```js
books = JSON.stringify(books)
```

### Mostre os livros nesse formato no console:
```js
console.log( '\nLivros em formato string:' );
console.log(books);
// '[{"name":"A Game of Thrones","pages":694},{"name":"javascript Eloquente","pages":472}]'
```

### Converta os livros novamente para objeto.
```js
books = JSON.parse(books)
console.log( '\nAgora os livros são objetos novamente:' );
console.log(books);
// [ { name: 'A Game of Thrones', pages: 694 },
//   { name: 'javascript Eloquente', pages: 472 } ]
```

### Mostre no console todas as propriedades e valores de todos os livros, no formato abaixo:
`"[PROPRIEDADE]: [VALOR]"`
```js
for(let i = 0; i < books.length; i++) {
  for(let props in books[i]) {
    console.log(`${props} : ${books[i][props]}`)
  }
}
// name : A Game Of Thrones
// pages : 694
// name : javascript Eloquente
// pages : 472
```

### Crie um array chamado `myName`. Cada item desse array deve ser uma letra do seu nome. Adicione seu nome completo no array.
```js
let myName = ['g', 'u', 's', 't', 'a', 'v', 'o']
```

### Juntando todos os itens do array, mostre no console seu nome.
```js 
console.log( '\nMeu nome é:' );
console.log(myName.join(''))
// gustavo
```


### Ainda usando o objeto acima, mostre no console seu nome invertido.
```js
console.log( '\nMeu nome invertido é:' );
console.log(myName.reverse())
// [ 'o', 'v', 'a', 't', 's', 'u', 'g' ]
```

### Mostre todos os itens do array acima, odenados alfabéticamente.
```js
console.log( '\nAgora em ordem alfabética:' );
console.log(myName.sort())
// [ 'a', 'g', 'o', 's', 't', 'u', 'v' ]
```