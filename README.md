ПРИВЕТ!!!

![screenshot of sample](https://github.com/serega89ynao/preloader/blob/master/img/4.png)

Для того чтобы данный прелоуд работал нужно произвести некоторые действия.

После открывающего тега 
```html
<body>
```
 вставить следующий html код
```html
<!-- Preloader -->
    <div id="load">
        <div class="preloader-box">
            <div class="preloader-wr">
                <div class="red"></div>
                <div class="yellow"></div>
                <div class="blue"></div>
                <div class="green"></div>
            </div>
        </div>
    </div>
    <!-- End Preloader -->
```


Подключить файл `"preloader.min.css"`.
```html
<head>
<link href="css/preloader.min.css" rel="stylesheet">
</head>
```

Вставить следующий скрипт в Ваш файл.js 
```javascript
// Preloader
$(window).on('load', function () {
	$('#load').delay(1000).fadeOut('slow');
});
// End Preloader
```

Где `delay(1000)` врямя задержки анимации после загрузки страницы в `милисекундах`.
Время выставляется на Ваше усмотрение.
