<!--
  DyexaHub — "Full Chaos Mode" GitHub README (Phase 1)
  Single-file README.md — Dual-mode (dark/light) — Inline SVG + Live widgets
  Author: Andre (DyexaHub) — Information Systems Student · Computer & Network Engineer · Tech Creator
-->

<!-- ===========================
     HEADER: Neon Cyber Hero
     Uses inline SVG (animated) — works as image on GitHub
   =========================== -->

<p align="center">
  <!-- Data-URI SVG hero — keep it compact but expressive. -->
  <img alt="DyexaHub Cyber Hero" src='data:image/svg+xml;utf8,
  <svg xmlns="http://www.w3.org/2000/svg" width="980" height="260" viewBox="0 0 980 260">
    <defs>
      <linearGradient id="gA" x1="0" x2="1">
        <stop offset="0" stop-color="%2306f"/>
        <stop offset="1" stop-color="%23b95cff"/>
      </linearGradient>
      <filter id="glow" x="-20%" y="-20%" width="140%" height="140%">
        <feGaussianBlur stdDeviation="6" result="coloredBlur"/>
        <feMerge>
          <feMergeNode in="coloredBlur"/>
          <feMergeNode in="SourceGraphic"/>
        </feMerge>
      </filter>
      <style><![CDATA[
        .bg { fill: #0b0d10; }
        .panel { fill: url(%23gA); opacity: .12; }
        .title { font-family: Inter, Roboto, Arial, sans-serif; font-size: 36px; fill: white; font-weight: 700; }
        .subtitle { font-family: Inter, Roboto, Arial, sans-serif; font-size: 12.5px; fill: #d6d6d6; }
        .neon { filter: url(%23glow); }
        .ty { font-family: "Source Code Pro", monospace; font-size: 14px; fill: #bfe9ff; }
      ]]></style>
    </defs>

    <rect width="100%" height="100%" class="bg"/>
    <rect x="18" y="18" rx="14" ry="14" width="944" height="224" class="panel"/>

    <!-- Holographic avatar circle -->
    <g transform="translate(40,40)">
      <circle cx="68" cy="68" r="64" fill="none" stroke="url(%23gA)" stroke-width="3" opacity="0.9"/>
      <g class="neon">
        <circle cx="68" cy="68" r="42" fill="none" stroke="%2306f" stroke-opacity="0.25" stroke-width="10">
          <animate attributeName="r" values="40;46;40" dur="6s" repeatCount="indefinite"/>
        </circle>
        <text x="10" y="78" class="ty">DyexaHub</text>
      </g>
    </g>

    <!-- Main title -->
    <g transform="translate(150,46)">
      <text class="title">Andre — <tspan style="fill: url(%23gA)">DyexaHub</tspan></text>
      <text x="0" y="40" class="subtitle">Information Systems Student · Computer & Network Engineer · Tech Creator</text>
    </g>

    <!-- Animated typing (SMIL) -->
    <g transform="translate(150,90)">
      <text id="typing" class="ty" y="0">I build systems, networks, and chaos —</text>
      <text id="cursor" x="320" y="0" class="ty">|</text>

      <animate xlink:href="#typing" attributeName="opacity" values="1;1" dur="12s" repeatCount="indefinite"/>
      <animate xlink:href="#cursor" attributeName="opacity" values="1;0" dur="0.8s" repeatCount="indefinite"/>
    </g>

    <!-- mini badges -->
    <g transform="translate(150,130)" font-family="Inter,Arial">
      <rect x="0" y="0" rx="6" ry="6" width="156" height="28" fill="%2306f" opacity="0.08"/>
      <text x="12" y="18" class="ty">📡 Network | Linux | Cloud</text>

      <rect x="170" y="0" rx="6" ry="6" width="196" height="28" fill="%23b95cff" opacity="0.06"/>
      <text x="182" y="18" class="ty">🛠️ DevOps · Containers · Automation</text>

      <rect x="384" y="0" rx="6" ry="6" width="232" height="28" fill="%2306f" opacity="0.06"/>
      <text x="396" y="18" class="ty">🤖 AI · ML · Creative Coding</text>
    </g>

    <!-- bottom neon stripe -->
    <rect x="18" y="218" rx="8" ry="8" width="944" height="6" fill="url(%23gA)" opacity="0.85"/>
  </svg>'/>
</p>

---

<!-- ===========================
     BADGES & LIVE STATS
   =========================== -->

<p align="center">
  <!-- GitHub dynamic widgets -->
  <img src="https://github-readme-stats.vercel.app/api?username=DyexaHub&show_icons=true&theme=dark&hide_border=true&count_private=true" alt="DyexaHub GitHub Stats" height="140"/>
  &nbsp;
  <img src="https://github-readme-streak-stats.herokuapp.com?user=DyexaHub&theme=dark&hide_border=true" alt="streak" height="140"/>
  &nbsp;
  <img src="https://github-profile-trophy.vercel.app/?username=DyexaHub&theme=gruvbox&no-frame=true" alt="trophies" height="140"/>
</p>

---

<!-- ===========================
     ABOUT / DIGITAL BIOGRAPHY (FUTURISTIC)
   =========================== -->

## 🧬 Digital Biography — _An Origin Story (excerpt)_

> _I was compiled from midnight commits and the quiet whir of lab servers. Born in the glow of terminal alerts, I learned routing protocols the way poets learn meter—by listening to the cadence of packets. I am Andre. I call myself DyexaHub. My mind is an array: Information Systems logic, low-level packet empathy, and a taste for generative chaos. I don't just configure networks; I choreograph them._  

**Key roles:**  
- Information Systems Student — formal logic, databases, business processes.  
- Computer & Network Engineer — TCP/IP, routing, firewalls, VLANs, wireless systems.  
- Visionary Tech Creator — automation, cloud-native design, AI-assisted tools, creative code.

---

<!-- ===========================
     SKILLS GALAXY PREVIEW
     (Aesthetic grid with many logos)
   =========================== -->

## 🌌 Skills Galaxy — (hover for chaos ✨)

> _The galaxy below is a curated chaos of the tools, languages, frameworks, OSes, and platforms that sculpt my craft. Colors mean nothing — everything is connected._

<!-- Skill badge grid — mix of shields/simpleicons images -->
<p align="center">
  <!-- row 1: languages -->
  <img src="https://img.shields.io/badge/-Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/-JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JS"/>
  <img src="https://img.shields.io/badge/-TypeScript-319795?style=for-the-badge&logo=typescript&logoColor=white" alt="TS"/>
  <img src="https://img.shields.io/badge/-Go-00ADD8?style=for-the-badge&logo=go&logoColor=white" alt="Go"/>
  <img src="https://img.shields.io/badge/-Rust-000000?style=for-the-badge&logo=rust&logoColor=white" alt="Rust"/>
  <img src="https://img.shields.io/badge/-C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white" alt="C++"/>

  <br/>

  <!-- row 2: frontend -->
  <img src="https://img.shields.io/badge/-React-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React"/>
  <img src="https://img.shields.io/badge/-Vue-4FC08D?style=for-the-badge&logo=vue.js&logoColor=white" alt="Vue"/>
  <img src="https://img.shields.io/badge/-Svelte-FF3E00?style=for-the-badge&logo=svelte&logoColor=white" alt="Svelte"/>
  <img src="https://img.shields.io/badge/-Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white" alt="Next"/>
  <img src="https://img.shields.io/badge/-Tailwind-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind"/>

  <br/>

  <!-- row 3: backend & db -->
  <img src="https://img.shields.io/badge/-Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white" alt="Node"/>
  <img src="https://img.shields.io/badge/-Django-092E20?style=for-the-badge&logo=django&logoColor=white" alt="Django"/>
  <img src="https://img.shields.io/badge/-Flask-000000?style=for-the-badge&logo=flask&logoColor=white" alt="Flask"/>
  <img src="https://img.shields.io/badge/-PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Postgres"/>
  <img src="https://img.shields.io/badge/-MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL"/>
  <img src="https://img.shields.io/badge/-MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB"/>

  <br/>

  <!-- row 4: cloud & infra -->
  <img src="https://img.shields.io/badge/-AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="AWS"/>
  <img src="https://img.shields.io/badge/-Azure-0078D4?style=for-the-badge&logo=microsoft-azure&logoColor=white" alt="Azure"/>
  <img src="https://img.shields.io/badge/-GCP-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white" alt="GCP"/>
  <img src="https://img.shields.io/badge/-Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker"/>
  <img src="https://img.shields.io/badge/-Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" alt="K8s"/>

  <br/>

  <!-- row 5: DevOps & infra tools -->
  <img src="https://img.shields.io/badge/-Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white" alt="Terraform"/>
  <img src="https://img.shields.io/badge/-Ansible-EE0000?style=for-the-badge&logo=ansible&logoColor=white" alt="Ansible"/>
  <img src="https://img.shields.io/badge/-Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white" alt="Prometheus"/>
  <img src="https://img.shields.io/badge/-Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white" alt="Grafana"/>
  <img src="https://img.shields.io/badge/-ELK-005571?style=for-the-badge&logo=elastic&logoColor=white" alt="ELK"/>

  <br/>

  <!-- row 6: AI & data -->
  <img src="https://img.shields.io/badge/-PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch"/>
  <img src="https://img.shields.io/badge/-TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" alt="TensorFlow"/>
  <img src="https://img.shields.io/badge/-HuggingFace-FE6A02?style=for-the-badge&logo=huggingface&logoColor=white" alt="HuggingFace"/>
  <img src="https://img.shields.io/badge/-OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white" alt="OpenAI"/>

  <br/>

  <!-- row 7: design & creative -->
  <img src="https://img.shields.io/badge/-Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white" alt="Figma"/>
  <img src="https://img.shields.io/badge/-Blender-F5792A?style=for-the-badge&logo=blender&logoColor=white" alt="Blender"/>
  <img src="https://img.shields.io/badge/-AfterEffects-9999FF?style=for-the-badge&logo=adobe-after-effects&logoColor=white" alt="AE"/>
  <img src="https://img.shields.io/badge/-Premiere-990000?style=for-the-badge&logo=adobe-premiere-pro&logoColor=white" alt="Premiere"/>

  <br/>

  <!-- row 8: OS & Distros -->
  <img src="https://img.shields.io/badge/-Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white" alt="Ubuntu"/>
  <img src="https://img.shields.io/badge/-Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white" alt="Debian"/>
  <img src="https://img.shields.io/badge/-Arch-1793D1?style=for-the-badge&logo=arch-linux&logoColor=white" alt="Arch"/>
  <img src="https://img.shields.io/badge/-Kali-557C94?style=for-the-badge&logo=kali-linux&logoColor=white" alt="Kali"/>
  <img src="https://img.shields.io/badge/-OpenWrt-000000?style=for-the-badge&logo=openwrt&logoColor=white" alt="OpenWrt"/>

  <br/>

  <!-- row 9: networking & protocols -->
  <img src="https://img.shields.io/badge/-Cisco-1BA0CC?style=for-the-badge&logo=cisco&logoColor=white" alt="Cisco"/>
  <img src="https://img.shields.io/badge/-MikroTik-FF6A00?style=for-the-badge&logo=mikrotik&logoColor=white" alt="MikroTik"/>
  <img src="https://img.shields.io/badge/-BGP-7C4DFF?style=for-the-badge&logo=internet-explorer&logoColor=white" alt="BGP"/>
  <img src="https://img.shields.io/badge/-Wireshark-0B6DAF?style=for-the-badge&logo=wireshark&logoColor=white" alt="Wireshark"/>
  <img src="https://img.shields.io/badge/-iptables-7C7C7C?style=for-the-badge&logo=linux&logoColor=white" alt="iptables"/>

  <br/>

  <!-- row 10: misc (100+ implied) -->
  <em>+ Many more: Bash, PowerShell, VIM, NeoVim, Git, GH Actions, Jenkins, CircleCI, Selenium, Puppeteer, Redis, RabbitMQ, Nginx, Apache, HAProxy, OpenVPN, WireGuard, Zabbix, Netdata, SaltStack, Salt, Packer, Vagrant, VirtualBox, VMware, QEMU, KVM, iPerf, Nmap, Burp Suite, Metasploit, GNS3, EVE-NG, LXC, Podman, LXD, Grafana Loki, Jaeger, ArgoCD, Flux, SRE tooling, and many OS/tool combos — too many to list but they orbit here.</em>
</p>

---

<!-- ===========================
     3D GALAXY (SVG ILLUSION)
   =========================== -->

## 🪐 3D Galaxy — Tech Constellation (SVG illusion)

<p align="center">
<!-- Inline SVG galaxy — animated orbiting tech nodes -->
<img alt="Skills Galaxy" src='data:image/svg+xml;utf8,
<svg xmlns="http://www.w3.org/2000/svg" width="760" height="420" viewBox="0 0 760 420">
  <defs>
    <linearGradient id="g1" x1="0" x2="1"><stop offset="0" stop-color="%2306f"/><stop offset="1" stop-color="%23b95cff"/></linearGradient>
    <style><![CDATA[
      .bg { fill: #040507; }
      .node { font-family: Arial, sans-serif; font-size: 11px; fill: white; cursor: default; }
      .orbit { stroke: rgba(180,180,255,0.06); stroke-width: 1; }
      .dot { fill: url(%23g1); filter: drop-shadow(0 0 8px rgba(100,60,255,0.22)); }
    ]]></style>
  </defs>

  <rect width="100%" height="100%" class="bg"/>

  <!-- center -->
  <g transform="translate(380,210)">
    <circle r="36" fill="url(%23g1)" opacity="0.85"/>
    <text x="-28" y="6" fill="#0b0e12" font-size="10" font-family="Source Sans Pro, Arial">DyexaHub</text>
  </g>

  <!-- orbit rings -->
  <g transform="translate(380,210)" fill="none">
    <circle r="80" class="orbit"/>
    <circle r="140" class="orbit"/>
    <circle r="210" class="orbit"/>
  </g>

  <!-- orbiting nodes with SMIL rotation (illusion) -->
  <g transform="translate(380,210)">
    <g id="o1">
      <circle class="dot" cx="80" cy="0" r="8"/>
      <text class="node" x="92" y="4">Python</text>
    </g>
    <g id="o2">
      <circle class="dot" cx="140" cy="0" r="7"/>
      <text class="node" x="152" y="4">Kubernetes</text>
    </g>
    <g id="o3">
      <circle class="dot" cx="210" cy="0" r="7.2"/>
      <text class="node" x="222" y="4">AWS</text>
    </g>

    <!-- rotation animations -->
    <animateTransform xlink:href="#o1" attributeName="transform" type="rotate" from="0" to="360" dur="12s" repeatCount="indefinite"/>
    <animateTransform xlink:href="#o2" attributeName="transform" type="rotate" from="180" to="-180" dur="18s" repeatCount="indefinite"/>
    <animateTransform xlink:href="#o3" attributeName="transform" type="rotate" from="90" to="-270" dur="24s" repeatCount="indefinite"/>
  </g>
</svg>'/>
</p>

---

<!-- ===========================
     LINUX CORNER — terminal-styled showcase
   =========================== -->

## 🐧 Linux Corner — Terminal Snapshot

> Terminal theme: `Neon Noir` — a sample of commands and outputs that show system & network mastery.

```bash
# dyexa@dyexahub ~ $ uname -a
Linux dyexa 6.4.0-0-generic #1 SMP PREEMPT Fri Nov  8 2025 x86_64 GNU/Linux

# network topology snapshot (simulated)
$ ip a show eth0
2: eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc fq_codel state UP group default qlen 1000
    inet 192.168.88.42/24 brd 192.168.88.255 scope global eth0
    inet6 fe80::deed:beef/64 scope link 

# basic route
$ ip route show
default via 192.168.88.1 dev eth0 proto static

# quick nmap (local lab)
$ nmap -sS -Pn 192.168.88.0/24
Nmap scan report for 192.168.88.1
Host is up (0.0020s latency).
PORT    STATE SERVICE
22/tcp  open  ssh
80/tcp  open  http

# container snapshot
$ docker ps --format "table {{.Names}}\t{{.Image}}\t{{.Status}}"
NAME                IMAGE               STATUS
web_proxy           nginx:1.23          Up 3 hours
data_ingest         dyexa/ingest:latest Up 45m
net-sim             dyexa/net-lab:alpha Up 2d
