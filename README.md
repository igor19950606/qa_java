**Финальный проект 6 спринта**

Тебя пригласили помочь зоологам: они исследуют семейство кошачьих. Чтобы записывать наблюдения, учёные используют специальную программу. Тебе предстоит протестировать часть программы.

Загляни в шпаргалки, чтобы вспомнить материал спринта.

Чтобы увеличить покрытие, нужно вызвать каждый метод каждого класса в отдельном тесте. Для каждой ветки условия напиши отдельный тест. Некоторым веткам понадобится параметризованный тест.

Проект состоит из обязательного и дополнительного заданий. Дополнительное задание не влияет на оценку, но поможет получить больше опыта.

**Обязательное задание**

1. Привяжи GitHub к тренажёру. Как только ты это сделаешь, в списке репозиториев автоматически появится qa_java. Там будет заготовка проекта, в которой нужно дописать код. Подробнее — в инструкции.
2. Собери Maven-проект: подключи Jacoco, Mockito и JUnit.
3. Класс Lion не должен зависеть от класса Feline. Используй принцип инъекции зависимостей.
4. Напиши моки с помощью Mockito. Какие именно понадобятся — определи самостоятельно.
5. Напиши тесты на классы Feline, Cat и Lion.
6. Подумай, где можно применить параметризацию. Реализуй параметризованные тесты.
7. Оцени покрытие с помощью Jacoco: оно должно быть не менее 100% для классов Feline, Cat и Lion..

**Дополнительное задание**

1. Создай класс льва Алекса из мультфильма «Мадагаскар». Он будет наследником обычного льва.

Помимо обычных методов у него есть свои:
* getFriends() возвращает список имён его друзей — зебры Марти, бегемотихи Глории и жирафа Мелман;
* getPlaceOfLiving() возвращает место, где он живёт — Нью-Йоркский зоопарк.

Также нужно переопределить метод getKittens(), потому что у Алекса нет львят. А ещё — написать свой конструктор, так как в классе Lion нет дефолтного конструктора. Алекс самец, поэтому в конструктор класса Lion всегда будет передаваться одно и то же значение.

2. Покрой тестами созданный класс.

**Как будут оценивать твою работу**

Для основного задания
1. Нейминг элементов корректный. Если не помнишь правила, посмотри в шпаргалку.
2. В pom.xml подключены Jacoco, Mockito и JUnit.
3. В pom.xml нет ничего лишнего.
4. Тесты лежат в src/test/java.
5. Класс Lion не зависит от класса Feline. Код написан с инъекцией зависимости.
6. В тестах используются моки.
7. В тестах используется параметризация.
8. Классы Feline, Cat и Lion покрыты тестами на 100%
9. Параметризованные тесты должны быть вынесены в отдельный класс.
10. Сделан отчёт с помощью Jacoco. Не забудь закоммитить отчёт. Открой консоль, перейди в папку проекта и выполни команды:

Добавляем папку с отчетом Jacoco к отслеживаемым файлам. Ключ -f пригодится, если папка target указана в .gitignore

git add -f .\target\site\jacoco\.

Выполняем коммит

git commit -m "add jacoco report"

Отправляем файлы в удалённый репозиторий

git push
10. В проекте используется Java 11.

**Для дополнительного задания**
1. Написан дополнительный класс — лев Алекс.
2. Класс лев Алекс покрыт тестами.

**Как сдать работу**

Нужно сдать проект через GitHub. Прочитай инструкцию.

**Прежде чем сдать проект**

Проверь себя по чек-листу. Он поможет разобраться: проект правильно загружен на GitHub или нет. Если загрузишь решение неправильно, ревьюер вернёт его на доработку.

Информация о проекте

**Зависимости**

| Технология | Версия |
|------|------|
| Java  | 11   | 
| JUnit  | 4.13.2|
| Mockito  | 3.9.0 | 
| Jacoco   | 0.8.7| 

**Настройка**:

Установить Java 11. Установить Maven 3.9.0. Установить Google Chrome.

**Запуск проекта:**

"mvn clean test"
