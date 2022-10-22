# 🚀 TypeScript 처음 시작하기
타입스크립트에 첫 입문하면서 노마드코더님의 강의 [Typescript로 블록체인 만들기](https://nomadcoders.co/typescript-for-beginners/lobby)를 들으며 실습하고 정리한 기록입니다.

</br></br>

## 💙 typeScript ➕ VScode
타입스크립트와 vs코드가 같은 마이크로 소프트에서 만들었기 때문에 호환이 아주잘되어서 개발자 경험이 좋다.

</br></br>

## ⚠️ Why not JavaScript
* 타입스크립트는 자바스크립트에 비해 **타입 안전성**이 좋다. => 개발자 경험이 좋다. 버그를 줄일 수 있다. 런타임 에러 줄인다. 생산성 증대시킨다.
* 자바스크립트는 타입 안전성이 없다.
* 자바스크립트는 되도록 에러를 보여주지 않으려 알아서 처리하는 일이 많다. 이게 개발자에게 별로 도움이 안된다.
```js
/*
😳 자바스크립트는 이렇게 이상한 코드도 실행시켜준다.
다른 언어에선 꿈도 못 꿀 일
*/

[1, 2, 3, 4] + false //'1,2,3,4false'
//배열 + 불리언 = 스트링(불리언도 스트링으로 합쳐짐)


function divide(a,b){
    return a / b
}
divide(2,3) //0.6666666666666666
divide("xxxxxxxx") //NaN (코드 실행을 막아주고 있지 않다. 이게 실행되면 안되는 거지😫!!)

//인자로 숫자를 전달해야 하는지 문자를 전달해야하는지, 몇개의 인자를 전달해야하는지 이런것들을 정해서 잘못보냈으면 체크해야 한다!!
```
* 런타임 에러는 콘솔 안에서 일어나는 에러이다. (이런 에러는 유저의 컴퓨터에서 코드가 실행될 때만 일어나는 에러일 수도 있다.)
* 자바스크립트 런타임 오류는 유저나 매니저나 동료 개발자들이 알아차리고 알려주는 경우가 많다! 
```js
const nico = { name: "nico" }
nico.hello() //Uncaught TypeError: nico.hello is not a function

/*지금처럼 ⚠️컴퓨터가 실행시키고 나서 에러를 출력하는 것이 아니라⚠️
실행시키기 전에 hello()라는 함수가 없다는 걸 알려주고 ✨"고치면 실행시켜줄게!"✨가 가장 좋다.*/
```
* **말도안되는 코드**를 **실행이아니라 작성 단계부터** 바로잡는 것! 그게 바로 타입스크립트가 자바스크립트보다 진화된 면이라고 볼 수 있다.

</br></br>

## 🤔 How TypeScript Works
* 타입스크립트는 strongly typed programmin language 강력한 타입을 가진 프로그래밍 언어이다.
* 타입스크립트로 작성한 코드는 자바스크립트로 변환된다.[타입스크립트 플레이그라운드](https://www.typescriptlang.org/play?#code/PTAEHUFMBsGMHsC2lQBd5oBYoCoE8AHSAZVgCcBLA1UABWgEM8BzM+AVwDsATAGiwoBnUENANQAd0gAjQRVSQAUCEmYKsTKGYUAbpGF4OY0BoadYKdJMoL+gzAzIoz3UNEiPOofEVKVqAHSKymAAmkYI7NCuqGqcANag8ABmIjQUXrFOKBJMggBcISGgoAC0oACCbvCwDKgU8JkY7p7ehCTkVDQS2E6gnPCxGcwmZqDSTgzxxWWVoASMFmgYkAAeRJTInN3ymj4d-jSCeNsMq-wuoPaOltigAKoASgAywhK7SbGQZIIz5VWCFzSeCrZagNYbChbHaxUDcCjJZLfSDbExIAgUdxkUBIursJzCFJtXydajBBCcQQ0MwAUVWDEQC0gADVHBQGNJ3KAALygABEAAkYNAMOB4GRonzFBTBPB3AERcwABS0+mM9ysygc9wASmCKhwzQ8ZC8iHFzmB7BoXzcZmY7AYzEg-Fg0HUiQ58D0Ii8fLpDKZgj5SWxfPADlQAHJhAA5SASPlBFQAeS+ZHegmdWkgR1QjgUrmkeFATjNOmGWH0KAQiGhwkuNok4uiIgMHGxCyYrA4PCCJSAA)로 실험해 볼 수 있다.
* 타스 ➡️ 자스로 변환하는 이유는 브라우저와 Node.js가 타스가 아니라 자스를 이해하기 때문이다. 
* 타입스크립트가 그저 자바스크립트를 변환해 줄 뿐이라면 어떻게 우리를 보호해 주는 걸까?? ➡️ 타입스크립트 코드가 자바스크립트로 변환되기 **전**에 타스가 먼저 우리의 코드를 확인한 다음에 자스에서 바보같은 실수가 일어나지 않게 보호장치를 발동시킨다! **타입스크립트 코드에 에러가 있으면 자스로 아예 컴파일이 되지 않는다.** 이런 보호장치가 유저가 코드를 실행하는 런타임에 발생하는 게 아니다.
