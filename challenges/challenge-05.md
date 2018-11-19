### Crie uma variável qualquer, que receba um array com alguns valores aleatórios
- ao menos 5 - (fica por sua conta os valores do array).
```js
var arr = ['gustavo', 12, 5, 2, 1.7];
```

### Crie uma função que receba um array como parâmetro, e retorne esse array.
```js
const myFunction = arg => arg;
```

### Imprima o segundo índice do array retornado pela função criada acima.
```js
myFunction(arr)[1]; // 12
```

### Crie uma função que receba dois parâmetros: o primeiro, um array de valores; e o segundo, um número. A função deve retornar o valor de um índice do array que foi passado no primeiro parâmetro. O índice usado para retornar o valor, deve ser o número passado no segundo parâmetro.
```js
const otherFunction = (arg, indice) => arg[indice];
```

### Declare uma variável que recebe um array com 5 valores, de tipos diferentes.
```js
var arr = ['string', 2, 7.5, false, null];
```

### Invoque a função criada acima, fazendo-a retornar todos os valores do último array criado.
```js
otherFunction(arr, 0) // 'string'
otherFunction(arr, 1) // 1
otherFunction(arr, 2) // 7.5
otherFunction(arr, 3) // false
otherFunction(arr, 4) // null
```

### Crie uma função chamada `book`, que recebe um parâmetro, que será o nome do livro. Dentro dessa função, declare uma variável que recebe um objeto com as seguintes características:
- esse objeto irá receber 3 propriedades, que serão nomes de livros;
- cada uma dessas propriedades será um novo objeto, que terá outras 3
propriedades:
    - `quantidadePaginas` - Number (quantidade de páginas)
    - `autor` - String
    - `editora` - String
- A função deve retornar o objeto referente ao livro passado por parâmetro.
- Se o parâmetro não for passado, a função deve retornar o objeto com todos
os livros.
```js
function book(pLivro) {
    let livros = {
        aGameOfThrones: {
            quantidadePaginas: 694,
            autor: 'George R. R. Martin',
            editora: 'Bantam Spectra'
        },
        fightClub: {
            quantidadePaginas: 208,
            autor: 'Chuck Palahniuk',
            editora: 'W. W. Norton'
        },
        javascriptEloquente: {
            quantidadePaginas: 472,
            autor: 'Marijn Haverbeke',
            editora: 'No Starch Press'
        }
    }
    if (pLivro !== undefined) {
        return livros[pLivro];
    }
    return livros
}
```

### Usando a função criada acima, imprima o objeto com todos os livros.
```js
book()
```

### Ainda com a função acima, imprima a quantidade de páginas de um livro qualquer, usando a frase:
`"O livro [NOME_DO_LIVRO] tem [X] páginas!"`
```js
console.log(`O livro 'A Game of Thrones' tem ${book('aGameOfThrones').quantidadePaginas} paginas!`);
```

### Ainda com a função acima, imprima o nome do autor de um livro qualquer, usando a frase:
`"O autor do livro [NOME_DO_LIVRO] é [AUTOR]."`
```js
console.log(`O autor do livro 'Fight Club' é ${book('fightClub').autor}.`)
```

### Ainda com a função acima, imprima o nome da editora de um livro qualquer, usando a frase:
`"O livro [NOME_DO_LIVRO] foi publicado pela editora [NOME_DA_EDITORA]."`
```js
console.log(`O livro 'Javascript Eloquente' foi publicado pela editora ${book('javascriptEloquente').editora}.`)
```