# whitemanz.github.io
Игорь Шкурлапов - Landing-Page
========================
Работа выполнена в рамках обучения на курсе: "Front-End разработчик".
EasyCode - школа IT-специалистов.
-----------------------------------------
**Задание: верстка по предоставленному макету.**
### 1.) В проекте был использован Фреймворк: [Bootstrap  Currently v3.3.7.]( https://getbootstrap.com/docs/3.3/)
***
### 2.) Задействованы подключения внешних и локальных шрифтов.

#### Внешние шрифты - (размещение на удалённых серверах):

**- Иконочные шрифты:** (внешние) - [Fontawesome]( https://fontawesome.com/icons?d=gallery&m=free)

Подключение в style.css
```scss
<link href="https://use.fontawesome.com/releases/v5.0.6/css/all.css" rel="stylesheet">
```
**- Шрифты для текста.** (внешние) - [Google fonts]( https://fonts.google.com/)

`(Dosis: normal, regular, «Open Sans»: normal, regular )`

Подключение в style.css
```scss
<link href="https://fonts.googleapis.com/css?family=Dosis:300,400|Open+Sans:300,400" rel="stylesheet">
```
#### Локальные шрифты - (размещение в папка проекта- fonts):

**- Иконочные шрифты:** (локальные) - icons-et

Подключение в style.css
```scss
<link href="css/et-line.css" rel="stylesheet">
```
**- Шрифты для текста.** (локальные)

`(Dosis: normal, regular, «Open Sans»: normal, regular)`

Дублирующие шрифты, на тот случай если возникнет проблема с загрузкой Google fonts.
Подключение с использованием правила @font-face, в style.css

```scss
 @font-face {
    font-family: 'Open Sans';
    src: url('../fonts/subset-OpenSans-Light.eot');
    src: url('../fonts/subset-OpenSans-Light.eot?#iefix') format('embedded-opentype'),
    url('../fonts/subset-OpenSans-Light.woff2') format('woff2'),
    url('../fonts/subset-OpenSans-Light.woff') format('woff'),
    url('../fonts/subset-OpenSans-Light.svg#OpenSans-Light') format('svg');
    font-weight: 300;
    font-style: normal;
}
```
***
### 3.) В проекте использовались такие компоненты bootstrap как:

- navbar – меню хедера, в том числе и мобильное меню.
- nav-tabs – переключатели табов с содержимым (картинки, текст)
- progress bar – анимационный уровень, шкала навыков.
- carousel – слайдер.
***

### 4.) Для построения модели сайта были задействованы следующие  стандартные классы:

**Bootstrap классы:**
`container, container-fluid, text-center, row, col-lg-4, col-lg-6, col-md-4, col-md-6, col-sm-6, col-sm-12, col-xs-12, hidden-xs, btn, btn-default, fade, img-responsive, clearfix, col-md-offset-1, pull-left, pull-right.`

**Собственные:**
`title, section-small, section-light, section-dark, section-gray, text, btn-dark, marker, marker-dark, marker-light, marker-black.`

***
### 5.) В проекте использованы медиа запросы: - @media all.
Для выбора всех типов устройств. Если не указывать ключевое слово all, оно будет использовано в медиазапросе по умолчанию.

Подключение в style.css
```scss
/* MEDIA Lets Talk -start */
@media (max-width: 1199px) {
    .lets-talk {
        height: auto;
        padding: 100px 0px 40px;
    }
    .lets-talk img {
        margin-top: -130px;
    }
}
@media (max-width: 991px) {
    /* TEST on (768px) */
    .lets-talk img {
        margin-top: 30px;
        display: inline-block;
        max-width: 66%;
    }
    .lets-talk .row > div {
        text-align: center;
    }
}
/* MEDIA Lets Talk - END */
```
**Запросы были использованы для следующих диапазонов разрешений:**

```html
@media (max-width: 1199px) для разрешений в диапазоне 992-1199px
@media (max-width: 991px) для разрешений в диапазоне 768 – 991px
@media (min-width: 767px) для разрешений в диапазоне  480-767px
@media (max-width: 479px) для разрешений в диапазоне 320-479px
```

**Разметка была перестроена для следующих разделов и секций.**

|   @media   |Header| City |About studio|Let’s Talk|Choose us|Slider|Portfolio|Like |Latest News|News Letter|Contact|
|:----------:|:----:|:----:|:----------:|:--------:|:-------:|:----:|:-------:|:---:|:---------:|:---------:|:-----:|
|*max-width:*|      |      |            |          |         |      |         |     |           |           |       |
|   *1199px* |      |      |     `X`    |    `X`   |   `X`   |  `X` |   `X`   |     |    `X`    |           |       |
|    *991px* |      |  `X` |     `X`    |    `X`   |   `X`   |      |   `X`   |     |    `X`    |           |       |
|    *767px* |      |  `X` |     `X`    |          |   `X`   |      |   `X`   |     |    `X`    |    `X`    |  `X`  |
|    *479px* |      |      |            |          |         |      |   `X`   | `X` |    `X`    |    `X`    |  `X`  |
|*min-width:*|      |      |            |          |         |      |         |     |           |           |       |
|   *767px*  |  `X` |      |            |          |         |      |         |     |           |           |       |

***
***Проект был протестирован в следующих браузерах:***  Google Chrome, Mozilla Firefox, Microsoft Edge.

> 2018г. EasyCode. курс "Front-End разработка."

разработчик: Шкурлапов Игорь
