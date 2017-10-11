Preloader

ПРИВЕТ!!!

Для того чтобы данный прелоуд работал нужно произвести некоторые действия.

После открывающего тега <body> вставить следующий html код

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
