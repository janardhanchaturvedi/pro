$(function(){

	$('.btn_menu').click(function(){
		$('.menu ul').slideToggle();
	});
	$('.news_slider').slick({
		slidesToShow: 1,
		prevArrow: $('.left'),
		nextArrow: $('.right'),
	});	
	$('.slick_slider').slick({
		slidesToShow: 1,
		prevArrow: $('.prev'),
		nextArrow: $('.next'),
	});
	
	
	$('.popup-with-form').magnificPopup({
		type: 'inline',
		preloader: false,
		focus: '#name',

		// When elemened is focused, some mobile browsers in some cases zoom in
		// It looks not nice, so we disable it:
		callbacks: {
			beforeOpen: function() {
				if($(window).width() < 700) {
					this.st.focus = false;
				} else {
					this.st.focus = '#name';
				}
			}
		}
	});
	$("#menu, #btn_top").on("click","a", function (event) {
        //отменяем стандартную обработку нажатия по ссылке
        event.preventDefault();
        //забираем идентификатор бока с атрибута href
        var id  = $(this).attr('href'),
        //узнаем высоту от начала страницы до блока на который ссылается якорь
            top = $(id).offset().top;
        //анимируем переход на расстояние - top за 1500 мс
        $('body,html').animate({scrollTop: top}, 1500);
    });

	new WOW().init();
	
});


