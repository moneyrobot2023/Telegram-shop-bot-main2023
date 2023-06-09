![greeting_git](https://github.com/moneyrobot2023/Telegram-shop-bot-main2023/blob/main/imgonline-com-ua-Resize-OzNWk0sJ1OtAoaA5.jpg?raw=true)


# 🔷 # Телеграм-shopBot
Это пример магазина проката настольных игр с админ-панелью, базой данных и платежной картой в мессенджере Telegram, который написан с использованием Aiogram Python.

## Что он может сделать?
```/start``` для начала. Бот отправит приветственное сообщение. <br>
```/home```. Бот отобразит разметку главного меню.<br>
```/choose```. Бот покажет некоторые товары из базы данных.<br>

## Главное меню
![home_menu_purple](https://user-images.githubusercontent.com/99086730/163854200-4ede9147-ae99-47a2-9257-d20e5b6fa263.png)

## ⚙️ Функции

### 🎮 Выберите игру
После нажатия на ``🎮 Нажмите кнопку `Выбрать игру", и бот отправит ограниченное количество товаров из базы данных. Ограничение 5. 
Каждое сообщение с товаром содержит изображение товара, название, цену за день, цену за неделю и сумму депозита. 
Также под сообщением есть две встроенные кнопки ``Арендовать " название игры `на день`" и ""Арендовать" название игры "на неделю``. Оба добавляют игру в корзину.

![product_bg_white](https://user-images.githubusercontent.com/99086730/163853567-16d50359-bd1c-42e6-8fc4-73732a5e996e.png)

### ✉️ Предложите игру
Позволяет пользователю предлагать игру. Предложение сохраняется в базе данных.

### 🖌 Спроси
Позволяет пользователю задать вопрос. Вопрос автоматически отправляется в чат администратора.

### 🗑 Тележка
После нажатия на кнопку `🗑 Корзина` бот отправит сообщение с информацией о карточке пользователя и отобразит меню корзины. В этом меню пользователь может  
``✂️ Удалить из корзины``, который в основном удаляет определенный товар из корзины. Также пользователь может ``🟢 Оформить заказ``.  
После этого пользователь сможет выбирать между способами оплаты и доставки.
![cart_menu](https://user-images.githubusercontent.com/99086730/163855921-4837f0aa-9182-42a9-a33c-7788543dc231.png)

## 📟 Панель администратора
Администратор должен создать новый чат, в который он должен добавить бота. Бот проверит, действительно ли администратор является администратором чата, и
если это так, он отправит сообщение с меню панели администратора.
![admin_panel_menu](https://user-images.githubusercontent.com/99086730/163856717-37cc017e-32af-4477-b1a6-ae62eb69baa7.png)

### 📪 Доступный набор
После нажатия на кнопку `📪 Установить доступно` администратору будет предложено написать название игры, которая будет установлена доступной. После отправки сообщения с названием
игры бот обновит информацию о наличии товара в базе данных.

### 🎲 Добавить игру
После нажатия на ``🎲 При нажатии кнопки `Добавить игру" администратору будет предложено написать некоторую информацию о новой игре для добавления. После выполнения описанных действий бот добавит игру
в базу данных.

### 💥 Удалить игру
После нажатия на кнопку `💥 Удалить игру` администратору будет предложено написать название игры, которую он хочет удалить. После этого игра будет удалена из
базы данных.

## 💳 Платежная карта
Пользователь может расплатиться с помощью платежной карты. Я использовал Qiwi p2p, чтобы заставить это работать. Он просто создает счет и отправляет URL-адрес пользователю. После этого пользователь должен нажать на 
Кнопка `Проверить платеж`. Если он успешно оплатил счет, данные о заказе будут сохранены в базе данных, а также отправлены администратору.
