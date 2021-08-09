<!DOCTYPE html>
<html lang="tr">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Solve Portfolio</title>
    <link
      rel="icon"
      href="data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22><text y=%22.9em%22 font-size=%2290%22>🎯</text></svg>"
    />
    <link rel="stylesheet" href="style.css" />
    <link
      rel="stylesheet"
      href="https://use.fontawesome.com/releases/v5.15.3/css/all.css"
      integrity="sha384-SZXxX4whJ79/gErwcOYf+zWLeJdY/qpuqC4cAa9rOGUstPomtqpuNWT9wdPEn2fk"
      crossorigin="anonymous"
    />
  </head>
  <body>
    <section id="main" class="center">
      <div id="particles-js"></div>
      <div class="user_info">
        <h1 class="user_name">Solve </h1>
        <p>Front-End & Android Developer</p>
        <button class="btn">About Us</button>
      </div>
    </section>

    <!-- about -->
    <section class="about center" id="About">
      <h1 class="about_heading">Hakkımda</h1>
      <p>
        Selam! Ben Solve ve ben web & android geliştiricisiyim.<br />
        Tasarımdan çok çeşitli becerilere sahibim,<br />
        Kotlin + Java(Android) + HTML + CSS + Javascript'e.
      </p>
    </section>
    <section class="skills center" id="Skills">
      <p class="skill_head">Becerilerim</p>
      <div class="skill_box center">
        <div class="box">
          <i class="fab fa-android fa-4x"></i>
          <p>Kotlin</p>
        </div>
        <div class="box">
          <i class="fab fa-java fa-4x"></i>
          <p>Java(Android)</p>
        </div>
        <div class="box">
          <i class="fab fa-html5 fa-4x"></i>
          <p>HTML</p>
        </div>
        <div class="box">
          <i class="fab fa-css3-alt fa-4x"></i>
          <p>CSS</p>
        </div>
        <div class="box">
          <i class="fab fa-js-square fa-4x"></i>
          <p>Javascript</p>
        </div>
        <div class="box">
          <i class="fab fa-node-js fa-4x"></i>
          <p>Node JS</p>
        </div>
      </div>
    </section>

    <section class="projects center" id="Projects">
      <h1 class="project_heading">Projelerim</h1>
      <div class="container center">
        <div class="main_box center">
          <div class="icon center">
            <i class="fas fa-sitemap"></i>
          </div>
          <div class="box">
            <h1>Bu site</h1>
            <p>
              Bu projenin kaynak kodu.
            </p>
            <div class="links">
              <a
                href="https://github.com/solvebey/solvebey.github.io"
                target="_blank_"
                >Github Repo<i class="fas fa-arrow-right"></i
              ></a>
            </div>
          </div>
        </div>
        <div class="main_box center">
          <div class="icon center">
            <i class="fas fa-hashtag"></i>
          </div>
          <div class="box">
            <h1>Hmm.. Proje Yok gibi duruyor</h1>
            <p>Çok Projem Yok ama yakında buralar dolacak :)</p>
            <div class="links">
              <a
                href=""
                target="_blank_"
                >Github Repo<i class="fas fa-arrow-right"></i
              ></a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- footer -->
    <footer class="center">
      <h1>Buralarda Aktifim.</h1>
      <div class="social_media_icons">
        <a href="https://www.instagram.com/solvebey/" target="_blank_"
          ><i class="fab fa-instagram"></i
        ></a>
        <a href="https://github.com/solvebey" target="_blank_"
          ><i class="fab fa-github"></i
        ></a>
        <a href="https://discord.com/users/852804973183500329" target="_blank_"
        ><i class="fab fa-discord"></i
      ></a>
      </div>
      <div class="center">
      <p> Bu website Solve  tarafından yazılmıştır.
    </p>
     </div>
    </footer>

    <!-- Toggle -->
    <div class="toggle center active" id="toggle">
      <div class="box center">
          <a href="#main" class="links center"> 
            <i class="fas fa-home"></i>
            <p>Home</p>
          </a>
      </div>
      <div class="box center">
          <a href="#About" class="links center"> 
            <i class="fas fa-address-card"></i>
            <p>About</p>
          </a>
        <input type="checkbox" name="" id="btn" />
          <a href="#Skills" class="links center"> 
            <i class="fas fa-sliders-h"></i>
            <p>Skills</p>
          </a>
      </div>
      <div class="box">
          <a href="#Projects" class=" links center"> 
            <i class="fas fa-tasks"></i>
            <p>Projects</p>
          </a>
      </div>
    </div>

    <script src="https://cdnjs.cloudflare.com/ajax/libs/particles.js/2.0.0/particles.min.js"></script>
    <script src="particles.js"></script>
    <script>
      const toggle = document.getElementById("toggle");
      const btn = document.getElementById("btn");
      const links = document.querySelectorAll(".links");

      btn.addEventListener("click", (e) => {
        toggle.classList.toggle("active");
      });
      links.forEach((e) => {
        e.addEventListener("click", () => {
        toggle.classList.toggle("active");
        })
      });
    </script>
  </body>
</html>
