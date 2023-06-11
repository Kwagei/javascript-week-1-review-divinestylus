# <strong> Sam B. Morris (@divinestylus) </strong> | JavaScript Assignment #4 
### Due Sunday, June 11, 2023 | 11:59 PM
<br>

### <strong> Problem Sets </strong>

1. Write a function that takes an array of numbers and returns the sum of the array.

```js
function arraySum(numbers) {
    let sum = 0;
    for (let i = 0; i < numbers.length; i++) {
        sum += numbers[i];
    }
    return sum;
}

arraySum([2,4,5,6,78,8]);
```

2. Write a function that takes an array of strings and returns the longest string in the array.

```js
let arr = ['Sam', 'Kpetermini', 'Nathan', 'Carlos', 'Blessing', 'James', 'Albin','Ben', 'Emmanuel'];

function longestStr(string) {
    let longStr = '';
    for (let i = 0; i < string.length; i++) {
        if (string[i].length > longStr.length) {
            longStr = string[i];
        }
    }
    return longStr;
}

longestStr(arr);
```

3. Write a function that takes an array of numbers and returns an array of the even numbers in the array.

```js
let arr = [1,2,4,6,334,6,65,6,2,34,,546,6544,653,677,77845453,3,44,5,6,65765,67566];

function evenArray(numbers) {
    let evenNum = [];
    for (let i = 0; i < numbers.length; i++) {
        if (numbers[i] % 2 === 0) {
            evenNum[evenNum.length] = numbers[i];
        }
    }
    return evenNum;
}

evenArray(arr);
```

4. Write a function that takes an array of numbers and returns an array of the numbers in reverse order.

```js
let arr = [100, 90, 80, 70, 60, 50, 40, 30, 20, 10, 0];

function reverseArray(numbers) {
    let reverseArr = [];
    for (let i = numbers.length -1; i >= 0; i--) {
        reverseArr[reverseArr.length] = numbers[i];
    }
    return reverseArr;
}

reverseArray(arr);
```

5. A word is given, write a function to tell if the word is a Palindrome.

```js
let palindromeStr = 'Level';

function isPalindrome(word) {
    word = word.toLowerCase();
    let palindrome = '';
    for (let i = word.length -1; i >= 0; i--) {
        palindrome += word[i];
    }
    if (palindrome === word) {
        return 'A palindrome';
    } else {
        return 'Not a palindrome';
    }
}

isPalindrome(palindromeStr);
```

6. Create a person object and create a method on the person object to update the name on the person object.

```js
let person = {
    name: 'Sam',
    male: true,
    nationality: 'Liberian',
    lonestarNum: 0880442708,
    orangeNum: 0776442708,
    email: 'divinestylus@gmail.com',
    updateName: function(newName) {
        this.name = newName;
    }
}

person.updateName('Sam B. Morris');
person.name;
```

7. Create an array of objects representing books. Each book should have properties for title and author. Write a function that takes the array of books and returns an array of book titles.

```js
let bookCollection = [{title: 'How to Win Friends and Influence People', author: 'Dale Carnegie'},
             {title: 'Business Strategy', author: 'Brian Tracy'},
             {title: 'The Da Vinci Code', author: 'Dan Brown'},
             {title: '48 Laws of Power', author: 'Robert Greene'},
             {title: 'The Richest Man in Babylon', author: 'George S. Clason'},
             {title: 'Why Nations Fail', author: 'Daron Acemoglu & James A. Robinson'},
             {title: 'The Art of War', author: 'SunTzu'},
             {title: 'Thinking for a Change', author: 'John C. Maxwell'},
             {title: 'Think and Grow Rich', author: 'Napoleon Hill'}];

function bookTitle(books) {
    let bookTtl = [];
    for (let i = 0; i < books.length; i++) {
        bookTtl[bookTtl.length] = books[i].title;
    }
    return bookTtl;
}

bookTitle(bookCollection);
```

8. Create an array of objects representing students. Each student should have properties for name and grade. Write a function that takes the array of students and returns an array of student names who have a grade higher than 90.

```js
let studentList = [{name: 'Francis Reeves', grade: 100},
                   {name: 'Tom Gbeyai', grade: 95},
                   {name: 'Michael Sherman', grade: 85},
                   {name: 'James Flomo', grade: 97},
                   {name: 'Aaron Sackie', grade: 88},
                   {name: 'Joshua Biley', grade: 78},
                   {name: 'Garrison Matthews', grade: 99},
                   {name: 'Stanley Dahn', grade: 70},
                   {name: 'Clementine Varney', grade: 76},
                   {name: 'Emmanuel Ngafua', grade: 92}];

function aStudents(students) {
    let aStud = [];
    for (let i = 0; i < students.length; i++) {
        if (students[i].grade > 90) {
            aStud[aStud.length] = students[i].name;
        }
    }
    return aStud;
}

aStudents(studentList);
```

9. Given an array of numbers, write a function that returns a new array with the numbers sorted in descending order.

```js
let arr = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100];

function descendingNum(numbers) {
    let descNum = [];
    for (let i = numbers.length; i >= 0; i--) {
        descNum[descNum.length] = numbers[i];
    }
    return descNum;
}

descendingNum(arr);
```

10. Create an object called "circle" with properties radius. Create a method on the object that calculates the circumference of the circle based on its radius.

```js
let circle = {
    pi: 3.14159,
    getCircum: function(radius) {
        let circum = 0;
        circum = 2 * this.pi * radius;
        return circum;
    }
}

circle.getCircum(30);
```
