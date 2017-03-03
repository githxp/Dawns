//首页

$(document).ready(function() {
    var $nav = $('header .nav');
    var $attention = $nav.find('.attention');
    var $arrow = $nav.find('.arrow');
    var $attentionQrcode = $nav.find('.attention-qrcode');

    var $content = $('.content');
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

    window.onscroll = function() {
        var offset =  window.pageYOffset || document.documentElement.scrollTop || document.body.scrollTop;
        if(offset > 300 && offset < 1000) {
            $('section.intro1').find('img').addClass('animate');
        } else if(offset > 1100 && offset < 1700) {
            $('section.intro2').find('img').addClass('animate');
        } else if(offset > 1900 && offset < 2300) {
            $('section.intro3').find('img').addClass('animate');
        } else if(offset > 2400) {
            $('section.intro4').find('img').addClass('animate');
        }
    }

    $('.charge_list li').click(function(){
        $(this).addClass('active').siblings().removeClass('active')
    })
});
