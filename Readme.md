# Контрольная работа

## Перечень задач:
1. [Создать репозиторий на GitHub](#task1)
2. [Нарисовать блок схему алгоритма](#task2)
3. [Снабдить репозиторий оформленным текстовым описанием (файл Readмe.md)](#task3)
4. [Написать программу, решающую поставленную задачу](#task4)
5. [Использовать контроль версий в работе над этим небольшим проектом (не должно быть так что все залито одним коммитом, как минимум этап 2, 3 и 4 должны быть расположены в разных коммитах)](#task5)

## Результаты решений:
### <a name="task1"></a>1. Создать репозиторий на GitHub
Ссылка на созданный репозиторий -> [github.com/arhangel2i/Control_Work][id1]

### <a name="task2"></a>2. Нарисовать блок схему алгоритма
Блок схема алгоритма расположенна непосредственно на самом репозитории -> [block_diagram.png][id2]

>т.к. в алгоритме есть сокращенные места или в псевдо коде использованны операторы присуще определенному языку см. сноски
### <a name="task3"></a>3. Снабдить репозиторий оформленным текстовым описанием (файл ReadMe.md)
Ссылка на файл Readme -> [Readme.md][id3]

### <a name="task4"></a>4. Написать программу, решающую поставленную задачу
>***Задача:*** Написать программу, которая из имеющегося массива строк формирует массив из строк, длина которых меньше либо равна 3 символа. первоначальный массив можно ввести с клавиатуры, либо задать на старте выполнения алгоритма<br/>*При решении не рекомендуеться пользоваться коллекциями, лучше обойтись исключительно массивами*

Ссылка на файл Program.cs -> [Source/Program.cs][id4]

В коде используются операторы которые были рассмотрены самостоятельно

- операторы по преобразованию текста в массив и обратно:
```C#
//оператор .Split
//строка преобразуеться в массив где разделителем между элементами является ,
//например
string strLine = "шорох,порох,высота";
string[] inArr = strLine.Split(",");
//результатом выполнения будет
//inArr[0]="шорох" : inArr[1]="порох" : inArr[2]="высота"

//оператор .Join
//преобразует массив в текстовую строку разделяя элементы , 
string resultJoin = string.Join(",", inArr);
//результатом выполнения будет
//resultJoin="шорох,порох,высота"
```
- оператор для увеличения размера массива
```C#
//оператор Array.Resize
//увеличивает размер массива с сохранением данных находящихся в нем
string[] outArr = new string[1];
outArr[0]="Hello";
Array.Resize(ref outArr, outArr.Length + 1);
outArr[1]="World";
//результатом выполнения будет
// outArr[0]="Hello" : outArr[1]="World"
```
### <a name="task5"></a>5. Использовать контроль версий в работе над этим небольшим проектом (не должно быть так что все залито одним коммитом, как минимум этап 2, 3 и 4 должны быть расположены в разных коммитах)

Ссылка на список коммитов -> [https://github.com/arhangel2i/Control_Work/commits/master][id5]

[id1]: https://github.com/arhangel2i/Control_Work
[id2]: block_diagram.png
[id3]: Readme.md
[id4]: Source/Program.cs
[id5]: https://github.com/arhangel2i/Control_Work/commits/master