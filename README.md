<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Monisha Ramani Portfolio</title>
<style>
    /* ===== Reset ===== */
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; }
    body { scroll-behavior: smooth; }

    a { text-decoration: none; color: inherit; }

    section { min-height: 100vh; display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center; color: white; padding: 60px 20px; background-size: cover; background-position: center; position: relative; }

    /* ===== Overlay for readability ===== */
    section::before {
        content: "";
        position: absolute;
        top: 0; left: 0; width: 100%; height: 100%;
        background: rgba(0,0,0,0.5);
        z-index: 0;
    }

    section * { position: relative; z-index: 1; }

    h2 { font-size: 2.5rem; margin-bottom: 40px; text-transform: uppercase; letter-spacing: 2px; }
    p { max-width: 700px; margin: 20px auto; font-size: 1.2rem; line-height: 1.6; }

    /* ===== Header ===== */
    header { background: url('./premium_photo-1683309567322-e95b9f182dcc.jpg') center/cover no-repeat; min-height: 100vh; display: flex; flex-direction: column; justify-content: center; align-items: center; color: white; text-align: center; }
    header h1 { font-size: 4rem; margin-bottom: 10px; animation: slideIn 1s forwards; }
    header p { font-size: 1.5rem; opacity: 0.9; animation: fadeIn 2s forwards; }
    
    @keyframes slideIn { from { transform: translateY(-50px); opacity:0; } to { transform: translateY(0); opacity:1; } }
    @keyframes fadeIn { from { opacity:0; } to { opacity:1; } }

    /* ===== About Section ===== */
    #about { background: url('./images.jpg') center/cover no-repeat; flex-direction: row; flex-wrap: wrap; gap: 40px; }
    .about img { width: 300px; border-radius: 15px; transition: transform 0.5s; }
    .about img:hover { transform: scale(1.05); }
    .about-text { max-width: 600px; text-align: left; }

    /* ===== Skills Section ===== */
    #skills { background: url('./ripped-notes-rectangle-frame-vector_53876-109026.jpg') center/cover no-repeat; }
    .skills { display: flex; flex-wrap: wrap; justify-content: center; gap: 20px; }
    .skill { background: rgba(255,255,255,0.2); padding: 20px; border-radius: 10px; width: 150px; transition: transform 0.3s, background 0.3s; cursor: pointer; }
    .skill:hover { transform: translateY(-10px); background: rgba(255,255,255,0.4); }

    /* ===== Projects Section ===== */
    #projects { background: url('https://images.unsplash.com/photo-1504384308090-c894fdcc538d?fit=crop&w=1950&q=80') center/cover no-repeat; }
    .projects { display: flex; flex-wrap: wrap; justify-content: center; gap: 20px; }
    .project-card { background: rgba(255,255,255,0.15); backdrop-filter: blur(10px); padding: 30px; border-radius: 15px; width: 350px; transition: transform 0.3s, box-shadow 0.3s; }
    .project-card:hover { transform: translateY(-10px); box-shadow: 0 8px 20px rgba(0,0,0,0.3); }
    .project-card h3 { color: #FFD700; margin-bottom: 15px; }

    /* ===== Contact Section ===== */
    #contact { background: url('./download.jpg') center/cover no-repeat; flex-direction: column; }
    .contact a { margin: 10px; padding: 12px 25px; border-radius: 25px; border: 2px solid white; color: white; transition: all 0.3s; display: inline-block; }
    .contact a:hover { background: white; color: #333; transform: scale(1.1); }

    /* ===== Footer ===== */
    footer { background: #111; color: white; text-align: center; padding: 20px; }

    /* ===== Responsive ===== */
    @media(max-width:768px) { .about { flex-direction: column; text-align: center; } .about-text { text-align: center; } }

</style>
</head>
<body>

<!-- ===== Header ===== -->
<header>
    <h1>Monisha Moti Ramani</h1>
    <p>Tech Professional | Full Stack Developer | Frontend Enthusiast</p>
</header>

<!-- ===== About Me ===== -->
<section id="about">
    <h2>About Me</h2>
    <div class="about">
        <img src="./WhatsApp Image 2025-05-20 at 18.20.18 (1).png" alt="Monisha Ramani">
        <div class="about-text">
            <p>Hello! I'm Monisha, a passionate Tech Professional skilled in Java, ReactJS, Spring Boot, and AWS. I have completed internships at Lotfair Solutions and Allianz, working on data models, dashboards, and software projects. I love creating interactive web applications and solving challenging problems.</p>
        </div>
    </div>
</section>

<!-- ===== Skills ===== -->
<section id="skills">
    <h2>Skills</h2>
    <div class="skills">
        <div class="skill">Java</div>
        <div class="skill">ReactJS</div>
        <div class="skill">Spring Boot</div>
        <div class="skill">AWS</div>
        <div class="skill">SQL</div>
        <div class="skill">HTML & CSS</div>
    </div>
</section>

<!-- ===== Projects ===== -->
<section id="projects">
    <h2>Projects</h2>
    <div class="projects">
        <div class="project-card" style="font-size: medium;">
            <h3>English Letters Detector</h3>
            <p>A ReactJS and MediaPipe project detecting hand gestures to recognize English letters in real-time.</p>
        </div>
        <div class="project-card">
            <h3>Pharmacy Website</h3>
            <p>Designed an interactive website using HTML, CSS, and JavaScript with responsive UI and smooth animations.</p>
        </div>
    </div>
</section>

<!-- ===== Contact ===== -->
<section id="contact">
    <h2>Contact Me</h2>
    <div class="contact">
        <a href="mailto:monisha@example.com">Email Me</a>
        <a href="https://www.linkedin.com/in/monisha-ramani" target="_blank">LinkedIn</a>
        <a href="https://github.com/monisha-ramani" target="_blank">GitHub</a>
    </div>
</section>

<!-- ===== Footer ===== -->
<footer>
    <p>&copy; 2025 Monisha Moti Ramani. All rights reserved.</p>
</footer>

</body>
</html>
