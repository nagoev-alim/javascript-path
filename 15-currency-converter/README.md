## 📦 Currency Converter Component

### Обзор

Данный код представляет собой TypeScript-класс CurrencyConverter, который создает веб-приложение для конвертации валют.

- **Импорт библиотек и ресурсов:**

В этом разделе происходит импорт необходимых зависимостей, таких как стили, библиотеки для уведомлений, данные о
странах, иконки и Axios для работы с HTTP-запросами.

- **Интерфейс `ExchangeRateResponse`:**

Этот интерфейс описывает структуру данных, ожидаемых в ответе от сервера при запросе курса обмена валют. Это позволяет типизировать данные и облегчить их обработку.

- **Класс `CurrencyConverter`:**

Этот класс представляет собой основную логику приложения. В конструкторе `CurrencyConverter` вызывается метод `initialize()`, который инициализирует приложение.

- **Основные методы класса `CurrencyConverter`:**

- `private createDOM()`: Этот метод создает структуру DOM, вставляя HTML-разметку на страницу. Она включает в себя форму для ввода суммы и выбора валют, а также элементы для отображения результата и иконку для переключения валют. 
- `private setupEventListeners()`: Этот метод устанавливает обработчики событий для формы и других элементов. Например, он реагирует на отправку формы, изменение выбора валюты и клик на иконке переключения валют.
- `private getExchange()`: Этот метод вызывается при инициализации приложения и выполняет запрос курса обмена валют. 
- `private handleSubmit(event: Event)`: Этот метод обрабатывает событие отправки формы. Он собирает данные из формы, выполняет проверки на заполненность полей и, при необходимости, отображает уведомления. 
- `private handleChange(event: Event)`: Этот метод реагирует на изменение выбора валюты и обновляет изображение флага соответствующей страны. 
- `private handleSwitch()`: Этот метод обрабатывает событие переключения валют между "From" и "To". Он меняет выбранные валюты и обновляет изображения флагов. 
- `private async fetchData(amount: string, from: string, to: string)`: Этот метод выполняет HTTP-запрос к API для получения данных о курсе обмена валюты и отображает результат на странице. 
- `private message(text: string, classname: string')`: Этот метод используется для отображения уведомлений с заданным текстом и стилями.

---

#### 🌄 Preview:

![App Preview](https://lh3.googleusercontent.com/drive-viewer/AITFw-x73KjSZEs3jit2zGVs9Bd27D1ri4H9hv_lDUZG-lh4vpQJ6MpU2boA-EQq2X3L8HMRsKxAN1beR3aTqYtU6aOAuRMV6g=s1600)


-----

#### 🙌 Author: [@nagoev-alim](https://github.com/nagoev-alim)
