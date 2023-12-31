# Test Task Sir Game Unity Developer

![первая сцена](/README_Additional_materials/shooter3d.gif)

Тестовое задание на вакансию Unity Developer, в котором было необходимо реализовать в Unity 2020.2.3.f1 шутер с двумя типами противников, предметами, управлением по джойстику и автоматическую стрельбу. 

![первая сцена](/README_Additional_materials/long.png)

Был устроен генератор предметов и размеров карты, в завимости от которого расставлялись объекты на сцене.
Так же был реализован моб генератор с настраиваемым количеством мобов. 

![первая сцена](/README_Additional_materials/square.png)

Была реализована система Хп, но не показана графически, так же не было реализована победа путем выхода, а лишь победа после уничтожения всех противников. А так же не реализована автоматическая стрельба по противнику.

При большем количестве времени было бы изменена система движения, поворотов мобов и стрельба по игроку, а так же визуальная составляющая.

![первая сцена](/README_Additional_materials/short.png)


Сам текст тестового задания представлен ниже:

```
Задача: реализовать базовый геймплей игры в стиле Archero.
Технологии: Unity3D (версия 2020.2.3.F1), C#.
Обязательные условия:
игровое поле заранее заданных размеров, вид сверху;
наличие 2х типов поведения противников;
наличие непроходимых по земле и непростреливаемых препятствий;
возможность управлять героем с помощью джойстика (движение);
герой должен получать монетки за убийство врагов;
• камера на любых соотношениях сторон всегда охватывает всё игровое
поле.
Дополнительный функционал (будет плюсом):
• эффекты попадания снарядов / смерти (формально);
несколько типов оружия игрока;
• умные противники: каждое перемещение ставит или приближает моба к
прямой видимости игроком;
меню/окно паузы (базовый функционал UI/окон);
дополнительные типы поведения противников.
Время выполнения: мы предлагаем для выполнения тестового задания 2-3
рабочих дня. Если по определенным причинам вам необходимо чуть больше
времени для реализации задания, пожалуйста, заблаговременно сообщите нам
об этом.
Главный критерий оценки - качество кода (читабельность, оптимальность,
переносимость, отсутствие ошибок и так далее), а не графическая
составляющая.
Команда Sir Games ценит время и усилия, затраченные на выполнение
тестового задания, и мы хотим детально изучить вашу работу, поэтому ответ
вышлем в течении 1-2 рабочих дня с момента получения выполненного
тестового задания.
Техническое задание
Описание геймплея: при старте игры происходит спаун противников в
случайной области верхних 2/3 игрового поля и спаун игрока в центре нижней
границы игрового поля. Сразу после расстановки идёт 3х-секундный отсчёт,
после него начинается геймплей.
Главный персонаж свободно перемещается по полю (с учётом препятствий) и
стреляет снарядами во врагов - стрельба ведётся в автоматическом режиме,
пока персонаж стоит на месте
Противники перемещаются согласно своей логике и также ведут стрельбу стоя.
При столкновении снаряда с противником или главным персонажем наносится
урон, снаряд исчезает. При столкновении противника и персонажа, персонажу
наносится урон, взаимопроникновение невозможно Главный персонаж:
Персонаж полностью подконтролен игроку, перемещается с помощью
джойстика, во время передвижения он обращен лицевой стороной по вектору
движения, после остановки он начинает слежение за ближайшим противником
с помощью поворота вокруг своей оси и автоматическую стрельбу в его
направлении.
Характеристики персонажа:
скорость передвижения;
количество HP;
• скорость стрельбы - урон за выстрел.
Противники:
После старта игры противники включают логику поведения, она состоит из:
перемещения на более выгодную позицию;
стрельбы при условии неподвижности.
Исходное состояние - неподвижность.
Типы противников:
•наземный (перемещение блокируется препятствиями);
летающий (перемещается над препятствиями).
Характеристики противников:
• скорость передвижения;
дальность передвижения;
время неподвижности;
количество HP:
скорость стрельбы;
урон за выстрел.
Цель игры: выжить, убить всех противников и выйти через «открытые двери»
в верхней части уровня.
```