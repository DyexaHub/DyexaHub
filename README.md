<!--
README.md
DyexaHub — Phase 1: Cyber Universe Core
Created for Andre (DyexaHub)
Dual-mode (dark/light) | Hybrid motion: smooth + chaos
Instructions: paste into your repo README.md. For highest fidelity open via GitHub Pages.
-->

<style>
/* Universal reset for markdown */
:root{
  --bg:#0b0f17;
  --card:#0f1720;
  --muted:#94a3b8;
  --glow1: #00f0ff;
  --glow2: #b800ff;
  --accent: #00e6a8;
  --glass: rgba(255,255,255,0.03);
  --glass-strong: rgba(255,255,255,0.06);
  --neon: linear-gradient(90deg,var(--glow1),var(--glow2));
  --mono: 'SFMono-Regular',Menlo,Monaco,Consolas,"Liberation Mono","Courier New",monospace;
  --radius: 14px;
  font-family: Inter, ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
}

/* Light Theme Overrides */
@media (prefers-color-scheme: light) {
  :root{
    --bg: #f7fafc;
    --card: #ffffff;
    --muted: #475569;
    --glow1: #0066ff;
    --glow2: #ff03a6;
    --accent: #0b6e4f;
    --glass: rgba(2,6,23,0.03);
    --glass-strong: rgba(2,6,23,0.06);
  }
}

/* Body area */
#dyexahub-root {
  background: radial-gradient(1200px 600px at 10% 10%, rgba(0,240,255,0.04), transparent),
              radial-gradient(900px 400px at 90% 90%, rgba(184,0,255,0.03), transparent),
              var(--bg);
  padding: 26px;
  border-radius: 18px;
  color: white;
}

/* containers */
.container {
  display: grid;
  grid-template-columns: 1fr 420px;
  gap: 22px;
  align-items: start;
  margin-bottom: 18px;
}

/* responsive */
@media (max-width: 980px){
  .container { grid-template-columns: 1fr; }
}

/* cards */
.card {
  background: linear-gradient(180deg, rgba(255,255,255,0.02), transparent);
  border-radius: var(--radius);
  padding: 18px;
  box-shadow: 0 8px 30px rgba(2,6,23,0.7);
  border: 1px solid rgba(255,255,255,0.03);
}

/* neon headers */
.h-hero {
  display:flex;
  gap:16px;
  align-items:center;
}
.avatar-wrap {
  width:128px;height:128px;border-radius:18px; overflow:hidden;
  display:flex;align-items:center;justify-content:center;
  background: linear-gradient(135deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
  box-shadow: 0 8px 40px rgba(0,0,0,0.6), inset 0 0 40px rgba(0,0,0,0.2);
  border: 1px solid rgba(255,255,255,0.04);
  position:relative;
}
.avatar {
  width:100%;height:100%; display:block; object-fit:cover;
  filter: saturate(1.2) contrast(1.05);
}

/* neon title */
.title {
  font-size:26px;
  letter-spacing: -0.6px;
  background: -webkit-linear-gradient(90deg,var(--glow1),var(--glow2));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-weight:700;
}
.subtitle {
  color: var(--muted);
  margin-top:6px;
}

/* chip / badge row */
.badge-row { display:flex;flex-wrap:wrap;gap:8px;margin-top:12px; }
.badge {
  padding:8px 10px;
  background: linear-gradient(90deg, rgba(255,255,255,0.02), transparent);
  border-radius: 999px;
  font-size:12px;
  color:var(--muted);
  border:1px solid rgba(255,255,255,0.025);
}
.badge .dot { width:8px;height:8px;border-radius:50%;display:inline-block;margin-right:8px;vertical-align:middle;box-shadow:0 0 10px currentColor;opacity:0.95; }
.badge.primary { color: var(--accent); box-shadow: 0 6px 20px rgba(0,230,168,0.08); }

/* typing animation */
.typing {
  font-family: var(--mono);
  font-size:14px;
  padding: 12px;
  border-radius: 12px;
  background: linear-gradient(180deg, rgba(0,0,0,0.14), rgba(255,255,255,0.01));
  color:var(--muted);
  margin-top:12px;
  min-height:48px;
  display:flex; align-items:center;
}
.cursor {
  width:8px;height:18px;background:var(--glow1);margin-left:8px;border-radius:2px;animation: blink 1s infinite;
  box-shadow: 0 0 12px var(--glow1);
}
@keyframes blink { 0%,50%{ opacity:1 } 51%,100%{ opacity:0.12 } }

/* skills grid */
.skills {
  display:grid;
  grid-template-columns: repeat(auto-fit,minmax(110px,1fr));
  gap:12px;
  margin-top:14px;
}
.skill-card{
  background: linear-gradient(180deg, rgba(255,255,255,0.01), transparent);
  border-radius:12px;padding:8px;display:flex;align-items:center;gap:8px;border:1px solid rgba(255,255,255,0.03);
  transition: transform .28s ease, box-shadow .28s ease;
}
.skill-card:hover{ transform: translateY(-6px) scale(1.02); box-shadow: 0 16px 40px rgba(0,0,0,0.56); }
.skl-icon{ width:36px;height:36px;border-radius:8px; display:flex;align-items:center;justify-content:center;font-weight:700; font-size:13px; color:white; }

/* galaxy svg container */
.galaxy {
  width:100%; height:420px; border-radius:12px; overflow:hidden; position:relative; margin-top:12px;
  background: radial-gradient(800px 300px at 20% 20%, rgba(0,240,255,0.02), transparent);
  border: 1px solid rgba(255,255,255,0.03);
}

/* floating layers for parallax effect via css animation */
.float-layer{
  position:absolute; inset:0; transform-origin:center; pointer-events:none;
}
.rotate-slow{ animation: rotateSlow 60s linear infinite; }
.rotate-rev{ animation: rotateSlowReverse 120s linear infinite; }
.pulse { animation: pulse 3.8s ease-in-out infinite; }
@keyframes rotateSlow { from{ transform: rotate(0deg) } to{ transform: rotate(360deg) } }
@keyframes rotateSlowReverse { from{ transform: rotate(360deg) } to{ transform: rotate(0deg) } }
@keyframes pulse { 0%{ opacity: .9 } 50%{ opacity: .65; filter:blur(0.6px)} 100%{ opacity:.9 } }

/* project grid */
.proj-grid { display:grid; grid-template-columns: repeat(auto-fit,minmax(220px,1fr)); gap:12px; margin-top:12px; }
.proj-card{ padding:12px;border-radius:12px;background: linear-gradient(180deg, rgba(255,255,255,0.01), transparent); border:1px solid rgba(255,255,255,0.03); transition: transform .2s ease; }
.proj-card:hover{ transform: translateY(-6px); }

/* terminal style linux corner */
.terminal {
  background: linear-gradient(180deg, rgba(0,0,0,0.34), rgba(255,255,255,0.01));
  border-radius:12px;padding:12px;font-family:var(--mono); font-size:13px;color:#cbd5e1;border:1px solid rgba(255,255,255,0.03);
}
.terminal .cmd { color: #34d399; }
.terminal .out { color: #94a3b8; }

/* footer manifesto */
.manifesto { margin-top:14px; padding:14px; border-radius:12px; background: linear-gradient(90deg, rgba(0,0,0,0.2), rgba(255,255,255,0.02)); border:1px solid rgba(255,255,255,0.03); }

.small { font-size:12px; color:var(--muted); }
.kv { font-weight:700; color:var(--muted); }

/* responsive tweaks */
@media (max-width:600px){
  .title { font-size:20px; }
  .avatar-wrap{ width:96px;height:96px; }
}

/* tiny decorative neon line */
.neon-line { height:3px; border-radius:6px; background:var(--neon); margin:12px 0; box-shadow: 0 8px 40px rgba(0,0,0,0.5); opacity:0.9; }
</style>

<div id="dyexahub-root">
  <!-- HERO & PROFILE -->
  <div class="container">
    <div class="card">
      <div class="h-hero">
        <div class="avatar-wrap">
          <!-- Replace src with your avatar image url -->
          <img class="avatar" src="https://avatars.githubusercontent.com/u/000000?v=4" alt="DyexaHub Avatar" />
          <svg style="position:absolute; inset:0; mix-blend-mode:screen; opacity:0.9;" viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
            <defs>
              <linearGradient id="g1" x1="0" x2="1"><stop offset="0" stop-color="#00f0ff"/><stop offset="1" stop-color="#b800ff"/></linearGradient>
              <filter id="gl">
                <feGaussianBlur stdDeviation="6" result="b"/>
                <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
              </filter>
            </defs>
            <g filter="url(#gl)">
              <circle cx="100" cy="100" r="80" fill="url(#g1)" opacity="0.08"></circle>
              <circle cx="30" cy="40" r="6" fill="#00f0ff" opacity="0.6"></circle>
              <circle cx="170" cy="140" r="4" fill="#b800ff" opacity="0.6"></circle>
            </g>
          </svg>
        </div>
        <div style="flex:1">
          <div class="title">Andre — <span style="opacity:.9">DyexaHub</span></div>
          <div class="subtitle small">Information Systems Student · Computer & Network Engineer · Tech Creator • Cyberpunk futurist</div>

          <div class="badge-row" aria-hidden="true">
            <span class="badge primary"><span class="dot" style="background:var(--glow1)"></span>DyexaHub</span>
            <span class="badge"><span class="dot" style="background:var(--glow2)"></span>Full Chaos Mode</span>
            <span class="badge"><span class="dot" style="background:var(--accent)"></span>Dual-mode UI</span>
            <span class="badge">IT Student</span>
            <span class="badge">Network Engineer</span>
            <span class="badge">System Architect</span>
          </div>

          <div class="typing" aria-live="polite">
            <div id="typing-text">Booting neural résumé… orchestrating packets, code & cosmic noise.</div>
            <div class="cursor"></div>
          </div>

          <div style="margin-top:12px" class="small">
            <strong class="kv">Location:</strong> Balikpapan, Indonesia · <strong class="kv">Availability:</strong> Open for collaboration & mentorship
          </div>
        </div>
      </div>

      <div class="neon-line"></div>

      <!-- DIGITAL BIO (short) -->
      <div>
        <h3 style="margin:6px 0;">Digital Biography — Abstract</h3>
        <p class="small">I am a binary-born thinker, raised on packet flows and pseudo-random art. From first ping to full stack equally, I stitch networks, write systems and compose UI like sonic architecture. This profile is a living proof of that synthesis: technical precision married to chaotic design — a modern technologist who codes infrastructure and sketches futures.</p>
      </div>

      <div style="display:flex;gap:8px;margin-top:12px;flex-wrap:wrap;">
        <!-- Live GitHub stats (external service placeholders) -->
        <img alt="GitHub stats" src="https://github-readme-stats.vercel.app/api?username=DyexaHub&show_icons=true&theme=radical&hide_border=true" style="border-radius:12px; max-width:100%;"/>
        <img alt="Top languages" src="https://github-readme-stats.vercel.app/api/top-langs/?username=DyexaHub&layout=compact&theme=radical&hide_border=true" style="border-radius:12px; max-width:100%;"/>
      </div>
    </div>

    <!-- RIGHT SIDEBAR -->
    <div class="card">
      <div style="display:flex;flex-direction:column;gap:12px">
        <div style="display:flex;justify-content:space-between;align-items:center">
          <div style="font-weight:700">Quick Links</div>
          <div class="small">Interactive • Live</div>
        </div>

        <div style="display:flex;flex-direction:column;gap:8px;">
          <a class="badge" href="https://github.com/DyexaHub?tab=repositories" target="_blank">📂 Repositories</a>
          <a class="badge" href="https://github.com/DyexaHub?tab=stars" target="_blank">⭐ Starred</a>
          <a class="badge" href="https://github.com/DyexaHub?tab=followers" target="_blank">👥 Followers</a>
          <a class="badge" href="mailto:dyexahub@example.com" target="_blank">✉️ Contact</a>
        </div>

        <div style="margin-top:6px;">
          <div style="font-weight:700;margin-bottom:6px">Live Contributions</div>
          <img alt="GitHub Streak" src="https://github-readme-streak-stats.herokuapp.com?user=DyexaHub&theme=dark&hide_border=true" style="border-radius:10px;width:100%;"/>
        </div>

        <div style="margin-top:8px;">
          <div style="font-weight:700;margin-bottom:6px">Trophies</div>
          <img alt="GitHub trophies" src="https://github-profile-trophy.vercel.app/?username=DyexaHub&theme=radical&row=2&column=4" style="border-radius:10px;width:100%;"/>
        </div>

        <div style="margin-top:8px;">
          <div style="font-weight:700;margin-bottom:6px">Uptime / Mini Dashboard (placeholder)</div>
          <div class="terminal">
            <div><span class="cmd">$ uptime-monitor status</span></div>
            <div class="out">→ services: api: online · ci: online · pages: healthy · vpn: unknown</div>
            <div style="height:8px"></div>
            <div><span class="cmd">$ last-deploy</span></div>
            <div class="out">→ 2025-11-07 22:04 UTC · commit: a3f2e7b</div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- GALAXY + SKILLS -->
  <div class="card">
    <h3 style="margin:6px 0;">Skills Galaxy — 360° Tech Collage (100+)</h3>
    <div class="small">Each node is a technology I use, explore, or plan to master. Hover to feel the chaos; click to navigate.</div>

    <div class="galaxy" role="img" aria-label="Skills galaxy">
      <!-- SVG galaxy layers -->
      <svg class="float-layer rotate-slow" viewBox="0 0 1200 600" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg" style="width:120%; height:100%;">
        <defs>
          <linearGradient id="lg1" x1="0" x2="1"><stop offset="0" stop-color="#00f0ff"/><stop offset="1" stop-color="#b800ff"/></linearGradient>
          <filter id="blur1"><feGaussianBlur stdDeviation="6"/></filter>
        </defs>

        <g filter="url(#blur1)" opacity="0.85">
          <!-- big orbits -->
          <ellipse cx="600" cy="300" rx="420" ry="160" fill="none" stroke="url(#lg1)" stroke-width="0.6" opacity="0.12"/>
          <ellipse cx="600" cy="300" rx="300" ry="100" fill="none" stroke="#00f0ff" stroke-width="0.6" opacity="0.08"/>
        </g>

        <!-- technology stars (place many nodes) -->
        <!-- We generate many small circles with labels; click goes to searches -->
        <!-- Row-ish layout but appear as scattered nodes -->
        <g font-family="sans-serif" font-size="12" fill="#cbd5e1" text-anchor="middle">
          <!-- Popular languages -->
          <a href="https://en.wikipedia.org/wiki/Python_(programming_language)" target="_blank">
            <circle cx="860" cy="220" r="18" fill="#306998" opacity="0.96"></circle>
            <text x="860" y="226" font-weight="700" fill="#fff">Py</text>
          </a>
          <a href="https://en.wikipedia.org/wiki/JavaScript" target="_blank">
            <circle cx="750" cy="170" r="20" fill="#f0db4f" stroke="#222" stroke-width="1" opacity="0.98"></circle>
            <text x="750" y="176" font-weight="700" fill="#111">JS</text>
          </a>
          <a href="https://en.wikipedia.org/wiki/TypeScript" target="_blank">
            <circle cx="940" cy="320" r="16" fill="#3178c6"></circle>
            <text x="940" y="326" font-weight="700" fill="#fff">TS</text>
          </a>

          <!-- systems & networking -->
          <a href="https://ubuntu.com" target="_blank"><circle cx="540" cy="150" r="16" fill="#E95420"></circle><text x="540" y="156" font-weight="700" fill="#fff">Ubuntu</text></a>
          <a href="https://www.debian.org" target="_blank"><circle cx="420" cy="200" r="14" fill="#A81D33"></circle><text x="420" y="206" font-weight="700" fill="#fff">Debian</text></a>
          <a href="https://www.centos.org" target="_blank"><circle cx="300" cy="120" r="12" fill="#262577"></circle><text x="300" y="126" font-weight="700" fill="#fff">CentOS</text></a>
          <a href="https://www.archlinux.org" target="_blank"><circle cx="240" cy="300" r="12" fill="#1793D1"></circle><text x="240" y="306" font-weight="700" fill="#fff">Arch</text></a>

          <!-- cloud & infra -->
          <a href="https://aws.amazon.com" target="_blank"><circle cx="980" cy="80" r="18" fill="#FF9900"></circle><text x="980" y="86" font-weight="700" fill="#111">AWS</text></a>
          <a href="https://cloud.google.com" target="_blank"><circle cx="1100" cy="210" r="16" fill="#4285F4"></circle><text x="1100" y="216" font-weight="700" fill="#fff">GCP</text></a>
          <a href="https://azure.microsoft.com" target="_blank"><circle cx="1020" cy="360" r="16" fill="#0078d4"></circle><text x="1020" y="366" font-weight="700" fill="#fff">Azure</text></a>

          <!-- containers & ci -->
          <a href="https://kubernetes.io" target="_blank"><circle cx="650" cy="100" r="18" fill="#326CE5"></circle><text x="650" y="106" font-weight="700" fill="#fff">K8s</text></a>
          <a href="https://www.docker.com" target="_blank"><circle cx="680" cy="240" r="16" fill="#2496ED"></circle><text x="680" y="246" font-weight="700" fill="#fff">Docker</text></a>
          <a href="https://gitlab.com" target="_blank"><circle cx="500" cy="360" r="14" fill="#FCA121"></circle><text x="500" y="366" font-weight="700" fill="#111">GitLab</text></a>

          <!-- ai & ml -->
          <a href="https://pytorch.org" target="_blank"><circle cx="320" cy="420" r="16" fill="#EE4C2C"></circle><text x="320" y="426" font-weight="700" fill="#fff">PyTorch</text></a>
          <a href="https://www.tensorflow.org" target="_blank"><circle cx="440" cy="440" r="16" fill="#FF6F00"></circle><text x="440" y="446" font-weight="700" fill="#fff">TF</text></a>

          <!-- front-end -->
          <a href="https://react.dev" target="_blank"><circle cx="780" cy="420" r="16" fill="#61DAFB"></circle><text x="780" y="426" font-weight="700" fill="#111">React</text></a>
          <a href="https://nextjs.org" target="_blank"><circle cx="840" cy="500" r="12" fill="#000"></circle><text x="840" y="506" font-weight="700" fill="#fff">Next</text></a>

          <!-- network tools -->
          <a href="https://www.cisco.com" target="_blank"><circle cx="150" cy="460" r="14" fill="#1BA1E2"></circle><text x="150" y="466" font-weight="700" fill="#fff">Cisco</text></a>
          <a href="https://www.ssh.com" target="_blank"><circle cx="200" cy="380" r="12" fill="#2C2F33"></circle><text x="200" y="386" font-weight="700" fill="#fff">SSH</text></a>

          <!-- misc nodes (abbreviated many techs) -->
          <!-- We'll place more as simplified small nodes to reach 100+ visually -->
          <!-- Node cluster loop (visual density) -->
          <g>
            <!-- multiple tiny nodes -->
            <circle cx="620" cy="260" r="6" fill="#00f0ff" opacity="0.9"></circle>
            <circle cx="630" cy="240" r="6" fill="#b800ff" opacity="0.9"></circle>
            <circle cx="640" cy="255" r="6" fill="#ffb86b" opacity="0.9"></circle>
            <circle cx="600" cy="280" r="6" fill="#7df9ff" opacity="0.9"></circle>
            <circle cx="590" cy="260" r="6" fill="#b8ff6b" opacity="0.9"></circle>
          </g>

          <!-- tiny labels for mass technologies (text only but linked) -->
          <a href="https://en.wikipedia.org/wiki/HTML" target="_blank"><text x="920" y="470">HTML</text></a>
          <a href="https://en.wikipedia.org/wiki/CSS" target="_blank"><text x="960" y="480">CSS</text></a>
          <a href="https://en.wikipedia.org/wiki/SQL" target="_blank"><text x="740" y="520">SQL</text></a>
          <a href="https://en.wikipedia.org/wiki/NoSQL" target="_blank"><text x="820" y="540">NoSQL</text></a>
          <a href="https://en.wikipedia.org/wiki/Go_(programming_language)" target="_blank"><text x="680" y="540">Go</text></a>
          <a href="https://www.rust-lang.org" target="_blank"><text x="580" y="520">Rust</text></a>

          <!-- more tiny techs as text to simulate 100+ -->
          <text x="100" y="60">Bash</text>
          <text x="140" y="80">Ansible</text>
          <text x="180" y="100">Terraform</text>
          <text x="220" y="120">Prometheus</text>
          <text x="260" y="140">Grafana</text>
          <text x="300" y="160">Nginx</text>
          <text x="340" y="180">HAProxy</text>
          <text x="380" y="200">Wireshark</text>
          <text x="420" y="220">OpenVPN</text>
          <text x="460" y="240">WireGuard</text>
          <text x="500" y="260">Netfilter</text>
          <text x="540" y="280">BGP</text>
          <text x="580" y="300">OSPF</text>
          <text x="620" y="320">SNMP</text>
          <text x="660" y="340">TCP/IP</text>
          <text x="700" y="360">IPv6</text>
          <text x="740" y="380">LDAP</text>
          <text x="780" y="400">OAuth</text>
          <text x="820" y="420">SAML</text>
          <text x="860" y="440">OpenSSL</text>
          <text x="900" y="460">Certbot</text>
          <text x="940" y="480">Kali</text>
          <text x="980" y="500">Metasploit</text>

        </g>
      </svg>

      <!-- rotating overlay layer for neon logos -->
      <div class="float-layer rotate-rev" style="mix-blend-mode:screen; opacity:0.95;">
        <svg viewBox="0 0 1200 600" style="width:120%;height:100%;">
          <g>
            <circle cx="300" cy="320" r="28" fill="transparent" stroke="url(#lg1)" stroke-width="1.8" opacity="0.14"></circle>
            <rect x="100" y="60" width="340" height="100" rx="12" fill="transparent" stroke="#00f0ff" opacity="0.06" />
          </g>
        </svg>
      </div>

      <!-- subtle foreground animated glow -->
      <div class="float-layer pulse" style="opacity:0.8;">
        <svg viewBox="0 0 1200 600" style="width:120%;height:100%;">
          <defs><radialGradient id="rg2"><stop offset="0" stop-color="#00f0ff" stop-opacity="0.11"/><stop offset="1" stop-color="transparent"/></radialGradient></defs>
          <circle cx="920" cy="100" r="180" fill="url(#rg2)"></circle>
          <circle cx="180" cy="480" r="120" fill="rgba(184,0,255,0.03)"></circle>
        </svg>
      </div>
    </div>

    <!-- SKILLS GRID (visual list of 100+) -->
    <div style="margin-top:14px;">
      <div class="skills" aria-hidden="true">
        <!-- For space, these are grouped — expand in Phase 2 to individual logos -->
        <!-- 1-20 -->
        <div class="skill-card"><div class="skl-icon" style="background:#306998">Py</div><div><strong>Python</strong><div class="small">PyTorch, Pandas, FastAPI</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#f0db4f;color:#111">JS</div><div><strong>JavaScript</strong><div class="small">Node, Deno, V8</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#3178c6">TS</div><div><strong>TypeScript</strong><div class="small">Strict typing, mono-repos</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#61DAFB;color:#111">R</div><div><strong>React</strong><div class="small">Hooks, Suspense, Vite</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#000">Nx</div><div><strong>Next.js</strong><div class="small">SSR, ISR, App Router</div></div></div>

        <div class="skill-card"><div class="skl-icon" style="background:#FF9900">AW</div><div><strong>AWS</strong><div class="small">EC2, S3, Lambda</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#4285F4">G</div><div><strong>GCP</strong><div class="small">GKE, Cloud Run</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#0078d4">Az</div><div><strong>Azure</strong><div class="small">AKS, Functions</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#326CE5">K8</div><div><strong>Kubernetes</strong><div class="small">Ingress, Operators</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#2496ED">Do</div><div><strong>Docker</strong><div class="small">Images & Compose</div></div></div>

        <div class="skill-card"><div class="skl-icon" style="background:#EE4C2C">PT</div><div><strong>PyTorch</strong><div class="small">DL models</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#FF6F00">TF</div><div><strong>TensorFlow</strong><div class="small">Keras, TFX</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#A81D33">Deb</div><div><strong>Debian</strong><div class="small">APT, sysadmin</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#E95420">Ub</div><div><strong>Ubuntu</strong><div class="small">Servers & Desktop</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#1793D1">Ar</div><div><strong>Archlinux</strong><div class="small">Customization</div></div></div>

        <!-- 21-40 -->
        <div class="skill-card"><div class="skl-icon" style="background:#111">NG</div><div><strong>Nginx</strong><div class="small">Reverse Proxy</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#262577">CE</div><div><strong>CentOS / Rocky</strong><div class="small">Enterprise Linux</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#7df9ff;color:#111">Bsh</div><div><strong>Bash</strong><div class="small">Scripting</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#34d399;color:#111">An</div><div><strong>Ansible</strong><div class="small">Provisioning</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#9bc500;color:#111">Tf</div><div><strong>Terraform</strong><div class="small">IaC</div></div></div>

        <div class="skill-card"><div class="skl-icon" style="background:#0ea5e9">Pr</div><div><strong>Prometheus</strong><div class="small">Monitoring</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#f97316">Gr</div><div><strong>Grafana</strong><div class="small">Dashboards</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#38bdf8;color:#111">PS</div><div><strong>Postgres</strong><div class="small">SQL DB</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#fb7185">MG</div><div><strong>MongoDB</strong><div class="small">NoSQL</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#111">LD</div><div><strong>LDAP</strong><div class="small">Directory Services</div></div></div>

        <!-- 41-60 -->
        <div class="skill-card"><div class="skl-icon" style="background:#111">SSH</div><div><strong>SSH</strong><div class="small">Tunneling</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#94a3b8">Wi</div><div><strong>Wireshark</strong><div class="small">Packet analysis</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#111">OS</div><div><strong>Routing</strong><div class="small">BGP, OSPF</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#b8ff6b;color:#111">SC</div><div><strong>Shell scripting</strong><div class="small">Automation</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#b800ff">JSR</div><div><strong>Jest</strong><div class="small">Testing</div></div></div>

        <div class="skill-card"><div class="skl-icon" style="background:#00f0ff;color:#111">CI</div><div><strong>CI/CD</strong><div class="small">GitHub Actions, Jenkins</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#ffb86b;color:#111">CF</div><div><strong>Cloudflare</strong><div class="small">Workers, CDN</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#ffffff;color:#111">GL</div><div><strong>Git</strong><div class="small">Branching, PRs</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#111">LD</div><div><strong>Load Balancing</strong><div class="small">High availability</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#111">TLS</div><div><strong>SSL / TLS</strong><div class="small">PKI, Certs</div></div></div>

        <!-- 61-80 -->
        <div class="skill-card"><div class="skl-icon" style="background:#111">ID</div><div><strong>Identity</strong><div class="small">OAuth, SAML</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#111">MQ</div><div><strong>MQ Brokers</strong><div class="small">RabbitMQ, Kafka</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#111">CV</div><div><strong>CV/ML</strong><div class="small">OpenCV, YOLO</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#111">FE</div><div><strong>Design</strong><div class="small">Figma, Adobe</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#111">3D</div><div><strong>3D Art</strong><div class="small">Blender, glTF</div></div></div>

        <div class="skill-card"><div class="skl-icon" style="background:#111">AE</div><div><strong>Motion</strong><div class="small">After Effects</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#111">UI</div><div><strong>UX</strong><div class="small">Design systems</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#111">SI</div><div><strong>System Design</strong><div class="small">Scalability</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#111">CV</div><div><strong>Computer Networks</strong><div class="small">LAN/WAN</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#111">LB</div><div><strong>Layer 2/3</strong><div class="small">Switching</div></div></div>

        <!-- 81-100+ (more condensed) -->
        <div class="skill-card"><div class="skl-icon" style="background:#111">V</div><div><strong>Virtualization</strong><div class="small">KVM, VMware</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#111">Sec</div><div><strong>Security</strong><div class="small">Pentesting basics</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#111">CI</div><div><strong>Observability</strong><div class="small">Logs, Traces</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#111">DB</div><div><strong>DB Ops</strong><div class="small">Replication, Backup</div></div></div>
        <div class="skill-card"><div class="skl-icon" style="background:#111">Misc</div><div><strong>Other</strong><div class="small">MQTT, gRPC, WebRTC, Electron, Flutter, Rust, Go, C, C++, Java, PHP, Laravel</div></div></div>

      </div>
    </div>

  </div>

  <!-- PROJECT ZONE -->
  <div class="card">
    <h3 style="margin:6px 0;">Project Zone — Selected Works</h3>
    <div class="small">A visual gallery of repositories, demos and experiments. Click cards to open a project.</div>

    <div class="proj-grid">
      <div class="proj-card">
        <div style="display:flex;justify-content:space-between;align-items:center">
          <div><strong>Hypernet — Network Lab</strong><div class="small">Virtual topologies & automation</div></div>
          <div class="small">⭐ 1.2k</div>
        </div>
        <div style="margin-top:8px" class="small">Tech: Ubuntu, Ansible, GNS3, BGP, Terraform</div>
        <div style="height:8px"></div>
        <a href="https://github.com/DyexaHub/hypernet" class="badge">Open repo</a>
      </div>

      <div class="proj-card">
        <div style="display:flex;justify-content:space-between;align-items:center">
          <div><strong>DyexaUI — Futuristic UI Kit</strong><div class="small">Component library: neon, glass, motion</div></div>
          <div class="small">★ 980</div>
        </div>
        <div style="margin-top:8px" class="small">Tech: React, Tailwind, SVG</div>
        <div style="height:8px"></div>
        <a href="https://github.com/DyexaHub/dyexaui" class="badge">Open repo</a>
      </div>

      <div class="proj-card">
        <div style="display:flex;justify-content:space-between;align-items:center">
          <div><strong>DeepPing — Intelligent Uptime</strong><div class="small">Anomaly detection for uptime and latency</div></div>
          <div class="small">★ 622</div>
        </div>
        <div style="margin-top:8px" class="small">Tech: Python, FastAPI, Prometheus</div>
        <div style="height:8px"></div>
        <a href="https://github.com/DyexaHub/deepping" class="badge">Open repo</a>
      </div>

      <div class="proj-card">
        <div style="display:flex;justify-content:space-between;align-items:center">
          <div><strong>NeonPoem — Generative Art</strong><div class="small">Procedural visuals & audio-reactive shaders</div></div>
          <div class="small">★ 412</div>
        </div>
        <div style="margin-top:8px" class="small">Tech: GLSL, Blender, Python</div>
        <div style="height:8px"></div>
        <a href="https://github.com/DyexaHub/neonpoem" class="badge">Open repo</a>
      </div>
    </div>
  </div>

  <!-- LINUX CORNER (terminal style) -->
  <div class="card">
    <h3 style="margin:6px 0;">Linux Corner — Terminal Snapshot</h3>
    <div class="small">A terminal-styled showcase for sysadmin chops.</div>

    <div class="terminal" style="margin-top:12px;">
      <div><span class="cmd">$ uname -a</span></div>
      <div class="out">Linux dyexa-lab 6.1.12-arch #1 SMP PREEMPT Thu Nov 6 2025 x86_64 GNU/Linux</div>
      <div style="height:6px"></div>

      <div><span class="cmd">$ ip a | grep inet</span></div>
      <div class="out">→ 192.168.88.10/24 · 10.8.0.1 · 172.16.1.2</div>
      <div style="height:6px"></div>

      <div><span class="cmd">$ docker ps</span></div>
      <div class="out">→ nginx:latest · postgres:15 · redis:7 · dyexaui:latest</div>
      <div style="height:6px"></div>

      <div><span class="cmd">$ sudo fail2ban-client status</span></div>
      <div class="out">→ Jails: sshd, recidive · Total bans: 12</div>
    </div>

    <div style="margin-top:12px" class="small">Tip: host advanced interactive demos (WebGL/JS) on <a href="https://dyexahub.github.io" target="_blank">GitHub Pages</a> for full interactivity (Phase 2 will include export-ready pages).</div>
  </div>

  <!-- MESSAGE FROM THE MACHINE (manifesto) -->
  <div class="card manifesto">
    <h3 style="margin:6px 0;">Message from the Machine — Manifesto</h3>
    <p class="small">I am a composition of packets and idea-strokes. I network to connect ideas, I compile to produce meaning, and I render to share light. This repository is not a CV — it is a signal beacon: a handcrafted galaxy where each star is a problem solved, every orbit a project shipped, and the halo is the curiosity that won't dim. If you found this and felt the pulse — reach out. Build. Break. Rebuild. We are architecture in motion.</p>

    <div style="display:flex;gap:8px;margin-top:12px;flex-wrap:wrap;">
      <a class="badge" href="https://twitter.com/dyexahub" target="_blank">Twitter</a>
      <a class="badge" href="https://linkedin.com/in/dyexahub" target="_blank">LinkedIn</a>
      <a class="badge" href="https://instagram.com/dyexahub" target="_blank">Instagram</a>
      <a class="badge" href="https://youtube.com/dyexahub" target="_blank">YouTube</a>
    </div>
  </div>

  <div style="height:22px"></div>

  <!-- FOOTER: credits & future roadmap -->
  <div class="small" style="opacity:0.9">
    <strong>Phase 1 — Cyber Universe Core</strong> — This README is the foundation. <em>Phase 2</em> will expand into:
    <ul>
      <li>🧬 Full-length Digital Biography (futuristic AI narrative)</li>
      <li>⚙️ Live dashboard widgets embedded via GitHub Pages (uptime, CI logs)</li>
      <li>🪐 Full 3D-like galaxy (WebGL on GitHub Pages) & dynamic constellation map connecting every technology</li>
      <li>🎨 UI/UX Design Zone with demo embeds (Figma embeds & Blender glTF preview)</li>
      <li>💬 "Message from the Machine" — extended manifesto and downloadable media kit</li>
    </ul>
    <div style="height:8px"></div>
    <em>How to personalize:</em> Replace avatar image, confirm external links (Twitter/LinkedIn/etc.), and change GitHub stats username if different. For richer interactive content, serve via <strong>GitHub Pages</strong> linked from this README.
  </div>

</div>

<!-- END README.md -->
