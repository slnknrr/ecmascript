# ecmascript
suggestion for ECMAScript &amp; JavaScript

# [2023-12-09] #
<a href="https://github.com/slnknrr/ecmascript/blob/main/suggest%202023-12-09.md">`suggest #1`</a> (2023-12-09/1) for custum concate types:<br>
```JavaScript
//@insecure when object; use class for this.<someInternalVariable>
//@deprecated caller: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/caller
//@deprecated arguments (includes callee): https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/arguments
var allInOne=Object.assign(function allInOne(skipNormalArgsProcessing) {
  for (var function_ of allInOne.functions) {
    function_(skipNormalArgsProcessing);
  }
},{
  Function(param) {
    allInOne.functions.push(param)
  },
  functions=[];
}

allInOne+func1+func2+func3;allInOne();

//not actual: var myInt=new BigInt('23');myInt.add('23223232323332323232323232323232323232323')
//actual:
class BigInt { constructor(){...}; String(){/*howto*/}; Number(){/*howto*/}; Self() {/**/}... } //'Self' for ++/--
var myInt=new BigInt();
myInt++; myInt++; myInt+14+'2323326327263761873683216812368213687321'
console.log(myInt)
```
`console.log` <- `2323326327263761873683216812368213687337`<br>
for more see <a href="https://github.com/slnknrr/ecmascript/blob/main/suggest%202023-12-09.md">`suggest #1`</a>
