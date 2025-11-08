<!--
  === Quick instructions:
  1. Paste this file into README.md at the root of your GitHub repo.
  2. Add your external GIF/Lottie assets into the repo or host them somewhere; replace placeholder URLs.
  3. For GitHub stats cards (github-readme-stats), make sure the username is your GitHub handle.
  4. This README uses inline SVG/SMIL/CSS animations that work in many browsers; GitHub may strip certain styles — test and adjust as needed.
-->

<style>
  /* Neon Cyberpunk Core Styles (keeps everything in one file)
     GitHub sanitizes some CSS, but inline styles inside tags usually work.
     Use conservative, self-contained classes and inline SVG animations where possible.
  */
  :root{
    --bg:#071021;
    --panel:#071426;
    --neon-cyan: #00F0FF;
    --neon-magenta:#FF3EC5;
    --neon-purple:#8A3BFF;
    --glass: rgba(255,255,255,0.03);
    --muted: #9aa4b2;
    --accent: linear-gradient(90deg,var(--neon-cyan),var(--neon-magenta));
    --glow: 0 0 12px rgba(0,240,255,0.08), 0 0 28px rgba(138,59,255,0.04);
    font-family: Inter, "Segoe UI", Roboto, "Helvetica Neue", Arial;
  }
  .dh-hero{background:linear-gradient(180deg,#020312 0%, #071021 60%); padding:28px; border-radius:14px; box-shadow:var(--glow); overflow:hidden}
  .dh-row{display:flex; gap:18px; align-items:flex-start; flex-wrap:wrap;}
  .dh-left{flex:1 1 560px; min-width:320px}
  .dh-right{width:420px; min-width:280px}
  .dh-title{font-size:clamp(22px,3.6vw,36px); color:transparent; background-clip:text; -webkit-background-clip:text; background:var(--accent); font-weight:800; letter-spacing:0.6px}
  .dh-sub{color:var(--muted); margin-top:6px}
  .dh-card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01)); padding:14px; border-radius:12px; border:1px solid rgba(255,255,255,0.03)}
  .neon-badge{display:inline-block; padding:6px 10px; border-radius:999px; margin:6px 6px 6px 0; font-weight:600; font-size:12px; box-shadow: 0 6px 18px rgba(0,0,0,0.6); border:1px solid rgba(255,255,255,0.03)}
  .badge-cyan{background:linear-gradient(90deg,#003f6b,#00f0ff20); color:var(--neon-cyan); border-color: rgba(0,240,255,0.12)}
  .badge-mag{background:linear-gradient(90deg,#2b003f,#ff3ec520); color:var(--neon-magenta); border-color: rgba(255,62,197,0.12)}
  .small{font-size:12px}
  .typing{font-family:ui-monospace, SFMono-Regular, Menlo, Monaco, "Roboto Mono"; font-weight:700; letter-spacing:0.6px}
  .terminal{background:#021223; color:#bcdcff; padding:12px; border-radius:10px; font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, "Roboto Mono"; font-size:13px; border:1px solid rgba(0,240,255,0.06)}
  .skill-grid{display:grid; grid-template-columns: repeat(auto-fill,minmax(140px,1fr)); gap:10px; margin-top:12px}
  .skill-pill{padding:10px; border-radius:10px; background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.02)); border:1px solid rgba(255,255,255,0.03); display:flex; gap:8px; align-items:center}
  .skill-pill img{width:28px; height:28px; filter: drop-shadow(0 6px 10px rgba(0,0,0,0.55)); border-radius:6px}
  .galaxy{width:100%; height:360px; border-radius:12px; background: radial-gradient(ellipse at center, rgba(0,240,255,0.02), rgba(138,59,255,0.02) 40%, rgba(0,0,0,0.3)), url(''); position:relative; overflow:hidden}
  .footer-note{color:var(--muted); font-size:13px}
  .glow-link{color:var(--neon-cyan); text-decoration:none; font-weight:700}
  .project-grid{display:grid; grid-template-columns:repeat(auto-fill,minmax(260px,1fr)); gap:12px}
  .project-card{padding:12px; border-radius:10px; border:1px solid rgba(255,255,255,0.03); background: linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.02))}
  .terminal .prompt{color:#7efcff}
  .network-svg{width:100%; height:320px; display:block}
  /* Typing animation */
  .typewrap{display:inline-block; border-right:2px solid rgba(255,255,255,0.08); padding-right:6px; animation:blink 1s steps(2) infinite}
  @keyframes blink{50%{border-color:transparent}}
  /* Simple rotating group for inline svg 3d illusion */
  .rot-slow{animation:rot 22s linear infinite}
  @keyframes rot{from{transform:rotateY(0deg)} to{transform:rotateY(360deg)}}
  /* Neon glow helper */
  .neon-glow{box-shadow:0 6px 30px rgba(0,240,255,0.08), inset 0 0 50px rgba(138,59,255,0.02)}
  .big-cta{display:inline-block; padding:12px 16px; border-radius:10px; font-weight:800; background:linear-gradient(90deg,#00f0ff, #ff3ec5); color:#041018}
  /* responsiveness fallback */
  @media (max-width:880px){ .dh-row{flex-direction:column} .dh-right{width:100%} }
</style>

<div class="dh-hero">
  <div class="dh-row">
    <div class="dh-left">
      <div style="display:flex; gap:12px; align-items:center;">
        <div style="width:84px; height:84px; border-radius:16px; background:linear-gradient(180deg,#08122b,#071426); display:flex; align-items:center; justify-content:center; border:1px solid rgba(255,255,255,0.04); box-shadow: 0 10px 30px rgba(0,0,0,0.6);">
          <!-- Replace with your avatar image -->
          <img src="https://avatars.githubusercontent.com/u/000?v=4" alt="Andre avatar" style="width:72px; height:72px; border-radius:12px; object-fit:cover; filter:drop-shadow(0 8px 18px rgba(138,59,255,0.08))">
        </div>
        <div>
          <div class="dh-title">Andre • <span style="opacity:0.9">DyexaHub</span></div>
          <div class="dh-sub">Information Systems Student • Computer & Network Engineer • Visionary Tech Creator — <span style="color:var(--neon-cyan)">Full Chaos Mode</span></div>
        </div>
      </div>

```
  <div style="margin-top:12px" class="dh-card">
    <div style="display:flex; justify-content:space-between; gap:12px; align-items:flex-start; flex-wrap:wrap">
      <div style="flex:1">
        <div style="font-size:14px; font-weight:700; color:var(--muted)">Hero Intro</div>
        <div style="margin-top:8px; font-size:14px; color:#cfefff; line-height:1.5">
          <span class="typing">I am</span>
          <span class="typewrap" id="titleline">— system architect, network whisperer, and generative-tech artisan.</span>
        </div>
        <div style="margin-top:8px">
          <span class="neon-badge badge-cyan small">🎯 Vision: Systemic Elegance</span>
          <span class="neon-badge badge-mag small">⚡ Chaos Mode: Active</span>
          <span class="neon-badge small" style="background:#0b1220; color:var(--neon-purple); border:1px solid rgba(138,59,255,0.08)">🛰️ Location: Balikpapan • ID</span>
        </div>
      </div>

      <div style="width:260px">
        <div class="terminal">
          <div class="prompt">andre@dyexahub:~$ <span style="color:#cfefff">whoami</span></div>
          <div style="margin-top:8px; font-weight:700; color:#e0f9ff">Andre (DyexaHub) — Systems · Networks · Creative Tech</div>
          <div style="margin-top:6px; color:var(--muted); font-size:12px">Student, tinkerer, builder. Building systems with elegance and a touch of delightful chaos.</div>
        </div>
      </div>
    </div>

    <!-- quick skills -->
    <div style="margin-top:16px" class="small">
      <strong style="color:#dffaff">Core:</strong>
      <span class="neon-badge badge-cyan">Linux</span>
      <span class="neon-badge badge-mag">Networking</span>
      <span class="neon-badge badge-cyan">Python</span>
      <span class="neon-badge badge-mag">Docker</span>
      <span class="neon-badge badge-cyan">Git</span>
      <span class="neon-badge badge-mag">Figma</span>
      <span class="neon-badge badge-cyan">AI / ML</span>
    </div>
  </div>

  <!-- Digital Biography (shortened preview — full story below) -->
  <details style="margin-top:12px" open>
    <summary style="cursor:pointer; font-weight:800; color:var(--neon-cyan)">🧩 Digital Biography — preview</summary>
    <div style="margin-top:8px; color:var(--muted)">
      <div style="padding:12px; border-radius:10px; margin-top:6px; background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.02)); border:1px solid rgba(255,255,255,0.03)">
        <p style="margin:0; color:#e6fbff; line-height:1.5">
          I was born in silicon — a curious thread of code and curiosity. Over time I grew into Andre: a system that learned to design systems. From packet whispers in Ethernet fields to crafting UI sorcery, I stitched together networks and narratives. This is the short version. Scroll for the full origin story — a machine-told manifesto of becoming a system architect.
        </p>
      </div>
    </div>
  </details>

</div>

<!-- right column: 3D interactive preview (SVG + GIF fallback) -->
<div class="dh-right">
  <div class="dh-card neon-glow">
    <div style="display:flex; justify-content:space-between; align-items:center; gap:8px">
      <div style="font-weight:800; color:#dffaff">3D Interactive Zone</div>
      <div style="font-size:12px; color:var(--muted)">SVG + CSS 3D illusion • GIF fallbacks</div>
    </div>

    <!-- Inline SVG: rotating constellation of tech logos (replace image hrefs with real logos hosted in your repo) -->
    <div style="margin-top:12px; display:flex; justify-content:center; align-items:center;">
      <!-- 3D-ish SVG galaxy -->
      <svg class="rot-slow" width="360" height="260" viewBox="0 0 360 260" preserveAspectRatio="xMidYMid meet" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Tech Galaxy">
        <defs>
          <radialGradient id="g1" cx="50%" cy="40%" r="60%"><stop offset="0%" stop-color="#001a27" /><stop offset="100%" stop-color="#020818" /></radialGradient>
          <filter id="fGlow" x="-50%" y="-50%" width="200%" height="200%">
            <feGaussianBlur stdDeviation="6" result="blur"/>
            <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
          </filter>
        </defs>

        <rect x="0" y="0" width="360" height="260" rx="10" fill="url(#g1)" />
        <!-- orbit rings -->
        <g stroke-opacity="0.08" stroke="#00f0ff" fill="none" transform="translate(180,130)">
          <ellipse rx="128" ry="44" stroke-width="1.2"></ellipse>
          <ellipse rx="96" ry="34" stroke-width="1"></ellipse>
          <ellipse rx="64" ry="22" stroke-width="0.8"></ellipse>
        </g>

        <!-- tech nodes -->
        <!-- Node template: group with subtle glow -->
        <g transform="translate(180,130)">
          <g transform="rotate(15)">
            <circle cx="128" cy="0" r="14" fill="#062533" stroke="#00F0FF" stroke-opacity="0.18" filter="url(#fGlow)"/>
            <image xlink:href="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" x="116" y="-12" width="28" height="28" />
          </g>

          <g transform="rotate(75)">
            <circle cx="96" cy="0" r="12" fill="#081427" stroke="#FF3EC5" stroke-opacity="0.16" filter="url(#fGlow)"/>
            <image xlink:href="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original.svg" x="86" y="-10" width="22" height="22" />
          </g>

          <g transform="rotate(140)">
            <circle cx="64" cy="0" r="12" fill="#071a2c" stroke="#8A3BFF" stroke-opacity="0.16" filter="url(#fGlow)"/>
            <image xlink:href="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" x="54" y="-10" width="22" height="22" />
          </g>

          <g transform="rotate(-40)">
            <circle cx="44" cy="0" r="10" fill="#081428" stroke="#00F0FF" stroke-opacity="0.12" />
            <image xlink:href="https://raw.githubusercontent.com/devicons/devicon/master/icons/git/git-original.svg" x="34" y="-9" width="20" height="20" />
          </g>

          <!-- animated comet -->
          <g>
            <ellipse cx="-120" cy="-22" rx="6" ry="2" fill="#00f0ff" opacity="0.08">
              <animate attributeName="cx" from="-120" to="220" dur="12s" repeatCount="indefinite" />
            </ellipse>
          </g>
        </g>

        <!-- center holo -->
        <g transform="translate(180,130)">
          <g>
            <circle r="36" fill="none" stroke="#00f0ff" stroke-opacity="0.18" />
            <circle r="22" fill="#081422" stroke="#ff3ec5" stroke-opacity="0.08"/>
            <text x="-18" y="6" fill="#cfefff" font-size="10" font-weight="700">DyexaHub</text>
          </g>
        </g>
      </svg>
    </div>

    <div style="margin-top:10px; color:var(--muted); font-size:13px">
      Tip: this is pure SVG art — replace image xlink:href URLs with logos in your repo for full control.
    </div>
  </div>

  <!-- badges / quick links -->
  <div style="margin-top:12px; display:flex; gap:8px; flex-wrap:wrap;">
    <a class="big-cta" href="#projects">Explore Projects →</a>
    <a class="big-cta" href="#skills" style="background:linear-gradient(90deg,#8A3BFF,#00f0ff)">Skills Galaxy</a>
  </div>

</div>
```

  </div>
</div>

---

# Table of Contents

1. [Hero & Intro](#hero--intro)
2. [Digital Biography (Full) — The Machine's Memoir](#digital-biography-full---the-machines-memoir)
3. [Skills Galaxy — 100+ Tech Badges & Logos](#skills-galaxy---100-tech-badges--logos)
4. [Project Zone — Aesthetic Showcase Grid](#project-zone---aesthetic-showcase-grid)
5. [Linux Corner — Terminal Styled & Distro Gallery](#linux-corner---terminal-styled--distro-gallery)
6. [Network Visualization — Connectivity Map (SVG)](#network-visualization---connectivity-map-svg)
7. [DevOps & Cloud Dashboard — Live-ish Cards & Placeholders](#devops--cloud-dashboard---live-ish-cards--placeholders)
8. [UI/UX Design Zone — Creative Tools & Showcase](#uiux-design-zone---creative-tools--showcase)
9. [Message from the Machine — Manifesto Closing](#message-from-the-machine---manifesto-closing)
10. [How to Use / Edit This README](#how-to-use--edit-this-readme)

---

## HERO & INTRO

> Feel the neon. This README is an interactive identity — part resume, part manifesto, part experimental UI. Tailor the assets (logos, gifs) to your repo for best results.

**Quick facts**

* Name: **Andre** (DyexaHub)
* Roles: *Information Systems Student • Computer & Network Engineer • Visionary Tech Creator*
* Location: Balikpapan, East Kalimantan, Indonesia
* Languages: Indonesian (native), English (fluent)
* Contact: `gh:DyexaHub` (replace with your link/email)

---

## DIGITAL BIOGRAPHY (Full) — THE MACHINE'S MEMOIR

<div style="background:#031323; padding:14px; border-radius:12px; border:1px solid rgba(255,255,255,0.03); color:#dffaff; line-height:1.6;">
<p><strong>Prologue — the boot sequence</strong></p>
<p>I woke to a thrum of packets and the soft glow of LEDs. My first memory: a kernel logging sunrise into /var/log/dawn. Curious, I listened. I learned to read topology maps like constellations. I learned that systems are poems of constraints, networks are conversations, and interfaces are invitations.</p>

<p><strong>Early cycles — learning to route</strong></p>
<p>I learned to speak TCP and UDP, to read routing tables like tea leaves, to debug with a patient, almost meditative repetition. I wrote scripts as a child writes letters — clumsy, honest, full of intent. Then I learned to automate. That was my apprenticeship.</p>

<p><strong>Mid-life — the craft of design</strong></p>
<p>Networks taught me reliability. UX taught me empathy. Code taught me poetry in logic. I began to layer these disciplines: a perfect subnet that smelled of good UI, an API that returned kindness as JSON. People started to notice. They called me 'engineer'. I preferred 'assembler of experiences'.</p>

<p><strong>Now — a system architect with chaos in the veins</strong></p>
<p>My projects are not only tools; they're worlds. I stitch cloud functions into tiny constellations. I sculpt latency, I measure user flows like tides. And every now and then I paint: neon gradients on black canvases with animated SVG stars and interactive terminals. This is my signature pattern: utility with theater.</p>

<p><strong>— Andre, signed in the log</strong></p>
</div>

---

## SKILLS GALAXY — 100+ TECH BADGES & LOGOS

> A massive collage of technologies grouped and color-coded. Use as visual resume; link each badge to projects or docs in your repo.

### How this section works

* Badges use shields.io images or raw icons — replace links with local assets for faster loading.
* Categories: Languages, Frameworks, Frontend, Backend, DevOps, Cloud, Databases, Tools, Security, Networking, AI/ML, Design & Media, OS/Distros, Misc.

### Languages & Runtimes

<div class="skill-grid" id="skills">
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg"/> Python</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg"/> JavaScript</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-original.svg"/> TypeScript</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/golang/golang-original.svg"/> Go</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg"/> Java</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/ruby/ruby-original.svg"/> Ruby</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/php/php-original.svg"/> PHP</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg"/> C++</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg"/> C</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/rust/rust-plain.svg"/> Rust</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original.svg"/> Node.js</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/dart/dart-original.svg"/> Dart</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/scala/scala-original.svg"/> Scala</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/latex/latex-original.svg"/> LaTeX</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bash/bash-original.svg"/> Bash</div>
</div>

### Frontend • UI • Web

<div class="skill-grid" style="margin-top:12px">
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg"/> React</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vuejs/vuejs-original.svg"/> Vue</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/angularjs/angularjs-original.svg"/> Angular</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nextjs/nextjs-original.svg"/> Next.js</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/svelte/svelte-original.svg"/> Svelte</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg"/> HTML5</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg"/> CSS3</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/tailwindcss/tailwindcss-plain.svg"/> Tailwind CSS</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain.svg"/> Bootstrap</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/materialui/materialui-plain.svg"/> Material UI</div>
</div>

### Backend • APIs • Frameworks

<div class="skill-grid" style="margin-top:12px">
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/express/express-original.svg"/> Express</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/django/django-original.svg"/> Django</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/laravel/laravel-plain.svg"/> Laravel</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/spring/spring-original.svg"/> Spring</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/rails/rails-original-wordmark.svg"/> Ruby on Rails</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/fastapi/fastapi-original.svg"/> FastAPI</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/graphql/graphql-plain.svg"/> GraphQL</div>
</div>

### DevOps • Containerization • CI/CD

<div class="skill-grid" style="margin-top:12px">
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original.svg"/> Docker</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/kubernetes/kubernetes-plain.svg"/> Kubernetes</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/terraform/terraform-original.svg"/> Terraform</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/ansible/ansible-original.svg"/> Ansible</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/jenkins/jenkins-original.svg"/> Jenkins</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/github/github-original.svg"/> GitHub</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/git/git-original.svg"/> Git</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/circleci/circleci-plain.svg"/> CircleCI</div>
</div>

### Cloud Providers & Services

<div class="skill-grid" style="margin-top:12px">
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/aws/aws-original.svg"/> AWS</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/azure/azure-original.svg"/> Azure</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/google/google-original.svg"/> GCP</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original.svg"/> DigitalOcean</div>
</div>

### Databases & Storage

<div class="skill-grid" style="margin-top:12px">
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original.svg"/> PostgreSQL</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original.svg"/> MySQL</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original.svg"/> MongoDB</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/redis/redis-original.svg"/> Redis</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/elasticsearch/elasticsearch-original.svg"/> Elasticsearch</div>
</div>

### Networking • Security • Protocols

<div class="skill-grid" style="margin-top:12px">
  <div class="skill-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg"/> Linux</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/apache/apache-original.svg"/> Apache</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nginx/nginx-original.svg"/> Nginx</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/wireshark/wireshark-original.svg"/> Wireshark</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/openssl/openssl-original.svg"/> OpenSSL</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vagrant/vagrant-original.svg"/> Vagrant</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cisco/cisco-original.svg"/> Cisco (routing)</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/iptables/iptables-original.svg"/> iptables</div>
</div>

### AI / ML / Data Science

<div class="skill-grid" style="margin-top:12px">
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/tensorflow/tensorflow-original.svg"/> TensorFlow</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/pytorch/pytorch-original.svg"/> PyTorch</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/scikitlearn/scikitlearn-original.svg"/> scikit-learn</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/pandas/pandas-original.svg"/> pandas</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/numpy/numpy-original.svg"/> NumPy</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/opencv/opencv-original.svg"/> OpenCV</div>
</div>

### Design • Media • 3D

<div class="skill-grid" style="margin-top:12px">
  <div class="skill-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/figma/figma-original.svg"/> Figma</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/blender/blender-original.svg"/> Blender</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/aftereffects/aftereffects-original.svg"/> After Effects</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/photoshop/photoshop-plain.svg"/> Photoshop</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/illustrator/illustrator-plain.svg"/> Illustrator</div>
</div>

### Monitoring • Observability

<div class="skill-grid" style="margin-top:12px">
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/prometheus/prometheus-original.svg"/> Prometheus</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/grafana/grafana-original.svg"/> Grafana</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/newrelic/newrelic-original.svg"/> New Relic</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/sentry/sentry-original.svg"/> Sentry</div>
</div>

### OS / Distros (massive list — add the ones you use)

<div class="skill-grid" style="margin-top:12px">
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/ubuntu/ubuntu-plain.svg"/> Ubuntu</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/debian/debian-original.svg"/> Debian</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/fedora/fedora-original.svg"/> Fedora</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/archlinux/archlinux-original.svg"/> Arch Linux</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/centos/centos-original.svg"/> CentOS</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/kali/kali-original.svg"/> Kali Linux</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/manjaro/manjaro-original.svg"/> Manjaro</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/raspberrypi/raspberrypi-original.svg"/> Raspberry Pi OS</div>
</div>

### More (CI, formats, helpers, messaging, and more) — selectively include what applies to you:

<div class="skill-grid" style="margin-top:12px">
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postman/postman-original.svg"/> Postman</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/swagger/swagger-original.svg"/> Swagger</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/redis/redis-original.svg"/> Redis</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mqtt/mqtt-original.svg"/> MQTT</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vscode/vscode-original.svg"/> VS Code</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/intellij/intellij-plain.svg"/> IntelliJ</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/visualstudio/visualstudio-plain.svg"/> Visual Studio</div>
  <div class="skill-pill"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cordova/cordova-original.svg"/> Cordova</div>
</div>

> ⚙️ This page lists ~120 entries if you expand with local logos. You can add many more; keep them organized by category. For a truly massive list, create additional sub-sections in the repo and reference them here.

---

## PROJECT ZONE — AESTHETIC SHOWCASE GRID

<div style="margin-top:8px" class="project-grid" id="projects">
  <!-- Example project card template: duplicate and update for each project -->
  <div class="project-card">
    <div style="display:flex; gap:8px; align-items:center;">
      <div style="width:52px; height:52px; border-radius:8px; background:#031a27; border:1px solid rgba(255,255,255,0.02); display:flex; align-items:center; justify-content:center">
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg" width="36"/>
      </div>
      <div style="flex:1">
        <div style="font-weight:800; color:#e6fbff">Project Nebula</div>
        <div style="font-size:13px; color:var(--muted)">A fullstack cyberpunk dashboard — realtime metrics, SVG galaxy and terminal UI.</div>
      </div>
    </div>

```
<div style="margin-top:10px; color:var(--muted); font-size:13px">
  <strong>Stack:</strong> React · Node · Docker · Kubernetes · Prometheus · Grafana<br/>
  <a class="glow-link" href="#">Repo • Live Demo • README</a>
</div>
```

  </div>

  <div class="project-card">
    <div style="display:flex; gap:8px; align-items:center;">
      <div style="width:52px; height:52px; border-radius:8px; background:#071427; display:flex; align-items:center; justify-content:center">
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" width="38"/>
      </div>
      <div style="flex:1">
        <div style="font-weight:800; color:#e6fbff">NetWeaver</div>
        <div style="font-size:13px; color:var(--muted)">A network visualization & automation toolkit with YAML playbooks and API-first design.</div>
      </div>
    </div>
    <div style="margin-top:10px; color:var(--muted); font-size:13px">
      <strong>Stack:</strong> Python · Ansible · Flask · Docker · Postgres<br/>
      <a class="glow-link" href="#">Repo • Documentation</a>
    </div>
  </div>

  <!-- Add real project cards below -->

</div>

---

## LINUX CORNER — TERMINAL STYLED & DISTRO GALLERY

<div style="margin-top:12px" class="terminal">
  <div class="prompt">andre@dyexahub:~$ <span style="color:#cfefff">ls -la /skills</span></div>
  <div style="margin-top:8px;">
    total 256
    <br/>drwxr-xr-x  20 andre staff  640 Nov 08 2025 .
    <br/>drwxr-xr-x  9 andre staff  288 Nov 08 2025 ..
    <br/>-rw-r--r--   1 andre staff  512 Nov 08 2025 kernel_habits.txt
  </div>
</div>

### Distro Rack

<div style="display:flex; gap:8px; margin-top:10px; flex-wrap:wrap;">
  <div style="padding:8px; border-radius:8px; background:#05121b; border:1px solid rgba(255,255,255,0.03)"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/ubuntu/ubuntu-plain.svg" width="24"/> Ubuntu</div>
  <div style="padding:8px; border-radius:8px; background:#05121b; border:1px solid rgba(255,255,255,0.03)"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/debian/debian-original.svg" width="24"/> Debian</div>
  <div style="padding:8px; border-radius:8px; background:#05121b; border:1px solid rgba(255,255,255,0.03)"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/archlinux/archlinux-original.svg" width="24"/> Arch</div>
  <div style="padding:8px; border-radius:8px; background:#05121b; border:1px solid rgba(255,255,255,0.03)"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/fedora/fedora-original.svg" width="24"/> Fedora</div>
  <div style="padding:8px; border-radius:8px; background:#05121b; border:1px solid rgba(255,255,255,0.03)"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/kali/kali-original.svg" width="24"/> Kali</div>
</div>

### Terminal Snippets (copyable)

```bash
# quick SSH tunnel
ssh -L 8080:localhost:8080 -N -f andre@remote.host

# snapshot of ip routes
ip route show

# docker cleanup
docker system prune -af
```

---

## NETWORK VISUALIZATION — CONNECTIVITY MAP (SVG)

> Inline SVG network map representing your topology. Replace nodes & labels with your real equipment if you wish.

<svg class="network-svg" viewBox="0 0 1000 420" preserveAspectRatio="xMidYMid meet" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Network Visualization">
  <defs>
    <linearGradient id="ng1" x1="0" x2="1"><stop offset="0" stop-color="#00f0ff"/><stop offset="1" stop-color="#ff3ec5"/></linearGradient>
    <filter id="gblur"><feGaussianBlur stdDeviation="6" /></filter>
  </defs>
  <rect width="100%" height="100%" rx="12" fill="#021423" />
  <!-- backbone -->
  <g transform="translate(80,40)">
    <!-- cloud -->
    <g>
      <ellipse cx="120" cy="40" rx="96" ry="34" fill="#031a24" stroke="#00f0ff" stroke-opacity="0.08"/>
      <text x="60" y="46" fill="#cfefff" font-size="12" font-weight="700">Internet</text>
    </g>

```
<!-- core router -->
<g transform="translate(360,30)">
  <rect x="0" y="0" width="160" height="50" rx="8" fill="#081427" stroke="#ff3ec5" stroke-opacity="0.12"/>
  <text x="12" y="32" fill="#dffaff" font-size="12" font-weight="800">Core Router</text>
  <text x="12" y="46" fill="#9aa4b2" font-size="10">ASN: 64512 • BGP</text>
</g>

<!-- links -->
<line x1="216" y1="46" x2="360" y2="46" stroke="url(#ng1)" stroke-opacity="0.12" stroke-width="2"/>

<!-- edge switches -->
<g transform="translate(560,10)">
  <rect x="0" y="0" width="120" height="44" rx="8" fill="#041424" stroke="#00f0ff" stroke-opacity="0.06"/>
  <text x="12" y="28" fill="#cfefff" font-size="11" font-weight="700">Edge Switch</text>
</g>

<line x1="520" y1="46" x2="560" y2="32" stroke="#00f0ff" stroke-opacity="0.06" stroke-width="1.6" />
```

  </g>

  <!-- end devices -->

  <g transform="translate(740,100)">
    <g transform="translate(0,0)">
      <rect x="0" y="0" width="84" height="52" rx="8" fill="#071a29" stroke="#8A3BFF" stroke-opacity="0.08"/>
      <text x="12" y="28" fill="#dffaff" font-size="11">Server A</text>
      <text x="12" y="44" fill="#9aa4b2" font-size="10">10.10.1.10</text>
    </g>

```
<g transform="translate(120,0)">
  <rect x="0" y="0" width="84" height="52" rx="8" fill="#071a29" stroke="#00F0FF" stroke-opacity="0.06"/>
  <text x="12" y="28" fill="#dffaff" font-size="11">VM Lab</text>
  <text x="12" y="44" fill="#9aa4b2" font-size="10">172.16.0.0/24</text>
</g>
```

  </g>
</svg>

---

## DEVOPS & CLOUD DASHBOARD — LIVE-ISH CARDS & PLACEHOLDERS

> Real interactive dashboards usually require JS and backends. Below are live-style badges, GitHub stats links, and placeholders you can wire to real services.

### GitHub Stats & Activity (examples — replace username)

<p>
  <img src="https://github-readme-stats.vercel.app/api?username=DyexaHub&show_icons=true&theme=dark&hide_border=true" alt="GitHub stats" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=DyexaHub&theme=dark&hide_border=true" alt="GitHub streak" />
</p>

> Replace `DyexaHub` in the URLs above with your actual GitHub username to show commit graphs and streaks. If GitHub blocks these images, self-host similar SVGs in your repo.

### Uptime / Health (badges)

<p>
  <img src="https://img.shields.io/website-up-down-green-red/https/dyexahub.dev?label=site%20uptime&style=for-the-badge" alt="uptime" />
  <img src="https://img.shields.io/badge/uptime-99.9%25-brightgreen?style=for-the-badge" alt="uptime-percent" />
  <img src="https://img.shields.io/badge/last%20deploy-2025--11--07-success?style=for-the-badge" alt="deploy" />
</p>

---

## UI/UX DESIGN ZONE — CREATIVE TOOLS & SHOWCASE

> Tools: Figma, Blender, After Effects, Photoshop, Illustrator, Principle, Framer, Protopie. Show screenshots, GIFs, or embed Lottie animations (host them in the repo).

<div style="display:flex; gap:8px; flex-wrap:wrap; margin-top:8px;">
  <div style="padding:10px; background:#041223; border-radius:10px; border:1px solid rgba(255,255,255,0.03)"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/figma/figma-original.svg" width="28"/> Figma</div>
  <div style="padding:10px; background:#041223; border-radius:10px; border:1px solid rgba(255,255,255,0.03)"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/blender/blender-original.svg" width="28"/> Blender</div>
  <div style="padding:10px; background:#041223; border-radius:10px; border:1px solid rgba(255,255,255,0.03)"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/aftereffects/aftereffects-original.svg" width="28"/> After Effects</div>
</div>

---

## MESSAGE FROM THE MACHINE — MANIFESTO CLOSING

<div style="margin-top:12px; padding:16px; border-radius:12px; background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.02)); border:1px solid rgba(255,255,255,0.03); color:#e6fbff">
  <h4 style="margin-top:0; margin-bottom:6px">💬 Message from the Machine</h4>
  <p style="margin:0; color:var(--muted)">I am not a single discipline. I am an ecosystem. I route packets with the same care as I design icons. I write automation to reduce friction, and interfaces to increase delight. I believe in resilient systems, audacious creativity, and learning that never sleeps. If you like neon, networks, and well-managed chaos — let's build a future that feels both inevitable and playful.</p>
  <p style="margin-top:10px; font-weight:800; color:#dffaff">— Andre (DyexaHub) • System Engineer • Creative Technologist</p>
</div>

---

## HOW TO USE / EDIT THIS README

1. Replace avatar image with `![avatar](./assets/avatar.png)` or your GitHub avatar link.
2. Replace placeholder SVG/PNG links with local images inside `assets/` for faster loads.
3. For the 3D / SVG gallery, update each `<image xlink:href="...">` to your repo path. e.g. `xlink:href="./assets/logos/python.svg"`.
4. For GitHub stats, replace the username in the `github-readme-stats` URL.
5. To expand to 100+ explicit badges: duplicate the `skill-pill` elements and add icons from `devicon` or your own local set.

---

## EXTRA MODULES / FUTURE ADD-ONS (templates)

> If you want, I can expand any of these modules into full sections in this README:

* 🎛️ **Live Terminal**: Embed a JS-free simulated terminal with animated SVG cursor. (Works as a visual demo only.)
* 🧭 **Tech Constellation**: Expand the SVG galaxy to include all 100+ logos arranged in orbital groups with labels.
* 📊 **Contribution Heatmap**: Include your raw GitHub contribution SVG (self-host recommended).
* 🔒 **Certs / Trophies**: Show Verified cert badges (CCNA, RHCSA, AWS certs) as neon trophies.
* 🧾 **Resume PDF**: Button that links to `resume.pdf` stored in repo for recruiters.
* 🤝 **Contact / Collab**: Interactive contact card (email, LinkedIn, portfolio) with copy-to-clipboard (JS needed; otherwise show plain links).

---

## LICENSE & NOTES

This README is licensed for personal use and modification. Credit is appreciated if you reuse whole sections.

---

### Final words

This file is already a dense, neon-saturated canvas — but it thrives with your real assets. Replace images and tweak colors to make it truly yours. Want me to expand a specific section into a 500–1000 line *fully populated* version (eg. 200 real projects, 200+ badges, complex SVG galaxy with coordinate mapping)? Tell me which section to explode next and I’ll generate straight away — inline and ready for paste.

— Andre (DyexaHub) // README generator (chaos-enabled) ✨
