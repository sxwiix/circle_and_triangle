# Приложение: "Geometry"


## Описание функционала:

Эта библиотека предоставляет классы для вычисления площади круга и треугольника. Также включает метод для проверки, является ли треугольник прямоугольным.

## Структура проекта
    geometry/
      __init__.py
      shapes.py
      tests.py
    main.py

## Установка

1. Скачайте или клонируйте проект в рабочую директорию.
2. Убедитесь, что у вас установлена версия Python 3.7 или выше.
### Использование
   1. Импортируйте библиотеку:
   В файле main.py импортируйте необходимые классы из библиотеки geometry:
    ```python
     from geometry import Circle, Triangle
    ```
2. Создайте объекты фигур и вызовите методы для вычисления площади или проверки свойств фигур:
    ```python

    def main():
        # Создание круга
        circle = Circle(5)
        print(f"Площадь круга: {circle.area()}")

        # Создание треугольника
        triangle = Triangle(3, 4, 5)
        print(f"Площадь треугольника: {triangle.area()}")

        # Проверка, является ли треугольник прямоугольным
        if triangle.is_right_triangle():
            print("Треугольник является прямоугольным.")
        else:
            print("Треугольник не является прямоугольным.")
    
        if __name__ == "__main__":
            main()
    ```
3. Запустите программу:
Откройте терминал, перейдите в директорию проекта и выполните команду:
   ```python
    python main.py
   ```
   Вы должны увидеть следующий вывод:

   ```python
   Площадь круга: 78.53981633974483
   Площадь треугольника: 6.0
   Треугольник является прямоугольным.
   ```
## Юнит-тесты

1. Структура тестов:       
Тесты находятся в файле geometry/tests.py. Они проверяют корректность вычислений и определение прямоугольного треугольника.

2. Запуск тестов:   
В терминале выполните команду:
   ```python
   python -m unittest geometry.tests
   ```
   Если все тесты прошли успешно, вы увидите следующий вывод:
   ```python
   ...
   ----------------------------------------------------------------------
   Ran 4 tests in 0.001s
   
   OK

   ```
   