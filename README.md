# π TypeScript μ²μ μμνκΈ°

νμμ€ν¬λ¦½νΈμ μ²« μλ¬Ένλ©΄μ λΈλ§λμ½λλμ κ°μ [Typescriptλ‘ λΈλ‘μ²΄μΈ λ§λ€κΈ°](https://nomadcoders.co/typescript-for-beginners/lobby)λ₯Ό λ€μΌλ©° μ€μ΅νκ³  μ λ¦¬ν κΈ°λ‘μλλ€.

</br></br>

## π typeScript β VScode

νμμ€ν¬λ¦½νΈμ vsμ½λκ° κ°μ λ§μ΄ν¬λ‘ μννΈμμ λ§λ€μκΈ° λλ¬Έμ νΈνμ΄ μμ£Όμλμ΄μ κ°λ°μ κ²½νμ΄ μ’λ€.

</br></br>

## β οΈ Why not JavaScript

- νμμ€ν¬λ¦½νΈλ μλ°μ€ν¬λ¦½νΈμ λΉν΄ **νμ μμ μ±**μ΄ μ’λ€. => κ°λ°μ κ²½νμ΄ μ’λ€. λ²κ·Έλ₯Ό μ€μΌ μ μλ€. λ°νμ μλ¬ μ€μΈλ€. μμ°μ± μ¦λμν¨λ€.
- μλ°μ€ν¬λ¦½νΈλ νμ μμ μ±μ΄ μλ€.
- μλ°μ€ν¬λ¦½νΈλ λλλ‘ μλ¬λ₯Ό λ³΄μ¬μ£Όμ§ μμΌλ € μμμ μ²λ¦¬νλ μΌμ΄ λ§λ€. μ΄κ² κ°λ°μμκ² λ³λ‘ λμμ΄ μλλ€.

```js
/*
π³ μλ°μ€ν¬λ¦½νΈλ μ΄λ κ² μ΄μν μ½λλ μ€νμμΌμ€λ€.
λ€λ₯Έ μΈμ΄μμ  κΏλ λͺ» κΏ μΌ
*/

[1, 2, 3, 4] + false; //'1,2,3,4false'
//λ°°μ΄ + λΆλ¦¬μΈ = μ€νΈλ§(λΆλ¦¬μΈλ μ€νΈλ§μΌλ‘ ν©μ³μ§)

function divide(a, b) {
  return a / b;
}
divide(2, 3); //0.6666666666666666
divide('xxxxxxxx'); //NaN (μ½λ μ€νμ λ§μμ£Όκ³  μμ§ μλ€. μ΄κ² μ€νλλ©΄ μλλ κ±°μ§π«!!)

//μΈμλ‘ μ«μλ₯Ό μ λ¬ν΄μΌ νλμ§ λ¬Έμλ₯Ό μ λ¬ν΄μΌνλμ§, λͺκ°μ μΈμλ₯Ό μ λ¬ν΄μΌνλμ§ μ΄λ°κ²λ€μ μ ν΄μ μλͺ»λ³΄λμΌλ©΄ μ²΄ν¬ν΄μΌ νλ€!!
```

- λ°νμ μλ¬λ μ½μ μμμ μΌμ΄λλ μλ¬μ΄λ€. (μ΄λ° μλ¬λ μ μ μ μ»΄ν¨ν°μμ μ½λκ° μ€νλ  λλ§ μΌμ΄λλ μλ¬μΌ μλ μλ€.)
- μλ°μ€ν¬λ¦½νΈ λ°νμ μ€λ₯λ μ μ λ λ§€λμ λ λλ£ κ°λ°μλ€μ΄ μμμ°¨λ¦¬κ³  μλ €μ£Όλ κ²½μ°κ° λ§λ€!

```js
const nico = { name: 'nico' };
nico.hello(); //Uncaught TypeError: nico.hello is not a function

/*μ§κΈμ²λΌ β οΈμ»΄ν¨ν°κ° μ€νμν€κ³  λμ μλ¬λ₯Ό μΆλ ₯νλ κ²μ΄ μλλΌβ οΈ
μ€νμν€κΈ° μ μ hello()λΌλ ν¨μκ° μλ€λ κ±Έ μλ €μ£Όκ³  β¨"κ³ μΉλ©΄ μ€νμμΌμ€κ²!"β¨κ° κ°μ₯ μ’λ€.*/
```

- **λ§λμλλ μ½λ**λ₯Ό **μ€νμ΄μλλΌ μμ± λ¨κ³λΆν°** λ°λ‘μ‘λ κ²! κ·Έκ² λ°λ‘ νμμ€ν¬λ¦½νΈκ° μλ°μ€ν¬λ¦½νΈλ³΄λ€ μ§νλ λ©΄μ΄λΌκ³  λ³Ό μ μλ€.

</br></br>

## π€ How TypeScript Works

- νμμ€ν¬λ¦½νΈλ strongly typed programmin language κ°λ ₯ν νμμ κ°μ§ νλ‘κ·Έλλ° μΈμ΄μ΄λ€.
- νμμ€ν¬λ¦½νΈλ‘ μμ±ν μ½λλ μλ°μ€ν¬λ¦½νΈλ‘ λ³νλλ€.[νμμ€ν¬λ¦½νΈ νλ μ΄κ·ΈλΌμ΄λ](https://www.typescriptlang.org/play?#code/PTAEHUFMBsGMHsC2lQBd5oBYoCoE8AHSAZVgCcBLA1UABWgEM8BzM+AVwDsATAGiwoBnUENANQAd0gAjQRVSQAUCEmYKsTKGYUAbpGF4OY0BoadYKdJMoL+gzAzIoz3UNEiPOofEVKVqAHSKymAAmkYI7NCuqGqcANag8ABmIjQUXrFOKBJMggBcISGgoAC0oACCbvCwDKgU8JkY7p7ehCTkVDQS2E6gnPCxGcwmZqDSTgzxxWWVoASMFmgYkAAeRJTInN3ymj4d-jSCeNsMq-wuoPaOltigAKoASgAywhK7SbGQZIIz5VWCFzSeCrZagNYbChbHaxUDcCjJZLfSDbExIAgUdxkUBIursJzCFJtXydajBBCcQQ0MwAUVWDEQC0gADVHBQGNJ3KAALygABEAAkYNAMOB4GRonzFBTBPB3AERcwABS0+mM9ysygc9wASmCKhwzQ8ZC8iHFzmB7BoXzcZmY7AYzEg-Fg0HUiQ58D0Ii8fLpDKZgj5SWxfPADlQAHJhAA5SASPlBFQAeS+ZHegmdWkgR1QjgUrmkeFATjNOmGWH0KAQiGhwkuNok4uiIgMHGxCyYrA4PCCJSAA)λ‘ μ€νν΄ λ³Ό μ μλ€.
- νμ€ β‘οΈ μμ€λ‘ λ³ννλ μ΄μ λ λΈλΌμ°μ μ Node.jsκ° νμ€κ° μλλΌ μμ€λ₯Ό μ΄ν΄νκΈ° λλ¬Έμ΄λ€.
- νμμ€ν¬λ¦½νΈκ° κ·Έμ  μλ°μ€ν¬λ¦½νΈλ₯Ό λ³νν΄ μ€ λΏμ΄λΌλ©΄ μ΄λ»κ² μ°λ¦¬λ₯Ό λ³΄νΈν΄ μ£Όλ κ±ΈκΉ?? β‘οΈ νμμ€ν¬λ¦½νΈ μ½λκ° μλ°μ€ν¬λ¦½νΈλ‘ λ³νλκΈ° **μ **μ νμ€κ° λ¨Όμ  μ°λ¦¬μ μ½λλ₯Ό νμΈν λ€μμ μμ€μμ λ°λ³΄κ°μ μ€μκ° μΌμ΄λμ§ μκ² λ³΄νΈμ₯μΉλ₯Ό λ°λμν¨λ€! **νμμ€ν¬λ¦½νΈ μ½λμ μλ¬κ° μμΌλ©΄ μμ€λ‘ μμ μ»΄νμΌμ΄ λμ§ μλλ€.** μ΄λ° λ³΄νΈμ₯μΉκ° μ μ κ° μ½λλ₯Ό μ€ννλ λ°νμμ λ°μνλ κ² μλλ€.

</br></br>

## π₯ Implicit Types vs Explicit Types

- μ΄λ€ μΈμ΄μμ  λ³μλ₯Ό μ€μ νλ€λ©΄ κ·Έ λ³μμ νμμ΄ λ­μ§ μ ν΄μ€μΌνλ€.(μ΄ λ³μλ ν­μ μ«μμ¬μΌν΄, λ¬Έμ₯μ΄μ΄μΌν΄ λ±) νμ€λ μ΄λ° μ κ·Όλ²μ + aλ₯Ό μΆκ°νλ€.
- νμμ€ν¬λ¦½νΈλ **λ°μ΄ν°μ λ³μμ νμμ λͺμμ μΌλ‘ μ μνλ λ°©λ²**μ μ¨λ, μλλ©΄ **κ·Έλ₯ JavaScriptμ²λΌ λ³μλ§ μμ±νκ³  λμ΄κ°λ** λλ€. μ΄λλ νμ€κ° νμμ μΆλ‘ ν΄ μ€λ€!!π

```js
//π νμ€μ μλ νμ μΆλ‘  κΈ°λ₯ νμ©νκΈ° (Implicit)

let a = 'hello'; //μ΄λ κ² μ μ΄μ€λ νμ€κ° μμμ "μ! aλ string νμμ΄κ΅¬λ!!"ν¨
a = 'bye'; //κ°μ string νμμΌλ‘ λ°κΎΈκΈ° λλ¬Έμ νμ€κ° λΆν μν¨
a = 1; //stringμμ numberνμμΌλ‘ λ°κΎΈλ €λκΉ νμ€κ° λΆνν¨π‘

//π νμ€μκ² μΉμ νκ² νμ μλ €μ£ΌκΈ° (Explicit)

let b: boolean = 'x'; // bλ booleanνμμ΄μ΄μΌ νλ€κ³  μλ €μ€¬λλ° string λ£μΌλκΉ νμ€κ° λΆννλ€.π‘

//νμ§λ§ κ²°κ΅­ μλμ λ μ½λλ κ°μΌλ―λ‘, λλλ‘ μ§§μ μͺ½μ μ ννλ κ²μ μΆμ²νλ€.
let c = false; //π μΆμ² (Implicit)
let c: boolean = false;
```

- νμ§λ§ λͺμμ (explicit) νμλ μ μ©νκ² μ°μΈλ€. (μλ₯Ό λ€μ΄ λ¨Όμ  κ°μ ν λΉνμ§ μμ κ²½μ°μ νμμ λͺμν΄μ€μΌ νλ€.)

```js
//beforeπ©
let a = [];
a.push('1');
a.push(2); //νμ€μ λ³΄νΈλ₯Ό λͺ»λ°μ β‘οΈ μλ¬κ° λμ§ μλλ€.π

//afterβ¨
let b: number[] = []; //number arrλΌκ³  λ―Έλ¦¬ μ μΈνλ€.
b.push('1'); //νμ€μ λ³΄νΈλ₯Ό λ°μ β‘οΈ μλ¬κ° λλ€.π
b.push(2);
```

</br></br>

## π± Types of TS

### π£ basic νμ

- μ§κΈκΉμ§ λ±μ₯ν κΈ°λ³Έμ μΈ νμλ€μ μ¬μ©λ²μ μλμ κ°λ€.

```js
//Implicit Types π
let a = 1;
let b = 'i1';
let c = true;
let d = [1, 2];
let e = ['i1', '2'];
let f = [true, false];

//Explicit Types (νμν κ²½μ°κ° μλλΌλ©΄ Implicit Types μΆμ²)
let a: number = 1;
let b: string = 'i1';
let c: boolean = true;
let d: number[] = [1, 2];
let e: string[] = ['i1', '2'];
let f: boolean[] = [true, false];
```

</br>

### π£ κ°μ²΄μ νμ

- κ°μ²΄μ νμμ κΈ°λ³Έμ μΌλ‘ `let name: {key: type;} = {key: value;}`μμΌλ‘ μ μ μ μλ€.
- κ°μ²΄ λ΄λΆμ ν€κ° μμ μλ μμ μλ, μλ€λ©΄ μ΄λ€ νμμΌλ‘ μ‘΄μ¬ν  κ±΄μ§ μ νλ €λ©΄ `key?: type`λ₯Ό μ μΌλ©΄ λλ€.

```js
let player: {
  name: string,
  age?: number, //β = playerμ ageλ₯Ό κ°μ§ μλ, μλ μλ μλ€.
} = {
  name: 'nico', //βλ₯Ό μ¨μ€μ ageλ₯Ό μ§μ νμ§ μμλ μλ¬κ° λμ§ μλλ€.
};

// βοΈ if(player.age < 10){ //βλ₯Ό μ¨μ€¬κΈ° λλ¬Έμ, undefinedκ° λμ€λ©΄ μ λλ‘ λΉκ΅λ₯Ό ν  μ μλ€. β‘οΈ μλ¬κ° λλ€.π
if (player.age && player.age < 10) {
  // λ¨Όμ  μ²΄ν¬λΆν° ν΄μ€λ€λ μ‘°κ±΄μ λ£μΌλ©΄ ν΅κ³Ό so sweet...π¬ λ€μ ν΄..
}

player.age = 3;
player.age = '3'; //νμ€μ λ³΄νΈλ₯Ό λ°μ β‘οΈ μλ¬κ° λλ€.π
```

</br>

### π£ Alias νμ

- κ°μ λͺ¨μκ³Ό νμμ κ°μ²΄λ₯Ό μ¬λ¬κ° λ§λ€λ, μμ κ°μ λ°©μμ μ½λ μ€λ³΅μ΄ λ§μ΄ μΌμ΄λλ€. μ΄λλ λ°λ‘ κ°μ²΄ μ μ²΄λ₯Ό νμμΌλ‘ μ§μ νμ¬ μ°λ λ°©λ²λ μλ€.
- μ΄λ° λ°©λ²μ΄ λ°λ‘ **Alias νμ**μ΄λΌκ³  νλ€.

```js
// π§Ή Alias νμμΌλ‘ κ°μ²΄ νν μμ²΄λ₯Ό νμμΌλ‘ μ§μ νκΈ°
type Age = number;
type Name = string;
type Player = {
  //uppercase λ‘ typeμ μ§μ νλκ² κ΄λ‘
  name: string, //1οΈβ£name: Name κ°λ₯
  age?: number, //2οΈβ£age?: Age κ°λ₯
  /*
  μμμ Ageμ Namgeμ νμμ λ°λ‘ Alias νμμΌλ‘ μ ν΄μ€¬κΈ° λλ¬Έμ
  1οΈβ£μ΄λ2οΈβ£μ κ°μ ννλ κ°λ₯νλ€.
  */
};

let nico: Player = {
  name: 'nico',
};
let lynn: Player = {
  name: 'lynn',
  age: 3,
};
```

</br>

### π£ ν¨μ νμ

- ν¨μκ° λ¦¬ν΄νλ κ°μ νμμ μ ν΄μ€μ μμ μ μΈ ν¨μλ₯Ό λ§λ€ μλ μλ€.
- λ¬Όλ‘  ν¨μμ μΈμκ° λ°μ νμλ μ§μ ν  μ μλ€.

```js
//π© before
function playerMaker(name: string) {
  return {
    name,
  };
}

const nico = playerMaker('nico');
nico.age = 12; //ageλΌλ νλ‘νΌν°λ₯Ό return κ°μ μ μν΄ λμ§ μμμ μ€λ₯λ¨

//β¨ after
type Player = {
  name: string,
  age?: number,
};
function playerMaker(name: string): Player {
  //π₯return ν  κ°μ²΄κ° Player νμμ κ°κ² λ  κ²μ΄λΌκ³  μλ €μ£ΌκΈ°
  return {
    name,
  };
}

const nico = playerMaker('nico');
nico.age = 12; //ageλΌλ νλ‘νΌν°λ₯Ό return κ°μ μ μν΄ λμ§ μμμ μ€λ₯λ¨

//π arrow function ver.
type Player = {
  name: string,
  age?: number,
};
const playerMaker = (name: string): Player => ({ name });
const nico = playerMaker('nico');
nico.age = 12;
```

</br>

### π£ readonly μμ±μ΄ ν¬ν¨λ νμ

- `readonly`μμ±μ μ€μ μμλ€μ **μ½κΈ° μ μ©**μΌλ‘ λ§λ€ μ μλ€.

```js
type Player = {
  readonly name: string; //π μ½κΈ° μ μ© μ΅μ μΆκ°
  age?: number;
};
const playerMaker = (name:string) : Player => ({name})
const nico = playerMaker("nico")
nico.age = 12
nico.name = "las" //readonlyμΈλ° nameμ λ°κΎΈλ €λκΉ β‘οΈ μλ¬λ΄μ μλ €μ€π
```

- μ΄ readonly κ°λ₯μ λ°°μ΄μ΄λ stringμμλ μμ£Ό μ μ©νλ€.

```js
const numbers: readonly number[] = [1,2,3,4]
numbers.push(1) //readonlyμΈλ° μΆκ°νλ €νλκΉ β‘οΈ μλ¬λ΄μ μλ €μ€π

const names : readonly string[] = ["nico","lynn"]
names.push('las') //readonlyμΈλ° μΆκ°νλ €νλκΉ β‘οΈ μλ¬λ΄μ μλ €μ€π
names.filter(name => name === "nico" ? true : false) //πfilterλ map λ± μ immutableμ΄λ―λ‘ readonlyμ μλ°°λμ§ μμμ μ€λ₯λ₯Ό λ΄μ§ μλλ€.
```

</br>

### π£ Tuple

- tupleμ μ΅μ lengthκ° λͺμ΄κ³ , νΉμ  μμΉμ νΉμ  νμμ΄ μμ΄μΌ νλ λ°°μ΄ μ‘°κ±΄μ κ±Έ μ μλ€.

```js
const player: [string, number, boolean] = ['nico', 12, false];
//μ΅μ 3κ°μ μμλ₯Ό κ°μ ΈμΌνλ€.
//μμμ μμλ μ°¨λ‘λλ‘ string,number,booleanμ΄μ΄μΌ νλ€.
player[0] = 1; //stringμλ¦¬μ numberμΆκ° β‘οΈ μλ¬λ΄μ μλ €μ€π
```

- tupleμμλ `readonly`μ΅μμ κ²°ν©ν  μ μλ€.

```js
const player: readonly [string, number, boolean] = ['nico', 12, false]
player[0] = 'hi'
```

</br>

### π£ undefined, null κ·Έλ¦¬κ³  any νμ

```js
let a: undefined = undefined; //undefinedμ νμμ undefinedμ΄λ€.
let b: null = null; //nullμ νμμ nullμ΄λ€.
```

- any νμμ TypeScriptλ‘ λΆν° νμΆνλ νμΆκ΅¬μ΄λ€.
- κ°λμ©μ anyλ₯Ό μ¨μΌν  λλ μλ€ but!! anyλ₯Ό μΈκ±°λ©΄ λ­νλ¬ νμ€λ₯Ό μ°λ μΆμ΄ κΆμ₯νμ§ μλλ€.ππ»

```js
let c: any; //ν λΉλμ§ μμ λ³μλ anyλΌλ νμμ΄ λλ€. === let c
let d = []; //μλ¬΄ νμλ μ νμ§ μμ λ°°μ΄μ any[] νμμ΄λλ€.

const e: any[] = [1, 2, 3, 4];
const f: any = true;
e + f; //μ΄κ² κ°λ₯ν΄μ§λ€. κ·Έλ₯ jsμ²λΌ
```

</br>

### π£ unknown νμ

- λ§μ½ apiλ‘ λΆν° μλ΅μ λ°λλ° κ·Έ νμμ΄ λ­μ§ λͺ¨λ₯Έλ€λ©΄ `unknown`νμμ μΈ μ μλ€.
- anyνμκ³Ό λΉμ·νμ§λ§ anyλ³΄λ€ unknownμ΄ λ μμ νλ€. μ΄μ λ unknownκ°μΌλ‘ μμμ μννλ κ²μ ν©λ²μ μ΄μ§ μκΈ° λλ¬Έ

```js
//π© before
let a: unknown;
let b = a + 1; //λ­κ° λ€μ΄μ¬μ§ λͺ¨λ₯΄λλ° λνλ€κ³ ? β‘οΈ μ νμ€λ λ°λμΌπ

//β¨ after
let a: unknown;
if (typeof a === 'number') {
  let b = a + 1;
}
if (typeof a === 'string') {
  let b = a.toUpperCase();
}
```

</br>

### π£ void νμ

- void > unknown > never μμΌλ‘ μμ£Ό μ°μ.
- voidλ μλ¬΄κ²λ return νμ§ μλ ν¨μμ ν΄λΉνλ νμμ΄λ€.
- ν¨μμ return λ¬Έμ΄ μκ±°λ ν΄λΉ return λ¬Έμμ λͺμμ  κ°μ λ°ννμ§ μμ λ ν­μ μ μΆλλ νμμ΄λ€.

```js
function hello() {
  console.log('this function is void type!');
}
hello().toUpperCase(); //μλ¬΄κ²λ λ¦¬ν΄μνλλ° λλ¬Έμλ‘ λ°κΎΌλ€κ³ ? β‘οΈ μ νμ€λ λ°λμΌπ

//μ°Έκ³ λ‘ μλμ κ°μΌλ―λ‘ κ΅³μ΄ μλμ²λΌ λͺμν  νμκ° μλ€.
function hello(): void {
  console.log('this function is void type!');
}
```

</br>

### π£ never νμ

- κ±°μ μΈμΌ μμΌλ μμλκΈ°
- neverλ ν¨μκ° μ λ returnνμ§ μμ λ λ°μνλ€.
- ν¨μκ° μμΈλ₯Ό throwνκ±°λ νλ‘κ·Έλ¨ μ€νμ μ’λ£ν¨μ μλ―Ένλ€.

```js
//π© before
function hello(): never {
  return 'X'; //μ λλ‘ return νλ©΄ μλλλ° μ λ¦¬ν΄ν΄? β‘οΈ μ νμ€λ λ°λμΌπ
}

//β¨ after
function hello(): never {
  throw new Error('X'); //return νμ§ μκ³  μ€λ₯λ₯Ό λ°μμν€λ ν¨μλκΉ okay
}
```

- λλ `never`μ νμμ΄ λκ°μ§ μΌ μλ μλ μν©μ λ°μν  μ μλ€.

```js
function hello(name: string | number) {
  //helloλΌλ ν¨μκ° μΈμλ‘ string νΉμ numberμΈ nameμ μΈμλ‘ λ°μ
  if (typeof name === 'string') {
    name; //πμ΄ nameμ νμμ 'string'μ΄λ€.
  } else if (typeof name === 'number') {
    name; //πμ΄ nameμ νμμ 'number'μ΄λ€.
  } else {
    //μΈμκ° λ§κ² λ€μ΄μ€λ©΄ μ΄ μ½λλ μ λ μ€νλμ§ μμμΌ νλ€.
    name; //πμ΄ nameμ νμμ β¨'never'β¨μ΄λ€.
  }
}
```

</br></br>

## π functions

### π Call Signature

- call signatrueλ κΈ°λ³Έμ μΌλ‘ λ§μ°μ€λ₯Ό μ¬λ Έμ λ λ³΄κ²λλ μ‘°κ±΄λ€μ λ§νλ€.μ΄λ»κ² ν¨μλ₯Ό νΈμΆν΄μΌνλμ§ μλ €μ€λ€.μΈμμ νμκ³Ό λ°ν νμμ μλ €μ€λ€.
  ![call signature](./call-signature.png)
- call signatureλ₯Ό λ¨Όμ  μ μΈνλ€ = νμμ λ¨Όμ  μ μΈνλ€.
- ν¨μλ₯Ό κ΅¬ννκΈ° μ μ μΈμμ λ¦¬ν΄μ νμλΆν° μ νλ λ°©λ²μ κΉλνλ€. μ²«λ²μ§Έλ‘ νμμ μκ°νλλ‘ ν΄μ£Όκ³ , κ·Έ λ€μ κ΅¬μ²΄μ μΌλ‘ μ½λλ₯Ό μ μΌλ©΄, νμμ΄ μ€μ  μ½λλ λΆλ¦¬λμ κ°λμ±λ μ’λ€.

```js
type Add = (a: number, b: number) => number; //πcall signatures
// type Add = {
//     (a:number,b:number) : number;
// } //μ΄λ κ² μ μν  μλ μμ.
const add: Add = (a, b) => a + b;
//λμ΄μ μΈμμ return κ°μ νμμ μ μ΄μ£Όμ§ μμλ λλ€.
```

</br>

### π Overloading

- μΈλΆ ν¨ν€μ§λ λΌμ΄λΈλ¬λ¦¬λ₯Ό μ¬μ©ν  λ, κ·Έ μΉκ΅¬λ€μ΄ μ€λ²λ‘λ©μ μμ²­ λ§μ΄ μ. λλ¬Έμ μ°λ¦¬κ° μ€λ²λ‘λ©μ μ§μ  μμ±νμ§ μμλ μμλλ κ²μ΄ μ€μνλ€.
- μ€λ²λ‘λ©μ **ν¨μκ° μλ‘λ€λ₯Έ μ¬λ¬κ°μ call signaturesλ₯Ό κ°μ§κ³  μμ λ** λ°μλλ€.
- λ€μλ§ν΄ μ€λ²λ‘λ©μ **μ¬λ¬κ°μ call signaturesλ₯Ό κ°κ³ μλ ν¨μ**μ΄λ€.

```js
type Add = {
    //AddλΌλ νμμ 1οΈβ£λ‘λ, 2οΈβ£λ‘λ κ΅¬νλ  μ μλ€.
    (a:number,b:number) : number //1οΈβ£
    (a:number,b:string) : number //2οΈβ£
}
const add: Add = (a,b) => { //aλ numberνμ, bλ numberλ stringνμμ΄λ€.
    //κ·Έλ₯ a+bλ₯Ό λ¦¬ν΄νκ² μμ±νλ©΄ bκ° stringμΌ κ²½μ° num + stringμμν νμμ€νΈλ¦½νΈ μ€λ₯κ° λ°μνλ€.
    if(typeof b === "string") return a //stringμΌλ λ°λ‘ μ²λ¦¬ν΄μ€λ€.
    else return a+b
}
```

- μλ μ€μ¬λ‘ λ³λ‘ μμ±ν  μΌ μλ μ½λκ³ , μλμμ μ°λ¦¬κ° ν¨ν€μ§λ λΌμ΄λΈλ¬λ¦¬λ₯Ό μΈ λ λ§μ£ΌμΉ  μ μλ overloadμ μμλ₯Ό λ³Ό μ μλ€.

```js
//Next.jsμ μ½λ μμ
//κ°μ²΄λ‘λ, stringμΌλ‘λ μΈμλ₯Ό λκ²¨μ€ μ μλ€.
Router.push({
  path: "/home",
  state: 1
})

Router.push("/home")

//μκ° κ°λ₯νκ±΄ μλμ κ°μ΄ μ€λ²λ‘λλ‘ μ μνκΈ° λλ¬Έμ΄λ€.

type Config = {
  path: string,
  state: object
}

type Push = {
  (path:string) : void //μλ¬΄κ²λ λ¦¬ν΄νμ§ μμΌλ―λ‘ void
  (config: Config) : void
}

const push : Push = (config) => {
  if(typeof config === "string") console.log(config)
  else {
      console.log(config.path, config.state)
    }
}
```

- signatureλ λ€λ₯΄κ³ , argumentsμ numberλ λ€λ₯Έ κ²½μ°κ° μμ μ μλ€.

```js
//π©before
type Add = {
  (a:number, b:number) : number
  (a:number, b:number, c:number) : number
}

const add:Add = (a, b, c) => { //cμΈμλ optionalνλ° κ·Έλ₯ λ£μ΄μ£Όκ³  μμ΄μ λΆννλ€.
  return a + b
}

//β¨after
type Add = {
  (a:number, b:number) : number
  (a:number, b:number, c:number) : number
}

const add:Add = (a, b, c?:number) => { //optionalν κ²μ λ§κ² λ£μ΄μ€λ€. optionalνκ³  λ€μ΄κ°κ±°λ©΄ numberμΌκ±°μΌ!!
  if(c) return a + b + c
  return a + b
}

add(1,2)
add(1,2,3)
```

</br>

### π Polymorphism

- Polymorphismμ 'λ€νμ±'(many diffrent structures)μ λ»νλ€. (poly = many,several,much, morphos = form,structure)
- overloadingννΈλ₯Ό ν΅ν΄ 2-3κ°μ parameterλ₯Ό κ°μ§ μ μμμ νμΈνλ€.
- μ΄λ°μμΌλ‘ call signatureμ μΆκ°ν  νμλ€μ΄ κΈΈμ΄μ§ λ, λ λμ λ°©μμ΄ Polymorphismμ΄λ€.(λ¬Όλ‘  call signatureμ νμ©νλ λ°©λ²λ μλμ νμ§λ§, Polymorphismμ΄ λ κΉλ)
- ν¨μλ₯Ό μ¬μ©ν  λλ concrete typeμ κ°μ λ£μ΄μ£Όκ² μ§λ§, ν¨μμ call signatureλ₯Ό μμ±ν  λ concrete typeμ μ μ μμ λλ μλ€. μ΄λ Polymorphismμ μ¬μ©νλ€κ³  λ΄λ λλ€.
- **concrete type** μ΄λ number, boolean, string, void, unknown λ± μμμ μ΄μ  κΉμ§ λμ¨ νμμ λ§νλ€.
- **generic type**μ genericμ placeholderλ₯Ό μλ―Ένλ€.concrete typeμ μ¬μ©νλ λμ μ μΈ μ μλ€. placeholderλ₯Ό μμ±νκ³ , κ·Έκ² λ­μ§ μΆλ‘ ν΄μ ν¨μλ₯Ό μ¬μ©νλ€.
- **μ λ€λ¦­μ μ μΈ μμ μ΄ μλλΌ μμ± μμ μ νμμ λͺμνμ¬ νλμ νμλ§μ΄ μλ λ€μν νμμ μ¬μ©ν  μ μλλ‘ νλ κΈ°λ²μ΄λ€.**

```js
//π©before
type SuperPrint = { //Call Signatureμμ±
  (arr: number[]):void
  (arr: boolean[]):void
  (arr: string[]):void
  // (arr: (number|boolean)[]): void
}

const superPrint: SuperPrint = (arr) => {
  arr.forEach(i => console.log(i))
}

superPrint([1,2,3,4])
superPrint([true,false,true,true])
superPrint(["a","b","c"])
superPrint([1,2,true,false]) //βοΈμ΄λΆλΆμμ μ€λ₯ λ°μ!(call signature μμ±λμ΄ μμ§ μλ€. π€¦λ§¨λ  μ΄λ κ² μΆκ°ν΄μ£Όλ©΄ μμ£Ό νΌκ³€νλ€.)

//β¨after
type SuperPrint = {
  <TypePlaceholder>(arr: TypePlaceholder[]):void
  /*
  μ΄ Call Sginatureκ° generic typeμ λ°λ λ€λ κ²μ μλ €μ€λ€.
  μ΄λ TypePlaceholderλ generic typeμ μ΄λ¦μΌλ‘,
  μ΄λ€ κ²μ΄λ  λ¬΄κ΄νλ,β­οΈ<T>λ <V>λ₯Ό λ§μ΄ μ΄λ€.β­οΈ

  λ§μ call signature typeμ μλ€μ΄
  generic typeμ¬μ©μΌλ‘ νλ°©μ μ λ¦¬λμλ€!!π§Ή
  */
}

const superPrint: SuperPrint = (arr) => {
  arr.forEach(i => console.log(i))
}

superPrint([1,2,3,4])
superPrint([true,false,true,true])
superPrint(["a","b","c"])
superPrint([1,2,true,false])

//πfeature upgrade
type SuperPrint = {
  <T>(arr: T[]): T
  //μ΄λ²μ T(generic)λ°°μ΄μ λ°μμ κ·Έμ€ νλλ₯Ό λ¦¬ν΄νλ€κ³  μλ €μ£ΌκΈ°
}

const superPrint: SuperPrint = (arr) => arr[0]

const a = superPrint([1,2,3,4]) //number
const b = superPrint([true,false,true,true]) //boolean
const c = superPrint(["a","b","c"]) //string
const d = superPrint([1,2,true,false,"hello"]) //string|number|boolean
```

- `any[]`λ₯Ό μ¬μ©νλκ²κ³Ό λ­κ°λ€λ₯΄λ μΆμ μλ μμ§λ§, `any[]`λ₯Ό μ¬μ©νλ©΄ λμ΄μ νμμ΄ μ§μΌμ£Όμ§ μλλ€. μλ₯Ό λ€μ΄ λ°λ‘ μ μ½λμμ a,b,c,dμ νμμ΄ λͺ¨λ `any`κ° λλ€. κ·ΈλΌ μ€μ§μ μΌλ‘ κ·Έ λ³μλ€μ νμ©ν΄μ `d.toUpperCase()`λ±μ μ€λ₯λ₯Ό λΏλ €μ€μΌ ν  λμλ μ€λ₯λ₯Ό λ΄μ§ μλλ€. dλ`number`μΈλ°!
- generic typeμΌλ‘ call signatureλ₯Ό μμ±νλ©΄, ν¨μλ₯Ό μ¬μ©ν λ κ·Έ μ¬μ©μ μΌμΉνλ νμμΌλ‘ call signatureλ₯Ό μΆλ‘ ν΄ λμ²΄ν΄μ λ³΄μ¬μ€λ€.
  ![Polymorphism](./polymorphism01.png)
  ![Polymorphism](./polymorphism02.png)
- μ΄ λ°©μλ§κ³ λ λ€λ₯Έ λ°©μμΌλ‘ genericμ μ¬μ©νλ λ°©μμ΄ μ‘΄μ¬νκ³ , μ€μ¬λ‘ reactμμ  κ·Έκ±Έ λ λ§μ΄ μ΄λ€.
- generci typeλ μ¬λ¬κ°μ call signatureλ₯Ό μ¬μ©ν  μ μλ€.

```js
type SuperPrint = { <T, M>(arr: T[], b: M): T };
const superPrint: SuperPrint = (arr) => arr[0];
const a = superPrint([1, 2, 3, 4], '');
```

- generic typeμ μ€μ λ‘ μ΄λ»κ² μ¬μ©ν κΉ? μ¬μ€ generic typeμ νμ©ν΄μ¬ call signatureμ μμ±ν  μΌμ κ±°μ μμ κ²μ΄λ€. **λΌμ΄λΈλ¬λ¦¬λ₯Ό λ§λ€κ±°λ, λ€λ₯Έ κ°λ°μκ° μ¬μ©ν  κΈ°λ₯μ κ°λ°νλ κ²½μ°**μ μ λ€λ¦­μ΄ μ μ©νλ€.
- generic typeμ μ¬μ©νλ λλ€λ₯Έ μμλ μλλ₯Ό μ°Έκ³ νλ€.

```js
/*
π© before
generic typeμ λ¨Όμ  μ μΈνκ³  ν¨μλ₯Ό λ§λ€μ΄μ κ·Έ νμμ μμ°λλ°
μ‘°κΈ μ΄λ €μλ³΄μ¬μ κ²μ΄ λκ² μκΉ
*/
type SuperPrint = <T>(a: T[]) => T;

const superPrint: SuperPrint = (a) => a[0];

const a = superPrint([1, 2, 3, 4]);
const b = superPrint([true, false, true]);
const c = superPrint(['a', 'b', 'c']);
const d = superPrint([1, 2, true, false, 'hello']);

/*
π€ after
generic typeμ μμ±νλ λΆλΆκ³Ό κ·Έ νμμ μ΄μ©ν ν¨μλ₯Ό λ§λλ κ³Όμ μ
νλλ‘ ν©μ³μ μμ±ν λ²μ ! μ‘°κΈ λ λ³΅μ‘νκ² μκΈ΄κ±° κ°κΈ°λ νλ€.
*/
function superPrint<V>(a: V[]) {
  return a[0];
}

const a = superPrint([1, 2, 3, 4]);
const b = superPrint([true, false, true]);
const c = superPrint(['a', 'b', 'c']);
const d = superPrint([1, 2, true, false, 'hello']);

/*
π«  if
μλμ κ°μ΄ μμ±ν  μμ μ€λ₯κ° λλ€.
νμμ€ν¬λ¦½νΈκ° generic typeμΌλ‘ μ μΆν΄ λ§λ€μ΄λμ 
numberλ₯Ό λ¦¬ν΄νλ call signatureμ 
μ§μ  booleanμ΄λΌκ³  νμμ overwrite(λ?μ΄μ°κΈ°)λ₯Ό νλ €νκΈ° λλ¬Έ!
π ν­μ νμμ€ν¬λ¦½νΈκ° νμμ μ μΆνλλ‘ νλ κ²μ΄ μ’λ€.
*/
const a = superPrint < boolean > [1, 2, 3, 4]; //βοΈ
```

- μ΄λ°μλ generic typeμ λ€λ₯Έ νμμ λ£μ΄μ νμ₯ν΄ μ¬μ©ν  μλ μλ€. typeλΌλ¦¬ μ¬μ¬μ©μ΄ κ°λ₯νλ€.
- β¨**λ§μ½ λ§μ κ²λ€μ΄ μλ ν° νμ νλλ₯Ό κ°μ§κ³  μλλ°, κ·Έ μ€ νλκ° λ¬λΌμ§ μ μλ νμ**μ΄λΌλ©΄, κ±°κΈ°μ genericμ λ£μΌλ©΄ λλ€.κ·ΈλΌ κ·Έ νμμ λ§μ΄ μ¬μ¬μ©ν  μ μκ²λλ€.

```js
/*
μλμ 1οΈβ£,2οΈβ£,3οΈβ£ μ λͺ¨λ generic type μ μμ±νκ³  κ·Έ νμμ λ λ€λ₯Έ νμμ λ£μ΄μ μ¬μ©ν¨μΌλ‘μ¨ νμ₯ν΄μ μ¬μ©νλ λͺ¨μ΅μ λ³΄μ¬μ€λ€.
1οΈβ£,2οΈβ£,3οΈβ£λ λͺ¨λ κ°μ κΈ°λ₯μ νλ μ½λμ΄λ€.
*/

//1οΈβ£
type Player<E> = {
  //β¬οΈPlayerλΌλ νμμ gerneric typeμ λ°λλ€κ³  μλ €μ£Όκ³ 
  name: string,
  extraInfo: E, //β¬οΈμ¬κΈ°μ generic typeμ΄ μ°μΌκ±°λΌκ³  μλ €μ€λ€.
};

const sooryeon: Player<{ favFood: string }> = {
  /*β¬οΈPlayerλΌλ νμμ΄ generic νμμ μ μΈνλλ°
  κ·Έ νμμ κ°λ sooryeonμ΄λ λ³μμλ
  generic type μλ¦¬μ { favFood: string }μ κ°μ²΄λ₯Ό λ£μ΄μ μ¬μ©ν  κ²μ΄λ€.*/
  name: 'sooryeon',
  extraInfo: {
    favFood: 'wine', //β¬οΈμλ E generic νμμ΄ μλ μλ¦¬μ κ°μ²΄ λ€μ΄κ°
  },
};

//2οΈβ£
type Player<E> = {
  name: string,
  extraInfo: E,
};

type SooryeonPlayer = Player<{ favFood: string }>;

const sooryeon: SooryeonPlayer = {
  name: 'sooryeon',
  extraInfo: {
    favFood: 'wine',
  },
};

//3οΈβ£
type Player<E> = {
  name: string,
  extraInfo: E,
};

type SooryeonExtra = {
  //μ΄λ²μ SooryeonExtraλΌλ typeμ λ§λ€κ³  Playerνμμ μ λ€λ¦­ μμ λ£μ΄μ€λ€.
  favFood: string,
};
type SooryeonPlayer = Player<SooryeonExtra>;

const sooryeon: SooryeonPlayer = {
  name: 'sooryeon',
  extraInfo: {
    favFood: 'wine',
  },
};

const lynn: Player<null> = {
  name: 'lynn',
  extraInfo: null,
};
```

- μλμμ± κΈ°λ₯μ ν΅ν΄ νμΈν΄λ³΄λ©΄ λ°°μ΄μ λ§λλ Arrayμ­μ generic typeμ ν΅ν΄ λ§λ€μ΄μ§λ€λ κ²μ μ μ μλ€.
  ![GenericTypeArray](./generic-type.png)
- μμ κ°μ΄ μμ±λμ΄ μκΈ° λλ¬Έμ μ°λ¦¬λ μλμ κ°μ μ½λλ‘ λ°°μ΄μ λ§λ€ μ μλ€.

```js
type numberArr = Array<number>;
let a: numberArr = [1, 2, 3, 4];
```

- λ°λΌμ μλμ λ ν¨μλ λͺ¨λ κ°λ€.

```js
function printAllNumbers(arr: number[]) {}
function printAllNumbers(arr: Array<number>) {}
```

- μ΄λ―Έ λ§μ λΌμ΄λΈλ¬λ¦¬μμ tsμ gerneric typeμ νμ©νλ€. μλ₯Ό λ€μ΄ reactμμ useStateλ₯Ό μ¬μ©ν  λμλ gerneric typeμ νμ©νκΈ° λλ¬Έμ μλμ κ°μ΄ tsλ‘ νμ©νλ μ¬λ‘κ° λ§€μ° λ§λ€.

```js
useState<number>()
```

</br>

### π₯ Classes

- TSλ κ°μ²΄ μ§ν₯ νλ‘κ·Έλλ°μ νκΈ°μ μμ£Ό μ’λ€.
- TSλ‘ class λ₯Ό λ§λλ λ°©λ²μ μ΄ν΄λ³Έλ€.
- κΈ°λ³Έμ μΌλ‘ jsμ classμλ prviateμ΄λ publicμ κ°λμ΄ μμ§λ§, javaλ±μλ μλ€. tsλ μμ μ±μ μν΄μ privateκ³Ό publicμ μ¬μ©ν  μ μκ² ν΄μ£Όμ§λ§, λΉμ°ν μ»΄νμΌλ§ λ js νμΌμλ ν΄λΉ λΆλΆμ μ‘΄μ¬νμ§ μκ² λλ€.

```js
//β¨TS version
class Player {
    constructor(
        private firstName: string,
        private lastName: string,
        public nickname:string
    ){}
    //jsμμ constructor ν¨μμμ μ μΈλμΌ νλ this.λ³μ = λ³μ μμμ΄ κ°λ¨ν΄μ§λ€.
}
const nico = new Player("nico","las","λκΌ¬")
nico.firstName //βοΈμ»΄νλ μΈ: privateμ΄κΈ° λλ¬Έμ λΆν, λ³΄νΈλ°μ μ μλ€.
nico.nickname //βν΅κ³Ό: publicμ΄κΈ° λλ¬Έμ μ κ·Ό κ°λ₯

//β¨ JS version
"use strict";
class Player {
    constructor(firstName, lastName, nickname) {
        this.firstName = firstName;
        this.lastName = lastName;
        this.nickname = nickname;
    }
}
const nico = new Player("nico", "las", "λκΌ¬");
nico.firstName; //js versionμλ μ΄λ€ λΆνλ λ¨μ§ μκΈ° λλ¬Έμ λ³΄νΈλ°μ§ λͺ»νλ€.
nico.nickname;
```

- **μΆμ ν΄λμ€(abstract class)** λ λ€λ₯Έ ν΄λμ€κ° μμλ°μ μ μλ ν΄λμ€μ΄λ€. νμ§λ§ μ΄ ν΄λμ€λ μ§μ  μλ‘μ΄ μΈμ€ν΄μ€λ₯Ό λ§λ€ μλ μλ€.

```js
abstract class User{
  constructor(
        private firstName: string,
        private lastName: string,
        public nickname:string
    ){}
}

const testUser  = new User("nico", "las", "λκΌ¬");//βοΈμ»΄νλ μΈ: abstract class μμλ μλ‘μ΄ instanceλ₯Ό κ³§μ₯ λ§λ€ μ μλ€.

class Player extends User{}
const nico = new Player("nico", "las", "λκΌ¬");//βν΅κ³Ό: abstract classμμ λ°λ‘ μλ‘μ΄ instanceλ₯Ό λ§λ  κ²μ΄ μλλ―λ‘ ok

nico.nickname //μ‘°νκ°λ₯
```

- **μΆμν΄λμ€μ λ©μλ** λ λ§κ·Έλλ‘ μΆμ ν΄λμ€ μμ μ μΈλμ΄ μλ μΌλ°μ μΈ λ©μλλ₯Ό λ§νλ€.
- **μΆμ λ©μλ** λ μΆμ ν΄λμ€ λ΄λΆμ λ³΄ν΅ λ©μλμ λ€λ₯΄λ€. **λ©μλλ₯Ό ν΄λμ€ μμμ κ΅¬ννμ§ μμΌλ©° call siganatureλ§!! μμ±νλ€.**
- μΆμ λ©μλλ μΆμ ν΄λμ€λ₯Ό μμλ°λ λͺ¨λ  κ²λ€μ΄ κ΅¬νμ ν΄μΌνλ λ©μλλ₯Ό μλ―Ένλ€.κ΅¬νμ μ΄λ»κ² νλ  μκ΄μμ§λ§ κΌ­ νκΈ΄ ν΄μΌνλ€.

```js
//π€π€π€abstract class λ΄λΆμ λ©μλ μ¬μ©ν΄λ³΄κΈ°
abstract class User{
  constructor(
        private firstName: string,
        private lastName: string,
        public nickname:string
    ){}
    getFullName(){
      return `${this.firstName} ${this.lastName}`
    }
    // private getFullName(){
    //   return `${this.firstName} ${this.lastName}`
    // }
}

class Player extends User{}
const nico = new Player("nico", "las", "λκΌ¬");
nico.getFullName() //μ¬μ©κ°λ₯
//λ§μ½ λ©μλλ₯Ό privateμΌλ‘ λ°κΎΌλ€λ©΄ μ¬μ©μ΄ λΆκ°λ₯νλ€.


//π€π€π€ abstract methodλ₯Ό λ§λ€μ΄ μ¬μ©ν΄λ³΄κΈ°(with private property)
abstract class User{
  constructor(
        private firstName: string,
        private lastName: string,
        private nickname:string
    ){}
    abstract getNickName():void //getNickNameμ μΆμ λ©μλλΌ call signatureλ§ κ°λλ€.
    getFullName(){
      return `${this.firstName} ${this.lastName}`
    }
}

//class Player extends User{}//βοΈμ»΄νλ μΈ: abstarct method λ₯Ό μννμ§ μμλ€κ³  λΆν
class Player extends User{
  getNickName(){
    console.log(this.nickname) //βοΈμ»΄νλ μΈ: private propertyλ‘ λ§λ λ€λ©΄ κ·Έ ν΄λμ€λ₯Ό μμνμμ§λΌλ μ κ·Όν  μ μλ€.
    //πprivate propertyλ μΈμ€ν΄μ€λ λ¬Όλ‘ , μμ ν΄λμ€μμμ‘°μ°¨ μ κ·Όν  μ μλ propertyμ΄λ€. μμμμ μ κ·Όνκ³  μΆλ€λ©΄ privateμ΄ μλλΌ protectedλ₯Ό μ¨μΌ νλ€.
  }
}
const nico = new Player("nico", "las", "λκΌ¬");
nico.getFullName()


//πππ abstract methodλ₯Ό λ§λ€μ΄ μ¬μ©ν΄λ³΄κΈ°(with protected property)
/*
outsideλ‘ λΆν΄ λ³΄νΈλμ§λ§, μμ ν΄λμ€μμ  μ¬μ©λκΈ°λ₯Ό μνλ€λ©΄
privateμ΄ μλ, protectedλ₯Ό μ¬μ©νλ€.
*/
abstract class User{
  constructor(
        protected firstName: string,
        protected lastName: string,
        protected nickname:string
    ){}
    abstract getNickName():void
    getFullName(){
      return `${this.firstName} ${this.lastName}`
    }
}

class Player extends User{
  getNickName(){
    console.log(this.nickname)
    //βν΅κ³Ό: privateμ΄ μλλΌ protected propertyμ΄κΈ° λλ¬Έμ μμν΄λμ€μμ this.nicknameμ μ κ·Όν  μ μλ€.
  }
}
const nico = new Player("nico", "las", "λκΌ¬");
nico.getFullName()//βν΅κ³Ό
nico.nickname//βοΈμ»΄νλ μΈ: protected propertyλΌλ μΈμ€ν΄μ€μμ  μ κ·Ό λΆκ°
```

- μμμ κ° λ³μ μμ±(private,public,protected)μ λ°λΌ **μ κ·Ό κ°λ₯ν μμΉ**λ₯Ό μ λ¦¬νμλ©΄ μλμ κ°λ€.

|   κ΅¬λΆ    | μ μΈν ν΄λμ€ λ΄ | μμλ°μ ν΄λμ€ λ΄ | μΈμ€ν΄μ€ |
| :-------: | :--------------: | :----------------: | :------: |
|  private  |        β­        |         β         |    β    |
| protected |        β­        |         β­         |    β    |
|  public   |        β­        |         β­         |    β­    |

</br>

### π₯ Classes μ€μ  μ°μ΅ - μ¬μ  λ§λ€κΈ°

```js
type Words = {
  [key:string]: string
  //πWordsλΌλ νμμ΄ stringλ§μ propertyλ‘ κ°μ§λ μ€λΈμ νΈλΌκ³  μ ν΄μ£ΌκΈ°.
  //valueκ° μλλΌ keyμ νμμ μ ν΄μ£Όλ λ¬Έλ²μ΄λ€.
  //μ¬κΈ°μ [whatever:string]μ²λΌ μλ¬΄ μ΄λ¦μΌλ‘λ μ§μ κ°λ₯νλ€.
}

//μλλ keyκ°μ νμμ μ ν΄μ£Όλ κ²½μ°λ₯Ό νμΈμ°¨ μμ±ν μ½λ
let dict:Words = {
  "potato":"food",
  Number(1) :"number" //βοΈμ»΄νλ μΈ: key κ°μ λλ²μΌ μ μλ€.
}

//π© μΌμΌ νλ©΄ μλλ€.
class Dict {
  private words :Words //βοΈμ»΄νλ μΈ
  /*
  wordsλ initializerκ° μκ³  contructorμμ μ μλ
  signμ΄ μλκΈ° λλ¬Έμ μ»΄νλ μΈ λ°μ
  */
}

//π© κ·Έλ λ€κ³  μ΄λ κ²νλ©΄ contructorκ° wordsλ₯Ό μ§μ ν΄μ€ λ²λ¦°λ€.
class Dict {
  constructor(
    private words: Words
  ){}
}

// β¨μΌμΌ ν΄μΌνλ€.
class Dict {
  private words :Words //πν΄λμ€ λ΄λΆ λ³μμ μΈλΆ νμμ κ°μ Έλ€ λΆμ΄κ³  μκ³ ,
  constructor(){//πλ°λ‘ contructorλ‘ μ΄κΈ°ννλ κ²μ΄ μλλΌ μλμΌλ‘ μ΄κΈ°ν μμΌ°λ€.
    this.words = {}
  }
  add(word:Word){ //ππclassλ₯Ό νμμ²λΌ μ¬μ©νλ€. //μ¬μ μ μΆκ°νκΈ°
    if(this.words[word.term] === undefined){ //μ¬μ μ μ μλμ΄ μμ§μλ€λ©΄
      this.words[word.term] = word.def; //μλ‘ μ λλ€.
    }
  }
  def(term:string){ //μ¬μ  μ°Ύμλ³΄κΈ°
    return this.words[term]
  }
}

class Word {
  constructor(
    public term:string,
    public def:string,
  ){}
}

const kimchi = new Word("kimchi", "νκ΅­μ μμ");
const dict = new Dict();
dict.add(kimchi);
dict.def("kimchi") //νκ΅­μ μμ μΆλ ₯

```

- μ μ½λ μ λ¦¬ + μμν ν¬μΈνΈ μΆκ°

```js
type Words = {
  [key:string]: string
}

class Dict {
  private words :Words
  constructor(){
    this.words = {}
  }
  add(word:Word){
    if(this.words[word.term] === undefined){
      this.words[word.term] = word.def;
    }
  }
  def(term:string){
    return this.words[term]
  }
  static hello(){ //πstaticμ JSμλ μλ κ°λμ΄λ―λ‘ μ»΄νμΌλ§ νμλ λΆμ΄μλ€.
    return "hello"
  }
}

class Word {
  constructor(
    public readonly term:string,
    public readonly def:string,
  ){}
  /*
  μ¬κΈ°μ termκ³Ό defλ μ΄ν Dictν΄λμ€ λ΄λΆμμ μ‘°νλμΌ νκΈ° λλ¬Έμ
  publicμΌλ‘ μ μΈλμλ€.
  κ·Έλμ readonlyκ° μλ€λ©΄
  kimchi.def = 'xxx' μΌλ‘ λ³κ²½νλ κ²μ΄ κ°λ₯νλ€.
  */

}

const kimchi = new Word("kimchi", "νκ΅­μ μμ");
const dict = new Dict();
dict.add(kimchi);
dict.def("kimchi")
kimchi.def = "xxx" //βοΈμ»΄νλ μΈ: wordμμ readonlyλ‘ def propertyλ₯Ό μ§μ ν΄ μ£ΌμκΈ° λλ¬Έμ λ³κ²½μ΄ λΆκ°λ₯νλ€.
Dict.hello()

```

</br>

### π₯¨ Interfaces

- νμμ μλμ κ°μ΄ μμ λ‘­κ² λ§λ€μ΄μ μ¬μ©ν  μ μλ€.

```js
type Nickname = string;
type Health = number;
type Friends = Array<string>;

type Player = {
  nickname: Nickname,
  healthBar: Health,
  friends: Friends,
};

const nico: Player = {
  nickname: 'nico',
  healthBar: 10,
  friends: ['las'],
};

type Food = string;
const kimchi: Food = 'delicious';
```

- νμμ μ§μ λ μ΅μμΌλ‘λ§ μ νν  μλ μλ€.[λ§ν¬](https://www.typescriptlang.org/play?#code/PTAuE8AcFMAIBVoEMC2sC8sDOoBOBLAOwHNZAXccB92wFy7ZAW0cBLW2QAGWzAQzssBHm2QDIbAaMdkAYQ7EAR44AHJwDOdAGgBQIQCKjgDPbAAmOxAmDVlYgVjHAGoOARcdijAqBOAXVcA-EzR2xAiJOxAGqvdxsQDUDgSrHABquCRgE6aAdIApyaQgYBGQ0TAByXGgAE3DYAB9YcIAjABsAV2g4xPDwaFTUgHsAd3CAbkCoOAAJZFTQAAsMWABGBNgAVnaWgAYKyuCABVSkPNxmgG9pWFhCfABjAGtCVGgALmw8ImIZGdBQjcRUXdgGusaN2qR6hpkAX375wsIcWYXC2A3h0ehxzCmZnMlisUOtYAAiIGFcEnfaoNbgqLRGHTU7nBprDrSO5AA)

```js
//type Team = string μ΄λΌλ©΄ μ΄λ€ νμ΄λ¦μ΄λΌλ λμ¬ μ μμ§λ§,
//μλμ κ°μ΄ μ΅μμ μ§μ ν΄μ£Όλ©΄ μ΅μ μ€ νλλ§ μ¬μ©ν  μ μλ€.β¨
type Team = 'red' | 'blue' | 'yellow';
type Health = 1 | 5 | 10;

type Player = {
  nickname: string,
  team: Team,
  health: Health,
};

const nico: Player = {
  nickname: 'nico',
  team: 'red', //green μ°λ©΄ μ€λ₯λ¨
  health: 5, //8μ°λ©΄ μ€λ₯λ¨
};
```

- μ λ°©λ²λ€ μΈμλ μ€λΈμ νΈμ λͺ¨μμ μ€λͺνλ λ€λ₯Έ λ°©λ²μ μΈν°νμ΄μ€κ° μλ€.
- μ½κ°μ μ°¨μ΄μ μ μμ§λ§ κ±°μ λΉμ·νλ€.[λ§ν¬](https://www.typescriptlang.org/play?#code/C4TwDgpgBAKhCGBbKBeKByAThAJuqAPhgEYA2ArhPkeiBKaQPYDu6A3AFCiRQASCpYAAtUUAIyEoAVkliADJw4BLAHbAImAGbwAxtAAKpeHUxQA3hyhQVSnQGsVSCAC4oAZ2CZVAcwA0lqHUkVzgkfyshAWFXfnhBIX8AX0UdRhUPa1tGV0NjDVELKxt7R0QXDGLGdHDAhERXLFxqqAB6Fu9sCBUoQAeRwBcuqEASMcANTsAKhoDIuOjpX1aWgA5+obGOZKA)
- νμμ΄ λ€μν ννλ₯Ό μ§μ ν  μ μλ κ²μ λ°ν΄, interfaceλ **μ€λΈμ νΈμ ννλ₯Ό μ§μ νλ λ°**μλ§ μ°μΌ μ μλ€. react.jsλ‘ μμν  λ λ§μ΄ μ¬μ©νλ€.

```js
type Team = 'red' | 'blue' | 'yellow';
type Health = 1 | 5 | 10;

interface Hello = string //μ΄κ±΄ λΆκ°λ₯

interface Player { //interfaceλ μ€μ§ μ€λΈμ νΈ νν μ μν  λλ§ μΈ μ μλ€.
  //type Player = {} μ΄ νμλ§ λ¬λΌμ§
  nickname: string;
  team: Team;
  health: Health;
}

const nico: Player = {
  nickname: 'nico',
  team: 'red', //green μ°λ©΄ μ€λ₯λ¨
  health: 5, //8μ°λ©΄ μ€λ₯λ¨
};
```

- μ€λΈμ νΈλ₯Ό μ μν  λ, μΈν°νμ΄μ€λ classμ λ¬Έλ²μ΄ λΉμ·νμ¬ μ΅μν λ©΄λ μλ€. nicoλ interfaceμ¬μ© λ°©μμ μ νΈ

```js
interface User {
  readonly name: string;
}
interface Player extends User {}
//interfaceλ typeμ΄μ§λ§ extendsλ₯Ό μ¬μ©ν΄μ λ§μΉ ν΄λμ€μ κ°μ λ¬Έλ²μΌλ‘ μμλ°μ μ μλ€.
const nick: Player = {
  name: 'nico',
};

//λ§μ½ μ μμμ typeμΌλ‘ νλ©΄ μλμ κ°μμ§λ€.
type User = {
  name: string,
};
type Player = User & {};
const nico: Player = {
  name: 'nico',
};
```

- κ°μ interfaceλ₯Ό μ¬λ¬λ² μ μΈνλ©΄ νμμ€ν¬λ¦½νΈκ° μμμ ν©μ³μ€λ€. μ΄κ±΄ typeμΌλ‘ ν  μ μλ€. κ°μ μ΄λ¦μΌλ‘ λ§λ€μ΄μ§ interfaceλ μΆμ ν  μ μλ€.

```js
interface User {
  name: string;
}
interface User {
  lastName: string;
}
interface User {
  health: number;
}

const nico: User = {
  name: 'nico',
  lastName: 'n',
  health: 10,
};
```

- JSμμ  abstract class λΌλ κ°λμ΄ μ‘΄μ¬νμ§ μκΈ° λλ¬Έμ κ²°κ΅¬ μ»΄νμΌλ§ μ κ·Έλ₯ classλ‘ λ³νλ κ²μ νμΈν  μ μλ€. κ·ΈλΌ μ μΆμ ν΄λμ€λ₯Ό μ¬μ©νλ κ±ΈκΉ?? -> λ°λ‘ **νμ€νλ propertyμ λ©μλλ₯Ό κ°λλ‘ ν΄μ£Όλ μ²­μ¬μ§μ λ§λ€κΈ° μν΄** μΆμν΄λμ€λ₯Ό μ¬μ©νλ€.

```js

//1οΈβ£ abstract classμ¬μ©μ
abstract class User{ //μΆμν΄λμ€λ λ°λ‘ μΈμ€ν΄μ€λ₯Ό λ§λλ κ²μ νμ©νμ§ μλλ€.
  constructor(
    protected firstName:string,
    protected lastName:string,
  ){}
  abstract sayHi(name:string):string
  abstract fullName():string
}
class Player extends User{ //abstract class μμ
  //abstract method κ΅¬νν΄μΌν¨
  fullName(){
    return `${this.firstName} ${this.lastName}`
  }
  sayHi(name:string){
    return `Hello ${name}. My hame is ${this.fullName()}`
  }
}
//μ μ½λλ₯Ό jsλ‘ μ»΄νμΌ νλ©΄...
"use strict";
class User { //μ΄μ²λΌ abstract class λΆλΆμ΄ μΌλ° classλ‘ λ¨μμλ€.
    constructor(firstName, lastName) {
        this.firstName = firstName;
        this.lastName = lastName;
    }
}
class Player extends User {
    fullName() {
        return `${this.firstName} ${this.lastName}`;
    }
    sayHi(name:string) {
        return `Hello ${name}. My hame is ${this.fullName()}`;
    }
}

```

- abstract class κ° μ»΄νμΌλ§ν΄λ classλ‘ λ¨λ κ²κ³Ό λ¬λ¦¬ interfaceλ μ»΄νμΌλ§νλ©΄ μ¬λΌμ§λ€.
- interfaceκ° κ°λ²Όμ΄λ° μ΄λ»κ² νΉμ ννλ₯Ό λ°λ₯΄λλ‘ κ°μ ν κ²μΈκ°λ μλλ₯Ό μ°Έκ³ νλ€.

```js
//2οΈβ£ interfaceμ¬μ©μ
interface User{
  firstName: string,
  lastName: string,
  sayHi(name:string):string
  fullName():string
}
class Player implements User{}//βοΈμ»΄νλ μΈ: firstName,lastName,sayHi,fullNameμ μ λλ‘ μμνμ§ μμλ€κ³  μ»΄νλ μΈνλ€.
//μ΄λ‘μ μΈν°νμ΄μ€ + implementsλ₯Ό μ¬μ©ν΄μ abstract classλ₯Ό λμ²΄ν  μ μκ² λμλ€.

class Player implements User{
  constructor(
    /*
    πinterfaceλ₯Ό μ΄μ©νμ¬ classλ₯Ό λ§λ€ λλ private, protectedκ° λ  μ μλ€. λ°λμ publicμ΄μ¬μΌλ§ νλ€.
    */
    public firstName : string,
    public lastName: string
  ){}
  fullName() {
    return `${this.firstName} ${this.lastName}`;
    }
  sayHi(name:string) {
    return `Hello ${name}. My hame is ${this.fullName()}`;
  }
}

/*
extendsλ jsμλ μμ§λ§,
implementλ tsμ interfaceμλ§ μλ κ°λμ΄λ€.

λ°λΌμ interfaceμ implementsλ₯Ό μ¬μ©νλ©΄
μλμ κ°μ΄ jsλ‘ μ»΄νμΌλ§μ μλμ κ°μ΄
interfaceλ‘ μ μΈνλ μλ³Έ ν΄λμ€μΈ UserλΌλ classκ° λ¨μ§ μμ
λ κ°λ²Όμ΄ μ½λκ° λλ€.
*/
"use strict";
class Player {
    constructor(firstName, lastName) {
        this.firstName = firstName;
        this.lastName = lastName;
    }
    fullName() {
        return `${this.firstName} ${this.lastName}`;
    }
    sayHi(name) {
        return `Hello ${name}. My hame is ${this.fullName()}`;
    }
}

```

- λ¬Όλ‘  interfaceλ₯Ό μ¬μ©νλ©΄ νλ μ΄μμ μΈν°νμ΄μ€λ₯Ό λμμ μμν  μλ μλ€.

```js
interface User{
  firstName: string,
  lastName: string,
  sayHi(name:string):string
  fullName():string
}
interface Human{
  health: number
}
class Player implements User,Human{ //β¨λκ°μ§ classλ₯Ό μμνλ κΈ°μ 
  constructor(
    public firstName : string,
    public lastName: string,
    public health: number
  ){}
  fullName() {
    return `${this.firstName} ${this.lastName}`;
    }
  sayHi(name:string) {
    return `Hello ${name}. My hame is ${this.fullName()}`;
  }
}

//λ¬Όλ‘  interfaceλ typeμΌλ‘λ μ§μ ν  μ μμ΄ νΈλ¦¬ν μ λ μμ§λ§μ
function makeUser(user:User): User{
  return {
    firstName:"nico",
    lastName:"las",
    fullName: () => "xx",
    sayHi: (name) => "string"
  }
}

makeUser({
  firstName:"nico",
  lastName:"las",
  fullName: () => "xx",
  sayHi: (name) => "string"
})

```

- λ§μ§λ§μΌλ‘ typeκ³Ό interface λ³΅μ΅ν΄λ³Έλ€.

```js
//1οΈβ£ TYPE
type PlayerA = {
  name: string,
};
const playerA: PlayerA = {
  name: 'nico',
};
//typeμμ μμλ°κΈ°
type PlayerAA = PlayerA & {
  lastName: string,
};
// type PlayerAA = {
//   //βοΈλΆκ°λ₯
//   health: number,
// };
const playerAA: PlayerAA = {
  name: 'nico',
  lastName: 'xxx',
};

//2οΈβ£ INTERFACE
interface PlayerB {
  name: string;
}
const playerB: PlayerB = {
  name: 'nico',
};
interface PlayerBB extends PlayerB {
  lastName: string;
}
interface PlayerBB {
  //βκ°λ₯: interfaceλ propertyλ₯Ό μΆμ ν  μ μλ€.
  health: number;
}
const playerBB: PlayerBB = {
  name: 'nico',
  lastName: 'xxx',
  health: 10,
};

//typeκ³Ό interfaceλͺ¨λ Implementsλ₯Ό μ¬μ©ν΄μ class μμκ°λ₯νλ©°, μΆμ ν΄λμ€λ₯Ό λμ²΄ν  μ μλ€.
type PlayerA = {
  firstName:string
}
interface PlayerB {
  firstName:string
}
class UserA implements PlayerA{
  constructor(
    public firstName:string
  ){}
}
class UserB implements PlayerB{
  constructor(
    public firstName:string
  ){}
}
```

- μλλ κ°μμΌλ‘ local storageλ₯Ό κ΅¬νν΄λ³Έ μ½λμ΄λ€.genericκ³Ό polymolphism, class, interfaaceλ₯Ό ν©μ³μ sexyν μ½λλ₯Ό λ§λ€ μ μλ€. [λ§ν¬](https://www.typescriptlang.org/play?#code/JYOwLgpgTgZghgYwgAgMqrAeynA5hAHgBUA+ZAb2QHoqNs8JAfdsAOa5QF3HAP7uUAJBwDtHAcFuQApVIA1x5IE+xwCVDgAsXANZ2AByeQBBAAoBJQD6dyQCDjgHVXkgD3HADIuAM5bZTAADXJALhOAa8cAaq4AY65IBlWwBzdgBdH2gEM7AIuNodDj4gDodyICoE4AWqwBQyMgA2gDWEACeAFwAzmBQoLgAushpyETUVADMgPB-gMcERmYWnoA4g8gA4hAg0MAIAYA1A4CVY3qAJ00AdNEAvtHRCAA2cBkZyAAymAhwU0EMxGSUNACM1S1tHV3IgC4LgBntUmGALz2ALQ3MscgADjkAbnCQyFn0+EXoWMGEUjIAC8FFGpQATNUAMIzObWUCQWCICBhfDtHLHW73OIZCBgAAUyXSWRyIFwABpkG8pgBXCBpIgASnIDziYAAFsAMkMvgCkqkCqCafSANwPcZxKAQAC2mBeECJqUy2VyLLZyAAJhApviUJzubz-gwBSk8hKHvhCcSVWTcEzGRQNdKwLSoCBkAaeXyTcTzXFJchphA4FACeq4uyud7jfgQWCLeNJpgQFlPqryes46D2gB3RbLVZZwik3IkcPRUuZ2MQIZWgkAImSYAbTMrGdwxd5+MbHJ1U0wDYpDY5mHzoZQKUwtNbydTYGQACNMJhdXAQMX43mCys1jWCMvVyGQOW24e1xua3Wew2AB732fn49dvGEu8PinZelMoA)
- genericμ΄ νμλ‘ μ λ¬λλ κ²μ λ³Ό μλ μλ€.

```js
interface SStorage<T> { //StorageλΌκ³  μ΄λ―Έ μ μΈλ JSμ μΉμ€ν λ¦¬μ§ APIλ₯Ό μν μΈν°νμ΄μ€κ° μ‘΄μ¬νκΈ° λλ¬Έμ μ΄λ¦μ SStorageλ‘ μ ν¨
  [key:string] : T //3οΈβ£ μΈν°νμ΄μ€μμ Genericμ μ¬μ©νλ€.
}

class LocalStorage<T> { //1οΈβ£ Genericμ ν΄λμ€λ‘ λ³΄λ΄κ³ 
  private storage: SStorage<T> = {} //2οΈβ£Classκ° interfaceλ‘ genericμ λ³΄λ΄κ³ 
  set(key:string, value:T){
    this.storage[key] = value;
  }
  remove(key:string){
    delete this.storage[key]
  }
  get(key:string):T {
    return this.storage[key]
  }
  clear(){
    this.storage = {}
  }
}

const stringStorage = new LocalStorage<string>()
stringStorage.get("ket")
stringStorage.set("hello","how are you")
const booleanStorage = new LocalStorage<boolean>()
booleanStorage.get("xxx")
booleanStorage.set("xxx",true)
```
