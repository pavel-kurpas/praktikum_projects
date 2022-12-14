# Исследование данных о продажах игр

Имеются данные об играх, их продажах в разных регионах и оценках. Данные собраны из открытых источников и содержат информацию, актуальную на декабрь 2016 года.

Заказчик исследования — интернет-магазин игр, работающий по всему миру. **Цель проекта — выявить определяющие успешность игры закономерности**. Это позволит заказчику сделать ставку на потенциально популярный продукт и спланировать рекламные кампании.

Задачи исследования:

* выполнить предобработку данных
* изучить данные на предмет наличия в них особенностей и зависимостей
* протестировать статистические гипотезы по выборкам на основе данных

*Исследование включает в себя следующие этапы:*


1. Первичный обзор данных


2. Предобработка данных:
    * изменение стиля заголовков в датафрейме
    * обработка пропусков
    * устранение артефактов
    * обработка дубликатов
    * изменение типов данных
    * введение дополнительных столбцов с расчётными данными
    
    
3. Исследовательский анализ данных:
    * выбор базового периода прогнозирования
    * анализ распределения продаж в зависимости от игровых платформ
    * выявление связи между отзывами и продажами
    * анализ распределения по жанрам
    * составление портрета типичного пользователя для каждого региона


4. Статистический анализ данных:
    * проверка гипотезы о равенстве средних пользовательских оценок платформ Xbox One и PC
    * проверка гипотезы о равенстве средних пользовательских оценок жанров Action и Sports
    
Использовались библиотеки:
    - `pandas`
    - `matplotlib`
    - `seaborn`
    - `numpy`
    - `scipy`
    
    
**Результаты:**

1. В целом по миру в актуальном периоде (2014–2016 гг.) наиболее успешными и перспективными являются игры на платформах PS4 и Xbox One, относящиеся к жанрам Action, Shooter, Sports и Role-Playing. Наиболее прибыльным в среднем является жанр Shooter.


2. В Северной Америке и Европе лучше всего продаются игры для взрослой аудитории на платформах PS4 и Xbox One, относящиеся к жанрам Action и Shooter.


3. В Японии популярны игры на платформах 3DS и PS4, относящиеся к жанрам Role-Playing и Action и не имеющие маркировки ESRB (т.е., видимо, разработанные не европейскими или американскими студиями).


4. Оценки критиков лучше прогнозируют успешность игры, чем оценки пользователей.

В результате проверки двух гипотез статистическими методами были сделаны выводы о том, что при уровне значимости 5% средние пользовательские оценки игр на платформах Xbox One и PC совпадают на генеральной совокупности, а средние пользовательские оценки жанров Action и Sports, наоборот, значимо различаются.
