## 📦 Number Facts Component

### Обзор
Это простое веб-приложение, которое позволяет пользователям вводить числа и получать интересные факты о введенных числах. Приложение предоставляет удобный интерфейс и отображает полученные факты в реальном времени.

### Особенности

- Пользователи могут вводить числа в поле ввода.
- После отправки формы приложение получает случайный факт о введенном числе, используя внешний API.
- Факт отображается пользователю вместе с индикатором загрузки во время обработки запроса.
- В случае ошибки во время запроса отображается сообщение об ошибке.

### Обзор кода

### Класс: NumberFacts

- Этот класс представляет основной функционал приложения "Факты о числах".
- Он инициализирует элементы DOM, настраивает слушатели событий и обрабатывает отправку формы.

#### Свойства

- `form`: Хранит ссылку на элемент формы для ввода числа.
- `fact`: Хранит ссылку на элемент параграфа, где будет отображаться полученный факт.
- `spinner`: Хранит ссылку на элемент индикатора загрузки.
- `URL`: Константная строка, содержащая базовый URL для получения фактов о числах.
- `constructor()`: Инициализирует класс NumberFacts, вызывая метод `initialize()`.

#### Методы

- `initialize()`: Инициализирует класс, создавая структуру DOM и настраивая слушателей событий.
- `createDOM()`: Создает HTML-структуру для приложения, включая форму ввода и индикатор загрузки.
- `setupEventListeners()`: Настраивает слушателей событий, в частности для отправки формы.
- `handleSubmit(event)`: Обрабатывает отправку формы, получая факт на основе введенного числа и обновляя интерфейс соответственно.

## Зависимости

- [axios](https://github.com/axios/axios): Используется для выполнения HTTP-запросов для получения фактов о числах.
- `./style.scss`: Содержит стили приложения.
- `./utils/toast.ts`: Предоставляет утилиту для отображения всплывающих уведомлений (toast).

### Запуск приложения

1. Клонируйте репозиторий.
2. Откройте файл `index.html` в современном веб-браузере.

Этот документ в формате Markdown предоставляет обзор приложения "Факты о числах", его особенностей, структуры кода и зависимостей. Также он объясняет, как запустить приложение.


---

#### 🌄 Preview:

![App Preview](https://lh3.googleusercontent.com/drive-viewer/AITFw-yNX5KPVefjhOleEoWDVkwJhznC7QVxsLD4vOPXhp0lwDdjDlNSu5q_76a06QpifgIdFSN0sIg2h-uzQ6FN_I_MQQwVCg=s1600)


-----

#### 🙌 Author: [@nagoev-alim](https://github.com/nagoev-alim)
