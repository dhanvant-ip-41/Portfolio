# Ex01 Portfolio
## Date: 28-11-2025

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM

### index.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Anish | Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
    <nav>
        <h2 class="logo">ARUN</h2>
        <ul>
            <li><a href="#intro">Intro</a></li>
            <li><a href="#about">About Me</a></li>
            <li><a href="#education">Education</a></li>
            <li><a href="#skills-projects">Skills & Projects</a></li>
            <li><a href="#contact">Contact Me</a></li>
        </ul>
    </nav>
</header>

<!-- INTRO -->
<section id="intro" class="hero" href="#intro">
    <div class="overlay"></div>

    <div class="intro-content left-align">
        <h1 class="intro-title">Hi, I'm <span class="highlight">Arun</span> </h1>
        <p class="subtitle">AI • Cybersecurity • Robotics • Automation</p>
        <p class="intro-text">
            I build things that <strong>think, automate, and evolve.</strong>
        </p>    
    </div>
</section>

<!-- ABOUT -->
<section id="about" class="section" href="#about">
    <h1>About Me</h1>
    <p class="about-text">
        I'm a developer exploring the edge of technology — where <strong>AI, automation, and cybersecurity intersect.</strong><br><br>
        I love creating systems that solve real problems: from web applications to intelligent automation scripts and experimental defense-tech concepts.<br><br>
        Technology shouldn't just exist — it should <strong>react, learn, and protect.</strong>
    </p>

    <div class="about-icons">
        <span>🤖 AI & Machine Learning</span>
        <span>🛡 Ethical Hacking</span>
        <span>⚙ Robotics</span>
        <span>💻 Software Development</span>
    </div>

    <p class="closing-quote">"Learning. Building. Evolving — every day."</p>
</section>


<!-- EDUCATION -->
<section id="education" class="section" href="#education">
    <h1>Education</h1>
    
    <table class="education-table">
        <tr>
            <th>Year</th>
            <th>College / School</th>
            <th>Percentage / CGPA</th>
        </tr>
        <tr>
            <td>2024 - Present</td>
            <td>Saveetha Engineering College</td>
            <td>8.5 CGPA</td>
        </tr>
        <tr>
            <td>2023 - 2024</td>
            <td>Vidhya Sagar Global School</td>
            <td>91%</td>
        </tr>
        <tr>
            <td>2021 - 2022</td>
            <td>Vidhya Sagar Global School</td>
            <td>83%</td>
        </tr>
    </table>
</section>


<!-- SKILLS & PROJECTS -->
<section id="skills-projects" class="section" href="#skills-projects">
    <h1>Skills & Projects</h1>

    <div class="skills-grid">
        <span>🧠 HTML</span>
        <span>🎨 CSS</span>
        <span>⚙️ JavaScript</span>
        <span>📦 Bootstrap</span>
        <span>⚛️ React</span>
        <span>🐍 Python</span>
        <span>🔧 Git</span>
        <span>💻 Linux</span>
    </div>

    <div class="projects">
        <div class="card">
            <h3>Portfolio Website</h3><br>
            <p>A modern responsive portfolio built using HTML & CSS.</p>
        </div>
        <div class="card">
            <h3>Animated AI Extension</h3><br>
            <p>A simple interactive calculator built using JavaScript.</p>
        </div>
          <div class="card">
            <h3>Php & jQuery Profile page</h3><br>
            <p>A simple interactive calculator built using JavaScript.</p>
        </div>  
    </div>
</section>


<!-- CONTACT -->
<section id="contact" class="section" href="#contact">
    <h1>Contact Me</h1><br>
    <p>Email: anisharun@example.com</p>
    <p>LinkedIn: <a href="https://www.linkedin.com/in/arunsamy-d-3bb96132a/">arunsamy-d-3bb96132a</a></p>
</section>


<footer>
    <p>© 2025 Anish — All Rights Reserved</p>
</footer>

</body>
</html>
```

### style.css
``` css
/* ========= GLOBAL ========= */
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: "Poppins", sans-serif;
    background: linear-gradient(#d88888d9, #e7ccaed9, #88aaffd9);
    color: #222;
    scroll-behavior: smooth;
}

/* ========= NAV ========= */
header {
    width: 100%;
    position: fixed;
    top: 0;
    background: #ffffffd9;
    backdrop-filter: blur(10px);
    padding: 15px 50px;
    z-index: 10;
    box-shadow: 0 2px 12px rgba(0,0,0,0.05);
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 22px;
    font-weight: 600;
}

.cyan {
    color: #4c7cff;
    font-weight: bold;
}

nav ul {
    display: flex;
    gap: 25px;
}

nav ul li a {
    text-decoration: none;
    color: #444;
    font-weight: 500;
    transition: .3s;
}

nav ul li a:hover {
    color: #4c7cff;
}


/* ========= SECTION ========= */
.section {
    padding: 100px 10%;
    text-align: center;
}

/* ========= HERO ========= */
.hero {
    height: 100vh;
    width: 100%;
    background: url("profile.jpg") center/cover no-repeat;
    position: relative;
    display: flex;
    align-items: center;
    text-align: left;
    padding-left: 10%;
}

.hero .overlay {
    position: absolute;
    inset: 0;
    background: rgba(0,0,0,0.45);
}

/* Content container */
.intro-content {
    position: relative;
    color: white;
    max-width: 650px;
    padding: 20px;
}

/* LEFT ALIGN UTILITY */
.left-align {
    text-align: left;
}

/* Enlarged text */
.intro-title {
    font-size: 5rem;       /* larger title */
    font-weight: 700;
    line-height: 1.2;
    margin-bottom: 15px;
}

.subtitle {
    font-size: 1.75rem;    /* bigger subtitle */
    opacity: 0.85;
    margin-bottom: 20px;
}

.intro-text {
    font-size: 1.5rem;     /* bigger paragraph */
    opacity: 0.9;
    margin-bottom: 30px;
    line-height: 1.5;
}

.highlight { color: #4c7cff; }

.cta {
    padding: 18px 40px;
    font-size: 1.2rem;
    background: #4c7cff;
    color: white;
    border: none;
    border-radius: 6px;
    font-weight: 600;
    cursor: pointer;
    transition: .3s;
}

.cta:hover {
    transform: scale(1.05);
    box-shadow: 0 0 25px rgba(76,124,255,0.6);
}

/* ========= ABOUT ========= */
.about-text {
    max-width: 650px;
    margin: auto;
    line-height: 1.7;
    font-size: 1.75rem;
}

.about-icons {
    margin-top: 20px;
    font-size: 25px;
    display: flex;
    gap: 15px;
    flex-wrap: wrap;
    justify-content: center;
}

.closing-quote {
    margin-top: 20px;
    opacity: 0.6;
    font-style: italic;
}


/* ========= EDUCATION ========= */
.education-table {
    width: 80%;
    margin: auto;
    margin-top: 20px;
    border-collapse: collapse;
    background: white;
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 0 20px rgba(0,0,0,0.05);
}

.education-table th {
    background: #4c7cff;
    color: white;
    padding: 14px;
}

.education-table td {
    padding: 14px;
    border-bottom: 1px solid #eee;
}

.education-table tr:hover {
    background: #f1f4ff;
}


/* ========= SKILLS ========= */
.skills-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(120px,1fr));
    gap: 15px;
    margin: 30px auto;
    max-width: 650px;
}

.skills-grid span {
    padding: 12px;
    background: white;
    border-radius: 8px;
    font-weight: 500;
    box-shadow: 0 4px 12px rgba(0,0,0,0.05);
    transition: .3s;
}

.skills-grid span:hover {
    transform: translateY(-4px);
    box-shadow: 0 8px 20px rgba(0,0,0,0.1);
}


/* ========= PROJECT CARDS ========= */
.projects {
    display: flex;
    gap: 20px;
    margin-top: 30px;
    flex-wrap: wrap;
    justify-content: center;
}

.card {
    width: 260px;
    background: white;
    padding: 20px;
    border-radius: 10px;
    transition: .3s;
    box-shadow: 0 4px 14px rgba(0,0,0,0.06);
}

.card:hover {
    transform: translateY(-4px);
    box-shadow: 0 8px 25px rgba(0,0,0,0.12);
}


/* ========= FOOTER ========= */
footer {
    padding: 30px;
    background: white;
    margin-top: 50px;
    text-align: center;
    font-size: 14px;
    color: #666;
}
```

## OUTPUT

![alt text](<image2.png>)

![alt text](<image1.png>)

![alt text](<image3.png>)

![alt text](<image.png>)

## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.