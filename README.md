<p align = "center">МИНИСТЕРСТВО НАУКИ И ВЫСШЕГО ОБРАЗОВАНИЯ<br>
РОССИЙСКОЙ ФЕДЕРАЦИИ<br>
ФЕДЕРАЛЬНОЕ ГОСУДАРСТВЕННОЕ БЮДЖЕТНОЕ<br>
ОБРАЗОВАТЕЛЬНОЕ УЧРЕЖДЕНИЕ ВЫСШЕГО ОБРАЗОВАНИЯ<br>
«САХАЛИНСКИЙ ГОСУДАРСТВЕННЫЙ УНИВЕРСИТЕТ»</p>
<br><br><br><br><br><br>
<p align = "center">Институт естественных наук и техносферной безопасности<br>Кафедра информатики<br>Иванюшин Виталий петрович</p>
<br><br><br>
<p align = "center"><br><strong>Лабораторная работа №7.«CSS»</strong><br>01.03.02 Прикладная математика и информатика</p>
<br><br><br><br><br><br><br><br><br><br><br><br>
<p align = "right">Научный руководитель<br>
Соболев Евгений Игоревич</p>
<br><br><br>
<p align = "center">г. Южно-Сахалинск<br>2024 г.</p>
<br><br><br><br><br><br><br><br><br><br><br><br>

<h1 align = "center">Введение</h1>

<p><b>HTML</b> —  стандартизированный язык гипертекстовой разметки документов для просмотра веб-страниц в браузере. Веб-браузеры получают HTML документ от сервера по протоколам HTTP/HTTPS или открывают с локального диска, далее интерпретируют код в интерфейс, который будет отображаться на экране монитора.</p>
<p><b>CSS</b> — формальный язык описания внешнего вида документа, написанного с использованием языка разметки. Также может применяться к любым XML-документам, например, к SVG или XUL.</p>


<h1 style="text-align: center">Задачи JS</h1>
<ol>
    <li>Выполнить задания по JS</li>
</ol>



<h1 style="text-align: center">Решения HTML</h1>

<h2 style="text-align: center">Задания 1-5</h2>

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <script>

        //1
                    function findNumbersDivisibleBy(arr, divisor) 
            {
                return arr.filter(num => num % divisor === 0);
            }

            const numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
            const divisor = 2;

            const numbersDivisibleByDivisor = findNumbersDivisibleBy(numbers, divisor);
            console.log('Задание 1 = ' + numbersDivisibleByDivisor); // Выведет [2, 4, 6, 8, 10]

            
            //2
                        function isAnagram(str1, str2) {
                const cleanString = (str) => str.replace(/[^\w]/g, '').toLowerCase();
                
                const cleanStr1 = cleanString(str1);
                const cleanStr2 = cleanString(str2);

                if (cleanStr1.length !== cleanStr2.length) {
                    return false;
                }

                const sortedStr1 = cleanStr1.split('').sort().join('');
                const sortedStr2 = cleanStr2.split('').sort().join('');

                return sortedStr1 === sortedStr2;
            }

            const string1 = "клоун";
            const string2 = "уклон";

            if (isAnagram(string1, string2)) {
                console.log('Задание 2 = ' + "Строки являются анаграммами.");
            } else {
                console.log('Задание 2 = ' + "Строки не являются анаграммами.");
            }

            //3

                        function countVowels(str) {
                const vowels = ['a', 'e', 'i', 'o', 'u'];
                let count = 0;

                str = str.toLowerCase();

                for (let char of str) {
                    if (vowels.includes(char)) {
                        count++;
                    }
                }

                return count;
            }

            const inputString = "Hello, World!";
            const vowelsCount = countVowels(inputString);

            console.log('Задание 3 = ' + `Количество гласных в строке "${inputString}" равно ${vowelsCount}.`);

            //4
                            const height = 7; // задаем высоту треугольника

                for (let i = 1; i <= height; i++) {
                    let row = '';
                    for (let j = 1; j <= i; j++) {
                        row += '#';
                    }
                    console.log(row);
                }

            //5
                        for (let i = 1; i <= 100; i++) {
                if (i % 3 === 0 && i % 5 === 0) {
                    console.log('FizzBuzz');
                } else if (i % 3 === 0) {
                    console.log('Fizz');
                } else if (i % 5 === 0) {
                    console.log('Buzz');
                } else {
                    console.log(i);
                }

            }
    </script>
</body>
</html>
```
<h2 style="text-align: center">Задания 6-13</h2>

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <script>

        //6
        const size = 8; // размер доски
let board = '';

for (let i = 0; i < size; i++) {
    for (let j = 0; j < size; j++) {
        if ((i + j) % 2 === 0) {
            board += ' '; // добавляем пробел, если сумма координат четная
        } else {
            board += '#'; // добавляем решетку, если сумма координат нечетная
        }
    }
    board += '\n'; // добавляем символ новой строки после каждой строки
}

console.log(board);


//7
function min(a, b) {
    return a < b ? a : b;
}

// Пример использования функции
console.log('Задание 7 = ' + min(5, 3));


//8

function isEven(n) {
    if (n === 0) {
        return true;
    } else if (n === 1) {
        return false;
    } else if (n < 0) {
        return isEven(-n);
    } else {
        return isEven(n - 2);
    }
}

// Тестирование функции
console.log('Задание 8 = ' + isEven(50)); // Выведет true, так как 50 - чётное число
console.log('Задание 8 = ' + isEven(75)); // Выведет false, так как 75 - нечётное число
console.log('Задание 8 = ' + isEven(-1)); // Выведет false, так как мы используем рекурсию с положительными числами

//9

function countBs(str) {
    let count = 0;
    for (let i = 0; i < str.length; i++) {
        if (str.charAt(i) === 'B') {
            count++;
        }
    }
    return count;
}

function countChar(str, char) {
    let count = 0;
    for (let i = 0; i < str.length; i++) {
        if (str.charAt(i) === char) {
            count++;
        }
    }
    return count;
}

// Пример использования
let sampleString = "Bob has a blue ball.";
console.log('Задание 9 = ' + countBs(sampleString)); // Выведет количество символов 'B' в строке
console.log('Задание 9 = ' + countChar(sampleString, 'a')); // Выведет количество символов 'a' в строке



//10
function range(start, end, step = 1) {
    let arr = [];
    if (step > 0) {
        for (let i = start; i <= end; i += step) {
            arr.push(i);
        }
    } else {
        for (let i = start; i >= end; i += step) {
            arr.push(i);
        }
    }
    return arr;
}

function sum(arr) {
    let total = 0;
    for (let num of arr) {
        total += num;
    }
    return total;
}

let numbers = range(1, 10);
console.log(sum(numbers)); // Выведет сумму чисел от 1 до 10, то есть 55

let numbers2 = range(1, 10, 2);
console.log(numbers2); // Выведет [1, 3, 5, 7, 9]

let numbers3 = range(5, 2, -1);
console.log(numbers3); // Выведет [5, 4, 3, 2]

//11
function reverseArray(arr) {
    let reversedArr = [];
    for (let i = arr.length - 1; i >= 0; i--) {
        reversedArr.push(arr[i]);
    }
    return reversedArr;
}

function reverseArrayInPlace(arr) {
    for (let i = 0; i < Math.floor(arr.length / 2); i++) {
        let temp = arr[i];
        arr[i] = arr[arr.length - 1 - i];
        arr[arr.length - 1 - i] = temp;
    }
    return arr;
}

let originalArray = [1, 2, 3, 4, 5];
let reversedArray = reverseArray(originalArray);
console.log(reversedArray); // Выведет [5, 4, 3, 2, 1]

let arrayToReverse = [1, 2, 3, 4, 5];
reverseArrayInPlace(arrayToReverse);
console.log(arrayToReverse); // Выведет [5, 4, 3, 2, 1]


//12
function deepEqual(value1, value2) {
    if (value1 === value2) {
        return true;
    }

    if (value1 == null || typeof value1 != "object" || value2 == null || typeof value2 != "object") {
        return false;
    }

    let keys1 = Object.keys(value1);
    let keys2 = Object.keys(value2);

    if (keys1.length !== keys2.length) {
        return false;
    }

    for (let key of keys1) {
        if (!keys2.includes(key) || !deepEqual(value1[key], value2[key])) {
            return false;
        }
    }

    return true;
}

// Примеры использования функции deepEqual
let obj1 = {a: 1, b: {c: 2}};
let obj2 = {a: 1, b: {c: 2}};
console.log(deepEqual(obj1, obj2)); // Выведет true

let obj3 = {a: 1, b: {c: 3}};
console.log(deepEqual(obj1, obj3)); // Выведет false

//13
let arrayOfArrays = [[1, 2], [3, 4], [5, 6]];

let flattenedArray = arrayOfArrays.reduce((accumulator, currentArray) => {
    return accumulator.concat(currentArray);
}, []);

console.log(flattenedArray);
    </script>

</body>
</html>
```



<h1 align = "center">Вывод</h1>
<p>По итогу проделанной лабораторной работы, были выполнены задания по JS</p>
