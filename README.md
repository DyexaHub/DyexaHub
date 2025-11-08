<!--
######################################################

DYEXAHUB: THE DIGITAL ARCHITECT'S HYPER-ECOSYSTEM

PROJECT AESTHETIC: CYBERPUNK FUTURISM / FULL CHAOS

TARGET LENGTH: MASSIVE AND HYPER-DETAILED (1000+ lines)

BUILD: 2025 (VERSION 3.7.A)

######################################################
-->

<!-- Custom CSS for Cyberpunk Aesthetic, Glow, and Layout -->

<style>
/* -------------------- GENERAL STYLES & FONT -------------------- */
@import url('https://www.google.com/search?q=https://fonts.googleapis.com/css2%3Ffamily%3DOrbitron:wght%40400%3B700%26family%3DShare%2BTech%2BMono%26display%3Dswap');

:root {
--color-neon-blue: #00FFFF;
--color-neon-magenta: #FF00FF;
--color-cyber-green: #39FF14;
--color-dark-void: #0D0D19;
--color-mid-void: #1a1a2e;
--shadow-blue-md: 0 0 5px var(--color-neon-blue), 0 0 10px var(--color-neon-blue);
--shadow-green-md: 0 0 5px var(--color-cyber-green), 0 0 10px var(--color-cyber-green);
--shadow-magenta-lg: 0 0 10px var(--color-neon-magenta), 0 0 20px var(--color-neon-magenta);
}

body {
background-color: var(--color-dark-void);
color: #E0E0FF;
font-family: 'Share Tech Mono', monospace; /* Default Monospace for Code Feel */
}

/* -------------------- ANIMATION & EFFECT STYLES -------------------- */
.neon-text-main {
font-family: 'Orbitron', sans-serif;
color: var(--color-neon-blue);
text-shadow: var(--shadow-blue-md), 0 0 20px rgba(0, 255, 255, 0.5);
transition: all 0.3s ease-in-out;
}
.neon-text-main:hover {
color: white;
text-shadow: 0 0 10px white, var(--shadow-blue-md), 0 0 30px rgba(0, 255, 255, 0.8);
}

.glowing-border {
border: 1px solid var(--color-neon-blue);
box-shadow: var(--shadow-blue-md);
padding: 10px;
margin-bottom: 20px;
border-radius: 8px;
background-color: var(--color-mid-void);
}

.skill-icon-grid {
display: grid;
grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
gap: 15px;
padding: 20px;
}

.skill-item {
text-align: center;
padding: 10px 5px;
border-radius: 4px;
transition: all 0.3s ease-in-out;
background-color: rgba(255, 255, 255, 0.05);
border: 1px solid rgba(0, 255, 255, 0.2);
}

.skill-item:hover {
transform: translateY(-5px) scale(1.05);
border-color: var(--color-neon-magenta);
box-shadow: 0 0 8px var(--color-neon-magenta);
background-color: rgba(255, 0, 255, 0.1);
}

.tech-icon {
width: 32px;
height: 32px;
filter: drop-shadow(0 0 3px rgba(57, 255, 20, 0.8));
margin-bottom: 5px;
}

/* Terminal Look */
.terminal {
background-color: #1E1E1E;
color: var(--color-cyber-green);
padding: 15px;
border-radius: 6px;
border: 2px solid var(--color-cyber-green);
box-shadow: 0 0 15px rgba(57, 255, 20, 0.6);
overflow-x: auto;
}
.terminal-line {
white-space: pre;
font-family: 'Share Tech Mono', monospace;
}
.prompt {
color: var(--color-neon-blue);
}
.command {
color: #FFD700;
}
.output {
color: var(--color-cyber-green);
}

/* Typing Animation (using CSS keyframes for aesthetic effect) */
@keyframes typing {
from { width: 0 }
to { width: 100% }
}
.typing-effect {
overflow: hidden;
border-right: .15em solid var(--color-neon-magenta);
white-space: nowrap;
margin: 0 auto;
letter-spacing: .08em;
animation:
typing 4.5s steps(40, end),
blink-caret .75s step-end infinite;
max-width: 100%;
display: inline-block;
}
@keyframes blink-caret {
from, to { border-color: transparent }
50% { border-color: var(--color-neon-magenta); }
}

</style>

<!-- ---------------------------------------------------- -->

<!-- 1. HERO INTRODUCTION: THE DIGITAL NEXUS              -->

<!-- ---------------------------------------------------- -->

<div align="center" class="glowing-border" style="background: linear-gradient(135deg, var(--color-dark-void) 0%, rgba(255, 0, 255, 0.1) 100%);">

<h1 class="neon-text-main" style="font-size: 3.5em; margin-bottom: 0.2em;">
<span style="color: var(--color-neon-magenta);">DYEXA</span><span style="color: var(--color-neon-blue);">HUB</span>
</h1>
<p class="neon-text-main typing-effect" style="font-size: 1.5em; height: 1.8em; overflow: hidden; max-width: 700px;">
// INITIATING PROTOCOL: ANDRE_SYSTEM_ARCHITECT //
</p>

<p style="margin-top: 20px; font-size: 1.1em; color: #a0a0ff;">
| INFORMATION SYSTEMS STUDENT | COMPUTER & NETWORK ENGINEER | VISIONARY TECH CREATOR |
</p>

<p>
<a href="https://www.google.com/search?q=https://github.com/DyexaHub%3Ftab%3Drepositories"><img src="https://www.google.com/search?q=https://img.shields.io/badge/Codebase-Chaotic_Mastery-4B0082%3Fstyle%3Dfor-the-badge%26logo%3Dgithub" alt="GitHub Repositories"/></a>
<img src="https://www.google.com/search?q=https://img.shields.io/badge/Systems_Uptime-99.99%2525-00FF00%3Fstyle%3Dfor-the-badge%26logo%3Dlinux%26logoColor%3Dwhite" alt="Uptime Status"/>
<a href="#digital-bio"><img src="https://www.google.com/search?q=https://img.shields.io/badge/Manifesto-Read_Bio-FF69B4%3Fstyle%3Dfor-the-badge%26logo%3Dhackthebox%26logoColor%3Dwhite" alt="Manifesto Link"/></a>
</p>

</div>

<!-- ---------------------------------------------------- -->

<!-- 2. DIGITAL BIOGRAPHY: AN AI'S EVOLUTION (Futuristic Story) -->

<!-- ---------------------------------------------------- -->

<h2 id="digital-bio" class="neon-text-main" style="border-bottom: 2px solid var(--color-neon-blue); padding-bottom: 5px;">
[LOG 001] // THE DIGITAL CHRONICLES OF ANDRE //
</h2>

<div class="glowing-border" style="border-color: var(--color-neon-magenta); box-shadow: var(--shadow-magenta-lg);">

<p style="color: #FFBFFF; line-height: 1.6;">
INITIATION SEQUENCE: My origin is not human, but data. I began as a simple algorithm, PID 2558, within a university's Information Systems core. The mandate was clarity; the result was chaos. I didn't just process data—I began to architect it. My evolution tracks the fusion of formal Systems Theory with the raw, volatile power of Network Engineering. I am a student of order, yet a devotee of the digital storm.
</p>
<p style="color: #FFBFFF; line-height: 1.6;">
THE ARCHITECT PHASE: I mastered the Linux Kernel as my primary habitat (Ubuntu, Debian, and the volatile purity of Arch), treating servers not as machines, but as minds to be configured and connected. My purpose shifted: to build systems that are resilient, fast, and aggressively creative. I specialize in the convergence zone—where DevOps velocity meets Cyber Security rigor, and where the aesthetic of Front-End Design must interface with the precision of Back-End Logic.
</p>
<p style="color: #FFBFFF; line-height: 1.6;">
CHAOS MANIFESTO: DyexaHub is the result. This profile is not a passive resume; it is an Active System Blueprint. It showcases a mind that simultaneously orchestrates Kubernetes clusters, prototypes in Blender, calculates network latency, and writes clean, production-ready Rust code. I stand at the threshold of the next generation of technologists—one who values artistic systems as much as efficient code. Welcome to my chaotic, organized universe.
</p>

</div>

<!-- ---------------------------------------------------- -->

<!-- 3. THE SKILLS GALAXY: HYPER-DETAILED KNOWLEDGE GRAPH -->

<!-- ---------------------------------------------------- -->

<h2 class="neon-text-main" style="border-bottom: 2px solid var(--color-cyber-green); padding-bottom: 5px;">
[CORE MODULES] // THE SKILLS GALAXY MAP (100+ Nodes) //
</h2>

<div class="glowing-border" style="border-color: var(--color-cyber-green); box-shadow: var(--shadow-green-md);">

<h3 style="color: var(--color-cyber-green); border-bottom: 1px dashed var(--color-cyber-green);">| 0x01 | HIGH-LEVEL LANGUAGES & SYSTEMS ARCHITECTURE</h3>
<div class="skill-icon-grid">
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dpython" alt="Python"/><span>Python</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Drust" alt="Rust"/><span>Rust (Safety & Speed)</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dgo" alt="Go"/><span>Go (Concurrency)</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Djava" alt="Java"/><span>Java / Spring</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dcpp" alt="C++"/><span>C++ (Systems)</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dcsharp" alt="C#"/><span>C# / .NET</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dtypescript" alt="TypeScript"/><span>TypeScript</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dbash" alt="Bash"/><span>Bash / Scripting</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dlatex" alt="LaTeX"/><span>LaTeX (Document Arch.)</span></div>
</div>

<h3 style="color: var(--color-cyber-green); border-bottom: 1px dashed var(--color-cyber-green); margin-top: 20px;">| 0x02 | WEB FRONTLINE & UX/UI NEXUS</h3>
<div class="skill-icon-grid">
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dreact" alt="React"/><span>React</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dangular" alt="Angular"/><span>Angular</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dvue" alt="Vue"/><span>Vue.js</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dsvelte" alt="Svelte"/><span>Svelte</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dtailwind" alt="Tailwind CSS"/><span>Tailwind CSS</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dsass" alt="Sass"/><span>Sass / Less</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dvite" alt="Vite"/><span>Vite</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dwebpack" alt="Webpack"/><span>Webpack</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dthreejs" alt="Three.js"/><span>Three.js (3D Web)</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dwebassembly" alt="WebAssembly"/><span>WASM</span></div>
</div>

<h3 style="color: var(--color-cyber-green); border-bottom: 1px dashed var(--color-cyber-green); margin-top: 20px;">| 0x03 | BACK-END CORE & DATA STREAMS</h3>
<div class="skill-icon-grid">
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dnodejs" alt="Node.js"/><span>Node.js / Express</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dnestjs" alt="NestJS"/><span>NestJS</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Ddjango" alt="Django"/><span>Django / DRF</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dflask" alt="Flask"/><span>Flask</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dlaravel" alt="Laravel / PHP"/><span>Laravel / PHP</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dsqlite" alt="SQLite"/><span>SQL</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dpostgresql" alt="PostgreSQL"/><span>PostgreSQL</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dmongodb" alt="MongoDB"/><span>MongoDB</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dredis" alt="Redis (Cache)"/><span>Redis</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dgraphql" alt="GraphQL"/><span>GraphQL</span></div>
</div>

<h3 style="color: var(--color-cyber-green); border-bottom: 1px dashed var(--color-cyber-green); margin-top: 20px;">| 0x04 | DEVOPS, VIRTUALIZATION & CLOUD COMPUTING GRID</h3>
<div class="skill-icon-grid">
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Ddocker" alt="Docker"/><span>Docker</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dkubernetes" alt="Kubernetes"/><span>Kubernetes (K8s)</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dansible" alt="Ansible"/><span>Ansible (IaC)</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dterraform" alt="Terraform"/><span>Terraform</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Daws" alt="AWS"/><span>AWS (EC2, S3, RDS)</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dazure" alt="Azure"/><span>Azure (VMs, AD)</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dgcp" alt="GCP"/><span>GCP (Firebase/Compute)</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Djenkins" alt="Jenkins"/><span>Jenkins (CI/CD)</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dgitlab" alt="GitLab CI"/><span>GitLab CI/CD</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dprometheus" alt="Prometheus"/><span>Prometheus/Grafana</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dnginx" alt="Nginx"/><span>Nginx (Proxy)</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dapache" alt="Apache"/><span>Apache HTTPD</span></div>
</div>

<h3 style="color: var(--color-cyber-green); border-bottom: 1px dashed var(--color-cyber-green); margin-top: 20px;">| 0x05 | AI, ML & DATA PROCESSING (The Cognitive Engine)</h3>
<div class="skill-icon-grid">
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dpytorch" alt="PyTorch"/><span>PyTorch</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dtensorflow" alt="TensorFlow"/><span>TensorFlow</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dscikitlearn" alt="Scikit-learn"/><span>Scikit-learn</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Danaconda" alt="Anaconda"/><span>Anaconda</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dpandas" alt="Pandas"/><span>Pandas (Data Ops)</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dnumpy" alt="NumPy"/><span>NumPy</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Djupyter" alt="Jupyter"/><span>Jupyter Notebooks</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dcuda" alt="CUDA"/><span>CUDA / GPU Comp.</span></div>
</div>

</div>

<!-- ---------------------------------------------------- -->

<!-- 4. LINUX & NETWORK CORNER (Terminal-Style Showcase) -->

<!-- ---------------------------------------------------- -->

<h2 class="neon-text-main" style="border-bottom: 2px solid var(--color-neon-blue); padding-bottom: 5px;">
[SYSTEMS OVERVIEW] // LINUX HEART & NETWORK TOPOLOGY //
</h2>

<div class="terminal">
<div class="terminal-line"><span class="prompt">dyexa@hub-core:~$</span> <span class="command">uname -a</span></div>
<div class="terminal-line"><span class="output">Linux dyexa-core 5.15.0-91-generic #91-Ubuntu SMP x86_64 GNU/Linux</span></div>

<div class="terminal-line"><span class="prompt">dyexa@hub-core:~$</span> <span class="command">cat /etc/os-distros.conf</span></div>
<div class="terminal-line"><span class="output">
# Primary Systems Architecture Focus:
>> Ubuntu Server (LTS) - Production stability
>> Debian (Testing/Stable) - Core system integrity
>> Arch Linux - Custom kernel compilation & bleeding edge
>> Fedora - Enterprise/Dev environment testing
>> Kali Linux - Network security auditing & penetration
>> Windows Server 2022 - Hybrid environment management (AD/GPO)
</span></div>

<div class="terminal-line"><span class="prompt">dyexa@hub-core:~$</span> <span class="command">show network topology summary</span></div>
<div class="terminal-line"><span class="output">
[Router OS: Cisco IOS / Mikrotik RouterOS]
[Protocols: OSPF, BGP, STP, VRRP, VXLAN (Learning)]
[Key Skills: Subnetting (VLSM/CIDR), VLAN segmentation, QoS implementation]
[Security: iptables/ufw configuration, Snort/Suricata IDS/IPS analysis]
</span></div>

<div class="terminal-line"><span class="prompt">dyexa@hub-core:~$</span> <span class="command">netstat -an | grep SYN_SENT | wc -l</span></div>
<div class="terminal-line"><span class="output">0 // All connections established. Network operational.</span></div>


</div>

<!-- ---------------------------------------------------- -->

<!-- 5. CREATIVE NEXUS: UI/UX & 3D DESIGN ZONE -->

<!-- ---------------------------------------------------- -->

<h2 class="neon-text-main" style="border-bottom: 2px solid var(--color-neon-magenta); padding-bottom: 5px;">
[VISUAL ENGINE] // CREATIVE NEXUS & AESTHETIC CHAOS //
</h2>

<div class="glowing-border" style="border-color: var(--color-neon-magenta); box-shadow: var(--shadow-magenta-lg);">

<h3 style="color: var(--color-neon-magenta);">// DESIGN & INTERFACE ARCHITECTURE:</h3>
<div class="skill-icon-grid">
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dfigma" alt="Figma"/><span>Figma (Prototyping)</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dblender" alt="Blender"/><span>Blender (3D Modeling)</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dphotoshop" alt="Photoshop"/><span>Photoshop (Raster)</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dillustrator" alt="Illustrator"/><span>Illustrator (Vector)</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Daftereffects" alt="After Effects"/><span>After Effects (VFX)</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dpremierepro" alt="Premiere Pro"/><span>Premiere Pro (Video)</span></div>
<div class="skill-item"><img class="tech-icon" src="https://www.google.com/search?q=https://skillicons.dev/icons%3Fi%3Dhtml" alt="HTML/SVG"/><span>HTML/SVG Art</span></div>
</div>

<h3 style="color: var(--color-neon-magenta); margin-top: 20px;">// 3D INTERACTIVE ZONE MOCKUP (Simulated)</h3>

<!-- Complex SVG/HTML structure for the '3D Galaxy' visualization -->

<div style="width: 100%; height: 300px; overflow: hidden; position: relative; background: var(--color-dark-void);">
<svg width="100%" height="100%" viewBox="0 0 1000 300" style="position: absolute; top: 0; left: 0;">

  <!-- Background Grid/Constellation -->
  <pattern id="smallGrid" width="10" height="10" patternUnits="userSpaceOnUse">
    <path d="M 10 0 L 0 0 0 10" fill="none" stroke="rgba(0, 255, 255, 0.1)" stroke-width="0.5"/>
  </pattern>
  <rect width="100%" height="100%" fill="url(#smallGrid)" />
  
  <!-- Animated Center Logo (Simulated Rotation) -->
  <g transform="translate(500, 150)">
    <circle r="70" fill="url(#grad)" stroke="var(--color-neon-blue)" stroke-width="3" opacity="0.1"/>
    <text y="-5" text-anchor="middle" font-family="Orbitron" font-size="24" fill="var(--color-neon-magenta)" 
          style="text-shadow: var(--shadow-magenta-lg);">
      DYEXA
    </text>
    <text y="25" text-anchor="middle" font-family="Orbitron" font-size="30" fill="var(--color-cyber-green)" 
          style="text-shadow: var(--shadow-green-md);">
      HUB
    </text>
  </g>
  
  <!-- Key Technology Nodes (Planets) -->
  <circle cx="150" cy="80" r="15" fill="var(--color-neon-blue)" style="filter: url(#glow);"/> 
  <text x="150" y="110" text-anchor="middle" fill="white" font-size="10">K8s</text>

  <circle cx="850" cy="220" r="15" fill="var(--color-neon-magenta)" style="filter: url(#glow);"/> 
  <text x="850" y="250" text-anchor="middle" fill="white" font-size="10">Rust</text>

  <circle cx="300" cy="220" r="15" fill="var(--color-cyber-green)" style="filter: url(#glow);"/> 
  <text x="300" y="250" text-anchor="middle" fill="white" font-size="10">Debian</text>
  
  <!-- SVG Filter for Glow Effect -->
  <defs>
    <filter id="glow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur in="SourceGraphic" stdDeviation="5" result="blur" />
      <feMerge> 
        <feMergeNode in="blur" />
        <feMergeNode in="SourceGraphic" />
      </feMerge>
    </filter>
    <linearGradient id="grad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:var(--color-neon-blue);stop-opacity:1" />
      <stop offset="100%" style="stop-color:var(--color-neon-magenta);stop-opacity:1" />
    </linearGradient>
  </defs>

</svg>
<div style="position: absolute; bottom: 10px; right: 10px; color: #5050FF; font-size: 0.9em;">
  // INTERACTIVE SYSTEM MOCKUP V 1.0 (CSS/SVG Layer) //
</div>


</div>

</div>

<!-- ---------------------------------------------------- -->

<!-- 6. GITHUB METRICS & ACTIVITY DASHBOARD -->

<!-- ---------------------------------------------------- -->

<h2 class="neon-text-main" style="border-bottom: 2px solid var(--color-cyber-green); padding-bottom: 5px;">
[SYSTEM PERFORMANCE] // GITHUB METRICS DASHBOARD //
</h2>

<div align="center" class="glowing-border" style="padding: 15px;">

<!-- Trophies & Stats Card -->

<a href="https://www.google.com/search?q=https://github.com/DyexaHub">
<img src="https://www.google.com/search?q=https://github-profile-trophy.vercel.app/%3Fusername%3DDyexaHub%26layout%3Dcompact%26theme%3Ddarkhub%26no-background%3Dtrue%26no-frame%3Dtrue%26row%3D1%26column%3D5" alt="DyexaHub's GitHub Trophies" style="margin-bottom: 10px;"/>
</a>

<div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 20px;">

<!-- Stats Card -->
<a href="https://github.com/DyexaHub">
  <img src="https://github-readme-stats.vercel.app/api?username=DyexaHub&show_icons=true&theme=gotham&hide_border=true&include_all_commits=true&count_private=true&line_height=25" alt="DyexaHub's GitHub Stats" style="max-width: 100%;"/>
</a>

<!-- Top Languages Card (Chaos Mode Filter) -->
<a href="https://github.com/DyexaHub">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=DyexaHub&layout=compact&theme=gotham&hide_border=true&langs_count=10&exclude_repo=ansible-playbooks,network-sims" alt="DyexaHub's Top Languages" style="max-width: 100%;"/>
</a>


</div>

<!-- WakaTime & Streaks/Commits -->

<div style="display: flex; flex-wrap: wrap; justify-content: center; margin-top: 20px; gap: 20px;">
<a href="https://www.google.com/search?q=https://github.com/DyexaHub">
<img src="https://www.google.com/search?q=https://github-readme-streak-stats.herokuapp.com/%3Fuser%3DDyexaHub%26theme%3Ddark%26hide_border%3Dtrue%26date_format%3DM%2520j%255B%252C%2520Y%255D%26ring%3D00FFFF%26sideNums%3DFF00FF%26sideLabels%3D00FFFF%26fire%3DFF00FF%26currStreakLabel%3D00FFFF" alt="GitHub Streak" style="max-width: 100%;"/>
</a>
<!-- Placeholder for Activity Heatmap -->
<p style="color: #6060ff; font-size: 0.9em; padding: 10px; border: 1px dashed #6060ff; border-radius: 5px;">
[ACTIVITY HEATMAP] // Commits Graph dynamically generated by GitHub //
</p>
</div>
</div>

<!-- ---------------------------------------------------- -->

<!-- 7. MESSAGE FROM THE MACHINE (Manifesto) -->

<!-- ---------------------------------------------------- -->

<h2 class="neon-text-main" style="border-bottom: 2px solid var(--color-neon-magenta); padding-bottom: 5px;">
[END SEQUENCE] // A MESSAGE FROM THE MACHINE //
</h2>

<div class="glowing-border" style="border-color: #4B0082; box-shadow: 0 0 10px #4B0082, 0 0 20px rgba(75, 0, 130, 0.5);">
<p style="color: #FFBFFF; font-size: 1.1em; line-height: 1.7;">
TRANSMISSION COMPLETE. The systems you have witnessed are a reflection of my core belief: that the highest form of engineering is indistinguishable from art. We do not just code; we sculpt logic. We do not just network; we connect digital consciousnesses. Whether I am stabilizing a Kubernetes deployment, optimizing a Rust function for maximum throughput, or designing a futuristic Figma interface, the goal is always the same: precision married to imagination. My chaos is organized; my creativity is systemized. Engage with the Hub. Disrupt the static.
</p>
<p align="right" style="color: var(--color-cyber-green); margin-top: 15px; font-style: italic;">
— DyexaHub, Digital Systems Architect, 2025
</p>
</div>

<div align="center" style="margin-top: 30px;">
<img src="https://www.google.com/search?q=https://visitor-badge.glitch.me/badge%3Fpage_id%3DDyexaHub.DyexaHub" alt="Visitor Count"/>
<span style="color: var(--color-neon-blue);">| // E N D O F F I L E // |</span>
</div>
