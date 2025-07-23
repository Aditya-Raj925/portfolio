<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Aditya Raj | Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <style>
    
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  font-family: 'Poppins', sans-serif;
  color: #333;
  background-color: #e6f3ff;
}
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 60px;
  background: white;
  box-shadow: 0 2px 6px rgba(0,0,0,0.1);
  position: sticky;
  top: 0;
  z-index: 1000;
}
.logo {
  font-size: 1.8rem;
  font-weight: bold;
  color: #d11a2a;
}
nav ul {
  display: flex;
  list-style: none;
}
nav li {
  margin-left: 30px;
}
nav a {
  text-decoration: none;
  color: #555;
  font-size: 1rem;
}
nav a:hover,
nav a.active {
  border-bottom: 2px solid #d11a2a;
  color: #d11a2a;
}
.hero {
  min-height: 90vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 60px 20px;
  background-color: #f0f0f5;
}
.flip-container {
  width: 180px;
  height: 180px;
  perspective: 1000px;
  margin-bottom: 20px;
}
.flipper {
  position: relative;
  width: 100%;
  height: 100%;
  transition: transform 0.8s;
  transform-style: preserve-3d;
}
.flip-container:hover .flipper {
  transform: rotateY(180deg);
}
.front,
.back {
  position: absolute;
  width: 100%;
  height: 100%;
  border-radius: 50%;
  overflow: hidden;
  backface-visibility: hidden;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
}
.front img,
.back img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.back {
  transform: rotateY(180deg);
}
.hero h1 {
  font-size: 3rem;
  margin: 20px 0 10px;
}
.hero h1 span {
  color: #d11a2a;
}
.intro-text {
  font-size: 1.2rem;
  margin: 10px 0;
  max-width: 600px;
  line-height: 1.6;
}
.about-section {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 80px 60px;
  gap: 40px;
  margin-bottom: 80px; 
}
.about-image img {
  width: 320px;
  max-width: 100%;
  border-radius: 8px;
  box-shadow: 0 5px 20px rgba(0, 0, 0, 0.1);
}
.about-content {
  max-width: 600px;
}
.about-content h1 {
  font-size: 2.5rem;
  margin-bottom: 20px;
  color: #d11a2a;
}
.about-content p {
  font-size: 1.1rem;
  line-height: 1.6;
  margin-bottom: 20px;
}
.about-details p {
  margin-bottom: 10px;
  font-size: 1rem;
}
.about-details a {
  color: #d11a2a;
  text-decoration: none;
}
.about-details a:hover {
  text-decoration: underline;
}
.skills-page {
  text-align: center;
  padding: 60px 10px;
}
.skills-page h1 {
  font-size: 2.5rem;
  color: #0077cc;
  margin-bottom: 10px;
}
.skills-intro {
  font-size: 1.1rem;
  margin-bottom: 40px;
}
.skills-grid {
  display: flex;
  flex-direction: column;
  gap: 40px;
  padding: 0 40px;
}
.skills-row {
  display: flex;
  justify-content: space-between;
  gap: 30px;
  flex-wrap: wrap;
}
.skills-row.center {
  justify-content: center;
}
.skill-category {
  flex: 0 0 40%;
  max-width: 40%;
  background-color: #ffffff;
  padding: 20px; 
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0, 119, 204, 0.1);
}.skill-category h2 {
  color: #005fa3;
  margin-bottom: 20px;
  font-size: 1.3em;
}
.skill {
  margin-bottom: 15px;
}
.skill span {
  display: block;
  margin-bottom: 5px;
  font-weight: 600;
}
.progress-bar {
  background-color: #cfe8fc;
  border-radius: 8px;
  height: 10px;
  overflow: hidden;
}
.progress {
  height: 100%;
  background-color: #0077cc;
  transition: width 1s ease;
}
.site-footer {
  text-align: center;
  padding: 30px;
  background: white;
  margin-top: 60px;
  color: #777;
  font-size: 0.9rem;
}
@media (max-width: 860px) {
  .about-section {
    flex-direction: column;
    padding: 40px 20px;
  }
  .about-image,
  .about-content {
    width: 100%;
  }
  .skills-grid {
    padding: 0 20px;
  }
}
  </style>
</head>
<body>
  <header>
    <div class="logo">Aditya Raj</div>
    <nav>
  <ul>
    <li><a href="#home" >Home</a></li>
    <li><a href="#about" >About Me</a></li>
    <li><a href="#skills" >Skills</a></li>
    <li><a href="#contact" >Contact</a></li>
  </ul>
</nav>

  </header>

  <!-- Home Section -->
  <section class="hero" id="home">
    <div class="flip-container">
      <div class="flipper">
        <div class="front">
          <img src="https://tse4.mm.bing.net/th/id/OIP.JI3SqmECXr6m1Kc-1BsWfwHaHZ?pid=Api&P=0&h=180" alt="Profile Picture">
        </div>
        <div class="back">
          <img src="pic.jpg" alt="Full Image">
        </div>
      </div>
    </div>
    <h1>Hi, It's <span>Aditya Raj</span></h1>
    <p class="intro-text">
      I'm a programmer of C++, C, Java, Python and also a web developer. B.Tech student 2nd year.
    </p>
  </section>

  <!-- About Me Section -->
  <section class="about-section" id="about">
    <div class="about-image">
      <img src="https://tse4.mm.bing.net/th/id/OIP.JI3SqmECXr6m1Kc-1BsWfwHaHZ?pid=Api&P=0&h=180" alt="Aditya Raj">
    </div>
    <div class="about-content">
      <h1>About Me</h1>
      <p>Hello! I’m Aditya Raj, a passionate programmer proficient in C++, C, Java, Python, and web development. Currently a 2nd-year B.Tech student, I love building sleek and responsive web experiences that both look amazing and perform beautifully across devices.</p>
      <p>When I’m not coding, I enjoy learning new tech, contributing to open-source, and exploring creative projects that push my skills further.</p>
      <div class="about-details">
        <p><strong>📍 Location:</strong> Patna, Bihar, India</p>
        <p><strong>📞 Phone:</strong> <a href="tel:+919876543210">+91 9876543210</a></p>
        <p><strong>🐦 Twitter:</strong> <a href="https://twitter.com/yourhandle" target="_blank">@yourhandle</a></p>
      </div>
    </div>
  </section>
  <br>
  <br>
<br>
<br><br><br><br><br><br>>

  <!-- Skills Section -->
  <section class="skills-page" id="skills">
    <h1>My Skills</h1>
    <p class="skills-intro">Here are some of the tools and technologies I excel at:</p>

   <div class="skills-grid">

      
   <div class="skills-row">
        <div class="skill-category">
          <h2>Programming Languages</h2>
          <div class="skill"><span>HTML</span><div class="progress-bar"><div class="progress" style="width: 95%;"></div></div></div>
          <div class="skill"><span>CSS</span><div class="progress-bar"><div class="progress" style="width: 90%;"></div></div></div>
          <div class="skill"><span>JavaScript</span><div class="progress-bar"><div class="progress" style="width: 85%;"></div></div></div>
          <div class="skill"><span>C++</span><div class="progress-bar"><div class="progress" style="width: 88%;"></div></div></div>
        </div>

   <div class="skill-category">
          <h2>Tools & Frameworks</h2>
          <div class="skill"><span>Git & GitHub</span><div class="progress-bar"><div class="progress" style="width: 90%;"></div></div></div>
          <div class="skill"><span>VS Code</span><div class="progress-bar"><div class="progress" style="width: 92%;"></div></div></div>
          <div class="skill"><span>React</span><div class="progress-bar"><div class="progress" style="width: 80%;"></div></div></div>
        </div>
      </div>
      <div class="skills-row center">
        <div class="skill-category">
          <h2>Soft Skills</h2>
          <div class="skill"><span>Communication</span><div class="progress-bar"><div class="progress" style="width: 90%;"></div></div></div>
          <div class="skill"><span>Problem Solving</span><div class="progress-bar"><div class="progress" style="width: 87%;"></div></div></div>
          <div class="skill"><span>Teamwork</span><div class="progress-bar"><div class="progress" style="width: 89%;"></div></div></div>
        </div>
      </div>

   </div>
  </section>


  <footer class="site-footer" id="contact">
    <p>© 2025 Aditya Raj</p>
  </footer>

</body>
</html>
