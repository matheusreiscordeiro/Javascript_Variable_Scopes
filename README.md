# Javascript_Variable_Scopes

<br/>

Escopo em JavaScript refere-se ao alcance em que uma variável ou função pode ser acessada dentro do código. Existem dois tipos principais de escopo em JavaScript: escopo global e escopo local.

O escopo global refere-se a uma variável ou função que pode ser acessada de qualquer lugar dentro do código. Já o escopo local refere-se a uma variável ou função que só pode ser acessada dentro do bloco em que foi definido.

Aqui estão alguns exemplos de como o escopo funciona em JavaScript:

<br/>

> **Global**:

<br/>

```
let x = 5; // Variável global

function myFunction() {
  console.log(x); // A variável global x pode ser acessada dentro da função
}

myFunction(); // Output: 5
console.log(x); // Output: 5
```

<br/>

Neste exemplo, a variável x é definida fora da função myFunction(), tornando-a uma variável global que pode ser acessada de qualquer lugar dentro do código.

> **Função**:

<br/>

```
function myFunction() {
  let x = 5; // Variável local
  console.log(x); // A variável local x pode ser acessada dentro da função
}

myFunction(); // Output: 5
console.log(x); // Erro: x não está definida
```

<br/>

Neste exemplo, a variável x é definida dentro da função myFunction(), tornando-a uma variável local que só pode ser acessada dentro do bloco da função. Quando a função termina, a variável x é destruída e não pode ser mais acessada.

É importante observar que o escopo em JavaScript é baseado em blocos, o que significa que a variável pode ser acessada em qualquer bloco interno, mas não em blocos externos. Por exemplo:

<br/>

> **Bloco**:

<br/>

```
let x = 5;

if (x === 5) {
  let y = 10; // Variável local dentro do bloco if
  console.log(y); // Output: 10
}

console.log(y); // Erro: y não está definida fora do bloco if
```

<br/>

Neste exemplo, a variável y é definida dentro do bloco if, tornando-a uma variável local que só pode ser acessada dentro do bloco. Quando a execução sai do bloco, a variável y é destruída e não pode ser mais acessada fora dele.
