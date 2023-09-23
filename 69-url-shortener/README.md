## 📦 URL Shortener Component

### Обзор
Данный код представляет собой JavaScript-класс `Shortener`, который реализует функциональность сокращения URL-ссылок. Вот краткое описание его функций:

1. Инициализация класса и создание DOM-структуры:
  - Класс `Shortener` создается и инициализируется при его создании.
  - В методе `initialize()` инициализируется компонент, создавая DOM-структуру и устанавливая обработчики событий.
  - Метод `createDOM()` создает HTML-разметку для компонента, включая форму для ввода URL и кнопку отправки.

2. Установка обработчиков событий:
  - В методе `setupEventListeners()` устанавливаются обработчики событий для формы и кнопки копирования.

3. Обработка отправки формы:
  - В методе `handleSubmit()` обрабатывается событие отправки формы.
  - Получается значение URL из формы и выполняется его валидация.
  - Если URL не соответствует ожидаемому формату, выводится предупреждение, и изменяются классы элементов DOM.
  - Если URL валиден, отправляется запрос на сокращение URL с использованием внешнего API (axios).
  - Если запрос успешен, сокращенная ссылка выводится в поле ввода, и изменяются классы элементов DOM.
  - В случае ошибки также выводится сообщение об ошибке и изменяются классы.

4. Обработка копирования URL:
  - В методе `handleCopy()` обрабатывается событие копирования URL.
  - Если поле ввода не пусто, URL копируется в буфер обмена, и выводится сообщение об успешном копировании.

5. Изменение классов элементов DOM:
  - Метод `handleChangeClass()` изменяет классы элементов DOM в зависимости от успешности операции.
  - Например, если операция неуспешна, высота родительского элемента увеличивается, и текст кнопки в форме изменяется.

6. Создание экземпляра класса:
  - В конце кода создается экземпляр класса `Shortener`, и инициализируется вся функциональность компонента.

Класс `Shortener` позволяет пользователям вводить URL-ссылки, сокращать их, а затем копировать сокращенные ссылки в буфер обмена.

---

#### 🌄 Preview:

![App Preview](https://lh3.googleusercontent.com/drive-viewer/AITFw-zLV9V9amULXUZxCq-UwvZEY78_nLeIngHIPo5M79uvpOALd64XEEQ-8z5SknSEGMNdoE19kPZuUW3F_ApIhhWXuJ-JTg=s1600)


-----

#### 🙌 Author: [@nagoev-alim](https://github.com/nagoev-alim)
