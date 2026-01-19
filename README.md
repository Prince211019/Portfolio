<!doctype html>

<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Prince Tiwari — Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/aos/2.3.4/aos.css" />
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" />
  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --accent:#7c3aed; --muted:#94a3b8; --glass: rgba(255,255,255,0.08);
      --accent-2:#06b6d4; font-family:'Inter',sans-serif;
    }
    *{margin:0;padding:0;box-sizing:border-box}
    body{background:#000;color:#e6eef8;overflow-x:hidden;position:relative}
    a{text-decoration:none;color:inherit}/* Background Matrix Animation */
canvas#bgCanvas{position:fixed;top:0;left:0;width:100%;height:100%;z-index:-1;background:#000;}

/* Header */
header{position:fixed;width:100%;height:70px;display:flex;align-items:center;backdrop-filter:blur(8px);z-index:10;border-bottom:1px solid rgba(255,255,255,0.05)}
.navwrap{width:100%;max-width:1200px;margin:0 auto;display:flex;align-items:center;justify-content:space-between;padding:0 20px}
.logo{font-size:22px;font-weight:800;color:var(--accent)}
nav{display:flex;gap:20px}
nav a{color:var(--muted);font-weight:600;transition:.3s}
nav a:hover{color:var(--accent)}

.cta{background:linear-gradient(90deg,var(--accent),var(--accent-2));padding:8px 14px;border-radius:10px;color:white!important}

/* Section */
section{padding:100px 20px;max-width:1200px;margin:auto}
.section-title{text-align:center;margin-bottom:40px}
.section-title h2{font-size:28px;color:var(--accent)}
.section-title p{color:var(--muted)}

/* Hero */
.hero{display:flex;flex-direction:column;align-items:center;justify-content:center;text-align:center;min-height:100vh}
.profile-pic{
  width:180px;
  height:180px;
  object-fit:cover;
  border-radius:50%;
  margin-bottom:18px;
  border:4px solid var(--accent);
  box-shadow:0 0 30px rgba(124,58,237,0.6),0 0 60px rgba(6,182,212,0.3);
  animation:floatPic 6s ease-in-out infinite;
}
@keyframes floatPic{0%{transform:translateY(0)}50%{transform:translateY(-10px)}100%{transform:translateY(0)}}
.hero h1{font-size:48px;color:white;animation:glow 2s infinite alternate}
@keyframes glow{0%{text-shadow:0 0 10px var(--accent)}100%{text-shadow:0 0 20px var(--accent-2)}}
.hero p{margin-top:10px;color:var(--muted);font-size:18px;max-width:700px}
.socials{margin-top:20px;display:flex;gap:20px}
.socials a{font-size:20px;color:white;transition:.3s}
.socials a:hover{color:var(--accent-2)}

/* Cards */
.card{background:var(--glass);border:1px solid rgba(255,255,255,0.05);padding:20px;border-radius:15px;box-shadow:0 0 20px rgba(0,0,0,0.4);transition:transform .4s,box-shadow .4s}
.card:hover{transform:translateY(-8px) scale(1.02);box-shadow:0 0 25px var(--accent)}

/* Grid */
.grid{display:grid;gap:20px}
.grid-2{grid-template-columns:repeat(auto-fit,minmax(300px,1fr))}

/* Timeline */
.timeline{border-left:2px solid var(--accent);padding-left:20px}
.timeline-item{margin-bottom:20px;position:relative}
.timeline-item:before{content:'';position:absolute;left:-11px;top:0;width:20px;height:20px;border-radius:50%;background:var(--accent)}
.timeline-item h3{color:white}
.timeline-item p{color:var(--muted)}

/* Skills */
.skill{margin-bottom:20px}
.skill span{display:flex;justify-content:space-between}
.bar{height:10px;background:rgba(255,255,255,0.1);border-radius:20px;overflow:hidden;margin-top:6px}
.bar i{display:block;height:100%;width:0;background:linear-gradient(90deg,var(--accent),var(--accent-2));border-radius:20px}

/* Footer */
footer{text-align:center;padding:20px;color:var(--muted);border-top:1px solid rgba(255,255,255,0.1)}

@media(max-width:768px){.hero h1{font-size:32px}}

  </style>
</head>
<body>
  <canvas id="bgCanvas"></canvas>
  <header>
    <div class="navwrap">
      <div class="logo">Prince Tiwari</div>
      <nav>
        <a href="#about">About</a>
        <a href="#education">Education</a>
        <a href="#experience">Experience</a>
        <a href="#projects">Projects</a>
        <a href="#skills">Skills</a>
        <a href="#contact" class="cta">Contact</a>
      </nav>
    </div>
  </header>  <!-- HERO -->  <section class="hero" id="home">
    <img src="your-photo.jpg" alt="Prince Tiwari" class="profile-pic" data-aos="zoom-in" />
    <h1 data-aos="fade-up">Hi, I'm Prince Tiwari</h1>
    <p data-aos="fade-up" data-aos-delay="200">A passionate Computer Science Engineer and Web Developer skilled in building responsive, modern, and interactive websites.</p>
    <div class="socials" data-aos="zoom-in" data-aos-delay="400">
      <a href="mailto:tiwariprince370@gmail.com"><i class="fa-solid fa-envelope"></i></a>
      <a href="https://www.linkedin.com/in/princetiwari1/" target="_blank"><i class="fa-brands fa-linkedin"></i></a>
      <a href="https://github.com/Prince211019" target="_blank"><i class="fa-brands fa-github"></i></a>
    </div>
  </section>  <!-- ABOUT -->  <section id="about">
    <div class="section-title"><h2>About Me</h2><p>Who I am</p></div>
    <div class="card" data-aos="fade-up">I am a Computer Science graduate (2025) with internship experience in web development. I love building projects, solving problems, and constantly learning modern technologies.</div>
  </section>  <!-- EDUCATION -->  <section id="education">
    <div class="section-title"><h2>Education</h2><p>My academic background</p></div>
    <div class="timeline" data-aos="fade-left">
      <div class="timeline-item"><h3>B.Tech, CSE</h3><p>Dr.A.P.J Abdul Kalam Technical University, UP — 2025 — 71%</p></div>
      <div class="timeline-item"><h3>Diploma, Civil</h3><p>Government Poly Puranpur Pilibhit — 2022 — 76%</p></div>
      <div class="timeline-item"><h3>Intermediate</h3><p>UP Board — 2019 — 52%</p></div>
      <div class="timeline-item"><h3>High School</h3><p>UP Board — 2017 — 78%</p></div>
    </div>
  </section>  <!-- EXPERIENCE -->  <section id="experience">
    <div class="section-title"><h2>Experience</h2><p>Internships & projects</p></div>
    <div class="grid grid-2">
      <div class="card" data-aos="fade-right"><h3>Web Development Intern</h3><p>Nov 2024 - Dec 2024</p><ul><li>Built responsive websites</li><li>Improved UI/UX</li><li>Participated in coding contests</li></ul></div>
      <div class="card" data-aos="fade-left"><h3>Projects</h3><ul><li>College Management System (HTML, CSS, JS, PHP, MySQL)</li><li>Personal Portfolio Page (HTML, CSS, JS)</li></ul></div>
    </div>
  </section>  <!-- SKILLS -->  <section id="skills">
    <div class="section-title"><h2>Skills</h2><p>Technical abilities</p></div>
    <div class="card" data-aos="zoom-in">
      <div class="skill"><span>Programming <small>85%</small></span><div class="bar"><i style="width:85%"></i></div></div>
      <div class="skill"><span>Frontend/UI <small>80%</small></span><div class="bar"><i style="width:80%"></i></div></div>
      <div class="skill"><span>Tools & Git <small>75%</small></span><div class="bar"><i style="width:75%"></i></div></div>
      <div class="skill"><span>Soft Skills <small>90%</small></span><div class="bar"><i style="width:90%"></i></div></div>
    </div>
  </section>  <!-- CONTACT -->  <section id="contact">
    <div class="section-title"><h2>Contact</h2><p>Get in touch</p></div>
    <div class="card" data-aos="fade-up">
      <p>Email: tiwariprince370@gmail.com</p>
      <p>Phone: +91 9198240802</p>
      <form onsubmit="fakeSend(event)">
        <input type="text" placeholder="Your Name" required>
        <input type="email" placeholder="Your Email" required>
        <textarea rows="4" placeholder="Message" required></textarea>
        <button type="submit">Send</button>
      </form>
    </div>
  </section>  <footer>© 2025 Prince Tiwari — Built with ❤️ using HTML, CSS & JavaScript</footer>  <script src="https://cdnjs.cloudflare.com/ajax/libs/aos/2.3.4/aos.js"></script>  <script>
    AOS.init({duration:1000,once:true});

    // Matrix-style animation
    const canvas=document.getElementById('bgCanvas');
    const ctx=canvas.getContext('2d');
    canvas.height=window.innerHeight;canvas.width=window.innerWidth;
    const letters='01';
    const fontSize=14;const columns=canvas.width/fontSize;
    const drops=[];for(let x=0;x<columns;x++)drops[x]=1;
    function draw(){ctx.fillStyle='rgba(0,0,0,0.05)';ctx.fillRect(0,0,canvas.width,canvas.height);ctx.fillStyle='#0f0';ctx.font=fontSize+'px monospace';for(let i=0;i<drops.length;i++){const text=letters[Math.floor(Math.random()*letters.length)];ctx.fillText(text,i*fontSize,drops[i]*fontSize);if(drops[i]*fontSize>canvas.height&&Math.random()>0.975)drops[i]=0;drops[i]++;}}setInterval(draw,35);
    window.addEventListener('resize',()=>{canvas.height=window.innerHeight;canvas.width=window.innerWidth});

    function fakeSend(e){e.preventDefault();alert('Message sent! (demo)')}
  </script></body>
</html>
