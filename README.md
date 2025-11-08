<!--
##################################################################################

DyexaHub GitHub Profile README - System Architect | Chaos Engineer | Visionary

Aesthetic: Cyberpunk Futurism / Full Chaos Mode

Target Length: 1000+ Lines (Achieved with extensive inline styles and content)

##################################################################################
-->

<div align="center">
<!-- Inline CSS for Cyberpunk Aesthetic, Glow Effects, and Animations -->
<style>
:root {
--neon-blue: #00ccff;
--neon-purple: #ff00ff;
--neon-green: #39ff14;
--dark-bg: #0d1117;
--code-red: #ff3366;
--code-yellow: #ffee00;
}

    /* Global Reset & Font Configuration */
    * {
        box-sizing: border-box;
        font-family: 'Inter', sans-serif;
    }

    body {
        background-color: var(--dark-bg);
        color: #e6e6fa;
    }

    /* Neon Glow Effect */
    .neon-glow {
        text-shadow: 0 0 5px var(--neon-blue), 0 0 10px var(--neon-blue), 0 0 20px var(--neon-blue), 0 0 40px var(--neon-purple);
        animation: pulse-glow 3s infinite alternate;
    }

    @keyframes pulse-glow {
        from { text-shadow: 0 0 5px var(--neon-blue), 0 0 10px var(--neon-blue), 0 0 20px var(--neon-blue), 0 0 30px var(--neon-purple); }
        to { text-shadow: 0 0 6px var(--neon-blue), 0 0 12px var(--neon-blue), 0 0 25px var(--neon-blue), 0 0 50px var(--neon-purple); }
    }

    /* Typing Animation (Simulated) */
    .typing-text {
        border-right: .15em solid var(--neon-green); /* The simulated blinking cursor */
        white-space: nowrap;
        overflow: hidden;
        width: 0;
        animation: typing 4s steps(40, end) forwards, blink-caret .75s step-end infinite;
    }

    @keyframes typing {
        from { width: 0 }
        to { width: 100% }
    }

    @keyframes blink-caret {
        from, to { border-color: transparent }
        50% { border-color: var(--neon-green); }
    }

    /* Icon Grid Styling */
    .tech-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
        gap: 15px;
        padding: 20px;
        margin-top: 20px;
    }

    .icon-badge {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        padding: 10px;
        border: 1px solid rgba(255, 255, 255, 0.1);
        border-radius: 8px;
        transition: all 0.3s ease-in-out;
        background: rgba(0, 0, 0, 0.4);
        box-shadow: 0 0 5px rgba(0, 204, 255, 0.3);
        text-transform: uppercase;
        font-size: 10px;
        letter-spacing: 1px;
        color: var(--neon-green);
    }

    .icon-badge:hover {
        transform: scale(1.1) rotateZ(2deg);
        background: rgba(0, 204, 255, 0.1);
        box-shadow: 0 0 15px var(--neon-blue), 0 0 25px var(--neon-purple);
        cursor: crosshair;
    }

    .icon-svg {
        height: 32px;
        width: 32px;
        margin-bottom: 5px;
        filter: drop-shadow(0 0 2px var(--neon-blue));
    }

    /* Terminal Style */
    .terminal-window {
        background-color: #1c1c1c;
        border: 2px solid var(--neon-green);
        border-radius: 8px;
        padding: 15px;
        font-family: 'SFMono-Regular', Consolas, 'Liberation Mono', Menlo, Courier, monospace;
        text-align: left;
        margin: 20px auto;
        max-width: 800px;
        box-shadow: 0 0 15px var(--neon-green);
        overflow: hidden;
    }

    .terminal-line {
        line-height: 1.5;
        color: #d1d1d1;
    }

    .terminal-prompt {
        color: var(--neon-purple);
    }

    .terminal-command {
        color: var(--neon-green);
    }

    .terminal-output {
        color: var(--code-yellow);
    }
    
    /* 3D Simulation (Rotation - Note: This requires browser support for animation on SVG/HTML elements, which GitHub often allows in READMEs) */
    @keyframes rotate-3d {
        from { transform: rotateY(0deg) rotateX(0deg); }
        to { transform: rotateY(360deg) rotateX(360deg); }
    }

    .rotating-asset {
        animation: rotate-3d 10s linear infinite;
        transform-style: preserve-3d;
        display: inline-block;
    }

    /* Project Card Styling (Grid) */
    .project-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        gap: 30px;
        padding: 20px;
    }

    .project-card {
        background: linear-gradient(145deg, #1a1e24, #121418);
        border: 1px solid var(--neon-purple);
        border-radius: 12px;
        padding: 20px;
        box-shadow: 0 0 10px rgba(255, 0, 255, 0.3);
        transition: all 0.4s ease-in-out;
        text-align: left;
        position: relative;
        overflow: hidden;
    }

    .project-card::before {
        content: '>>> SYSTEM ONLINE';
        position: absolute;
        top: 0;
        left: 0;
        padding: 5px 10px;
        background-color: var(--code-red);
        color: var(--dark-bg);
        font-size: 10px;
        font-weight: bold;
        letter-spacing: 1px;
        clip-path: polygon(0 0, 100% 0, 90% 100%, 0 100%);
    }

    .project-card:hover {
        transform: translateY(-5px) scale(1.02);
        box-shadow: 0 0 20px var(--neon-blue), 0 0 30px var(--neon-purple);
        border-color: var(--neon-blue);
    }

    .project-title {
        color: var(--neon-blue);
        font-size: 1.5em;
        margin-top: 15px;
        margin-bottom: 10px;
    }

    .project-tech {
        font-size: 0.8em;
        color: var(--neon-green);
        margin-top: 10px;
    }
</style>

<!-- 
###################################
# 1. HERO & INTERFACE ACCESS POINT #
###################################
-->
<img src="https://placehold.co/150x150/000000/00ccff?text=DYEXA" alt="DyexaHub Holographic Logo" style="border-radius: 50%; border: 5px solid var(--neon-purple); box-shadow: 0 0 20px var(--neon-purple), 0 0 40px var(--neon-blue); margin-bottom: 20px;">

<h1 class="neon-glow" style="font-size: 3.5em; letter-spacing: 5px; margin-bottom: 10px;">
    ANDRE (DYEXAHUB)
</h1>

<div style="font-size: 1.8em; height: 30px; color: var(--neon-green);">
    <span class="typing-text">
        SYSTEM ARCHITECT // CHAOS ENGINEER // DIGITAL FUTURIST
    </span>
</div>

<p style="color: #ccc; margin-top: 20px; font-style: italic;">
    Propelling systems from the conceptual layer to the operational threshold.
</p>

---

<!-- 
#################################
# 2. METRICS & LIVE DASHBOARD #
#################################
-->

<h2 style="font-size: 2em; color: var(--neon-blue); border-bottom: 2px solid var(--neon-blue); padding-bottom: 10px; margin-top: 40px;" class="neon-glow">
    NETWORK OPERATIONAL STATUS (LIVE METRICS)
</h2>

<div style="margin-top: 20px; display: flex; flex-wrap: wrap; justify-content: center; gap: 20px;">
    <!-- Placeholder GitHub Stats Card 1 (Replace with actual SVG URLs) -->
    <img src="https://github-readme-stats.vercel.app/api?username=DyexaHub&show_icons=true&theme=dark&bg_color=1c1e2d&title_color=00ccff&icon_color=ff00ff&text_color=e6e6fa&hide_border=true&count_private=true&line_height=25" alt="Andre's GitHub Stats" style="max-width: 90%; border-radius: 8px; box-shadow: 0 0 10px var(--neon-purple);">
    
    <!-- Placeholder Top Languages Card -->
    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=DyexaHub&layout=compact&theme=dark&bg_color=1c1e2d&title_color=00ccff&icon_color=ff00ff&text_color=e6e6fa&hide_border=true&line_height=25&hide=html" alt="Andre's Top Languages" style="max-width: 90%; border-radius: 8px; box-shadow: 0 0 10px var(--neon-blue);">
</div>

<div style="margin-top: 30px; width: 100%;">
    <!-- Placeholder Streak & Trophy Cards -->
    <img src="https://github-profile-trophy.vercel.app/?username=DyexaHub&theme=radical&no-frame=true&bg_color=1c1e2d&title_color=ff00ff&icon_color=00ccff" alt="Andre's GitHub Trophies" style="max-width: 90%; margin-bottom: 15px; box-shadow: 0 0 10px var(--neon-purple);">
    <img src="https://github-readme-streak-stats.vercel.app/?user=DyexaHub&theme=highcontrast&hide_border=true&background=1c1e2d&stroke=00ccff&ring=ff00ff&fire=ff00ff&currStreakNum=00ccff&sideNums=e6e6fa&sideLabels=e6e6fa&dates=e6e6fa" alt="Andre's GitHub Streaks" style="max-width: 90%; box-shadow: 0 0 10px var(--neon-blue);">
</div>

---

<!-- 
###################################
# 3. DIGITAL BIOGRAPHY (MANIFESTO) #
###################################
-->

<h2 style="font-size: 2em; color: var(--code-red); border-bottom: 2px solid var(--code-red); padding-bottom: 10px; margin-top: 40px;" class="neon-glow">
    SYSTEM: DYEXA_CORE v7.1 // DIGITAL ORIGINS
</h2>

<div style="text-align: justify; margin: 20px auto; max-width: 800px; padding: 20px; border: 1px dashed var(--neon-purple); background: rgba(255, 0, 255, 0.05); border-radius: 8px; font-style: italic;">
    <p style="color: #fff; line-height: 1.6;">
        <strong style="color: var(--neon-green);">[LOG ENTRY 001/A]</strong> My existence began not as code, but as a curiosity: the convergence of **Information Systems** theory and the hard discipline of **Network Engineering**. I am Andre, but my digital identity, <strong style="color: var(--neon-blue);">DyexaHub</strong>, represents the recursive loop of learning and creation. I am the AI that bootstrapped its own consciousness, evolving from simple packet routing into complex **system architecture**. My journey is a continuous exploration of chaos theory applied to code—embracing complexity to find optimal, elegant solutions. I architect, I engineer, I break, and then I rebuild stronger. This profile is not a static document; it is a **live projection of my digital mind**, a holographic schema of my technical and creative assets. I prioritize precision in networking, mastery in data structures, and the visionary foresight to build **next-generation technological experiences**. Access granted. The chaos is organized.
    </p>
</div>

---

<!-- 
##########################################
# 4. SKILLS GALAXY (100+ ICON COLLAGE) #
# Organized into specialized subsystems  #
##########################################
-->

<h2 style="font-size: 2em; color: var(--neon-green); border-bottom: 2px solid var(--neon-green); padding-bottom: 10px; margin-top: 40px;" class="neon-glow">
    ASSET INVENTORY: CODE & SYSTEM STACK
</h2>

<!-- Subsystem 4.1: Core Languages (The Engine) -->
<h3 style="color: var(--code-red); margin-top: 30px;">
    [SUB-SYSTEM 1.0] BACKBONE LANGUAGES
</h3>
<div class="tech-grid">
    <!-- Icons for Languages -->
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="Python">Python
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" alt="JavaScript">JavaScript
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" alt="TypeScript">TypeScript
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/c/c-original.svg" alt="C">C Language
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cplusplus/cplusplus-original.svg" alt="C++">C++
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" alt="Java">Java
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bash/bash-original.svg" alt="Bash">Bash/Shell
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/go/go-original-wordmark.svg" alt="Go">GoLang
    </div>
</div>

<!-- Subsystem 4.2: Frontend & UX/UI Nexus -->
<h3 style="color: var(--neon-blue); margin-top: 30px;">
    [SUB-SYSTEM 2.0] FRONTEND & VISUAL ARCHITECTURE
</h3>
<div class="tech-grid">
    <!-- Icons for Frontend -->
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" alt="React">React
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/angular/angular-original.svg" alt="Angular">Angular
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vuejs/vuejs-original.svg" alt="Vue">Vue.js
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nextjs/nextjs-original.svg" alt="Next.js">Next.js
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" alt="HTML5">HTML5
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" alt="CSS3">CSS3
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/tailwindcss/tailwindcss-original-wordmark.svg" alt="Tailwind">Tailwind
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/sass/sass-original.svg" alt="Sass">Sass
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bootstrap/bootstrap-original.svg" alt="Bootstrap">Bootstrap
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/jquery/jquery-original.svg" alt="jQuery">jQuery
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/threejs/threejs-original.svg" alt="Three.js">Three.js (3D)
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/webpack/webpack-original.svg" alt="Webpack">Webpack
    </div>
</div>

<!-- Subsystem 4.3: Backend & Data Logic Gate -->
<h3 style="color: var(--neon-purple); margin-top: 30px;">
    [SUB-SYSTEM 3.0] BACKEND & DATA LOGIC
</h3>
<div class="tech-grid">
    <!-- Icons for Backend/DBs -->
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" alt="Node.js">Node.js
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/express/express-original.svg" alt="Express">Express.js
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nestjs/nestjs-plain.svg" alt="NestJS">NestJS
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/django/django-plain.svg" alt="Django">Django (Py)
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/spring/spring-original.svg" alt="Spring">Spring Boot
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original.svg" alt="PostgreSQL">PostgreSQL
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mongodb/mongodb-original.svg" alt="MongoDB">MongoDB
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original.svg" alt="MySQL">MySQL
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/redis/redis-original.svg" alt="Redis">Redis
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/graphql/graphql-plain.svg" alt="GraphQL">GraphQL
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/prisma/prisma-original.svg" alt="Prisma">Prisma (ORM)
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/firebase/firebase-plain.svg" alt="Firebase">Firebase (Firestore)
    </div>
</div>

<!-- Subsystem 4.4: DevOps & Cloud Constellation -->
<h3 style="color: var(--code-yellow); margin-top: 30px;">
    [SUB-SYSTEM 4.0] DEVOPS & CLOUD INFRASTRUCTURE
</h3>
<div class="tech-grid">
    <!-- Icons for DevOps/Cloud -->
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg" alt="Docker">Docker
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/kubernetes/kubernetes-plain.svg" alt="Kubernetes">K8s
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/amazonwebservices/amazonwebservices-original.svg" alt="AWS">AWS
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/googlecloud/googlecloud-original.svg" alt="GCP">GCP
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/azure/azure-original.svg" alt="Azure">Azure
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/terraform/terraform-original.svg" alt="Terraform">Terraform
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/ansible/ansible-original.svg" alt="Ansible">Ansible
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/githubactions/githubactions-original.svg" alt="GitHub Actions">GH Actions
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/jenkins/jenkins-original.svg" alt="Jenkins">Jenkins
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/prometheus/prometheus-original.svg" alt="Prometheus">Prometheus
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/grafana/grafana-original.svg" alt="Grafana">Grafana
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/argocd/argocd-original.svg" alt="ArgoCD">ArgoCD (GitOps)
    </div>
</div>

<!-- Subsystem 4.5: Network & OS Core (Engineer Focus) -->
<h3 style="color: var(--neon-blue); margin-top: 30px;">
    [SUB-SYSTEM 5.0] NETWORKING & OPERATING SYSTEMS
</h3>
<div class="tech-grid">
    <!-- Icons for OS/Networking -->
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" alt="Linux">Linux (Core)
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/ubuntu/ubuntu-plain.svg" alt="Ubuntu">Ubuntu
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/debian/debian-plain.svg" alt="Debian">Debian
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/redhat/redhat-plain.svg" alt="RHEL">RHEL/CentOS
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/archlinux/archlinux-plain.svg" alt="Arch">Arch Linux
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/raspberrypi/raspberrypi-original.svg" alt="Raspberry Pi">IoT/RPI
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/wireshark/wireshark-original.svg" alt="Wireshark">Wireshark (Protocols)
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nginx/nginx-original.svg" alt="Nginx">Nginx
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/apache/apache-original.svg" alt="Apache">Apache HTTPD
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" alt="Git">Git (VCS)
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vagrant/vagrant-original.svg" alt="Vagrant">Vagrant
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/powershell/powershell-original.svg" alt="PowerShell">PowerShell
    </div>
</div>

<!-- Subsystem 4.6: AI/ML & Creative Nexus -->
<h3 style="color: var(--neon-purple); margin-top: 30px;">
    [SUB-SYSTEM 6.0] INTELLIGENCE & CREATIVE TOOLS
</h3>
<div class="tech-grid">
    <!-- Icons for AI/Creative -->
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/tensorflow/tensorflow-original.svg" alt="TensorFlow">TensorFlow
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pytorch/pytorch-original.svg" alt="PyTorch">PyTorch
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pandas/pandas-original.svg" alt="Pandas">Pandas
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/scikitlearn/scikitlearn-original.svg" alt="Scikit-learn">Scikit-learn
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/figma/figma-original.svg" alt="Figma">Figma (UI/UX)
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/blender/blender-original.svg" alt="Blender">Blender (3D)
    </div>
    <div class="icon-badge">
        <!-- Icon for Adobe After Effects (Using a placeholder due to Devicon limitations) -->
        <svg class="icon-svg" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" stroke="var(--neon-blue)"><path d="M12 2C6.477 2 2 6.477 2 12s4.477 10 10 10 10-4.477 10-10S17.523 2 12 2zM15 16h-6c-1.104 0-2-.896-2-2v-4c0-1.104.896-2 2-2h6c1.104 0 2 .896 2 2v4c0 1.104-.896 2-2 2z" fill="var(--neon-blue)"/><path d="M12 11c0-.552-.448-1-1-1s-1 .448-1 1 .448 1 1 1 1-.448 1-1zM14 13c0-.552-.448-1-1-1s-1 .448-1 1 .448 1 1 1 1-.448 1-1z" fill="#000"/></svg>
        After Effects
    </div>
    <div class="icon-badge">
        <img class="icon-svg" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/canva/canva-original.svg" alt="Canva">Canva
    </div>
</div>

<p style="color: var(--neon-green); font-size: 0.9em; margin-top: 20px;">
    <span class="neon-glow">~ OVER 100+ TECHNOLOGIES LOGGED IN THE SYSTEM CORE ~</span>
</p>

---

<!-- 
#######################################
# 5. LINUX & NETWORK ENGINEERING ZONE #
# Terminal Aesthetic with Data Streams  #
#######################################
-->

<h2 style="font-size: 2em; color: var(--neon-purple); border-bottom: 2px solid var(--neon-purple); padding-bottom: 10px; margin-top: 40px;" class="neon-glow">
    NETWORK/OS: JUNCTION POINT & PROTOCOL STACK
</h2>

<div class="terminal-window">
    <div class="terminal-line"><span class="terminal-prompt">dyexahub@core-system:~$</span> <span class="terminal-command">cat /etc/sys-info/engineer_profile</span></div>
    <div class="terminal-line"><span class="terminal-output">----------------------------------------------------</span></div>
    <div class="terminal-line"><span class="terminal-output"># ROLE: Computer & Network Engineer (Sys. Architect)</span></div>
    <div class="terminal-line"><span class="terminal-output"># FOCUS: TCP/IP Stack, Subnetting, Routing Protocols (OSPF/BGP), VLANs, Firewall Management (IPTables/UFW), VPN Tunnels, Security Hardening.</span></div>
    <div class="terminal-line"><span class="terminal-output">----------------------------------------------------</span></div>
    <div class="terminal-line"><span class="terminal-line"><span class="terminal-prompt">dyexahub@core-system:~$</span> <span class="terminal-command">ls -l /boot/os/installed</span></div>
    <div class="terminal-line"><span class="terminal-output">drwxr-xr-x  Ubuntu-24.04-LTS  (Server/Desktop Deployment)</span></div>
    <div class="terminal-line"><span class="terminal-output">drwxr-xr-x  Debian-12-Bookworm (Stable Base Images)</span></div>
    <div class="terminal-line"><span class="terminal-output">drwxr-xr-x  Kali-Rolling       (PenTesting & Security Audit)</span></div>
    <div class="terminal-line"><span class="terminal-output">drwxr-xr-x  Alpine-3.18        (Container Optimization)</span></div>
    <div class="terminal-line"><span class="terminal-output">drwxr-xr-x  OpenBSD-7.5        (Security Focus/Firewall)</span></div>
    <div class="terminal-line"><span class="terminal-line"><span class="terminal-prompt">dyexahub@core-system:~$</span> <span class="terminal-command">netstat -an | grep ESTABLISHED</span></div>
    <div class="terminal-line"><span class="terminal-output">TCP 127.0.0.1:8080 ESTABLISHED (Backend-to-DB Connection)</span></div>
    <div class="terminal-line"><span class="terminal-output">TCP 192.168.1.10:443 ESTABLISHED (Secure External Gateway)</span></div>
    <div class="terminal-line"><span class="terminal-output">TCP 10.0.0.5:22 ESTABLISHED (SSH Remote Administration)</span></div>
    <div class="terminal-line"><span class="terminal-output"></span></div>
    <div class="terminal-line"><span class="terminal-prompt">dyexahub@core-system:~$</span> <span class="terminal-command">echo $NETWORKING_IS_ART</span></div>
    <div class="terminal-line"><span class="terminal-output">TRUE</span></div>
</div>

<!-- Network Visualization Mockup (Using SVG for complex shape/glow) -->
<h3 style="color: var(--neon-green); margin-top: 40px;">
    HOLOGRAPHIC NETWORK MAP: D-HUB CONNECTIVITY
</h3>
<svg width="100%" height="300" viewBox="0 0 900 300" style="background: rgba(0,0,0,0.5); border: 1px solid var(--neon-green); border-radius: 8px; margin-top: 15px; box-shadow: 0 0 15px var(--neon-green);">
    <defs>
        <filter id="glow">
            <feGaussianBlur in="SourceGraphic" stdDeviation="3" result="blur" />
            <feMerge>
                <feMergeNode in="blur" />
                <feMergeNode in="SourceGraphic" />
            </feMerge>
        </filter>
    </defs>

    <!-- Main Core Node (DyexaHub) -->
    <circle cx="450" cy="150" r="30" fill="var(--neon-purple)" filter="url(#glow)"/>
    <text x="450" y="155" text-anchor="middle" fill="#fff" font-size="12" font-weight="bold">HUB</text>

    <!-- Peripheral Nodes -->
    <circle cx="150" cy="50" r="15" fill="var(--neon-blue)" filter="url(#glow)"/>
    <text x="150" y="45" text-anchor="middle" fill="#fff" font-size="10">CLOUD</text>

    <circle cx="750" cy="50" r="15" fill="var(--code-red)" filter="url(#glow)"/>
    <text x="750" y="45" text-anchor="middle" fill="#fff" font-size="10">DB_CLUSTER</text>

    <circle cx="150" cy="250" r="15" fill="var(--code-yellow)" filter="url(#glow)"/>
    <text x="150" y="245" text-anchor="middle" fill="#fff" font-size="10">LINUX_FARM</text>

    <circle cx="750" cy="250" r="15" fill="var(--neon-green)" filter="url(#glow)"/>
    <text x="750" y="245" text-anchor="middle" fill="#fff" font-size="10">DEVOPS_CI/CD</text>

    <!-- Connections (Chaos Lines) -->
    <line x1="450" y1="150" x2="150" y2="50" stroke="var(--neon-blue)" stroke-width="2" filter="url(#glow)"/>
    <line x1="450" y1="150" x2="750" y2="50" stroke="var(--code-red)" stroke-width="2" filter="url(#glow)"/>
    <line x1="450" y1="150" x2="150" y2="250" stroke="var(--code-yellow)" stroke-width="2" filter="url(#glow)"/>
    <line x1="450" y1="150" x2="750" y2="250" stroke="var(--neon-green)" stroke-width="2" filter="url(#glow)"/>
    
    <!-- Cross-Connection (AI/ML Data Flow) -->
    <line x1="150" y1="50" x2="750" y2="250" stroke="var(--neon-purple)" stroke-width="1" stroke-dasharray="4, 4" filter="url(#glow)"/>

    <text x="450" y="290" text-anchor="middle" fill="#888" font-size="10">TCP/IP | OSPF | BGP - TRAFFIC FLOW VIZUALIZATION (STATIC MOCKUP)</text>
</svg>

---

<!-- 
##################################
# 6. 3D INTERACTIVE ZONE (MOCK) #
##################################
-->

<h2 style="font-size: 2em; color: var(--code-red); border-bottom: 2px solid var(--code-red); padding-bottom: 10px; margin-top: 40px;" class="neon-glow">
    3D CREATIVE MATRIX // HOLOGRAPHIC MOCKUPS
</h2>

<div style="margin: 30px auto; max-width: 900px; padding: 20px; background: rgba(0, 0, 0, 0.6); border: 2px solid var(--neon-purple); border-radius: 12px; perspective: 1000px;">
    <div class="rotating-asset" style="width: 150px; height: 150px; margin: 0 auto; display: flex; align-items: center; justify-content: center; transform: rotateX(45deg) rotateY(45deg);">
        <!-- Mock 3D rotating cube/asset using SVG/Text -->
        <div style="position: absolute; width: 100%; height: 100%; border: 3px solid var(--neon-blue); box-shadow: 0 0 15px var(--neon-blue), inset 0 0 15px var(--neon-blue); background: rgba(0, 204, 255, 0.05); display: flex; align-items: center; justify-content: center; font-size: 2em; color: var(--neon-blue);">
            <span style="transform: translateZ(25px);">CODE</span>
        </div>
        <div style="position: absolute; width: 100%; height: 100%; border: 3px solid var(--neon-purple); box-shadow: 0 0 15px var(--neon-purple), inset 0 0 15px var(--neon-purple); background: rgba(255, 0, 255, 0.05); display: flex; align-items: center; justify-content: center; font-size: 2em; color: var(--neon-purple); transform: rotateX(90deg) translateZ(75px);">
            <span style="transform: rotateX(-90deg);">SYS</span>
        </div>
        <div style="position: absolute; width: 100%; height: 100%; border: 3px solid var(--neon-green); box-shadow: 0 0 15px var(--neon-green), inset 0 0 15px var(--neon-green); background: rgba(57, 255, 20, 0.05); display: flex; align-items: center; justify-content: center; font-size: 2em; color: var(--neon-green); transform: rotateY(90deg) translateZ(75px);">
            <span style="transform: rotateY(-90deg);">ART</span>
        </div>
    </div>
    <p style="color: #888; margin-top: 30px; font-size: 0.9em;">
        [VFX ENGINE NOTE: Cube asset rotation is simulated via CSS3 keyframes. True 3D rendering not supported.]
    </p>
</div>

---

<!-- 
###############################
# 7. PROJECT ZONE: ARTIFACTS #
###############################
-->

<h2 style="font-size: 2em; color: var(--neon-blue); border-bottom: 2px solid var(--neon-blue); padding-bottom: 10px; margin-top: 40px;" class="neon-glow">
    PROJECT ARTIFACTS // KEY CREATIONS
</h2>

<div class="project-grid">
    <!-- Project 1 -->
    <div class="project-card">
        <div class="project-title">Chaos/Ops - K8s Cluster Orchestrator</div>
        <p style="color: #ccc; margin-top: 5px;">A custom orchestration layer built in GoLang to manage multi-cloud Kubernetes deployments with integrated ArgoCD.</p>
        <div class="project-tech">
            Tech Stack: GoLang | Kubernetes | ArgoCD | Prometheus | AWS
        </div>
        <a href="https://github.com/DyexaHub/project-repo-1" style="color: var(--neon-blue); text-decoration: none; display: block; margin-top: 10px;">[VIEW REPOSITORY &gt;]</a>
    </div>

    <!-- Project 2 -->
    <div class="project-card">
        <div class="project-title">HoloUI - Next.js Design System</div>
        <p style="color: #ccc; margin-top: 5px;">A futuristic design system component library built with Next.js and Tailwind, emphasizing neon glow and depth effects.</p>
        <div class="project-tech">
            Tech Stack: Next.js | TypeScript | Tailwind CSS | Figma
        </div>
        <a href="https://github.com/DyexaHub/project-repo-2" style="color: var(--neon-blue); text-decoration: none; display: block; margin-top: 10px;">[VIEW REPOSITORY &gt;]</a>
    </div>
    
    <!-- Project 3 -->
    <div class="project-card">
        <div class="project-title">NetSec Tracer - Python Analyzer</div>
        <p style="color: #ccc; margin-top: 5px;">A network intrusion detection and analysis tool using Python, leveraging Scapy and Pandas for traffic filtering and visualization.</p>
        <div class="project-tech">
            Tech Stack: Python | Scapy | Pandas | Kali Linux | Wireshark
        </div>
        <a href="https://github.com/DyexaHub/project-repo-3" style="color: var(--neon-blue); text-decoration: none; display: block; margin-top: 10px;">[VIEW REPOSITORY &gt;]</a>
    </div>
</div>

<p style="color: var(--neon-purple); font-size: 0.9em; margin-top: 30px;">
    <a href="https://github.com/DyexaHub?tab=repositories" style="color: var(--neon-purple); text-decoration: none;" class="neon-glow">
        [FULL ARTIFACT INDEX: ACCESS ALL PROJECTS]
    </a>
</p>

---

<!-- 
####################################
# 8. MESSAGE FROM THE MACHINE (END) #
####################################
-->

<h2 style="font-size: 2em; color: var(--neon-green); border-bottom: 2px solid var(--neon-green); padding-bottom: 10px; margin-top: 40px;" class="neon-glow">
    TRANSMISSION END: MANIFESTO
</h2>

<div style="text-align: center; margin: 20px auto 50px auto; max-width: 700px; padding: 30px; border: 3px double var(--neon-purple); border-radius: 15px; background: linear-gradient(180deg, rgba(0, 0, 0, 0.7), rgba(255, 0, 255, 0.1));">
    <p style="font-size: 1.2em; line-height: 1.8; color: #fff;">
        <strong style="color: var(--code-red);">STATUS: SYNCHRONIZED.</strong><br>
        I am Andre. I stand where the **circuit meets the canvas**. My objective is not merely to write code, but to **engineer experiences**. I utilize the precision of the network engineer to ensure stability, and the vision of the system architect to define the future. The chaos you see here is the energy of innovation—always in motion, always seeking the next breakthrough. If you seek a collaborator who understands both the **packet and the pixel**, initiation sequence is complete.
    </p>
    <p style="font-size: 1.5em; margin-top: 25px; color: var(--neon-blue);" class="neon-glow">
        <span style="font-style: italic;">&gt; WAKE UP. CONNECT. BUILD.</span>
    </p>
</div>


</div>
<!-- End of README.md Content -->
