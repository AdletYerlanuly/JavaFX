# JavaFX
Было выполнено 9 заданий на 9 недель:

#1 - Программирование на Java
Установил приложения intellij idea, scene builder, JDK.

#2 - Коллекции данных ArrayList и LinkedList
Поработал с коллекциями

Для работы с коллекциями необходимо подключить соответсвующие интерфейсы из java.util. 

При создании коллекции необходимо указать тип данных, имя, а также выделение памяти:
ArrayList<Float> numbers = new ArrayList<>(1);
LinkedList<String> names = new LinkedList<>();
	
#3 - Отслеживание исключений в Java
  Реалиизовал конструкцию try catch

Для добавления отслеживания ошибок можно прописать следующий код:
try { // В блоке try мы пытаемся выполнить какой-либо код
	// В нашем случае выполняем деление,
	// хотя также можно прописать открытие файлов, создание объекта на основе класса и так далее
	System.out.println(something / variable); 
} catch(ArithmeticException e) { // Указываем класс с ошибкой
	// Поскольку мы выполняли математические действия, то класс с ошибкой ArithmeticException
	
	// Выводим текст с ошибкой
	System.out.println("Текст ошибки: " + e);
}
#4 - Запись и чтение данных из файлов (Java io)
  Запись данных в файл

При записи данных в файл его изначально необходимо открыть. Для этого в языке Java используется класс «File»:
File file = new File("fileName.txt");
После открытия файла вы можете записать в него данные за счёт класса «PrintWriter»:
// Указываем файл для записи
// В качестве объекта передаем открытый файл на основе класса File
PrintWriter pw = new PrintWriter(file);

// Помещаем текст внутрь файла
pw.println("Working proccess");
В конце файл необходимо закрыть:
pw.close();
  
#5 - Работа с потоками данных (Threads)
  
  Для создания потоков можно использовать один из двух вариантов:
Создать класс, что будет унаследован от класса Threads.
Создать класс, что будет реализовывать интерфейс Runnable.
  
#6 - Создание приложения на JavaFx
  В Java создал Hello Application - главное страница проекта
  Для создания разметки можно прописывать код вручную или же воспользоваться программой Scene Builder. Программа позволяет создавать весь графический интерфейс, а также генерирует скелет класса контроллера для добавления функциональности к программе.

Для редактирования файлов в программе Scene Builder необходимо открыть нужный .fxml файл. В качестве первого объекта переместите объект Anchor Pane и на него переносите другие необходимые элементы программы.
  
#7 - Создание дополнительного окна
  За каждое отдельное окно в приложении отвечает отдельный fxml файл. Таких файлов может быть сколько угодно. Переключение между файлами осуществляется за счёт написания специального кода, который мы рассмотрим позже.

Для добавления функциональности необходимо прописать класс контроллер, что будет обрабатывать все нажатия на странице приложении. 

Функции в контроллере можно добавить лишь к тем объектам, для которых прописан специальный атрибут «id». Прописать атрибут можно через программу Scene Builder.

#8 - Окно с регистрацией на JavaFx
  Приложение будет состоять из трёх окон: 
окно регистрации;
окно авторизации;
главное окно, что будет показано лишь после авторизации пользователя.
	
#9 - Подключение базы данных к приложению (MySQL + JDBC)
  В качестве базы данных я  использовал MySQL, хотя можно использовать любую систему управления базами данных, например: Oracle, Firebird, Interbase, MS SQL Server, PostgreSQL и так далее.

Для работы с MySQL необходимо установить сервер, а также программу WorkBench, которая позволяет управлять базой данных при помощи удобного графического интерфейса. 

Через WorkBench создал базу данных, добавил в неё таблицы, в таблицы можем добавить поля и заполнить всё это различными значениями. 
