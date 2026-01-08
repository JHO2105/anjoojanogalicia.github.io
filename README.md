# Portfolio
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title></title>
  <style>
    body {
      margin: 0;
      font-family: 'Treasure Map Deadhand', Arial, sans-serif;
      background: #fdf6e3;
      color: #222;
    }
    header {
      background: url(https://uploads.onecompiler.io/43yxcwbky/449yagde4/1000000247.png) no-repeat center/cover;
      color: white;
      text-align: center;
      padding: 80px 20px;
    }
    header h1 {
      font-size: 3em;
      text-shadow: 2px 2px 6px black;
    }
    nav {
      display: flex;
      justify-content: center;
      background: #222;
      position: sticky;
      top: 0;
      z-index: 100;
    }
    nav a {
      color: white;
      text-decoration: none;
      padding: 15px 20px;
      transition: 0.3s;
    }
    nav a:hover {
      background: #f39c12;
    }
    section {
      padding: 50px 20px;
      text-align: center;
    }
    .skills-bar {
      background: #ddd;
      border-radius: 25px;
      margin: 10px auto;
      width: 60%;
      height: 25px;
      overflow: hidden;
    }
    .skills-fill {
      background: linear-gradient(to right, #f39c12, #e67e22);
      height: 100%;
      width: 0;
      text-align: right;
      padding-right: 10px;
      color: white;
      line-height: 25px;
      transition: width 2s ease;
    }
    footer {
      background: #222;
      color: white;
      text-align: center;
      padding: 15px;
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header id="home">
    <h1></h1>
    <p></p>
  </header>

  <!-- Navigation -->
  <nav>
    <a href="#home">Home</a>
    <a href="#about">About Me</a>
    <a href="#skills">Skills</a>
    <a href="#contact">Contact</a>
  </nav>

  <!-- About Section -->
  <section id="about">
    <h2>ANJO OJANO GALICIA</h2>
    <p>Hi! I’m Anjo Ojano Galicia the self-driven programmer who independently hunts down bugs, requirements, and solutions to create efficient and reliable software.</p>
    <img src="https://uploads.onecompiler.io/43yxcwbky/449ya8yt3/1000001859.png" alt="Profile" width="200">
  </section>

  <!-- Skills Section -->
  <section id="skills">
    <h2>MY SKILLS</h2>
    <p>Learned Skills</p>
    <div class="BAR"><div class="FILL" data-skill="100%">JAVA</div></div>
    <div class="BAR"><div class="FILL" data-skill="100%">JavaScript</div></div>
    <div class="BAR"><div class="FILL" data-skill="100%">HTML</div></div>
     <div class="BAR"><div class="FILL" data-skill="100%">PHP</div></div>
     <div class="BAR"><div class="FILL" data-skill="100%">GITHUB</div></div>
     <div class="BAR"><div class="FILL" data-skill="100%">PYTHON</div></div>
     <div class="BAR"><div class="FILL" data-skill="100%">CSS</div></div>
  </section>

  <!-- Contact Section -->
  <section id="contact">
    <h2>Contact Me</h2>
    <p>Email: <a href="mailto:anjoojanogalicia@gmail.com">anjoojanogalicia@gmail.com</a></p>
    <p>“Goo to Grow!”</p>
  </section>

  <!-- Footer -->
  <footer>
    <p>© 2026 Made with ANJO GALICIA: All Rights Reserved</p>
  </footer>

  <script>
    // Animate skill bars on scroll
    window.addEventListener("scroll", function(){
      let skills = document.querySelectorAll("FILL");
      skills.forEach(skill => {
        let rect = skill.getBoundingClientRect();
        if(rect.top < window.innerHeight){
          skill.style.width = skill.getAttribute("data-skill");
        }
      });
    });
  </script>

</body>
</html>
