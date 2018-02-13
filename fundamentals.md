**Общие основы C\#**

Прочитайте книгу "Карманный справочник по C\# 6.0." \([http://mirknig.su/knigi/programming/16081-c-60-karmannyy-spravochnik-fayly.html\](http://mirknig.su/knigi/programming/16081-c-60-karmannyy-spravochnik-fayly.html\)\)

##### Рефлексия

Рефлексия - это инструмент, который позволяет считывать информацию о типах сборки \(assembly types\) прямо во время выполнения программы. Она понадобится вам при выполнении следующего практического задания :\)

Полезные материалы:  
Рефлексия на метаните \(несколько запутанно описано\) [https://metanit.com/sharp/tutorial/14.1.php](https://metanit.com/sharp/tutorial/14.1.php)

Рефлексия на MSDN [https://docs.microsoft.com/ru-ru/dotnet/csharp/programming-guide/concepts/reflection](https://docs.microsoft.com/ru-ru/dotnet/csharp/programming-guide/concepts/reflection)

Хороший ресурс на английском \(с примерами кода\) [https://stackify.com/what-is-c-reflection/](https://stackify.com/what-is-c-reflection/)



**Практическая задача**

Создайте консольное приложение



Practice task: Create console app and implement examples from the book without looking at these examples.

TASK: - Refactor examples from previous step so that each example is located in a separate folder.

* Create special TestXXX classes for each example, where XXX is the name of the example \(i.e. TestExtensionMethods, TestNullPropagation\).

* In each of these classes implement a StartTest method, which outputs test data to console \(i.e. a string before and after applying extension method to it\).

* Implement a method which would call StartTest method for all example classes using reflection

* End goal : ability to add a TestXXX class with StartTest method, which would be called

automatically on program startup

