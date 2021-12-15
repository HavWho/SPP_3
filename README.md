# AssemblyBrowser (ТЗ)

### Необходимо реализовать графическую утилиту с использованием WPF для просмотра информации о составе произвольной .NET сборки. 
Содержимое загруженной сборки должно быть представлено в иерархическом виде (элемент управления TreeView): 
  - пространства имен; 
  - типы данных; 
  - поля, свойства и методы (информация о методах помимо имени должна включать сигнатуру, о полях и свойствах - тип).

#### Обязательным является применение MVVM, а также использование INotifyPropertyChanged и ICommand.

### Код лабораторной работы должен состоять из трех проектов:
  - библиотека, выполняющая сбор информации о сборке и построение удобной для отображения структу данных; (AssemblyBrowserLib)
  - модульные тесты для главной библиотеки; (Test и TestClass)
  - WPF-приложение, отображающее полученные данные о сборке.(View)

### Задание со звездочкой(*)
При построении дерева сборки необходимо учитывать объявленные в ней методы расширения (extension methods) и отображать их в составе класса, для которого объявлен метод
(а не в составе статического класса с методами расширения), с соответствующей пометкой. (методы помечены — "метод расширения")
