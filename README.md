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


<h1 style="text-align: center">Задачи CSS</h1>
<ol>
    <li>Выполнить задания по PHP и JS</li>
</ol>



<h1 style="text-align: center">Решения HTML</h1>

<h2 style="text-align: center">Задания 1-18</h2>

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
        // 1. 
        var str = 'hdfgv';
        console.log('Задание 1 = ' + str[0]); // 'h'
        console.log('Задание 1 = ' + str[1]); // 'd'
        console.log('Задание 1 = ' + str[4]); // 'v'
    </script>


    <script>
        // 2. 
        var secondsInHour = 60 * 60;
        console.log('Задание 2 = ' + secondsInHour);
    </script>


        <script>
                // 3.
            var num = 1;
            num += 12;
            num -= 14;
            num *= 5;
            num /= 7;
            num++;
            num--;
            console.log('Задание 3 = ' + num);

            // 4.
            var num = 3;
            alert('Задание 4 = ' + num);

            // 5.
            var a = 10;
            var b = 2;
            console.log('Задание 5 = ' + 'Сумма:', a + b);
            console.log('Задание 5 = ' + 'Разность:', a - b);
            console.log('Задание 5 = ' + 'Произведение:', a * b);
            console.log('Задание 5 = ' + 'Частное:', a / b);

            // 6.
            var c = 15;
            var d = 2;
            var result = c + d;
            console.log('Задание 6 = ' + result);

            // 7.
            var a = 10;
            var b = 2;
            var c = 5;
            console.log('Задание 7 = ' + 'Сумма:', a + b + c);
             
            // 8.
            var a = 17;
            var b = 10;
            var c = a - b;
            var d = 7;
            var result = c + d;
            console.log('Задание 8 = ' +  result);

            // 9.
            var secondsInHour = 60 * 60;
            var secondsInDay = secondsInHour * 24;
            var secondsInMonth = secondsInDay * 30; // упрощенно, без учета разной длины месяцев
            console.log('Задание 9 = ' + 'Секунд в часе:', secondsInHour);
            console.log('Задание 9 = ' + 'Секунд в сутках:', secondsInDay);
            console.log('Задание 9 = ' + 'Секунд в месяце:', secondsInMonth);

            // 10.
            var hour = new Date().getHours();
            var minute = new Date().getMinutes();
            var second = new Date().getSeconds();
            console.log('Задание 10 = ' + hour + ':' + minute + ':' + second);

            // 11.
            var number = 5;
            var square = Math.pow(number, 2);
            console.log('Задание 11 = ' + square);

            // 12.
            let arr = [1, 2, 3, 4, 5, 6];
            let sum = arr.reduce((acc, curr) => curr % 2 === 0 ? acc + Math.sqrt(curr) : acc, 0);
            console.log('Задание 12 = ' + sum);

            // 13.
            let applePrice = 1.15;
            let orangePrice = 2.30;
            let totalPrice = applePrice + orangePrice;
            console.log('Задание 13 = ' + totalPrice);

            // 14.
            let x = 5;
            alert('Задание 14 = ' + x++); // Выведет 5

            // 15.
            console.log('Задание 15 = ' + [ ] + false - null + true); // Выведет NaN

            // 16.
            let y = 1;
            let x1 = y = 2;
            console.log('Задание 16 = ' +  x1); // Выведет 2

            // 17.
            console.log('Задание 17 = ' + [ ] + 1 + 2); // Выведет "12"

            // 18.
            let a6 = 5 % 3; // 2
            let a7 = 3 % 5; // 3
            let a8 = 5 + '3'; // "53"
            let a9 = '5' - 3; // 2
            let a10 = 75 + 'кг'; // "75кг"

            console.log('Задание 18 = ' + a6 + ' ' + a7 + ' ' +  a8 + ' ' + a9 + ' ' + a10 );
            
        </script>

        
</body>
</html>
```
<h2 style="text-align: center">Задания 19-23</h2>

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
        // 19.
    let height = 23;
    let width = 10;
    let s = height * width;
    console.log('Задание 19 = ' + s);

    // 20.
    let heightC = 10;
    let dC = 4;
    let radius = dC / 2;
    let v = Math.PI * radius * radius * heightC;
    console.log('Задание 20 = ' + v);

    // 21.
    let S = 2000000;
    let p = 0.1;
    let years = 5;
    let perepl = S * p * years;
    console.log('Задание 21 = ' + perepl);

    // 22.
    let str = 'Привет';
    let num1 = 123;
    let flag = true;
    let txt = 'true';
    console.log('Задание 22 = ' + typeof str);
    console.log('Задание 22 = ' + typeof num1);
    console.log('Задание 22 = ' + typeof flag);
    console.log('Задание 22 = ' + typeof txt);

    // 23.
    function oppositeNumber(num) {
        return -num;
    }

    let number1 = 5;
    let opposite = oppositeNumber(number1);
    console.log('Задание 23 = ' + opposite);
</script>
</body>
</html>
```



<h1 align = "center">Вывод</h1>
<p>По итогу проделанной лабораторной работы, были выполнены задания по JS</p>
