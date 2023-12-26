
![image](https://user-images.githubusercontent.com/74331153/215797547-7d3eb3aa-baa1-4ab3-8c03-a28694db9b02.png)


**#----------------------------------------------------------------------><----------------------------------------------------------------------#**

**Snake** (Питон, Удав, Змейка, Червяк и др.) — компьютерная игра, уходящая корнями в системы 1970-х.
Наиболее известна версия от Nokia, впервые появившаяся в кнопочном телефоне Nokia 6110. Разработана финляндским разработчиком Танели Арманто.

**>>>GAME PROCESS<<<**

Игрок управляет длинным, тонким существом, напоминающим змею, которое ползает по плоскости (как правило, ограниченной стенками), собирая еду (или другие предметы), избегая столкновения с собственным хвостом и краями игрового поля (существуют варианты где при прохождении через край змея выходит из противоположного края поля). Каждый раз, когда змея съедает кусок пищи, она становится длиннее, что постепенно усложняет игру.

**>>>GAME CONTROLLER<<<**

![ArrowsLightSmall](https://user-images.githubusercontent.com/74331153/215792287-62462267-8e91-436d-a93a-00de9cc3a8c9.png)


**#----------------------------------------------------------------------><----------------------------------------------------------------------#**

![image](https://user-images.githubusercontent.com/74331153/215797306-6aa874d7-13ef-4b25-b5d0-5a3395092eef.png)


Создание основной конструкции окна в PyGame.\
Создание рабочего цикла игры.\
Стилизация вида окна игры.

**>>>PART_1<<<**

1. Создание основной конструкции окна в PyGame.
2. Создание рабочего цикла игры.
3. Стилизация вида окна игры.

**>>>PART_2<<<**

1. В цикл игры окна добавляем цикл событий.
2. Добавляем условие выхода из окна.

**>>>PART_3<<<**

1. Создаём описание игрового окна.
2. Указываем путь загрузки иконки игрового окна.
3. Устанавливаем иконку игрового окна.
4. Создаём переменные для размеров экрана вместо аргументов функции set_mode().

**>>>RESULT_1<<**

![image](https://user-images.githubusercontent.com/74331153/215781433-f9beb68a-42dc-4ef1-8bde-e552567e81e4.png)


![image](https://user-images.githubusercontent.com/74331153/215797204-3cd2aaf2-5ec2-4436-a984-eda5addc043b.png)

Отрисовка геометрических фигур.\
Создание цикла отрисовки.

**>>>PART_1<<<**

1. Нарисовали прямоугольник белого цвета с отступом (x=20,y=20) и размером 50x50.

**>>>PART_2<<<**

1. Создание переменных с цветами.
2. Создание базовых геометрических примитивов.

**>>>PART_3<<<**

1. Перенос отображения в цикл игры.
2. Создание рисунка из примитивов с помощью цикла.

**>>>RESULT_2<<**

![image](https://user-images.githubusercontent.com/74331153/215783100-380d1678-001a-489c-addf-02115a53b8ee.png)


![image](https://user-images.githubusercontent.com/74331153/215796987-4e955365-caf9-4006-9bd9-ccc0a963a744.png)


Внедрение FPS в проект.\
Управление объектом и его скоростью.

**>>>PART_1<<<**

1. Устанавливаем количество кадров в секунду (FPS).
2. Подключаем библиотеку Time.
3. Прописываем команду отрисовки объекта.

**>>>PART_2<<<**

1. Создаём события управления нажатием клавиатуры.
2. Добавляем управление объектом вправо.
3. Добавляем управление объектом влево.

**>>>PART_3<<<**

1. Изменяем значение переменной position_x.
2. Создаём переменные для кнопок управления.
3. Создаём событие управления кнопки UP.
4. Создаём событие управления кнопки DOWN.

**>>>RESULT_3<<**

![image](https://user-images.githubusercontent.com/74331153/215783254-ffead6db-b867-493a-a55f-cf4a040b7b05.png)
![SnakeGame_lesson3](https://user-images.githubusercontent.com/74331153/215893574-57ed00a7-2eec-43fc-b006-cf461655f91b.gif)


![image](https://user-images.githubusercontent.com/74331153/215796862-0de090d4-c32c-4a16-ad72-a01add335e40.png)

Коллизия в игре.\
Взаимодействие с объектами.\
Правильное управление змейкой.

**>>>PART_1<<<**

1. Создаём условие позиции объекта по осям координат.
2. Обрабатываем коллизию левой и верхней границ игрового экрана.

**>>>PART_2<<<**

1. Обрабатываем коллизию с нижней и правой границами.
2. Учим змейку отталкиваться от границ.

**>>>PART_3<<<**

1. Настраиваем отображение кубика, используя is_draw.
2. Проверяем коллизию с кубиком и делаем is_draw = False, если пересеклись с ним.

**>>>RESULT_4<<**

![image](https://user-images.githubusercontent.com/74331153/215783381-bcf0efb0-a99f-4324-b5d0-3d8567c8ddb0.png)
![SnakeGame_lesson4](https://user-images.githubusercontent.com/74331153/215893641-5727d88a-acb7-4407-9388-cfb35332e6be.gif)


![image](https://user-images.githubusercontent.com/74331153/215796516-8db07bd0-7c39-4cfe-84d9-1c1cc5cdcc84.png)

Создание класса и рефакторинг кода.\
Создание класса Snake.

**>>>PART_1<<<**

1. Создаём класс Snake, в который переупаковываем весь код управления змеёй.
2. Создаём методы управления по осям координат.
3. Переписываем код в цикле игры, заменяя управление именем класса.
4. Создаём метод отрисовки змейки.

**>>>PART_2<<<**

1. Создаём более точную структуру взаимодействия змейки с едой.
2. Меняем скорость и размер змейки относительно FPS игры.
3. Поправляем координаты коллизии.

**>>>PART_3<<<**

1. Создаём метод проверки еды.
2. Создаём условия проверки координат змейки и еды.
3. Создаём рандомное появление еды.

**>>>RESULT_5<<**

![image](https://user-images.githubusercontent.com/74331153/215795498-349f6841-2b0d-4c43-abca-14237592fc87.png)
![SnakeGame_lesson5](https://user-images.githubusercontent.com/74331153/215893665-7c0dcd4f-f06a-4297-8429-7118cfda25c2.gif)


![image](https://user-images.githubusercontent.com/74331153/215796181-28b5ef4e-a6e0-47ac-a0db-9222e4ccbcb1.png)

Создаем логику появления еды на игровом поле.\
Делаем рефактор кода управления змейкой.\
Создаём анимацию увеличения длины змейки.

**>>>PART_1<<<**

1. Программируем появление еды по всему полю игры.
2. Проверяем область заполнения и увеличиваем скорость.
3. Создаём условие, при котором еда не выходит за границы игрового окна.
4. Исправляем, возникшую ошибку в check_walls().

**>>>PART_2<<<**

1. Создаём метод управления def_move().
2. Создаём новые переменные в классе Snake.
3. Вносим изменения в методы управления.

**>>>PART_3<<<**

1. Переименовываем класс Snake в класс Snake_head.
2. Создаём класс Snake для тела змеи.
3. Переносим код движения из класса Snake_head в класс Snake.
4. Создаём переменные количества голов змеи.
5. Создаём метод def add_head.
6. Пишем код анимации добавления длины змеи.

**>>>RESULT_6<<**
![image](https://user-images.githubusercontent.com/74331153/215848358-722766bc-cd8e-4e31-83fe-1b8fbb9a8575.png)
![SnakeGame_lesson6](https://user-images.githubusercontent.com/74331153/215893703-f5331e2b-5f66-4f4c-acb3-f5da4421cead.gif)


![image](https://user-images.githubusercontent.com/74331153/215847999-ec5983d8-4dd3-4213-8ab7-5d754f71809d.png)

Добавление в игру текста.\
Создание счёта.\
Создаём логику проигрыша игрока.

**>>>PART_1<<<**

1. Подключаем все библиотеки через команду pygame init().
2. Создаём и настраиваем шрифт.
3. Рендерим надпись, которая будет выводиться на экран.
4. Выводим надпись через метод blit().

**>>>PART_2<<<**

1. Создаём переменную и надпись «Game over».
2. Вносим корректировки в цикл игры.
3. Создаём условия коллизии стенки, змейки и строки проигрыша.
4. Импортируем библиотеку Time.
5. Создаём условие проигрыша.

**>>>PART_3<<<**

1. Добавляем переменную счёта score_text.
2. Добавляем отображение текста счёта.
3. Переработаем метод def check_food.
4. Дорабатываем появление еды и пополнение счёта.

**>>>RESULT_7<<**

![image](https://user-images.githubusercontent.com/74331153/215847838-a46eb497-5623-42ff-8cb1-0d45fc102e37.png)
![SnakeGame_lesson7](https://user-images.githubusercontent.com/74331153/215893771-cd29e411-1824-42f6-b1de-f6392af90a4f.gif)


![image](https://user-images.githubusercontent.com/74331153/215849114-5835cc9f-1cc2-4cea-a5e1-7e9603eed3a7.png)

Рефакторинг кода:\
— коллизия тела змейки.\
— логика управления змейки.\
— появление еды.

**>>>PART_1<<<**

1. Исправить баг — столкновения с правой и нижней стеной.
2. Создать условие, при котором змея может врезаться в саму себя.

**>>>PART_2<<<**

1. Исправить баг — выход змейки за пределы игрового окна, путём добавления логического выражения and.
2. Исправить логику движения змейки влево, вправо, вверх и вниз, т.к. змейка идёт только в одном направлении.

**>>>PART_3<<<**

1. Исправление рандомных координат еды.
2. Создаём условие, исключающее появление еды на теле змейки.
3. Создаём цикл while is_repeat для постоянной проверки координат, появляющейся еды.

**>>>RESULT_8<<**

![image](https://user-images.githubusercontent.com/74331153/215850196-f3e6500a-8236-4a22-9a26-9971d4e79f12.png)
![SnakeGame_lesson8](https://user-images.githubusercontent.com/74331153/215893802-7ec401c8-2303-4b87-8e0d-bc6f606744e1.gif)


![image](https://user-images.githubusercontent.com/74331153/215853479-99d64913-b383-44b5-bc35-7ab8647ab084.png)

Создание сцены, титров и кнопки меню.\
Кнопки входа и выхода из игры.\
Изменение увета змейки и еды.\

**>>>PART_1<<<**

1. Создаём метод def main_menu().
2. Создаём цикл меню и логику отрисовки.
3. Указываем кнопки «Start» и «Exit».

**>>>PART_2<<<**

1. Создаём логику выбора пунктов меню.
2. Перемещаем и дорабатываем событийную модель.
3. Прописываем код запуска игры и выхода из игры.

**>>>PART_3<<<**

1. Создание метода изменения цвета змейки.
2. Прописываем условие изменения цвета змейки при соприкосновении с едой.
3. Изменение цвета еды.

**>>>RESULT_9<<**

![SnakeGame_Final](https://user-images.githubusercontent.com/74331153/215891815-6492274a-6af9-4d18-bd19-345b2a4218d3.gif)


На этом всё.
Остался баг с появлением еды на границах.


