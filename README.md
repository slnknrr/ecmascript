# ecmascript
suggestion for ECMAScript &amp; JavaScript

1. concate types //emulate some types like Integer, BigNumber, bitfield, custum digits for numbers, etc<br>
1.1. `<Type>.prototype.<Type>` (Array+String native or custum concate if you wanna)<br>
1.2. `<Type>.<Type>` (class custum concate):
```JavaScript
myInt=new BigInt('123');
myInt.add('21397627623187126863762183267123286126321872681368721637218321621381237632187')
```
to
```JavaScript
class BigInt { constructor(...) {...; this.Number = function howToConcatNumber() { ... }; this.String = function howToConcatString() { ... }; ....} ... }
myInt = new BigInt('123');
BigInt+1+'21397627623187126863762183267123286126321872681368721637218321621381237632186'
//-> BigInt#Number(1) <- is private (mb.) -> this.Number(1) -> howToConcatNumber(1);
//-> BigInt#String('21397627623187126863762183267123286126321872681368721637218321621381237632186') <- is private (mb.) -> this.String(1) -> howToConcatString(1);
```
rise, JS!
