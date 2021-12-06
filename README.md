# Курсовой проект “Основы Swift advanced”

В качестве курсового проекта вы разработаете модель ресторана, используя ООП.

Ваша команда разрабатывает приложение для ресторана. Вам предстоит разработать модель (костяк) всего приложения. Ваша основная задача создать абстракции и включить необходимые свойства и методы.

## Требования к коду
- Код должен запускаться без ошибок;
- Должен соблюдаться [стиль кода](https://github.com/netology-code/bios-2-homeworks/blob/master/swift-code-syle-guide.md);
- Обратите внимание на названия переменных и функций. Названия должны быть говорящими, но ёмкими.

## Алгоритм решения

1. Создайте следующие протоколы и определите в них свойства и методы.
    1.1. Ресторан
        Свойства: название, сотрудники, склад с продуктами, меню.
    1.2. Сотрудник
        Свойства: имя, пол, возраст, должность (менеджер, повар, официант и т.д.).
    1.3. Блюдо
         Свойства: тип блюда (салат, горячее, гарнир, десерт), ингредиенты (картофель, лук, мясо, соль), время приготовления, цена.
    1.4. Заказ
         Свойства: время получения заказа, время отдачи заказа, блюда в заказе, готовность.
2. Создайте следующие классы и структуры.
    2.1. Должности (менеджер, повар, официант и т.д.) подписать под протокол Сотрудник. Свойства и методы зависят от должности. Для поваров продумать несколько должностей. Каждый должен иметь метод “готовить”, но иметь еще свои методы. Например повар холодного цеха делает салаты, повар горячего цеха умеет варить и жарить, шеф-повар умеет все (можно сделать привязку к типу блюда).
    2.2. Конкретные блюда (подписать под протокол Блюда). Ингредиенты зависят от типа блюда. Например для яичницы нужны: яйца: масло, соль. Создать минимум 5 блюд.
    2.3. Заказ. Подписать под протокол Заказы.
3. Создайте хранилища:
    - продукты (ингредиенты), хранящиеся на складе с указанием количества (продумайте какой вид коллекции использовать). Создайте минимум 15 продуктов на складе.
    - заказы. Содержит в себе заказы.

Добавлять свои свойства и методы допустимо.
Продумайте, где можно и нужно использовать enum вместо стандартных свойств.

Задача co *. Необязательно задание.
Реализовать логику в методах. Например у официанта метод "принять заказ" добавляет в начало хранилища с заказами переданный заказ. Повар берет первый добавленный заказ из хранилища и готовит. В данном случае нужно разобраться с FIFO и LIFO. После приготовления устанавливается время приготовления и статус меняется на "готов". Можно учесть, что от типа блюда заказ может выполнить либо нужный повар либо шеф.
Вы можете реализовать любую логику на ваше усмотрение. Выше указано для примера. 

## Выполнение работы
1. Чтобы отправить работу на проверку, прикрепите архив с файлом .playground в личный кабинет.
2. При возникновении вопросов попробуйте найти ответ сначала сами. Умение искать ответы пригодится вам в профессиональной деятельности.
3. Посмотрите переписку в чате группы - возможно, недавно преподаватели отвечали на аналогичный вопрос кому-то из студентов.
4. На вопросы вида "Ничего не работает/не запускается/всё сломалось" преподаватели не смогут ответить без дополнительных уточнений. Сформулируйте вопрос более подробно и точно, чтобы помощь преподавателя была более четкой и адресной.
5. Не откладывайте выполнение курсового проекта на последний момент.
6. Преподаватели курса — работающие разработчики, которые кроме преподавания занимаются рабочими проектами. Их время ограничено, поэтому постарайтесь задавать правильные вопросы, чтобы получать быстрые ответы.
