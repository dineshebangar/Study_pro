
$(window).load(function() {
  if($('.flexslider').length > 0)
  {
    $('.flexslider').flexslider({
      animation: "slide",
      slideshowSpeed: 20000,
      animationLoop: true,
      pauseOnAction: false,
      pauseOnHover: false,
      slideshowSpeed: 20000
    });
  }
});



$(document).ready(function(){

  //get-started ga

/*  if($('.get-started-submit').length > 0){
     $('.get-started-submit').submit(function() {
        ga('send', 'event', 'form', 'click', 'download-btn');
    });
  }*/

  //whitepaper ga

/*   if($('.whitepaper-submit').length > 0){
     $('.whitepaper-submit').submit(function() {
         ga('send', 'event', 'form', 'click', 'download-btn');
    });
  }*/


  if($('.column').length > 0){
    $('.column:last-child').css({'margin-right':'0'})
  }

  if($('.cols-3').length > 0){
    $('.cols-3:last-child').css({'margin-right':'0'})
  }


  //fancybox close on escape.

  $( document ).on( 'keydown', function ( e ) {
    if ( e.keyCode === 27 ) {
      $.fancybox.close();
    }
  });

  /*if($('.slideup-data').length > 0)
   {
   $('.slideup-data ul').css('display','none');
   $('.slideup-data p').on('click',function(){
   $('.slideup-data ul').slideToggle();
   })
   }*/

   if(navigator.userAgent.match(/MSIE/i)){
    if($('input').length > 0){
      $('input[placeholder]').each(function(){
        var input = $(this);
        $(input).val(input.attr('placeholder'));

        $(input).focus(function(){
          if (input.val() == input.attr('placeholder')) {
            input.val('');
          }
        });

        $(input).blur(function(){
          if (input.val() == '' || input.val() == input.attr('placeholder')) {
            input.val(input.attr('placeholder'));
          }
        });
      });
    }
   }


  if($('.dwld-chkbox').length > 0)
  {
    $('.dwld-chkbox').change(function(){
      if($(this).is(':checked')){
        $(this).parent().next().removeClass('disabled');
      }else{
        $(this).parent().next().addClass('disabled');
      }
    });
  }

  /*---ui tabs---*/

  if($( "#tabs" ).length > 0)
  {
    $( "#tabs" ).tabs().addClass( "ui-tabs-vertical ui-helper-clearfix" );
    $( "#tabs li" ).removeClass( "ui-corner-top" ).addClass( "ui-corner-left" );
  }

  if($( "#izot-tabs" ).length > 0)
    $( "#izot-tabs" ).tabs();

  //$(".block-right").mCustomScrollbar();
  /*if($(".get-started ").length > 0)
   {
   $(".get-started .block-right").mCustomScrollbar({
   scrollButtons:{
   enable:true
   }
   });
   }*/

  if($('.server-stack').length > 0){
    var ele = $(".server-stack");
    ele.fancybox({
      'autoDimensions': false,
      'autoSize': false,
      'height': 'auto',
      'width':'960px',
      'afterShow' : function(){
        addScroll();
      },
      'afterClose':function(){
        $('.check-terms').css('color','#444444');
        $('#FirstName,#LastName,#Title,#Company,#Email').css('border','1px solid #CCCCCC');
        if(!navigator.userAgent.match(/MSIE/i))
        {
          $('#FirstName,#LastName,#Title,#Company,#Email').val('');
          $('#SDK_Terms__Conditions').attr('checked', false);
        }
      }
    });

    if(typeof open_overlay != "undefined")
      ele.click();

  }

  if($('.anatomy').length > 0){
    $(".anatomy").fancybox({
      'href': '/assets/AnatomyOfTheIIot.png',
      helpers:  {
        overlay: {
            locked: false
        }
      }
    });
  }

  if(navigator.userAgent.match(/MSIE 8.0/i)){
   if($( "#accordion" ).length > 0)
    $( "#accordion" ).accordion({
       heightStyle: "content",
       animate:false
    });
  }
  else
  {
    if($( "#accordion" ).length > 0)
      $( "#accordion" ).accordion({
        heightStyle: "content"
      });
  }

  if($(".video").length > 0)
  {
    $(".video").colorbox({
      iframe:true,
      innerWidth:960,
      innerHeight:500
    });

  }
});

function addScroll()
{
  $("#server-stack .wrap").mCustomScrollbar("destroy");
  $("#server-stack .wrap").mCustomScrollbar({
    scrollButtons:{
      enable:true
    },
    contentTouchScroll: true
  });
}

function checkEmail(email_field) {
      var email = email_field;
      var filter = /^([a-zA-Z0-9_\.\-])+\@(([a-zA-Z0-9\-])+\.)+([a-zA-Z0-9]{2,4})+$/;

      if (!filter.test($(email).val())) {
        email.focus;
        return false;
      }
      return true;
    }

