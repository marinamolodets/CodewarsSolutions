
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
   https://www.codewars.com/kata/58ba6fece3614ba7c200017f
   

```javaScript
function palindrome(num) { 
  if (typeof(num) !=='number' || num < 0) {
    return "Not valid";
  }
  let str = '' + num;
  for (let i = 0; i < Math.floor(str.length / 2); i++) {
    if (str[i] !== str[str.length - 1 - i]) {
      return false;
    }
  }
  return true;
}  
```
https://www.codewars.com/kata/555bfd6f9f9f52680f0000c5
```javascript
function reverseNumber(n) {
  if (n >= 0) {
    let arr = n.toString().split('').reverse();
    return +(arr.join(''));
  } else {
    n = n * (-1);
    let arr = n.toString().split('').reverse();
    return (-1) * (+(arr.join('')));
  }
} 
```
https://www.codewars.com/kata/58712dfa5c538b6fc7000569
```javascript
function countRedBeads(n) {
  if (n < 2) {
    return 0; 
  }
  return (n - 1) * 2;
}
```
https://www.codewars.com/kata/5aca48db188ab3558e0030fa
```javascript
function calcType(a, b, res) {
  if (res === a * b) return "multiplication";
  if (res === a / b) return "division";
  if (res === a + b) return "addition";
  if (res === a - b) return "subtraction";
}
```
https://www.codewars.com/kata/56747fd5cb988479af000028
```javacript
function getMiddle(s) {
  for (let i = 0; i <= s.length/2; i++) {
    if (s.length % 2 === 0) {
    return s[s.length/2-1] + s[s.length/2];
    } else {
    return s[Math.floor(s.length/2)];
    }
  }
}

```
https://www.codewars.com/kata/54ff3102c1bad923760001f3
``` javascript
  function getCount(str) {
    let vowelsCount = 0;
    for(i = 0; i < str.length; i++) { 
      if (str[i] === 'a' || str[i] === 'e' || str[i] === 'i' || str[i] === 'o' || str[i] === 'u') {
      vowelsCount ++;
      }
    }
  return vowelsCount;
  }
```
https://www.codewars.com/kata/52774a314c2333f0a7000688
```javascript
function validParentheses(str){
  const stack = [],  open = ['(', '{', '['],  close = [')', '}', ']'];
  for(let i = 0; i < str.length; i++){
    if(open.includes(str[i])) {
      stack.push(str[i]);
    } else {
      if(close.indexOf(str[i]) === open.indexOf( stack[stack.length - 1])) {
        stack.pop();
      } else {
        return false;
      }
    }
   }
    return stack.length === 0;
}
```
https://www.codewars.com/kata/56c22cdbe0c0f7cae2001789
```javascript 
    const avg = a => a.reduce((a,b) => a + b) / a.length;
```
https://www.codewars.com/kata/56747fd5cb988479af000028
```javascript
    function getMiddle(s) {
      for (let i = 0; i <= s.length/2; i++) {
        if (s.length % 2 === 0) {
        return s[s.length/2-1] + s[s.length/2];
        } else {
        return s[Math.floor(s.length/2)];
        }
      }
    }
```
https://www.codewars.com/kata/57073869924f34185100036d
```javascript
   function randomCase(x) {
     let xNew = '';
       for (let i = 0; i < x.length; i++) {
         if(Math.round(Math.random()) > 0) {
         xNew += x[i].toUpperCase();
         } else {
         xNew += x[i].toLowerCase();
         }
       } 
     return xNew;
   }
 ```
 https://www.codewars.com/kata/5aa736a455f906981800360d
 ```javascript
    function feast(beast, dish) {
      if (beast[0] === dish[0] && beast[beast.length-1] === dish[dish.length-1]) {
      return true;
      } 
      return false;
    }
 ```
 https://www.codewars.com/kata/59d9ff9f7905dfeed50000b0
 ```javascript
    function solve(arr){  
      let alp = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ';
      let arr1 = [];
      for (let i = 0; i < arr.length; i++) {
        let count = 0;
        for (let j = 0; j < arr[i].length; j++) {
          if ( j === alp.indexOf(arr[i][j].toUpperCase()) ) {
            count++;
          }
        }
        arr1.push(count);
      }
      return arr1;
    }
 ```
 https://www.codewars.com/kata/57eae20f5500ad98e50002c5
 ```javascript
    function noSpace(x){
      let str = x.replace(/ /gi, '');
      return str;
    }
 ```
 ```javascript
    function noSpace(x){
    return x.replace(/\s/g, "")
    }
 ```
 https://www.codewars.com/kata/55a70521798b14d4750000a4
 ```javascript
    function greet(name){
      return `Hello, ${name} how are you doing today?`;
    }
 ```
 https://www.codewars.com/kata/string-ends-with/train/javascript/5d4bc3487a52805e514b12ed
```javascript
    function solution(str, ending){
      if (str.slice(str.length - ending.length) === ending) {
      return true;
      } else {
      return false;
      }
    }
```
```javascript
    function solution(str, ending){
      if (str.slice(str.length - ending.length) === ending) {
      return true;
      } else {
      return false;
      }
    }
```
https://www.codewars.com/kata/5982619d2671576e90000017
```javascript
   function spongeMeme(s) {
     let newStr = '';
     for (let i = 0; i < s.length; i++) {
       if (i % 2 == 0) {
       newStr += s[i].toUpperCase();
       } else {
       newStr += s[i].toLowerCase();
       }
     }
     return newStr;
   }
```
https://www.codewars.com/kata/56f6ad906b88de513f000d96
```javascript
   function bonusTime(salary, bonus) {
     let superSalary = salary * 10;
     if (bonus === true) {
     return "£" + superSalary;
     } else {
     return "£" + salary;
     }
   }
```
https://www.codewars.com/kata/51e704f2d8dbace389000279
```javascript
   function arraysSimilar(arr1, arr2) {
     return JSON.stringify(arr1.sort()) === JSON.stringify(arr2.sort());
   }
```
```javascript
   function arraysSimilar(arr1, arr2) {
     if(arr1.length !== arr2.length) return false;
     
     arr1.sort();
     arr2.sort();
     
     for (let i = 0; i < arr1.length; i++) {
       if (arr1[i] !== arr2[i]) return false; 
     }
     return true;
   }
```
https://www.codewars.com/kata/5594463eaf1701909c0000d4
```javascript
    function arraySum(arr) {
      const b = arr.toString().split(',');
      let sum = 0;
      
      for (let i = 0; i < b.length; i++) {
        sum += Number.isNaN(Number(b[i]))? 0 : Number((b[i]));
      }
      return sum;
    }
```
https://www.codewars.com/kata/57a5b0dfcf1fa526bb000118
```javascript
   function distinct(a) {
     return [...new Set(a)];
   }
```
```javascript
   function distinct(a) {
     const items = {};
     const res = [];
     for (let i = 0; i < a.length; i++){
       if (!items[a[i]]) {
       res.push(a[i]);
       items[a[i]] = true;
       }
     }
     return res;
   }
```
