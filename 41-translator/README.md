## 📦 Translator Component

### Обзор
Данный код представляет собой приложение для перевода текста с одного языка на другой. Вот разбор действий, выполняемых кодом:

1. Импортируются необходимые модули и библиотеки, такие как стили, иконки Feather Icons, список стран, модуль для всплывающих уведомлений (toast) и библиотека для выполнения HTTP-запросов через axios.

2. Определяется интерфейс `ICountry`, который описывает структуру объекта страны с двумя свойствами: `value` (значение) и `name` (название).

3. Определяется класс `Translator`, который представляет собой основное приложение для перевода текста. Класс содержит приватные свойства для элементов DOM, такие как кнопки, текстовые поля и выпадающие списки.

4. Конструктор класса `Translator` инициализирует приложение, вызывая метод `initialize()`. Этот метод создает и добавляет элементы DOM в корневой элемент с идентификатором `#app` и настраивает обработчики событий.

5. Метод `createDOM()` создает интерфейс приложения, включая текстовые поля для ввода и вывода текста, кнопки, выпадающие списки для выбора языков, иконки и другие элементы.

6. Метод `setupEventListeners()` настраивает обработчики событий для кнопок и элементов интерфейса. Например, при нажатии на кнопку "Translate Text" вызывается метод `handleSubmit()`, который выполняет перевод текста.

7. Метод `handleSubmit()` выполняет перевод текста, отправляя запрос на сервер с помощью библиотеки axios. Ответ обрабатывается, и переведенный текст выводится в соответствующее текстовое поле. В случае ошибки выводится уведомление об ошибке.

8. Методы `handleExchange()`, `handleCopy()` и `handleSpeech()` обрабатывают события обмена языками, копирования текста и воспроизведения текста соответственно.

9. В конце кода создается экземпляр класса `Translator`, чтобы запустить приложение.

Этот код создает интерфейс для перевода текста между разными языками, предоставляет функциональность обмена языками, копирования текста и воспроизведения текста с использованием иконок Feather Icons и библиотеки axios для выполнения запросов к API перевода.

---

#### 🌄 Preview:

![App Preview](https://lh3.googleusercontent.com/drive-viewer/AITFw-znxfICe7HdSKTzwY2Q_Mwq5f5xP3WgGYRQXD3eM_Z7IgkG1alAijrB_rVCNoZ5NW149erRPtN7d3d8-3_E7T1JGxOtqQ=s1600)


-----

#### 🙌 Author: [@nagoev-alim](https://github.com/nagoev-alim)
