//首页

$(document).ready(function() {
    var $nav = $('header .nav');
    var $attention = $nav.find('.attention');
    var $arrow = $nav.find('.arrow');
    var $attentionQrcode = $nav.find('.attention-qrcode');

    var $content = $('.content');
    //var $downloadApple = $('.download .download-apple');
    var $dialogBk = $('.dialog-bk');
    var $dialog = $('.dialog');
    var scrollTop;

    $attention.hover(function() {
        $arrow.stop().show();
        $attentionQrcode.stop().slideDown();
    },function() {
        $attentionQrcode.stop().slideUp(function() {
            $arrow.stop().hide();
        });
    });

    //$downloadApple.click(function() {
    //    scrollTop = document.documentElement.scrollTop || document.body.scrollTop;
    //
    //    $content.css({
    //    	'width': $(document).width(),
    //        'position': 'fixed',
    //        'top': -scrollTop,
    //        'left': 0
    //    });
    //
    //    $dialogBk.css({
    //        'width': $(document).width(),
    //        'height':$(document).height()+30
    //    });
    //
    //    $dialogBk.fadeIn();
    //    $dialog.fadeIn();
    //});

    //$dialog.find('.button.sure').click(function() {
    //    $dialogBk.fadeOut();
    //    $dialog.fadeOut();
    //    $content.css('position','static');
    //    $('body').scrollTop(scrollTop);
    //});

    window.onscroll = function() {
        var offset = document.documentElement.scrollTop || document.body.scrollTop;

        if(offset > 300 && offset < 1000) {
            $('section.intro1').find('img').addClass('animate');
        } else if(offset > 1100 && offset < 1700) {
            $('section.intro2').find('img').addClass('animate');
        } else if(offset > 1900 && offset < 2600) {
            $('section.intro3').find('img').addClass('animate');
        } else if(offset > 2700 && offset < 3500) {
            $('section.intro4').find('img').addClass('animate');
        }
    }

    $('.charge_list li').click(function(){
        $(this).addClass('active').siblings().removeClass('active')
    })
});
