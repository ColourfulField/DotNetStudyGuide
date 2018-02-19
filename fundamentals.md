**Общие основы C\#**

Прочитайте книгу "Карманный справочник по C\# 6.0." \([http://mirknig.su/knigi/programming/16081-c-60-karmannyy-spravochnik-fayly.html\](http://mirknig.su/knigi/programming/16081-c-60-karmannyy-spravochnik-fayly.html%29\)

##### Рефлексия

Рефлексия - это инструмент, который позволяет считывать информацию о типах сборки \(assembly types\) прямо во время выполнения программы. Она понадобится вам при выполнении следующего практического задания :\)

Полезные материалы:  
Рефлексия на метаните \(несколько запутанно описано\) [https://metanit.com/sharp/tutorial/14.1.php](https://metanit.com/sharp/tutorial/14.1.php)

Рефлексия на MSDN [https://docs.microsoft.com/ru-ru/dotnet/csharp/programming-guide/concepts/reflection](https://docs.microsoft.com/ru-ru/dotnet/csharp/programming-guide/concepts/reflection)

Хороший ресурс на английском \(с примерами кода\) [https://stackify.com/what-is-c-reflection/](https://stackify.com/what-is-c-reflection/)

**Практическая задача**

1\) Откройте Visual Studio, и создайте консольное приложение. 

2\) Создайте несколько классов, каждый из которых будет содержать как минимум один метод с названием "StartTest". При вызове этого метода должен выполняться тестовый код, и результаты его вывода должны быть выведены в консоль соответственно результатам теста. Пример:

Вы пишете код для тестирования операторов out и ref. Ваш класс может называться "TestOutRef", а случае консольный вывод может выглядеть следующим образом:

-----Out/Ref Test-----

value before: 0

value after: 10

Тесты нужно писать для каждого раздела книги, который не был для вас абсолютно очевидным. Если все разделы книги были абсолютно очевидны, то нужно написать не меньше трех тестовых классов.

3\) Напишите в классе Program \(стартовый класс приложения\) код, который вызовет все ваши тестовые методы.

4\) Перепишите программу таким образом, чтобы при добавлении нового класса по шаблону. описанному в пункте 2, программа вызвала этот метод без добавления дополнительного кода \(кода, конструирующего объект нового класса, и вызывающего его вручную\).

5\) при написании кода  пытайтесь применять принципы SOLID.

* 
* Implement a method which would call StartTest method for all example classes using reflection

* End goal : ability to add a TestXXX class with StartTest method, which would be called

automatically on program startup

