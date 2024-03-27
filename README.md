[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=14490530&assignment_repo_type=AssignmentRepo)
# Описание

Это **неофициальный** вариант аттестационной работы. Для отработки доступно 40 задач разной сложности, разделенных по группам:

- [Числа (int, float)](#группа-числа)
- [Строки и символы](#группа-символы-и-строки)
- [Логический тип данных](#группа-логический-тип-данных)
- [Условный оператор (if), оператор выбора (case)](#группа-условный-оператор)
- [Циклы (for, while)](#группа-циклы)

Для каждой группы задач создан свой файл. Для помощи в решении задач используйте **только** те ресурсы, которые разрешены правилами работы.

## Правила и регламент проведения аттестации

[Аттестация: правила, рекомендации и порядок проведения](https://hexly.notion.site/d9289c18871c44508bc7c7f05a51d94f)

## Группа Числа

Решения должны быть размещены в файле numbers.js

Для запуска теста используйте команду **test-numbers**

### Задача 1
Напишите и экспортируйте функцию `calculateDistance()`, которая находит расстояние между двумя точками на числовой оси с заданными координатами x1 и x2.

**Параметры:**

- x1: координата первой точки.
- x2: координата второй точки.

**Пример использования**
```javascript
calculateDistance(0, 5); // 5
calculateDistance(-3, 2); // 5
```

### Задача 2
Даны три точки A, B, C на числовой оси. Точка C расположена между точками A и B. Напишите и экспортируйте функцию `calculateSegmentProduct()`, которая находит произведение длин отрезков AC и BC.

**Параметры:**

- A: координата точки A.
- B: координата точки B.
- C: координата точки C.

**Пример использования**
```javascript
calculateSegmentProduct(0, 5, 2); // 6
calculateSegmentProduct(-1, 12, 7); // 40
```

### Задача 3
Дан размер файла в байтах. Напишите и экспортируйте функцию `calculateKilobytes()`, которая, используя операцию деления нацело, находит количество полных килобайтов, которые занимает данный файл (1 килобайт = 1024 байта).

**Параметры:**

- fileSizeInBytes: размер файла в байтах.

**Пример использования**
```javascript
calculateKilobytes(2048); // 2
calculateKilobytes(5000); // 4
```

### Задача 4
Даны целые положительные числа A и B (A > B). Напишите и экспортируйте функцию `calculateSegments()`, которая, используя операцию деления, находит количество отрезков B, размещенных на отрезке A.

**Параметры:**

- lengthA: длина отрезка A.
- lengthB: длина отрезка B.

**Пример использования**
```javascript
calculateSegments(10, 3); // 3
calculateSegments(15, 4); // 3
```

### Задача 5
Дано двузначное число. Напишите и экспортируйте функцию `calculateDigitSum()`, которая находит сумму цифр данного двузначного числа.

**Параметры:**

- twoDigitNumber: двузначное число.

**Пример использования**
```javascript
calculateDigitSum(47); // 11
calculateDigitSum(89); // 17
```

### Задача 6
Дано трехзначное число. Напишите и экспортируйте функцию `swapHundredsAndTens()`, которая возвращает число, полученное при перестановке цифр сотен и десятков исходного числа.

**Параметры:**

- twoDigitNumber: двузначное число.

**Пример использования**
```javascript
swapHundredsAndTens(123); // 213
swapHundredsAndTens(987); // 897
```

### Задача 7
Дано целое число, большее 999. Напишите и экспортируйте функцию `getHundredsDigit()`, которая, используя одну операцию деления нацело и одну операцию взятия остатка от деления, находит цифру, соответствующую разряду сотен в записи этого числа. Если число не соответствует условию, функция возвращает 0.

**Параметры:**

- number: целое число, большее 999.

**Пример использования**
```javascript
getHundredsDigit(1234); // 2
getHundredsDigit(9876); // 7
getHundredsDigit(500); // 0
```

### Задача 8
С начала суток прошло N секунд. Напишите и экспортируйте функцию `getFullHours()`, которая находит количество полных часов, прошедших с начала суток.

**Параметры:**

- seconds: целое число секунд.

**Пример использования**
```javascript
getFullHours(3600); // 1
getFullHours(7200); // 2
getFullHours(18000); // 5
```

### Задача 9
Дни недели пронумерованы следующим образом: 0 — воскресенье, 1 — понедельник, 2 — вторник, ..., 6 — суббота. Дано целое число K, лежащее в диапазоне 1–365. Напишите и экспортируйте функцию `getDayOfWeek()`, которая определяет номер дня недели для K-го дня года, если известно, что в этом году 1 января (первый день) было понедельником.

**Параметры:**

- dayOfYear: целое число от 1 до 365.

**Пример использования**
```javascript
getDayOfWeek(1); // 1
getDayOfWeek(10); // 3
getDayOfWeek(365); // 2
```

### Задача 10
Даны целые положительные числа A, B, C. Напишите и экспортируйте функцию `countSquares()`, которая на прямоугольнике размера A × B размещает максимально возможное количество квадратов со стороной C (без наложений) и возвращает их количество.

**Параметры:**

- A: целое положительное число (ширина прямоугольника).
- B: целое положительное число (длина прямоугольника).
- C: целое положительное число (сторона квадрата).

**Пример использования**
```javascript
countSquares(6, 4, 2); // 4
countSquares(8, 5, 3); // 2
countSquares(10, 10, 5); // 4
```

## Группа Символы и строки

Решения должны быть размещены в файле strings.js

Для запуска теста используйте команду **test-strings**

### Задача 1
Дана строка. Напиши и экспортируй функцию `countUppercaseLetters()`, которая подсчитывает количество прописных латинских букв в данной строке.

**Параметры:**

- str: строка, в которой нужно подсчитать прописные латинские буквы.

**Пример использования**
```javascript
countUppercaseLetters('HellO, World!'); // 3
countUppercaseLetters('JavaScript123'); // 2
countUppercaseLetters('no uppercase'); // 0
```

### Задача 2
Даны целые положительные числа N1 и N2 и строки S1 и S2. Напишите и экспортируйте функцию `combineStrings()`, которая создает новую строку, содержащую первые N1 символов строки S1 и последние N2 символов строки S2 (в указанном порядке).

**Параметры:**

- N1: количество символов, которые нужно взять из начала строки S1.
- N2: количество символов, которые нужно взять из конца строки S2.
- S1: первая строка.
- S2: вторая строка.

**Пример использования**
```javascript
combineStrings(3, 2, 'Hello', 'World'); // 'Helld'
combineStrings(2, 4, 'JavaScript', 'Coding'); // 'Jading'
combineStrings(1, 3, 'Apple', 'Banana'); // 'Aana'
```

### Задача 3
Даны строки S и S0. Напиши функцию `containsSubstring()`, которая проверяет, содержится ли строка S0 в строке S. Если содержится, то функция возвращает true, если не содержится, то false.

**Параметры:**

- S: основная строка.
- S0: подстрока, которую нужно проверить на наличие в основной строке.

**Пример использования**
```javascript
containsSubstring('Hello, World!', 'World'); // true
containsSubstring('JavaScript', 'CSS'); // false
containsSubstring('Programming is fun', 'gram'); // true
containsSubstring('OpenAI', 'AI'); // true
```

### Задача 4
Даны строки S, S1 и S2. Напиши функцию `replaceSubstring()`, которая заменяет в строке S первое вхождение строки S1 на строку S2.

**Параметры:**

- S: основная строка.
- S1: подстрока, которую нужно заменить.
- S2: строка, которой нужно заменить первое вхождение S1.

**Пример использования**
```javascript
replaceSubstring('Hello, World!', 'World', 'Universe'); // 'Hello, Universe!'
replaceSubstring('JavaScript is amazing', 'is', 'will be'); // 'JavaScript will be amazing'
replaceSubstring('Programming is fun', 'Java', 'Python'); // 'Programming is fun'
replaceSubstring('OpenAI', 'AI', 'Artificial Intelligence'); // 'OpenArtificial Intelligence'
```

### Задача 5
Дана строка, состоящая из английских слов, разделенных пробелами. Напиши функцию `countWordsWithSameLetters()`, которая находит количество слов, начинающихся и заканчивающихся одной и той же буквой.

**Параметры:**

- sentence: строка с английскими словами, разделенными пробелами.

**Пример использования**
```javascript
countWordsWithSameLetters('Moon Mellow Muffin'); // 0
countWordsWithSameLetters('Racecar radar level Civic'); // 4
countWordsWithSameLetters('Language Model'); // 0
countWordsWithSameLetters('WOW'); // 1
```

### Задача 6
Дана строка, состоящая из слов. Напиши функцию `countWordsWithA()`, которая находит количество слов, содержащих хотя бы одну букву «A».

**Параметры:**

- sentence: строка, состоящая из слов.

**Пример использования**
```javascript
countWordsWithA('Apple Banana Cherry'); // 2
countWordsWithA('Hello World'); // 0
countWordsWithA('Aardvark Zebra Elephant'); // 3
countWordsWithA('This is a sample sentence.'); // 2
```

### Задача 7
Дана строка-предложение с избыточными пробелами между словами. Напиши функцию `normalizeSpaces()`, которая преобразует строку так, чтобы между словами был ровно один пробел.

**Параметры:**

- sentence: строка-предложение с избыточными пробелами.

**Пример использования**
```javascript
normalizeSpaces('  Hello   world! '); // 'Hello world!'
normalizeSpaces('  This  is   a   sample    sentence. '); // 'This is a sample sentence.'
normalizeSpaces('  Multiple    spaces  between    some words. '); // 'Multiple spaces between some words.'
```

### Задача 8
Дана строка, содержащая полное имя файла, то есть имя диска, список каталогов (путь), собственно имя и расширение. Напиши функцию `extractFileName()`, которая выделяет из этой строки имя файла (без расширения).

**Параметры:**

- fullFileName: полное имя файла.

**Пример использования**
```javascript
extractFileName('C:/Users/username/Documents/example.txt'); // 'example'
extractFileName('../index.html'); // 'index'
extractFileName('/home/user/images/photo.jpg'); // 'photo'
```

### Задача 9
Дана строка-предложение. Напиши функцию `encryptSentence()`, которая зашифровывает ее, помещая в начало все символы, расположенные на четных позициях строки, а затем, в обратном порядке, все символы, расположенные на нечетных позициях.

**Параметры:**

- sentence: исходная строка-предложение.

**Пример использования**
```javascript
encryptSentence('JavaScript'); // 'aacitprSvJ'
encryptSentence('Hello, World!'); // 'el,Wrd!lo olH'
encryptSentence('Hexlet'); // 'eltexH'
```

### Задача 10
Дана строка, содержащая латинские буквы и круглые скобки. Напиши функцию `checkBrackets()`, которая проверяет правильность расстановки скобок в строке.

**Возвращаемое значение:**

Если скобки расставлены правильно, вернуть число 0.
В противном случае вернуть:
- Номер позиции первой ошибочной закрывающей скобки, если есть лишняя закрывающая скобка.
- -1, если закрывающих скобок не хватает.

**Параметры:**

- expression: строка с латинскими буквами и круглыми скобками.

**Пример использования**
```javascript
checkBrackets('((a + b) * (c - d))'); // 0
checkBrackets(')a + b) * (c - d)('); // 1
checkBrackets('(a + b) * (c - d))'); // 18
checkBrackets('((a + b) * (c - d)'); // -1
```

## Группа Логический тип данных

Решения должны быть размещены в файле boolean.js

Для запуска теста используйте команду **test-boolean**

**При решении задач этого типа запрещено использование условий (if,  case)**

### Задача 1
Дано целое число A. Напиши функцию `isPositive()`, которая проверяет истинность высказывания: «Число A является положительным».

**Параметры:**

- A: целое число.

**Пример использования**
```javascript
isPositive(5); // true
isPositive(-3); // false
isPositive(0); // false
```

### Задача 2
Дано целое число A. Напиши функцию `isOdd()`, которая проверяет истинность высказывания: «Число A является нечетным».

**Параметры:**

- A: целое число.

**Пример использования**
```javascript
isOdd(5); // true
isOdd(8); // false
isOdd(-3); // true
```

### Задача 3
Даны два целых числа: A и B. Напиши функцию `checkInequality()`, которая проверяет истинность высказывания: «Справедливы неравенства A > 2 и B ≤ 3».

**Параметры:**

- A: целое число.
- B: целое число.

**Пример использования**
```javascript
checkInequality(4, 3); // true
checkInequality(1, 2); // false
checkInequality(5, 1); // true
```

### Задача 4
Даны два целых числа: A и B. Напиши функцию `checkInequality2()`, которая проверяет истинность высказывания: «Справедливы неравенства A ≥ 0 или B < –2».

**Параметры:**

- A: целое число.
- B: целое число.

**Пример использования**
```javascript
checkInequality2(4, -3); // true
checkInequality2(-1, -2); // false
checkInequality2(0, 1); // true
```

### Задача 5
Даны три целых числа: A, B, C. Напиши функцию `checkBetweenNumbers()`, которая проверяет истинность высказывания: «Значение числа B находится между числами A и C».

**Параметры:**

- A: целое число.
- B: целое число.
- C: целое число.

**Пример использования**
```javascript
checkBetweenNumbers(1, 2, 3); // true
checkBetweenNumbers(5, 5, 8); // false
checkBetweenNumbers(10, 7, 5); // true
```

### Задача 6
Дано целое число. Напиши функцию `checkOddThreeDigitNumber()`, которая проверяет истинность высказывания: «Данное число является нечетным трехзначным».

**Параметры:**

- number: целое число.

**Пример использования**
```javascript
checkOddThreeDigitNumber(135); // true
checkOddThreeDigitNumber(246); // false
checkOddThreeDigitNumber(-789); // true
checkOddThreeDigitNumber(2458); // false
checkOddThreeDigitNumber(031); // false
```

### Задача 7
Дано трехзначное число. Напиши функцию `checkUniqueDigits()`, которая проверяет истинность высказывания: «Все цифры данного числа различны».

**Параметры:**

- number: целое число.

**Пример использования**
```javascript
checkUniqueDigits(123); // true
checkUniqueDigits(122); // false
checkUniqueDigits(-987); // true
checkUniqueDigits(1234); // false
checkUniqueDigits(-77); // false
```

### Задача 8
Даны числа x и y. Напиши функцию `isSecondQuadrant()`, которая проверяет истинность высказывания: «Точка с координатами (x, y) лежит во второй координатной четверти».
![Координатные четверти](https://acmp.ru/asp/article/image.asp?id=535)


**Параметры:**

- x: координата точки по оси X.
- y: координата точки по оси Y.

**Пример использования**
```javascript
isSecondQuadrant(-2, 3); // true
isSecondQuadrant(5, -1); // false
isSecondQuadrant(-1, -2); // false
```

### Задача 9
Даны целые числа a, b, c, являющиеся сторонами некоторого треугольника. Напиши функцию `isIsoscelesTriangle()`, которая проверяет истинность высказывания: «Треугольник со сторонами a, b, c является равнобедренным».
![Типы треугольников](https://schoolfiles.ru/wp-content/uploads/2021/11/tablitsa-vidy-treugolnikov-768x543.jpg)


**Параметры:**

- a: длина первой стороны треугольника.
- b: длина второй стороны треугольника.
- c: длина третьей стороны треугольника.

**Пример использования**
```javascript
isIsoscelesTriangle(3, 4, 3); // true
isIsoscelesTriangle(5, 7, 8); // false
isIsoscelesTriangle(5, 5, 6); // true
```

### Задача 10
Даны координаты двух различных полей шахматной доски x1, y1, x2, y2 (целые числа, лежащие в диапазоне 1–8,нумерация начинается с левого верхнего угла доски). Напиши функцию `areSameColorFields()`, которая проверяет истинность высказывания: «Данные поля имеют одинаковый цвет».

**Параметры:**

- x1: горизонтальная координата первого поля.
- y1: вертикальная координата первого поля.
- x2: горизонтальная координата второго поля.
- y2: вертикальная координата второго поля.

**Пример использования**
```javascript
areSameColorFields(1, 1, 2, 2); // true
areSameColorFields(3, 4, 5, 6); // true
areSameColorFields(7, 8, 1, 3); // false
```

## Группа Условный оператор

Решения должны быть размещены в файле branching.js

Для запуска теста используйте команду **test-branching**

### Задача 1
Дано целое число. Если оно является положительным, то прибавь к нему 1; в противном случае не изменяй его. Напиши функцию `incrementIfPositive()`, которая принимает целое число и возвращает полученное число.

**Параметры:**

- number: целое число.

**Пример использования**
```javascript
incrementIfPositive(5); // 6
incrementIfPositive(-3); // -3
incrementIfPositive(0); // 0
```

### Задача 2
Даны два числа. Вывести порядковый номер меньшего из них. Напиши функцию `getIndexOfSmallerNumber()`, которая принимает два числа и возвращает порядковый номер меньшего числа.

**Параметры:**

- number1: первое число.
- number2: второе число.

**Пример использования**
```javascript
getIndexOfSmallerNumber(5, 8); // 1
getIndexOfSmallerNumber(10, 3); // 2
getIndexOfSmallerNumber(7, 7); // 1 (порядковый номер первого числа при равенстве)
```

### Задача 3
Даны три числа. Найти среднее из них (то есть число, расположенное между наименьшим и наибольшим). Напиши функцию `findMiddleNumber()`, которая принимает три числа и возвращает среднее из них.

**Параметры:**

- number1: первое число.
- number2: второе число.
- number3: третье число.

**Пример использования**
```javascript
findMiddleNumber(5, 8, 3); // 5
findMiddleNumber(10, 3, 8); // 8
findMiddleNumber(7, 7, 7); // 7
```

### Задача 4
Даны четыре целых числа, одно из которых отлично от трех других, равных между собой. Напиши функцию `findUniqueNumber()`, которая принимает четыре числа и возвращает порядковый номер числа, отличного от остальных.

**Параметры:**

- number1: первое число.
- number2: второе число.
- number3: третье число.
- number4: четвертое число.

**Пример использования**
```javascript
findUniqueNumber(5, 5, 5, 8); // 4
findUniqueNumber(2, 2, 7, 2); // 3
findUniqueNumber(1, 0, 1, 1); // 2
```

### Задача 5
Для данного вещественного числа x напиши функцию `calculateF()`, которая находит значение следующей функции f, принимающей значения целого типа:
- Если \( x < 0 \), то \( f(x) = 0 \).
- Если \( x \in [0,1), [2,3), \ldots \), то \( f(x) = 1 \).
- Если \( x \in [1,2), [3,4), \ldots \), то \( f(x) = -1 \).

**Параметры:**

- x: вещественное число.

**Пример использования**
```javascript
calculateF(-1); // 0
calculateF(0.5); // 1
calculateF(1.5); // -1
```

### Задача 6
Для данного целого числа n, находящегося в диапазоне 1–999, напиши функцию `describeNumber()`, которая выводит строку-описание числа вида:

- "четное двузначное число" для четных двузначных чисел,
- "нечетное двузначное число" для нечетных двузначных чисел,
- "четное трехзначное число" для четных трехзначных чисел,
- "нечетное трехзначное число" для нечетных трехзначных чисел,
- и так далее.

**Параметры:**

- n: целое число в диапазоне 1–999.

**Пример использования**
```javascript
describeNumber(24); // "четное двузначное число"
describeNumber(137); // "нечетное трехзначное число"
describeNumber(5); // "нечетное однозначное число"
```

### Задача 7
Для данного целого числа dayNumber в диапазоне 1–7, используя конструкцию **switch-case**, напиши функцию `getDayName()`, которая возвращает строку — название дня недели, соответствующее данному числу. В качестве значения **default** укажите "Invalid day number."

**Параметры:**

- dayNumber: целое число в диапазоне 1–7.

**Пример использования**
```javascript
getDayName(1); // "monday"
getDayName(4); // "thursday"
getDayName(7); // "sunday"
```

### Задача 8
Для данного номера единицы длины unitNumber (1 — дециметр, 2 — километр, 3 — метр, 4 — миллиметр, 5 — сантиметр.) и длины отрезка в этих единицах lengthInUnits (вещественное число), используя конструкцию **switch-case**, напиши функцию `convertToMeters()`, которая возвращает длину отрезка в метрах.

**Параметры:**

- unitNumber: целое число в диапазоне 1–5.
- lengthInUnits: вещественное число, длина отрезка в выбранных единицах.

**Пример использования**
```javascript
convertToMeters(3, 10); // 10
convertToMeters(1, 5); // 0.5
convertToMeters(5, 2000); // 20
```

### Задача 9
Для данного возраста age (целое число в диапазоне 20–69), используя конструкцию **switch-case**, напиши функцию `describeAge()`, которая возвращает строку-описание указанного возраста с правильным согласованием числа со словом "год".


**Параметры:**

- age: целое число в диапазоне 20–69.

**Пример использования**
```javascript
describeAge(20); // "двадцать лет"
describeAge(32); // "тридцать два года"
describeAge(41); // "сорок один год"
```

### Задача 10
Для данного числа number (целое число в диапазоне 100–999), используя конструкцию **switch-case**, напиши функцию `describeNumber2()`, которая возвращает строку-описание указанного числа.

**Параметры:**

- number: целое число в диапазоне 100–999.

**Пример использования**
```javascript
describeNumber(256); // "двести пятьдесят шесть"
describeNumber(814); // "восемьсот четырнадцать"
```

## Группа Циклы

Решения должны быть размещены в файле loops.js

Для запуска теста используйте команду **test-loops**

**При решении задач этого типа запрещено использование условий (if,  case)**

### Задача 1
Для двух целых чисел A и B (где A < B), напиши функцию `sumOfSquares()`, используя цикл **for**. Функция должна вернуть сумму квадратов всех целых чисел от A до B включительно.

**Параметры:**

- A: целое число.
- B: целое число, больше A.

**Пример использования**
```javascript
sumOfSquares(2, 5); // Вернет 54 (2^2 + 3^2 + 4^2 + 5^2)
sumOfSquares(1, 3); // Вернет 14 (1^2 + 2^2 + 3^2)
```

### Задача 2
Для числа A и целого числа N (где N > 0), напиши функцию `power()`, используя цикл **for**. Функция должна вернуть результат возведения числа A в степень N.

**Параметры:**

- A: целое число.
- N: целое число, больше 0.

**Пример использования**
```javascript
power(2, 3); // 8 (2^3)
power(5, 2); // 25 (5^2)
```

### Задача 3
Для целого числа N (где N > 0), напиши функцию `factorialProduct()`, используя цикл **for**. Функция должна вернуть произведение N! = 1 * 2 * ... * N в виде вещественного числа.

**Параметры:**

- N: целое число, больше 0.

**Пример использования**
```javascript
factorialProduct(3); // 6 (1 * 2 * 3)
factorialProduct(5); // 120 (1 * 2 * 3 * 4 * 5)
```

### Задача 4
Для целого числа N (где N > 1), напиши функцию `fibonacciSequence()`, используя цикл **for**. Функция должна выводить элемент последовательности  [чисел Фибоначчи](https://ru.wikipedia.org/wiki/%D0%A7%D0%B8%D1%81%D0%BB%D0%B0_%D0%A4%D0%B8%D0%B1%D0%BE%D0%BD%D0%B0%D1%87%D1%87%D0%B8)
под номером N.

**Параметры:**

- N: целое число, больше 1.

**Пример использования**
```javascript
fibonacciSequence(5); // 5 (1, 1, 2, 3, 5)
fibonacciSequence(8); // 21 (1, 1, 2, 3, 5, 8, 13, 21)
```

### Задача 5
Для целого числа N (где N > 0), напиши функцию `sumOfPowers()`, используя цикл **for**. Функция должна находить сумму выражения 1^1 + 2^2 + ... + N^N.

**Параметры:**

- N: целое число, больше 0.

**Пример использования**
```javascript
sumOfPowers(3); // 32 (1^1 + 2^2 + 3^3)
sumOfPowers(5); // 3413 (1^1 + 2^2 + 3^3 + 4^4 + 5^5)
```

### Задача 6
Для положительных чисел A и B (где A > B), напиши функцию `remainingLength()`, используя цикл **while**. Функция должна находить длину незанятой части отрезка A, на котором размещено максимально возможное количество отрезков длины B (без наложений).

**Параметры:**

- A: положительное число.
- B: положительное число, меньшее A.

**Пример использования**
```javascript
remainingLength(10, 3); // 1 (Вернет длину незанятой части отрезка 10 после размещения максимально возможного количества отрезков длины 3, суммарная длина которых равна 9)
remainingLength(15, 4); // 3
```

### Задача 7
Для целого числа N (где N > 0), являющегося некоторой степенью числа 2 (N = 2^K), напиши функцию `findExponent()`, используя цикл **while**. Функция должна найти целое число K — показатель этой степени.

**Параметры:**

- N: целое число, являющееся степенью числа 2.

**Пример использования**
```javascript
findExponent(8); // 3 (2^3 = 8)
findExponent(32); // 5
```

### Задача 8
Для целого числа N (где N > 1), найди наименьшее целое число K, для которого выполняется условие: сумма чисел от 1 до K (включительно) будет больше или равна N. Напиши функцию `findMinKAndSum()`, используя цикл **while**.


**Параметры:**

- N: целое число.

**Пример использования**
```javascript
findMinKAndSum(10); // 4 (1 + 2 + 3 + 4 = 10)
findMinKAndSum(20); // 6 (1 + 2 + 3 + 4 + 5 + 6 = 21)
```

### Задача 9
Даны целые положительные числа A и B. Найти их наибольший общий делитель (НОД), используя [алгоритм Евклида](https://ru.wikipedia.org/wiki/%D0%90%D0%BB%D0%B3%D0%BE%D1%80%D0%B8%D1%82%D0%BC_%D0%95%D0%B2%D0%BA%D0%BB%D0%B8%D0%B4%D0%B0) и цикл **while**. Напиши функцию `calculateGCD()`.


**Параметры:**

- A, B: целые положительные числа.

**Пример использования**
```javascript
calculateGCD(48, 18); // 6
calculateGCD(27, 81); // 27
```

### Задача 10
Дано целое число N (> 1), являющееся числом Фибоначчи. Найти целое число K — порядковый номер числа Фибоначчи N. Напиши функцию `findFibonacciIndex()`. Нумерация элементов чисел Фибоначчи начинается с первой единицы.

**Параметры:**

- N: целое число, являющееся числом Фибоначчи.

**Пример использования**
```javascript
findFibonacciIndex(13); // 7
findFibonacciIndex(55); // 10
```