<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Gaganajit Singh Kang | Networking | Cloud & DevOps</title>

    <meta name="description"
          content="Gaganajit Singh Kang - B.Voc Hardware & Networking student specializing in Networking, CCNA, Cloud Computing and DevOps.">

    <meta name="keywords"
          content="Gaganajit Singh Kang, Networking, CCNA, Cloud Computing, DevOps, AWS, Linux, Docker, Jenkins">

    <meta name="author" content="Gaganajit Singh Kang">

    <!-- Google Font -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;500;600;700&family=Inter:wght@400;500;600;700;800&display=swap"
          rel="stylesheet">

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: "Inter", sans-serif;
            background: #080b12;
            color: #e6edf3;
            line-height: 1.7;
        }

        ::selection {
            background: #00f7ff;
            color: #080b12;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        /* =========================
           NAVBAR
        ========================= */

        nav {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 1000;
            background: rgba(8, 11, 18, 0.88);
            backdrop-filter: blur(15px);
            border-bottom: 1px solid rgba(255, 255, 255, 0.08);
        }

        .nav-container {
            max-width: 1150px;
            margin: auto;
            padding: 18px 25px;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .logo {
            font-family: "Fira Code", monospace;
            font-size: 20px;
            font-weight: 700;
            color: #00f7ff;
        }

        .logo span {
            color: #ffffff;
        }

        .nav-links {
            display: flex;
            gap: 28px;
            list-style: none;
        }

        .nav-links a {
            color: #aeb8c5;
            font-size: 14px;
            transition: 0.3s;
        }

        .nav-links a:hover {
            color: #00f7ff;
        }

        /* =========================
           HERO
        ========================= */

        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            position: relative;
            overflow: hidden;
            padding: 120px 25px 80px;
        }

        .hero::before {
            content: "";
            position: absolute;
            width: 500px;
            height: 500px;
            background: rgba(0, 247, 255, 0.08);
            filter: blur(100px);
            border-radius: 50%;
            top: 5%;
            left: -150px;
        }

        .hero::after {
            content: "";
            position: absolute;
            width: 450px;
            height: 450px;
            background: rgba(91, 70, 255, 0.08);
            filter: blur(100px);
            border-radius: 50%;
            bottom: -150px;
            right: -100px;
        }

        .hero-container {
            max-width: 1150px;
            width: 100%;
            margin: auto;
            position: relative;
            z-index: 2;
        }

        .terminal-line {
            color: #00f7ff;
            font-family: "Fira Code", monospace;
            margin-bottom: 18px;
            font-size: 15px;
        }

        .hero h1 {
            font-size: clamp(42px, 7vw, 78px);
            line-height: 1.1;
            margin-bottom: 20px;
            font-weight: 800;
        }

        .hero h1 span {
            color: #00f7ff;
        }

        .hero h2 {
            font-family: "Fira Code", monospace;
            font-size: clamp(18px, 3vw, 27px);
            color: #aeb8c5;
            margin-bottom: 25px;
            font-weight: 500;
        }

        .hero p {
            max-width: 760px;
            color: #9ba7b5;
            font-size: 17px;
            margin-bottom: 35px;
        }

        .hero-buttons {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
        }

        .btn {
            padding: 13px 23px;
            border-radius: 8px;
            font-weight: 600;
            font-size: 14px;
            transition: 0.3s;
            border: 1px solid #00f7ff;
        }

        .btn-primary {
            background: #00f7ff;
            color: #080b12;
        }

        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 30px rgba(0, 247, 255, 0.2);
        }

        .btn-secondary {
            color: #00f7ff;
        }

        .btn-secondary:hover {
            background: rgba(0, 247, 255, 0.08);
            transform: translateY(-3px);
        }

        /* =========================
           GENERAL
        ========================= */

        section {
            padding: 100px 25px;
        }

        .container {
            max-width: 1150px;
            margin: auto;
        }

        .section-title {
            margin-bottom: 50px;
        }

        .section-title small {
            font-family: "Fira Code", monospace;
            color: #00f7ff;
            font-size: 14px;
        }

        .section-title h2 {
            font-size: 38px;
            margin-top: 8px;
        }

        .section-title p {
            color: #8d99a7;
            max-width: 700px;
            margin-top: 10px;
        }

        /* =========================
           ABOUT
        ========================= */

        .about-grid {
            display: grid;
            grid-template-columns: 1.5fr 1fr;
            gap: 35px;
        }

        .about-card {
            background: #0d1119;
            border: 1px solid #1d2633;
            padding: 30px;
            border-radius: 14px;
        }

        .about-card p {
            color: #aeb8c5;
            margin-bottom: 15px;
        }

        .education-item {
            padding: 15px 0;
            border-bottom: 1px solid #1d2633;
        }

        .education-item:last-child {
            border-bottom: none;
        }

        .education-item h3 {
            font-size: 16px;
            color: #ffffff;
        }

        .education-item p {
            margin: 3px 0;
            color: #8d99a7;
            font-size: 14px;
        }

        .education-item span {
            color: #00f7ff;
            font-family: "Fira Code", monospace;
            font-size: 12px;
        }

        /* =========================
           SKILLS
        ========================= */

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }

        .skill-card {
            background: #0d1119;
            border: 1px solid #1d2633;
            border-radius: 14px;
            padding: 25px;
            transition: 0.3s;
        }

        .skill-card:hover {
            transform: translateY(-6px);
            border-color: #00f7ff;
            box-shadow: 0 10px 35px rgba(0, 247, 255, 0.07);
        }

        .skill-icon {
            font-size: 30px;
            margin-bottom: 12px;
        }

        .skill-card h3 {
            margin-bottom: 15px;
            font-size: 18px;
        }

        .skill-list {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }

        .skill-list span {
            padding: 5px 10px;
            background: #151c27;
            border: 1px solid #273242;
            border-radius: 5px;
            font-family: "Fira Code", monospace;
            font-size: 12px;
            color: #b8c2cf;
        }

        /* =========================
           TRAINING
        ========================= */

        .timeline {
            position: relative;
            max-width: 850px;
        }

        .timeline::before {
            content: "";
            position: absolute;
            left: 9px;
            top: 0;
            bottom: 0;
            width: 2px;
            background: #1e2b39;
        }

        .timeline-item {
            position: relative;
            padding-left: 45px;
            margin-bottom: 40px;
        }

        .timeline-dot {
            position: absolute;
            left: 0;
            top: 5px;
            width: 20px;
            height: 20px;
            border-radius: 50%;
            background: #00f7ff;
            box-shadow: 0 0 15px rgba(0, 247, 255, 0.5);
        }

        .timeline-item h3 {
            font-size: 20px;
            margin-bottom: 5px;
        }

        .timeline-item .date {
            color: #00f7ff;
            font-family: "Fira Code", monospace;
            font-size: 13px;
        }

        .timeline-item p {
            color: #8f9ba8;
            margin-top: 8px;
        }

        /* =========================
           PROJECTS
        ========================= */

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 22px;
        }

        .project-card {
            background: #0d1119;
            border: 1px solid #1d2633;
            border-radius: 14px;
            padding: 28px;
            transition: 0.3s;
            display: flex;
            flex-direction: column;
        }

        .project-card:hover {
            transform: translateY(-7px);
            border-color: #00f7ff;
        }

        .project-number {
            color: #00f7ff;
            font-family: "Fira Code", monospace;
            font-size: 13px;
            margin-bottom: 15px;
        }

        .project-card h3 {
            font-size: 20px;
            margin-bottom: 12px;
        }

        .project-card p {
            color: #8f9ba8;
            font-size: 14px;
            margin-bottom: 20px;
            flex: 1;
        }

        .project-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 7px;
        }

        .project-tags span {
            font-size: 11px;
            color: #00f7ff;
            border: 1px solid #1c6670;
            padding: 4px 8px;
            border-radius: 4px;
        }

        /* =========================
           GITHUB
        ========================= */

        .github-box {
            background: linear-gradient(
                135deg,
                #0d1119,
                #101722
            );
            border: 1px solid #1d2633;
            border-radius: 16px;
            padding: 45px;
            text-align: center;
        }

        .github-box h3 {
            font-size: 27px;
            margin-bottom: 10px;
        }

        .github-box p {
            color: #8f9ba8;
            margin-bottom: 25px;
        }

        .github-stats {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 15px;
            margin-top: 30px;
        }

        .stat {
            padding: 20px;
            background: #080b12;
            border: 1px solid #1d2633;
            border-radius: 10px;
        }

        .stat strong {
            display: block;
            font-size: 25px;
            color: #00f7ff;
        }

        .stat span {
            color: #8f9ba8;
            font-size: 13px;
        }

        /* =========================
           CONTACT
        ========================= */

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }

        .contact-card {
            background: #0d1119;
            border: 1px solid #1d2633;
            padding: 25px;
            border-radius: 12px;
            text-align: center;
            transition: 0.3s;
        }

        .contact-card:hover {
            border-color: #00f7ff;
            transform: translateY(-5px);
        }

        .contact-card .icon {
            font-size: 28px;
            margin-bottom: 10px;
        }

        .contact-card h3 {
            font-size: 16px;
            margin-bottom: 5px;
        }

        .contact-card p {
            color: #00f7ff;
            font-size: 13px;
            word-break: break-word;
        }

        /* =========================
           FOOTER
        ========================= */

        footer {
            border-top: 1px solid #1d2633;
            padding: 35px 25px;
            text-align: center;
            color: #697586;
            font-size: 13px;
        }

        footer span {
            color: #00f7ff;
        }

        /* =========================
           RESPONSIVE
        ========================= */

        @media (max-width: 900px) {

            .skills-grid,
            .projects-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .about-grid {
                grid-template-columns: 1fr;
            }

            .contact-grid {
                grid-template-columns: 1fr 1fr;
            }
        }

        @media (max-width: 650px) {

            .nav-links {
                display: none;
            }

            .hero {
                padding-top: 130px;
            }

            .hero h1 {
                font-size: 43px;
            }

            .skills-grid,
            .projects-grid,
            .contact-grid,
            .github-stats {
                grid-template-columns: 1fr;
            }

            section {
                padding: 75px 20px;
            }

            .github-box {
                padding: 30px 20px;
            }
        }
    </style>
</head>

<body>

<!-- =========================
     NAVIGATION
========================= -->

<nav>
    <div class="nav-container">

        <a href="#home" class="logo">
            GSK<span>_</span>
        </a>

        <ul class="nav-links">
            <li><a href="#about">About</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#training">Training</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#github">GitHub</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>

    </div>
</nav>


<!-- =========================
     HERO
========================= -->

<section class="hero" id="home">

    <div class="hero-container">

        <div class="terminal-line">
            &gt; Hello World! I'm
        </div>

        <h1>
            Gaganajit Singh<br>
            <span>Kang.</span>
        </h1>

        <h2>
            Networking Student | Cloud & DevOps Enthusiast
        </h2>

        <p>
            B.Voc Hardware & Networking student with practical training
            in Networking, Advanced Networking and CCNA. Currently
            developing professional skills in Cloud Computing and DevOps,
            with a strong interest in infrastructure, automation and
            modern IT technologies.
        </p>

        <div class="hero-buttons">

            <a href="https://github.com/" target="_blank"
               class="btn btn-primary">
                View GitHub
            </a>

            <a href="#contact"
               class="btn btn-secondary">
                Connect With Me
            </a>

        </div>

    </div>

</section>


<!-- =========================
     ABOUT
========================= -->

<section id="about">

    <div class="container">

        <div class="section-title">

            <small>01 / ABOUT ME</small>

            <h2>Who I Am</h2>

            <p>
                Building my foundation in networking while moving toward
                Cloud Computing and DevOps.
            </p>

        </div>


        <div class="about-grid">

            <div class="about-card">

                <p>
                    I am <strong>Gaganajit Singh Kang</strong>, currently
                    pursuing B.Voc in Hardware & Networking from
                    <strong>SD College, Chandigarh Sector 32</strong>.
                </p>

                <p>
                    My technical journey started with networking, where I
                    completed two summer training programs focused on
                    Networking and Advanced Networking with CCNA.
                </p>

                <p>
                    I am currently pursuing a
                    <strong>Cloud + DevOps</strong> program at
                    <strong>TechCadd, Mohali</strong>, where I am expanding
                    my knowledge of cloud infrastructure, Linux,
                    automation, containers and DevOps practices.
                </p>

                <p>
                    My goal is to combine my networking foundation with
                    cloud and DevOps technologies to build, manage and
                    automate reliable IT infrastructure.
                </p>

            </div>


            <div class="about-card">

                <div class="education-item">

                    <span>EDUCATION</span>

                    <h3>B.Voc Hardware & Networking</h3>

                    <p>
                        SD College, Chandigarh Sector 32
                    </p>

                </div>


                <div class="education-item">

                    <span>TRAINING</span>

                    <h3>Networking & Advanced Networking</h3>

                    <p>
                        Summer Training • CCNA
                    </p>

                </div>


                <div class="education-item">

                    <span>CURRENTLY LEARNING</span>

                    <h3>Cloud + DevOps</h3>

                    <p>
                        TechCadd, Mohali
                    </p>

                </div>

            </div>

        </div>

    </div>

</section>


<!-- =========================
     SKILLS
========================= -->

<section id="skills">

    <div class="container">

        <div class="section-title">

            <small>02 / SKILLS</small>

            <h2>Technical Skills</h2>

            <p>
                Technologies and concepts I am learning and working with.
            </p>

        </div>


        <div class="skills-grid">

            <!-- Networking -->

            <div class="skill-card">

                <div class="skill-icon">🌐</div>

                <h3>Networking</h3>

                <div class="skill-list">

                    <span>CCNA</span>
                    <span>TCP/IP</span>
                    <span>OSI Model</span>
                    <span>Subnetting</span>
                    <span>Routing</span>
                    <span>Switching</span>
                    <span>LAN/WAN</span>
                    <span>DNS</span>

                </div>

            </div>


            <!-- Cloud -->

            <div class="skill-card">

                <div class="skill-icon">☁️</div>

                <h3>Cloud & DevOps</h3>

                <div class="skill-list">

                    <span>Cloud Computing</span>
                    <span>AWS</span>
                    <span>Linux</span>
                    <span>Docker</span>
                    <span>Git</span>
                    <span>GitHub</span>
                    <span>CI/CD</span>
                    <span>Jenkins</span>

                </div>

            </div>


            <!-- Tools -->

            <div class="skill-card">

                <div class="skill-icon">⚙️</div>

                <h3>Tools & Technologies</h3>

                <div class="skill-list">

                    <span>Ubuntu</span>
                    <span>Windows</span>
                    <span>VS Code</span>
                    <span>Git</span>
                    <span>GitHub</span>
                    <span>Docker</span>
                    <span>Linux CLI</span>

                </div>

            </div>


            <!-- Infrastructure -->

            <div class="skill-card">

                <div class="skill-icon">🖥️</div>

                <h3>Infrastructure</h3>

                <div class="skill-list">

                    <span>Servers</span>
                    <span>Networking</span>
                    <span>Cloud Infrastructure</span>
                    <span>System Administration</span>
                    <span>Deployment</span>

                </div>

            </div>


            <!-- Programming -->

            <div class="skill-card">

                <div class="skill-icon">💻</div>

                <h3>Programming & Scripting</h3>

                <div class="skill-list">

                    <span>HTML</span>
                    <span>CSS</span>
                    <span>Bash</span>
                    <span>Python</span>

                </div>

            </div>


            <!-- Learning -->

            <div class="skill-card">

                <div class="skill-icon">🚀</div>

                <h3>Currently Learning</h3>

                <div class="skill-list">

                    <span>AWS</span>
                    <span>Docker</span>
                    <span>Jenkins</span>
                    <span>CI/CD</span>
                    <span>Cloud</span>
                    <span>DevOps</span>

                </div>

            </div>

        </div>

    </div>

</section>


<!-- =========================
     TRAINING
========================= -->

<section id="training">

    <div class="container">

        <div class="section-title">

            <small>03 / TRAINING</small>

            <h2>My Learning Journey</h2>

            <p>
                Practical training and technical development.
            </p>

        </div>


        <div class="timeline">

            <div class="timeline-item">

                <div class="timeline-dot"></div>

                <span class="date">
                    SUMMER TRAINING
                </span>

                <h3>Networking Training</h3>

                <p>
                    Completed summer training focused on networking
                    fundamentals, network concepts, devices and
                    communication technologies.
                </p>

            </div>


            <div class="timeline-item">

                <div class="timeline-dot"></div>

                <span class="date">
                    SUMMER TRAINING
                </span>

                <h3>Advanced Networking & CCNA</h3>

                <p>
                    Completed advanced networking training with a focus
                    on CCNA concepts, routing, switching, IP addressing
                    and network infrastructure.
                </p>

            </div>


            <div class="timeline-item">

                <div class="timeline-dot"></div>

                <span class="date">
                    CURRENTLY PURSUING
                </span>

                <h3>Cloud + DevOps</h3>

                <p>
                    Currently pursuing Cloud + DevOps training at
                    TechCadd, Mohali, developing practical knowledge
                    of cloud infrastructure, Linux, containers,
                    automation and CI/CD.
                </p>

            </div>

        </div>

    </div>

</section>


<!-- =========================
     PROJECTS
========================= -->

<section id="projects">

    <div class="container">

        <div class="section-title">

            <small>04 / PROJECTS</small>

            <h2>Projects & Practice</h2>

            <p>
                A growing collection of networking, cloud and DevOps
                projects.
            </p>

        </div>


        <div class="projects-grid">


            <div class="project-card">

                <div class="project-number">
                    PROJECT_01
                </div>

                <h3>Networking Lab</h3>

                <p>
                    Practical networking exercises covering IP
                    addressing, subnetting, routing, switching and
                    network troubleshooting.
                </p>

                <div class="project-tags">

                    <span>CCNA</span>
                    <span>Networking</span>
                    <span>TCP/IP</span>

                </div>

            </div>


            <div class="project-card">

                <div class="project-number">
                    PROJECT_02
                </div>

                <h3>Cloud Infrastructure</h3>

                <p>
                    Learning and practicing cloud infrastructure
                    concepts with AWS, Linux systems and cloud-based
                    deployment workflows.
                </p>

                <div class="project-tags">

                    <span>AWS</span>
                    <span>Linux</span>
                    <span>Cloud</span>

                </div>

            </div>


            <div class="project-card">

                <div class="project-number">
                    PROJECT_03
                </div>

                <h3>Docker Application</h3>

                <p>
                    Practicing application containerization using
                    Docker and learning container lifecycle,
                    networking and deployment concepts.
                </p>

                <div class="project-tags">

                    <span>Docker</span>
                    <span>Linux</span>
                    <span>DevOps</span>

                </div>

            </div>


            <div class="project-card">

                <div class="project-number">
                    PROJECT_04
                </div>

                <h3>CI/CD Pipeline</h3>

                <p>
                    Learning to create automated build and deployment
                    workflows using GitHub and Jenkins.
                </p>

                <div class="project-tags">

                    <span>Jenkins</span>
                    <span>GitHub</span>
                    <span>CI/CD</span>

                </div>

            </div>


            <div class="project-card">

                <div class="project-number">
                    PROJECT_05
                </div>

                <h3>Linux Administration</h3>

                <p>
                    Hands-on practice with Linux commands, users,
                    permissions, processes, services and system
                    administration.
                </p>

                <div class="project-tags">

                    <span>Linux</span>
                    <span>Bash</span>
                    <span>Server</span>

                </div>

            </div>


            <div class="project-card">

                <div class="project-number">
                    PROJECT_06
                </div>

                <h3>DevOps Learning Lab</h3>

                <p>
                    A continuous learning environment for practicing
                    Git, Docker, Jenkins, cloud infrastructure and
                    deployment automation.
                </p>

                <div class="project-tags">

                    <span>DevOps</span>
                    <span>Docker</span>
                    <span>AWS</span>
                    <span>Jenkins</span>

                </div>

            </div>

        </div>

    </div>

</section>


<!-- =========================
     GITHUB
========================= -->

<section id="github">

    <div class="container">

        <div class="section-title">

            <small>05 / GITHUB</small>

            <h2>Open Source & GitHub</h2>

            <p>
                Explore my projects, experiments and learning journey.
            </p>

        </div>


        <div class="github-box">

            <h3>Building. Learning. Deploying. 🚀</h3>

            <p>
                I use GitHub to document my technical journey,
                practice projects and continuously improve my
                networking, cloud and DevOps skills.
            </p>

            <a href="https://github.com/"
               target="_blank"
               class="btn btn-primary">
                Visit My GitHub
            </a>


            <div class="github-stats">

                <div class="stat">

                    <strong>Networking</strong>

                    <span>
                        Core Foundation
                    </span>

                </div>


                <div class="stat">

                    <strong>Cloud</strong>

                    <span>
                        Currently Learning
                    </span>

                </div>


                <div class="stat">

                    <strong>DevOps</strong>

                    <span>
                        Currently Learning
                    </span>

                </div>

            </div>

        </div>

    </div>

</section>


<!-- =========================
     CONTACT
========================= -->

<section id="contact">

    <div class="container">

        <div class="section-title">

            <small>06 / CONTACT</small>

            <h2>Let's Connect</h2>

            <p>
                Interested in networking, cloud infrastructure and
                DevOps opportunities.
            </p>

        </div>


        <div class="contact-grid">


            <a href="https://github.com/"
               target="_blank"
               class="contact-card">

                <div class="icon">🐙</div>

                <h3>GitHub</h3>

                <p>
                    github.com/yourusername
                </p>

            </a>


            <a href="#"
               class="contact-card">

                <div class="icon">💼</div>

                <h3>LinkedIn</h3>

                <p>
                    Add LinkedIn Profile
                </p>

            </a>


            <a href="mailto:your-email@example.com"
               class="contact-card">

                <div class="icon">📧</div>

                <h3>Email</h3>

                <p>
                    your-email@example.com
                </p>

            </a>

        </div>

    </div>

</section>


<!-- =========================
     FOOTER
========================= -->

<footer>

    <p>
        © 2026 <span>Gaganajit Singh Kang</span>.
        Built with HTML & CSS.
    </p>

    <p>
        Networking • Cloud • DevOps • Continuous Learning
    </p>

</footer>


</body>
</html>
