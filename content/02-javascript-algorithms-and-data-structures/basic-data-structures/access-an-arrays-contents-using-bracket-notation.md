---
id: 5a661e0f1068aca922b3ef17
title: Acessando o conteúdo de um Array usando notação de colchetes
challengeType: 1
forumTopicId: 301149
dashedName: access-an-arrays-contents-using-bracket-notation
---

# --descrição--
A característica fundamental de toda estrutura de dados é, evidentemente, não só a possibilidade de armazenar dados, mas também a possibilidade de visualizar este dado por um determinado comando. Então, agora que aprendemos como criar um array, comecemos a pensar como acessaremos os dadps no interior dele.

Quando definimos um simples array como o debaixo, há três ítens dentro dele:

```js
let ourArray = ["a", "b", "c"];
```

Em um array, cada ítem tem um <dfn>índice</dfn>. Esse índice corresponde à sua posição no array e como você faz referência à ele. Entretanto, é importante ressaltar que o array no JavaScript começam com índice 0, nos informando que o primeiro elemento do array é o elemento da posição ***zero***, não 1. Para buscar um elemento de um array pôr o valor de seu índice entre conchetes e adicionar ao final do nome que usamos para definir o array. Isso é conhecido como <dfn>Notaçao de colchetes</dfn>. Por exemplo, se quisermos receber o valor `"a"` do ourArray e definir como valor de uma variável, podemos escrever o seguinte código:

```js
let ourVariavel = ourArray[0];
// ourVariavel é igual a "a"
```

Além de acessar o valor associado ao índice, você também pode determinar o valor de um elemento através de seu índice, da seguinte forma:

```js
ourArray[1] = "not b anymore";
// ourArray agora é ["a", "not b anymore", "c"];
```

Usando esta notação agora nós alteramos o valor do ítem de índice 1 de `"b"` para `"not b anymore"`.

# --instruções--

Para completar este desafio, defina a segunda posição (índice `1`) do `myArray` para o que quiser, que não seja `"b"`.

# --dicas--

`myArray[0]` deve ser igual a `"a"`

```js
assert.strictEqual(myArray[0], 'a');
```

`myArray[1]` não pode ser igual a `"b"`

```js
assert.notStrictEqual(myArray[1], 'b');
```

`myArray[2]` deve ser igual a `"c"`

```js
assert.strictEqual(myArray[2], 'c');
```

`myArray[3]` deve ser igual a `"d"`

```js
assert.strictEqual(myArray[3], 'd');
```

# --seed--

## --seed-contents--

```js
let myArray = ["a", "b", "c", "d"];
// Only change code below this line

// Only change code above this line
console.log(myArray);
```

# --solutions--

```js
let myArray = ["a", "b", "c", "d"];
myArray[1] = "e";
```
