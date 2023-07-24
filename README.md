# Homework / Домашнее задание :clipboard:
## goit-markup-hw-04
:us:
<details>
	<summary>English</summary>
	<ul>
		<li>Create a repository `goit-markup-hw-05`.</li>
		<li>Clone the created repository and copy the files of the previous work into it.</li>
		<li>Add decorative effects animation for layout pages <a href="https://www.figma.com/file/oTYBECAN79dXy19hzWObO4/Web-Studio-(Version-2.1)?node-id=1%3A836"><b>homework #5</b></a>.</li>
		<li>Set up `GitHub Pages` and add a link to the live page in the header of the GitHub-repository.</li>
	</ul>

## Eligibility criteria for a mentor

### Project

**`«A1»`** All styles are written in one `styles.css` file, which is located in the `css` folder.

**`«A2»`** Source code formatted with `Prettier`.

**`«A3»`** All images and text content are taken from the layout.

**`«A4»`** All HTML pages have a style normalizer [`modern-nomalize`](https://github.com/sindresorhus/modern-normalize).

**`«A5»`** The code is written as follows [**manual**](https://codeguide.co/).

**`«A6»`** The modal window script is included in the HTML in a separate file `modal.js`.

### Markup

**`«B1»`** Completed HTML markup of all layout elements.

**`«B2»`** Tags are used according to their semantic meaning.

## Formalization

**`«C1»`** Transitions have been made for all hover and focus effects (color, background, shadow). Time is `250ms`, time distribution function is `cubic-bezier(0.4, 0, 0.2, 1)`.

**`«C2»`** Transitions and animations explicitly specify the properties to be animated. There is no `all` value anywhere.

**`«C3»`** In the `What we do` section, text with a background is positioned on top of the image.

**`«C4»`** In the main navigation, using the `::after` pseudo-element, the link of the current page (on which the user is currently located) is underlined.

**`«C5»`** A blue overlay with text on the cards of the `Portfolio` page appears when you hover anywhere in the card.

**`«C6»`** The blue overlay in the `Portfolio` page cards slides out from the bottom, as shown [on video](./05-preview.gif).

**`«C7»`** Pseudo-elements do not have text content in the `content` property. They are used solely for decorative purposes.

### Modal window

**`«D1»`** The layout and design of the “backdrop” (dark translucent background) of the modal window has been completed.

**`«D2»`** The "backdrop" fills 100% of the height and width of the browser viewport and is fixed in it.

**`«D3»`** The layout and design of the modal window has been completed.

**`«D4»`** The modal window is vertically and horizontally positioned in the middle of the backdrop.

**`«D5»`** The layout and design of the close button of the modal window in the upper right corner has been completed.

**`«D6»`** The modal and the backdrop are initially hidden using the `is-hidden` class on the backdrop, whose selector uses the `visibility`, `opacity` and `pointer-events` properties.

**`«D7»`** If you remove the `is-hidden` class from the backdrop, the backdrop and modal window appear.

**`«D8»`** The appearance and hiding of the modal is animated with a transition with an arbitrary effect, such as `scale` or `translate`, and `opacity`.

## Opening/Closing a Modal Window

A modal window with an application form is opened by clicking on the button
`"Order a service"`. In order for the script to work, you must add to
markup special attributes by which the script searches for elements:

- `data-modal-open` - on the button to open the modal window.
- `data-modal-close` - on the close button of the modal window.
- `data-modal` - on the backdrop of the modal window.

After that, before the closing `body` tag, add the `script` tag with a link to
script file for modal window. You can see
[video-instruction](https://drive.google.com/file/d/1yasixN2K-9DdsYtKCJWVay9WbyTZai0t/view?usp=sharing).

```html
<body>
  <!-- All your markup, including modal markup -->

  <!-- Put before the closing body tag -->
  <script src="./js/modal.js"></script>
</body>
```

The script to be copied and pasted into the `modal.js` file.

```js
(() => {
  const refs = {
    openModalBtn: document.querySelector('[data-modal-open]'),
    closeModalBtn: document.querySelector('[data-modal-close]'),
    modal: document.querySelector('[data-modal]'),
  };

  refs.openModalBtn.addEventListener('click', toggleModal);
  refs.closeModalBtn.addEventListener('click', toggleModal);

  function toggleModal() {
    refs.modal.classList.toggle('is-hidden');
  }
})();
```
</details>
:ukraine:
<details>
<summary>Russian</summary>
 	<ul>
		<li>Создай репозиторий `goit-markup-hw-05`.</li>
		<li>Склонируй созданный репозиторий и скопируй в него файлы предыдущей работы.</li>
		<li>Добавь анимацию декоративных эффектов для страниц макета <a href="https://www.figma.com/file/oTYBECAN79dXy19hzWObO4/Web-Studio-(Version-2.1)?node-id=1%3A836"><b>homework #5</b></a>.</li>
		<li>Настрой `GitHub Pages` и добавь ссылку на живую страницу в шапку GitHub-репозитория.</li>
	</ul>
  
## Критерии приёма работы наставником

### Проект

**`«A1»`** Все стили написаны в одном файле `styles.css`, который находится в
папке `css`.

**`«A2»`** Исходный код отформатирован при помощи `Prettier`.

**`«A3»`** Все изображения и текстовый контент взяты из макета.

**`«A4»`** На всех HTML-страницах подключен нормализатор стилей
[`modern-nomalize`](https://github.com/sindresorhus/modern-normalize).

**`«A5»`** Код написан следуя [**руководству**](https://codeguide.co/).

**`«A6»`** Скрипт модального окна подключен в HTML отдельным файлом `modal.js`.

### Разметка

**`«B1»`** Выполнена HTML-разметка всех элементов макета.

**`«B2»`** Теги использованы согласно их семантического смысла.

## Оформление

**`«C1»`** Для всех эффектов ховера и фокуса (цвет, фон, тень) сделаны переходы.
Время - `250ms`, функция распределения времени - `cubic-bezier(0.4, 0, 0.2, 1)`.

**`«C2»`** В переходах и анимациях явно указаны анимируемые свойства. Нигде нет
значения `all`.

**`«C3»`** В секции `Чем мы занимаемся` текст с фоном спозиционирован поверх
изображения.

**`«C4»`** В главной навигации, при помощи псевдоэлемента `::after`, сделано
подчёркивание ссылки текущей страницы (на которой сейчас находится
пользователь).

**`«C5»`** Синий оверлей с текстом на карточках страницы `Портфолио` появляется
при ховере в любом месте карточки.

**`«C6»`** Синий оверлей в карточках страницы `Портфолио` выезжает снизу, как
показано [на видео](./05-preview.gif).

**`«C7»`** У псевдоэлементов нет текстового контента в свойстве `content`. Они
использованы исключительно для декоративного оформления.

### Модальное окно

**`«D1»`** Выполнена разметка и оформление «бекдропа» (тёмного полупрозрачного
фона) модального окна.

**`«D2»`** «Бекдроп» заполняет 100% высоты и ширины вьюпорта браузера и
фиксирован в нём.

**`«D3»`** Выполнена разметка и оформление модального окна.

**`«D4»`** Модальное окно вертикально и горизонтально спозиционировано
посередине бекдропа.

**`«D5»`** Выполнена разметка и оформление кнопки закрытия модального окна в
верхнем правом углу.

**`«D6»`** Изначально модальное окно и бекдроп скрыты при помощи класса
`is-hidden` на бекдропе, в селекторе которого используются свойства
`visibility`, `opacity` и `pointer-events`.

**`«D7»`** Если убрать с бекдропа класс `is-hidden` - появляется бекдроп и
модальное окно.

**`«D8»`** Появление и скрытие модального окна анимировано при помощи перехода с
произвольным эффектом, например `scale` или `translate`, и `opacity`.

## Открытие/закрытие модального окна

Модальное окно с формой заявки открывается по клику на кнопку
`"Заказать услугу"`. Для того чтобы скрипт сработал необходимо добавить в
разметку специальные атрибуты, по которым скрипт ищет элементы:

- `data-modal-open` - на кнопку открытия модального окна.
- `data-modal-close` - на кнопку закрытия модального окна.
- `data-modal` - на бекдроп модального окна.

После чего, перед закрывающим тегом `body` добавить тег `script` со ссылкой на
файл скрипта для модально окна. Можно посмотреть
[видео-инструкцию](https://drive.google.com/file/d/1yasixN2K-9DdsYtKCJWVay9WbyTZai0t/view?usp=sharing).

```html
<body>
  <!-- Вся твоя разметка, включая разметку модалки -->

  <!-- Ставим перед закрывающим тегом body -->
  <script src="./js/modal.js"></script>
</body>
```

Скрипт который необходимо скопировать и вставить в файл `modal.js`.

```js
(() => {
  const refs = {
    openModalBtn: document.querySelector('[data-modal-open]'),
    closeModalBtn: document.querySelector('[data-modal-close]'),
    modal: document.querySelector('[data-modal]'),
  };

  refs.openModalBtn.addEventListener('click', toggleModal);
  refs.closeModalBtn.addEventListener('click', toggleModal);

  function toggleModal() {
    refs.modal.classList.toggle('is-hidden');
  }
})();
```
</details>
