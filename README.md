<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Aboreto&family=Golos+Text:wght@500&family=PT+Serif&family=Ysabeau+Infant:ital,wght@0,1;0,100;0,200;0,300;1,1;1,100;1,200&display=swap" rel="stylesheet">
    <script src="https://kit.fontawesome.com/ca664d2fa9.js" crossorigin="anonymous"></script>
    <title>loungesports.com</title>
    <link rel="stylesheet" href="home.css">
</head>
<body>
  <!-- HEADER CONTAINER -->
  <div class="header-container">
    <h1 class="header1">THE LOUNGE SPORTS</h1>
    <nav>
      <ul>
        <li><a href="index.html">Inicio</a></li>
        <li><a href="betzone.html">BetZone</a></li>
        <li><a href="futbol.html" title="Futbol">Futbol</a></li>
        <li><a href="basquetbol.html" title="Basquetbol">Basquetbol</a></li>
        <li><a href="american_football.html" title="NFL">NFL</a></li>
      </ul>
    </nav>
  </div>

  <div class="breaking-news-bar">
    <div class="breaking-news-content">
      <span class="news-label">Resultados: </span>
      <marquee behavior="scroll" direction="left" onmouseover="this.stop();" onmouseout="this.start();">
        <a href="#" class="news-item"><img src="/boston celtics logo.png" width="25" height="25"> <p class="vs"> VS </p> <img src="./new york knicks logo.png" width="30" height="25"></a>
        <a href="#" class="news-item"><img src="/toronto raptors logo.png" width="25" height="25"> <p class="vs"> VS </p><img src="./washington wizards logo.png" width="25" height="25"></a>
        <a href="#" class="news-item"><img src="./milwaukee bucks logo.png" width="18" height="25"> <p class="vs"> VS </p> <img src="./chicago bulls logo.png" width="33" height="25"></a>
        <a href="#" class="news-item"><img src="/sacramento kings.png" width="20" height="25"> <p class="vs"> VS </p> <img src="./cleveland cavaliers logo.png" width="25" height="25"></a>
        <a href="#" class="news-item"><img src="/Newcastle Logo.png" width="25" height="25"> <p class="vs"> 1-1 </p> <img src="./Crystal Palace Logo.png" width="22" height="25"></a>
        <a href="#" class="news-item"><img src="./Nottingham Forest Logo.png" width="9" height="25"> <p class="vs"> 2-2 </p> <img src="./Luton Town FC Logo.png" width="25" height="25"></a>
        <a href="#" class="news-item"><img src="./Chelsea Logo.png" width="25" height="25"> <p class="vs"> 2-2 </p> <img src="./Arsenal FC Logo.png" width="18" height="25"></a>
        <a href="#" class="news-item"><img src="./Sheffield United Logo.png" width="25" height="25"> <p class="vs"> 1-2 </p> <img src="./Manchester United Logo.png" width="25" height="25"></a>
        <!-- Add more news items as needed -->
      </marquee>
    </div>
  </div>
  


  <!-- SLIDER CONTAINER -->
  <div id="slider-container">
    <div id="slider">
      <div class="slide"><img src="./cityvsnewcastle.jpg" alt="Noticia 1"></div>
      <div class="slide"><img src="realmadrid img2.jpg" alt="Noticia 2"></div>
      <div class="slide"><img src="columbuscrew1.jpg" alt="Noticia 3"></div>
      <!-- Añadir más slides según sea necesario -->
    </div>
    <div id="news-title">Título de la noticia</div>
  </div>
  
  <script>
    let currentIndex = 0;
    const slider = document.getElementById('slider');
    const slides = document.querySelectorAll('.slide');
    const newsTitle = document.getElementById('news-title');
  
    function showSlide(index) {
      const offset = -index * 100 + '%';
      slider.style.transform = 'translateX(' + offset + ')';
    }
  
    function updateNewsTitle(index) {
      // Añadir lógica para obtener el título de la noticia según el índice
      newsTitle.textContent = 'Título de la noticia ' + (index + 1);
    }
  
    function nextSlide() {
      currentIndex = (currentIndex + 1) % slides.length;
      showSlide(currentIndex);
      updateNewsTitle(currentIndex);
    }
  
    function prevSlide() {
      currentIndex = (currentIndex - 1 + slides.length) % slides.length;
      showSlide(currentIndex);
      updateNewsTitle(currentIndex);
    }
  
    // Mostrar la primera noticia al cargar la página
    showSlide(currentIndex);
    updateNewsTitle(currentIndex);
  
    // Agregar event listeners para los botones de siguiente y anterior
    document.addEventListener('keydown', function (event) {
      if (event.key === 'ArrowRight') {
        nextSlide();
      } else if (event.key === 'ArrowLeft') {
        prevSlide();
      }
    });

    setInterval(nextSlide, 4500);

  </script>
  


<!--NOTICIA PRINCIPAL DEL DÍA-->
  
    <!-- ZONA DE TIPS DE APUESTAS DEPORTIVAS 1 -->
    <div class="noticias">
      <div class="seccion-noticias">
          <img src="./cityvsnewcastle.jpg">
          <div id="news-title2"><a href="#">Título de la noticia</a></div>
      </div>
      <div class="seccion-noticias">
        <img src="./cityvsnewcastle.jpg">
          <div id="news-title2">Título de la noticia</div>
      </div>
      <div class="seccion-noticias">
        <img src="./cityvsnewcastle.jpg">
          <div id="news-title2">Título de la noticia</div>
      </div>
  </div>
  
    

  <div class="noticias">
    <div class="seccion-noticias">
        <img src="./lakers news post.png">
        <div id="news-title2"><a href="#">Título de la noticia</a></div>
    </div>
    <div class="seccion-noticias">
      <img src="./lakers news post.png">
      <div id="news-title2"><a href="#">Título de la noticia</a></div>
  </div>
  <div class="seccion-noticias">
    <img src="./lakers news post.png">
    <div id="news-title2"><a href="#">Título de la noticia</a></div>
</div>
</div>




<iframe id="sofa-standings-embed-1-52186"  width="32%" height="900px"  src="https://widgets.sofascore.com/embed/tournament/1/season/52186/standings/Premier%20League?widgetTitle=Premier League&showCompetitionLogo=true"  frameborder="0" scrolling="no" class="standings"></iframe>
<iframe id="sofa-standings-embed-36-52376" width="32%" height="900px"  src="https://widgets.sofascore.com/embed/tournament/36/season/52376/standings/LaLiga?widgetTitle=LaLiga&showCompetitionLogo=true" frameborder="0" scrolling="no" class="standings"></iframe>
<iframe id="sofa-standings-embed-42-52608" width="32%" height="900px"  src="https://widgets.sofascore.com/embed/tournament/42/season/52608/standings/Bundesliga?widgetTitle=Bundesliga&showCompetitionLogo=true" frameborder="0" scrolling="no" class="standings"></iframe>
<iframe id="sofa-standings-embed-177-54105" width="48%" height="900px" src="https://widgets.sofascore.com/embed/tournament/177/season/54105/standings/Eastern%20Conference?widgetTitle=Eastern Conference&showCompetitionLogo=true" frameborder="0" scrolling="no" class="standings"></iframe>
<iframe id="sofa-standings-embed-177-54105" width="48%" height="900px"src="https://widgets.sofascore.com/embed/tournament/177/season/54105/standings/Western%20Conference?widgetTitle=Western Conference&showCompetitionLogo=true" frameborder="0" scrolling="no" class="standings"></iframe>


  <!-- FOOTER -->
  <footer class="footer">
    <div class="footer-content">
      <div class="social-icons">
        <a href="#" class="social-link"><i class="fa-regular fa-user"></i></a>
        <a href="#" class="social-link"><i class="fab fa-youtube"></i></a>
        <a href="#" class="social-link"><i class="fab fa-twitter"></i></a>
        <a href="#" class="social-link"><i class="fab fa-instagram"></i></a>
        <!-- Add more social media icons and links as needed -->
      </div>
      <div class="web-page-name">THE LOUNGE SPORTS</div>
      <div class="copyright">
        &copy; <span id="current-year"></span> All rights reserved.
      </div>
    </div>
  </footer>
  
</body>
</html>
