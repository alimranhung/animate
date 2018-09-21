## Call for CSS
animate.css

## How to use for js. EXAMPLE Default Animate use
```
$(".single-portfolio-item").hover(function(){
  $(".portfolio-inner h2").removeClass("animated slideInUp");
  $(this).find(".portfolio-inner h2").addClass("animated slideInUp");
 });
 ```
 ## Homepage owlCarousel use for animate.
 
```
 var homepageArea = $('.homepage-area');
            homepageArea.owlCarousel({
               items:1,
                dots:true,
                autoplay:true,
                autoplayTimeout:1300,
                nav:true,
                loop:true,
                navText:["<i class='fa fa-angle-left'></i>", "<i class='fa fa-angle-right'></i>"], 
            });

            homepageArea.on('translate.owl.carousel', function(event) {
                $(".homepage-text h4").removeClass("animated bounceIn");
                $(".homepage-text h1").removeClass("animated jackInTheBox");
                $(".homepage-text p").removeClass("animated fadeIn");
            });

            homepageArea.on('translated.owl.carousel', function(event) {
                $(".homepage-text h4").addClass("animated bounceIn");
                $(".homepage-text h1").addClass("animated jackInTheBox");
                $(".homepage-text p").addClass("animated fadeIn");
            });

```
