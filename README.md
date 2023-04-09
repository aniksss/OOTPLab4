Розробити технічне завдання. Показати декомпонування завдання, де частина завдань має бути реалізована з використанням породжуючих патернів:
-	Макрокоманди. 
-	Шаблонний метод (Template Method).  

Технічне завдання
Ми повинні розробити додаток для продажу автомобілів, який буде включати в себе два типи магазинів: онлайн та фізичний. Для кожного типу магазинів буде застосовано шаблон CarShopTemplate для обробки процесу купівлі автомобілів. Додаток також повинен містити командний шаблон для підтримки відміни покупки. Клас BuyCarCommand буде виконувати процес купівлі, а клас CarShopMacroCommand дозволить здійснювати і скасовувати кілька покупок одночасно. Додаток має бути реалізований на мові програмування C#.

Декомпозиція (за типом назви задач в Jira):

1.	Розробка класу CarShopTemplate для обробки процесу купівлі автомобілів в онлайн та фізичному магазинах.

2.	Розробка командного шаблону для підтримки відміни покупки.

3.	Розробка класу BuyCarCommand для виконання процесу купівлі автомобіля.

4.	Розробка класу CarShopMacroCommand, що дозволяє здійснювати і скасовувати кілька покупок одночасно.

5.	Реалізація додатку на мові програмування C#.

Вимоги:

1.	Інтернет-магазин повинен мати можливість відображати інформацію про автомобілі, доступні для продажу.

2.	Інтернет-магазин повинен вміти обробляти замовлення, зроблені клієнтами.

3.	Інтернет-магазин повинен генерувати квитанцію для кожного успішного замовлення.

4.	Інтернет-магазин повинен надавати можливість клієнтам скасовувати замовлення.

5.	Інтернет-магазин повинен мати зручний користувацький інтерфейс, в якому легко орієнтуватися.

6.	Інтернет-магазин повинен бути легко масштабованим, щоб впоратися зі збільшенням трафіку та новими функціями.

Результати роботи:

1.	Код на C#, що реалізує шаблон Template Method для генерації квитанції.

2.	Код на C#, що реалізує паттерн Macro Command для обробки замовлень та скасувань.

3.	Юніт-тести, які перевіряють функціональність інтернет-магазину.

4.	Документація, що описує архітектуру та дизайн інтернет-магазину.

Обмеження:

1.	Веб-магазин повинен бути розроблений з використанням C#.

2.	Веб-магазин повинен використовувати шаблон Template Method для генерації квитанції.

3.	Для обробки замовлень та скасувань у веб-магазині має бути використаний паттерн Macro Command.

4.	Веб-магазин повинен бути спроектований з урахуванням збільшення трафіку та нових функцій.


Шаблонний метод: Клас CarShopTemplate визначає кроки для купівлі автомобіля і надає шаблонний метод BuyCar(), який викликає ці кроки. Підкласи OnlineCarShop та InStoreCarShop можуть перевизначати деякі з цих кроків, щоб реалізувати свою специфічну поведінку.

Макрокоманда: Інтерфейс ICommand визначає методи Execute() і Undo(), які використовуються для виконання і скасування команд. Клас BuyCarCommand реалізує інтерфейс ICommand та інкапсулює купівлю автомобіля в магазині. Клас CarShopMacroCommand реалізує інтерфейс ICommand та інкапсулює список команд, які можна виконувати та скасовувати разом.
