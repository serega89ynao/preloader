Preloader

ПРИВЕТ!!!

Для того чтобы данный прелоуд работал нужно произвести некоторые действия.

После открывающего тега <body> вставить следующий html код

Preloader
&lt;`div` id="load"&gt;
	&lt;div class="preloader-box"&gt;
		&lt;div class="preloader-wr"&gt;
			&lt;div class="red"&gt;&lt;/div&gt;
			&lt;div class="yellow"&gt;&lt;/div&gt;
			&lt;div class="blue"&gt;&lt;/div&gt;
			&lt;div class="green"&gt;&lt;/div&gt;
		&lt;/div&gt;
	&lt;/div&gt;
&lt;/div&gt;
End Preloader

Подключить файл " spincrement.css " между тегами <head></head>
<link href="css/pincrement.css" rel="stylesheet">

Вставить следующий скрипт в Ваш файл.js 

// Preloader
$(window).on('load', function () {
	$('#load').delay(1000).fadeOut('slow');
});
// End Preloader

Где delay(1000) врямя задержки анимации после загрузки страницы в милисекундах.
Время выставляется на Ваше усмотрение.
