
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
