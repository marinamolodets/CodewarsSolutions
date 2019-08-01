
![Hello, Friends](https://covchurch.org/children/wp-content/uploads/sites/18/2013/01/Hello-Friends-logo-300x209.png)

### My solutions:

https://www.codewars.com/kata/students-final-grade/solutions/javascript
```javascript
function finalGrade (exam, projects) {
  if(exam > 90 || projects > 10) return 100;
  if(exam > 75 & projects >= 5) return 90;
  if(exam > 50 & projects >= 2) return 75;
  return 0;
}
```
https://www.codewars.com/kata/57356c55867b9b7a60000bd7/solutions/solutions
```javascript
function basicOp(operation, value1, value2) {
    switch (operation) {
        case '+':
            return value1 + value2;
        case '-':
            return value1 - value2;
        case '*':
            return value1 * value2;
        case '/':
            return value1 / value2;
        default:
            return 0;
    }
}
```
https://www.codewars.com/kata/5583090cbe83f4fd8c000051
```javascript
function digitize(n) {
  let arr = [];
  do{
    arr.push(n % 10);
    n  = Math.floor(n / 10); 
  } while (n !== 0);
  return arr;  
}
```
https://www.codewars.com/kata/5761a717780f8950ce001473
```javascript
function calculateAge(num1, num2) {
  let a = num2 - num1;
  if (a == -1) {
    return 'You will be born in 1 year.';
  }
  if (a < -1) {
    return `You will be born in ${Math.abs(a)} years.`;
  }
  if (a == 1) {
    return 'You are 1 year old.';
  }
  if (a > 1) {
    return `You are ${a} years old.`;
  }
  return 'You were born this very year!';
  
//   if( num1 > num2 ){
//     let a = num1 - num2;
//     if (a == 1) {
//       return 'You will be born in 1 year.';
//     }
//     return `You will be born in ${a} years.`;
//   }
//   if( num1 < num2 ){
//     let a = num2 - num1;
//     if (a == 1) {
//       return 'You are 1 year old.';
//     }
//     return `You are ${a} years old.`;
//   }
//   return 'You were born this very year!';
}
```
https://www.codewars.com/kata/5808dcb8f0ed42ae34000031
```javascript
function switchItUp(number) {
switch (number) {
  case 0:
    return( 'Zero' );
    break;
  case 1:
    return( 'One' );
    break;
  case 2:
    return( 'Two' );
    break;
  case 3:
    return( 'Three' );
    break;
  case 4:
    return( 'Four' );
    break;
  case 5:
    return('Five' );
    break;
  case 6:
    return( 'Six' );
    break;
  case 7:
    return( 'Seven' );
    break;
  case 8:
    return( 'Eight' );
    break;
  case 9:
    return( 'Nine' );
    break;
  }
}
```
https://www.codewars.com/kata/576b93db1129fcf2200001e6
```javaScript
function sumArray(array) {
  if( array == null || array == undefined  || array == [] || array.length == 1 ) {
    return 0;
  }
  let sum = 0;
  let max = array[0];
  let min = array[0];
  for( let i = 0; i < array.length; i ++ ) {
    sum += array[i];
    if (array[i] > max) {
      max = array[i];
    }
    if (array[i] < min) {
      min = array[i];
    }
  }
  sum -= max + min; 
  if(Number.isNaN(sum)) {
  return 0;
  }
  return sum;
}
    
  
```
