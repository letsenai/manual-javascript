# Manual Básico de JavaScript para Web

## ➤ Introdução

### O que é JavaScript?

JavaScript é uma linguagem de programação utilizada para tornar páginas web interativas. Com ela, dá pra clicar em coisas, preencher formulários e ver mudanças na hora, sem precisar recarregar a página. Deixa tudo mais dinâmico e menos parado.

### Para que serve?

⭑ Criar interatividade em páginas web

⭑ Responder ações do usuário

⭑ Manipular elementos HTML

⭑ Validar formulários

⭑ Alterar estilos dinamicamente


### Relação com HTML e CSS

HTML = estrutura da página

CSS = aparência e estilo

JavaScript = comportamento e interatividade


## ➤ Formas de uso no HTML

### JavaScript dentro do HTML

꒰ ✉︎ ꒱ Pasta: ``` 01_script_no_html ```

HTML

```
<!DOCTYPE html>
<html>
<head>

  <title>Exemplo</title>

</head>
<body>

<button onclick="mostrarMensagem()">Clique aqui</button>

<script>
function mostrarMensagem() {
  alert("Hello World!");
}
</script>

</body>
</html>
```
### JavaScript em arquivo separado

꒰ ✉︎ ꒱ Pasta: ``` 02_script_externo ```

HTML

```
<script src="script.js"></script>

JavaScript (script.js):

function mostrarMensagem() {
  alert("Hello World!");
}
```

## ➤ Variáveis, tipos e escopo

### O que é uma variável?

É uma caixinha onde você guarda informações na memória, usado para armazenar um valor.

### Declaração de variáveis

```
var nome = "Ewerton";
let idade = 20;
const cidade = "Santa Catarina";
```

### Diferença entre var, let e const

var = escopo global ou de função

let = escopo de bloco

const = valor constante (não pode ser alterado)


### Exemplos 

**Exemplo com var**

```
var x = 10;
console.log(x);
```

**Exemplo com let**

```
let y = 20;
console.log(y);
```

**Exemplo com const**

```
const z = 30;
console.log(z);
```

## ➤ Escopo

### Escopo global

```
var a = 1;

function teste() {
   console.log(a);
}
```

### Escopo de função

```
function exemplo() {
  let x = 10;
  console.log(x);
 }

console.log(x); // erro: fora da função
```

A variável "x" foi criada dentro da função e não pode ser usada fora dela.

### Escopo de bloco

```
if (true) {
 let b = 2;
 console.log(b);
}

console.log(b); // erro: fora do bloco
```

A variável "b" só existe dentro do bloco.

### Var fora do bloco

```
var numero = 10;
if (true) {
 var numero = 20;
}

console.log(numero); 
```

var não respeita escopo de bloco, por isso o valor foi alterado.

## ➤ Operadores, comparações e lógica

### Operadores aritméticos

⭑ Adição (+): Soma dois valores. Também usado para concatenar strings.

⭑ Subtração (-): Subtrai o segundo operando do primeiro.

⭑ Multiplicação (*): Multiplica dois valores.

⭑ Divisão (/): Divide o primeiro operando pelo segundo.

### Comparações

console.log(5 == "5"); // true 

console.log(5 === "5"); // false 

console.log(5 != "5"); // false 

console.log(5 !== "5"); // true


⤷ **==** compara só o valor, enquanto **===** compara o valor e o tipo também.

⤷ O **===** é mais seguro porque evita confusão, já que não considera iguais coisas que têm tipos diferentes, tipo número e string.

### Operadores lógicos

⭑ E = &&

⭑ OU = ||

⭑ NÃO = !

## ➤ Estruturas condicionais

if

```
let idade = 18;

if (idade >= 18) {
console.log("Maior de idade");
}
```

if...else

```
if (idade >= 18) {
  console.log("Maior");
} else {
  console.log("Menor");
}
```
switch

```
let cor = "azul";

switch (cor) {
  case "azul":
    console.log("Cor azul");
    break;
  default:
    console.log("Outra cor");
}
```

### ➤ Estruturas de repetição

for

```
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

while

```
let i = 0;

while (i < 5) {
  console.log(i);
  i++;
}
```

### ➤ Funções

### O que é uma função?
















