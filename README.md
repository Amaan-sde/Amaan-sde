<!--
███████████████████████████████████████████████████████████████████████
██                                                                     ██
██   ⚡ AMAAN KHAN — GITHUB PROFILE README v3.0                       ██
██   [ CLASSIFIED // TOP 0.1% ENGINEER ]                              ██
██   [ RENDERING DIGITAL EXPERIENCE... ]                              ██
██                                                                     ██
███████████████████████████████████████████████████████████████████████
-->

<!-- ══════════════════════════════════════════════════════ -->
<!--  SECTOR 01 — ANIMATED HERO: BMW M5 RACING THROUGH CODE -->
<!-- ══════════════════════════════════════════════════════ -->

<div align="center">

<svg viewBox="0 0 900 220" width="100%" xmlns="http://www.w3.org/2000/svg" style="display:block">
  <defs>
    <!-- Carbon black background -->
    <linearGradient id="bgGrad" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#050A10"/>
      <stop offset="100%" stop-color="#0A1220"/>
    </linearGradient>
    <!-- Neon road gradient -->
    <linearGradient id="roadGrad" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%" stop-color="#00F5FF" stop-opacity="0"/>
      <stop offset="30%" stop-color="#00F5FF" stop-opacity="0.8"/>
      <stop offset="70%" stop-color="#1565FF" stop-opacity="0.8"/>
      <stop offset="100%" stop-color="#FF1744" stop-opacity="0"/>
    </linearGradient>
    <!-- Glow filter for car -->
    <filter id="glow" x="-40%" y="-40%" width="180%" height="180%">
      <feGaussianBlur in="SourceAlpha" stdDeviation="6" result="blur"/>
      <feFlood flood-color="#00F5FF" flood-opacity="0.9" result="color"/>
      <feComposite in="color" in2="blur" operator="in" result="glow"/>
      <feMerge>
        <feMergeNode in="glow"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <!-- Headlight glow -->
    <filter id="headlight" x="-100%" y="-100%" width="400%" height="400%">
      <feGaussianBlur stdDeviation="8" result="blur"/>
      <feFlood flood-color="#00F5FF" flood-opacity="1" result="color"/>
      <feComposite in="color" in2="blur" operator="in" result="glow"/>
      <feMerge>
        <feMergeNode in="glow"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <!-- Trail blur -->
    <filter id="trailBlur">
      <feGaussianBlur stdDeviation="2 0"/>
    </filter>
    <!-- Red accent glow -->
    <filter id="redGlow">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feFlood flood-color="#FF1744" flood-opacity="0.9" result="color"/>
      <feComposite in="color" in2="blur" operator="in" result="glow"/>
      <feMerge>
        <feMergeNode in="glow"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <filter id="scanlines">
      <feTurbulence type="fractalNoise" baseFrequency="0 0.15" numOctaves="1" result="noise"/>
      <feColorMatrix type="saturate" values="0" result="gray"/>
      <feComposite in="SourceGraphic" in2="gray" operator="arithmetic" k1="0" k2="1" k3="0.05" k4="0"/>
    </filter>
    <!-- Clip -->
    <clipPath id="mainClip">
      <rect width="900" height="220"/>
    </clipPath>
  </defs>
  <g clip-path="url(#mainClip)">
    <!-- Background -->
    <rect width="900" height="220" fill="url(#bgGrad)"/>
    <!-- Scan lines effect -->
    <rect width="900" height="220" fill="none" opacity="0.03">
      <animate attributeName="y" values="0;4;0" dur="0.1s" repeatCount="indefinite"/>
    </rect>
    <!-- Digital grid -->
    <g stroke="#00F5FF" stroke-width="0.3" opacity="0.08">
      <line x1="0" y1="55" x2="900" y2="55"/>
      <line x1="0" y1="110" x2="900" y2="110"/>
      <line x1="0" y1="165" x2="900" y2="165"/>
      <line x1="150" y1="0" x2="150" y2="220"/>
      <line x1="300" y1="0" x2="300" y2="220"/>
      <line x1="450" y1="0" x2="450" y2="220"/>
      <line x1="600" y1="0" x2="600" y2="220"/>
      <line x1="750" y1="0" x2="750" y2="220"/>
    </g>
    <!-- NEON HIGHWAY ROAD -->
    <rect x="0" y="148" width="900" height="3" fill="url(#roadGrad)" opacity="0.9"/>
    <!-- Road glow -->
    <rect x="0" y="148" width="900" height="3" fill="#00F5FF" opacity="0.3">
      <animate attributeName="opacity" values="0.3;0.7;0.3" dur="2s" repeatCount="indefinite"/>
    </rect>
    <!-- Dashed lane marker -->
    <g stroke="#1565FF" stroke-width="1.5" stroke-dasharray="30,20" opacity="0.6">
      <line x1="-60" y1="136" x2="900" y2="136">
        <animateTransform attributeName="transform" type="translate" values="0,0;50,0;0,0" dur="0.8s" repeatCount="indefinite"/>
      </line>
    </g>

    <!-- ████ BMW M5 RACING CAR SVG ████ -->
    <!-- Car travels from left to right -->
    <g filter="url(#glow)">
      <animateTransform attributeName="transform" type="translate"
        values="-220,0; 1100,0"
        dur="3.5s" repeatCount="indefinite" calcMode="spline"
        keySplines="0.25,0.1,0.25,1"/>

      <!-- MOTION BLUR TRAIL -->
      <g filter="url(#trailBlur)" opacity="0.35">
        <rect x="-160" y="112" width="160" height="35" rx="4" fill="#00F5FF"/>
        <rect x="-200" y="120" width="160" height="20" rx="2" fill="#1565FF" opacity="0.5"/>
      </g>
      <!-- Neon trail lines -->
      <line x1="-180" y1="125" x2="-5" y2="125" stroke="#00F5FF" stroke-width="1.5" opacity="0.7" filter="url(#trailBlur)"/>
      <line x1="-200" y1="130" x2="-5" y2="130" stroke="#1565FF" stroke-width="1" opacity="0.5" filter="url(#trailBlur)"/>
      <line x1="-150" y1="135" x2="-5" y2="135" stroke="#FF1744" stroke-width="0.8" opacity="0.4" filter="url(#trailBlur)"/>

      <!-- CAR BODY — BMW M5 silhouette -->
      <!-- Main body -->
      <path d="M10,130 Q18,112 35,108 L120,105 Q148,104 162,110 L168,130 Z"
            fill="#1a1a2e" stroke="#00F5FF" stroke-width="1.5"/>
      <!-- Roofline -->
      <path d="M40,108 Q55,96 80,93 Q105,90 130,95 Q148,99 158,108"
            fill="#0f0f1a" stroke="#00F5FF" stroke-width="1.2"/>
      <!-- Lower body sill -->
      <rect x="18" y="130" width="155" height="8" rx="2" fill="#0d0d1f" stroke="#1565FF" stroke-width="1"/>
      <!-- Front bumper aggressive -->
      <path d="M10,130 Q5,135 8,142 L25,142 L20,130 Z" fill="#FF1744" stroke="#FF1744" stroke-width="0.8"/>
      <!-- Rear diffuser -->
      <path d="M168,130 L175,132 L174,142 L158,142 L163,130 Z" fill="#1a1a2e" stroke="#00F5FF" stroke-width="0.8"/>
      <!-- M stripe accents -->
      <line x1="15" y1="120" x2="170" y2="120" stroke="#FF1744" stroke-width="0.8" opacity="0.8"/>
      <!-- Windows -->
      <path d="M45,108 Q58,98 78,95 Q98,92 118,95 Q135,98 148,106 L140,108 Q122,102 98,100 Q74,98 55,105 Z"
            fill="#0a1a35" stroke="#00F5FF" stroke-width="0.8" opacity="0.9"/>
      <!-- A pillar chrome -->
      <line x1="45" y1="108" x2="54" y2="94" stroke="#C0C0C0" stroke-width="1.2"/>
      <!-- BMW Kidney grille - front -->
      <ellipse cx="14" cy="122" rx="4" ry="5" fill="none" stroke="#C0C0C0" stroke-width="1"/>
      <ellipse cx="22" cy="122" rx="4" ry="5" fill="none" stroke="#C0C0C0" stroke-width="1"/>
      <!-- M badge -->
      <rect x="85" y="111" width="22" height="8" rx="1" fill="#1a1a2e"/>
      <text x="96" y="118" text-anchor="middle" fill="#00F5FF" font-size="5" font-family="monospace" font-weight="bold">M5</text>

      <!-- FRONT HEADLIGHTS (glowing) -->
      <g filter="url(#headlight)">
        <path d="M8,112 Q5,115 6,120 Q9,118 12,116 Z" fill="#00F5FF" opacity="0.95"/>
        <path d="M9,114 L4,115 L5,121 L10,120 Z" fill="#FFFFFF" opacity="0.8"/>
      </g>
      <!-- Headlight beam on road -->
      <polygon points="0,148; 30,148; 8,114" fill="#00F5FF" opacity="0.07"/>

      <!-- TAIL LIGHTS (red glow) -->
      <g filter="url(#redGlow)">
        <rect x="167" y="115" width="6" height="12" rx="1" fill="#FF1744" opacity="0.95"/>
        <rect x="165" y="125" width="8" height="4" rx="1" fill="#FF4500" opacity="0.8"/>
      </g>

      <!-- WHEELS with rotation animation -->
      <!-- Front wheel -->
      <g transform="translate(40,142)">
        <circle r="15" fill="#0d0d1f" stroke="#00F5FF" stroke-width="1.5"/>
        <circle r="8" fill="#1a1a2e" stroke="#C0C0C0" stroke-width="1"/>
        <g stroke="#C0C0C0" stroke-width="1">
          <animateTransform attributeName="transform" type="rotate" from="0" to="360" dur="0.4s" repeatCount="indefinite"/>
          <line x1="-7" y1="0" x2="7" y2="0"/>
          <line x1="0" y1="-7" x2="0" y2="7"/>
          <line x1="-5" y1="-5" x2="5" y2="5"/>
          <line x1="5" y1="-5" x2="-5" y2="5"/>
        </g>
        <circle r="4" fill="#FF1744"/>
        <circle r="15" fill="none" stroke="#00F5FF" stroke-width="0.5" opacity="0.4"/>
      </g>
      <!-- Rear wheel -->
      <g transform="translate(147,142)">
        <circle r="15" fill="#0d0d1f" stroke="#00F5FF" stroke-width="1.5"/>
        <circle r="8" fill="#1a1a2e" stroke="#C0C0C0" stroke-width="1"/>
        <g stroke="#C0C0C0" stroke-width="1">
          <animateTransform attributeName="transform" type="rotate" from="0" to="360" dur="0.4s" repeatCount="indefinite"/>
          <line x1="-7" y1="0" x2="7" y2="0"/>
          <line x1="0" y1="-7" x2="0" y2="7"/>
          <line x1="-5" y1="-5" x2="5" y2="5"/>
          <line x1="5" y1="-5" x2="-5" y2="5"/>
        </g>
        <circle r="4" fill="#FF1744"/>
        <circle r="15" fill="none" stroke="#00F5FF" stroke-width="0.5" opacity="0.4"/>
      </g>

      <!-- Wheel arches -->
      <path d="M20,142 Q40,125 60,142" fill="none" stroke="#00F5FF" stroke-width="1.2"/>
      <path d="M127,142 Q147,125 167,142" fill="none" stroke="#00F5FF" stroke-width="1.2"/>

      <!-- Ground reflection glow -->
      <ellipse cx="90" cy="158" rx="90" ry="6" fill="#00F5FF" opacity="0.08"/>
    </g>

    <!-- SPEED PARTICLES -->
    <g opacity="0.6">
      <circle r="1.5" fill="#00F5FF">
        <animate attributeName="cx" values="-50;950" dur="1.2s" repeatCount="indefinite"/>
        <animate attributeName="cy" values="138" dur="1.2s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0;1;1;0" dur="1.2s" repeatCount="indefinite"/>
      </circle>
      <circle r="1" fill="#1565FF">
        <animate attributeName="cx" values="-50;950" dur="0.9s" begin="0.3s" repeatCount="indefinite"/>
        <animate attributeName="cy" values="132" dur="0.9s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0;1;1;0" dur="0.9s" repeatCount="indefinite"/>
      </circle>
      <circle r="1.2" fill="#FF1744">
        <animate attributeName="cx" values="-50;950" dur="1.5s" begin="0.7s" repeatCount="indefinite"/>
        <animate attributeName="cy" values="143" dur="1.5s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0;1;1;0" dur="1.5s" repeatCount="indefinite"/>
      </circle>
    </g>

    <!-- CORNER ACCENTS HUD -->
    <!-- Top left -->
    <path d="M0,30 L0,0 L30,0" fill="none" stroke="#00F5FF" stroke-width="2" opacity="0.9"/>
    <!-- Top right -->
    <path d="M870,0 L900,0 L900,30" fill="none" stroke="#00F5FF" stroke-width="2" opacity="0.9"/>
    <!-- Bottom left -->
    <path d="M0,190 L0,220 L30,220" fill="none" stroke="#FF1744" stroke-width="2" opacity="0.9"/>
    <!-- Bottom right -->
    <path d="M870,220 L900,220 L900,190" fill="none" stroke="#FF1744" stroke-width="2" opacity="0.9"/>

    <!-- HUD TOP STATUS LINE -->
    <text x="20" y="18" fill="#00F5FF" font-size="8" font-family="monospace" opacity="0.8">[ SYSTEM ONLINE ]</text>
    <text x="20" y="30" fill="#1565FF" font-size="7" font-family="monospace" opacity="0.6">ENG: FULL-STACK // PWR: 1000+ DSA // STATUS: RUNNING</text>
    <text x="780" y="18" text-anchor="end" fill="#FF1744" font-size="8" font-family="monospace" opacity="0.8">[ WOTPAN LIVE ]</text>
    <text x="880" y="18" fill="#C0C0C0" font-size="8" font-family="monospace" opacity="0.5">⬤</text>

    <!-- HUD SPEEDOMETER CIRCLE (right side) -->
    <circle cx="860" cy="110" r="40" fill="none" stroke="#00F5FF" stroke-width="0.8" opacity="0.3"/>
    <circle cx="860" cy="110" r="35" fill="none" stroke="#1565FF" stroke-width="0.5" opacity="0.2"/>
    <text x="860" y="106" text-anchor="middle" fill="#00F5FF" font-size="10" font-family="monospace" font-weight="bold">MAX</text>
    <text x="860" y="118" text-anchor="middle" fill="#FFFFFF" font-size="8" font-family="monospace">SPEED</text>
    <circle cx="860" cy="110" r="40" fill="none" stroke="#FF1744" stroke-width="2"
      stroke-dasharray="188" stroke-dashoffset="47" opacity="0.7" transform="rotate(-90 860 110)">
      <animate attributeName="stroke-dashoffset" values="188;47;188" dur="3s" repeatCount="indefinite"/>
    </circle>

    <!-- M MOTORSPORT COLORED ACCENT BAR -->
    <rect x="0" y="215" width="400" height="5" fill="#1565FF"/>
    <rect x="400" y="215" width="100" height="5" fill="#FF1744"/>
    <rect x="500" y="215" width="400" height="5" fill="#C0C0C0"/>
  </g>
</svg>

</div>

<!-- ══════════════════════════════════════════════════════ -->
<!--   SECTOR 02 — NAME, TITLE, ANIMATED IDENTITY          -->
<!-- ══════════════════════════════════════════════════════ -->

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Orbitron&weight=900&size=50&duration=1500&pause=1200&color=00F5FF&center=true&vCenter=true&width=900&height=110&lines=AMAAN+KHAN;◼+AMAAN+KHAN+◼;═══+AMAAN+KHAN+═══" alt="AMAAN KHAN glitch title"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=18&duration=2500&pause=1000&color=C0C0C0&center=true&vCenter=true&width=900&height=50&lines=Software+Engineer+%7C+Building+Digital+Machines;Full-Stack+Architect+%7C+Cloud+%26+DevOps+Engineer;NestJS+%7C+Flutter+%7C+AWS+%7C+Docker+%7C+Kubernetes;NASA+Space+Apps+Challenger+%7C+AWS+Certified" alt="Amaan Khan subtitle"/>

</div>

<br/>

<!-- ══════════════════════════════════════════════════════ -->
<!--   SECTOR 03 — MISSION CONTROL HUD                     -->
<!-- ══════════════════════════════════════════════════════ -->

<div align="center">

<svg viewBox="0 0 900 130" width="100%" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="hudBg" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#050A10"/>
      <stop offset="100%" stop-color="#0A1628"/>
    </linearGradient>
    <filter id="panelGlow">
      <feGaussianBlur stdDeviation="3" result="blur"/>
      <feFlood flood-color="#00F5FF" flood-opacity="0.3" result="color"/>
      <feComposite in="color" in2="blur" operator="in" result="g"/>
      <feMerge><feMergeNode in="g"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>
  <rect width="900" height="130" fill="url(#hudBg)" rx="4"/>
  <!-- Panel borders -->
  <rect x="1" y="1" width="898" height="128" fill="none" stroke="#00F5FF" stroke-width="0.8" rx="4" opacity="0.4"/>
  <!-- Dividers -->
  <line x1="225" y1="10" x2="225" y2="120" stroke="#1565FF" stroke-width="0.5" opacity="0.5"/>
  <line x1="450" y1="10" x2="450" y2="120" stroke="#1565FF" stroke-width="0.5" opacity="0.5"/>
  <line x1="675" y1="10" x2="675" y2="120" stroke="#1565FF" stroke-width="0.5" opacity="0.5"/>
  <!-- TOP BAR -->
  <rect x="0" y="0" width="900" height="18" fill="#00F5FF" opacity="0.07" rx="4"/>
  <text x="450" y="13" text-anchor="middle" fill="#00F5FF" font-size="9" font-family="monospace" letter-spacing="4">⬤ MISSION CONTROL — AMAAN KHAN OPERATIONAL HUD ⬤</text>

  <!-- PANEL 1: SYSTEM STATUS -->
  <text x="113" y="42" text-anchor="middle" fill="#1565FF" font-size="9" font-family="monospace" letter-spacing="2">SYSTEM STATUS</text>
  <text x="113" y="72" text-anchor="middle" fill="#00F5FF" font-size="22" font-family="monospace" font-weight="bold">ONLINE</text>
  <circle cx="113" cy="90" r="5" fill="#00F5FF">
    <animate attributeName="opacity" values="1;0.2;1" dur="1.2s" repeatCount="indefinite"/>
  </circle>
  <text x="113" y="110" text-anchor="middle" fill="#C0C0C0" font-size="8" font-family="monospace">READY TO DEPLOY</text>

  <!-- PANEL 2: ENGINE -->
  <text x="337" y="42" text-anchor="middle" fill="#1565FF" font-size="9" font-family="monospace" letter-spacing="2">ENGINE TYPE</text>
  <text x="337" y="66" text-anchor="middle" fill="#FFFFFF" font-size="13" font-family="monospace" font-weight="bold">FULL-STACK</text>
  <text x="337" y="82" text-anchor="middle" fill="#00F5FF" font-size="11" font-family="monospace">ARCHITECTURE</text>
  <text x="337" y="110" text-anchor="middle" fill="#C0C0C0" font-size="8" font-family="monospace">NESTJS + FLUTTER + REACT</text>

  <!-- PANEL 3: POWER CORE -->
  <text x="562" y="42" text-anchor="middle" fill="#1565FF" font-size="9" font-family="monospace" letter-spacing="2">POWER CORE</text>
  <text x="562" y="66" text-anchor="middle" fill="#FFFFFF" font-size="13" font-family="monospace" font-weight="bold">CLOUD NATIVE</text>
  <text x="562" y="82" text-anchor="middle" fill="#00F5FF" font-size="11" font-family="monospace">INFRASTRUCTURE</text>
  <text x="562" y="110" text-anchor="middle" fill="#C0C0C0" font-size="8" font-family="monospace">AWS + DOCKER + KUBERNETES</text>

  <!-- PANEL 4: ACTIVE MISSION -->
  <text x="787" y="42" text-anchor="middle" fill="#FF1744" font-size="9" font-family="monospace" letter-spacing="2">ACTIVE MISSION</text>
  <text x="787" y="66" text-anchor="middle" fill="#FFFFFF" font-size="18" font-family="monospace" font-weight="bold">WOTPAN</text>
  <text x="787" y="82" text-anchor="middle" fill="#FF1744" font-size="11" font-family="monospace">LIVE PRODUCTION</text>
  <rect x="730" y="95" width="115" height="14" rx="3" fill="#FF1744" opacity="0.15" stroke="#FF1744" stroke-width="0.8"/>
  <text x="787" y="106" text-anchor="middle" fill="#FF1744" font-size="9" font-family="monospace">▶ RUNNING</text>
</svg>

<br/>

<!-- CONNECT BADGES — SLEEK HORIZONTAL -->
<p>
  <a href="https://linkedin.com/in/amaan-khan"><img src="https://img.shields.io/badge/◈_LINKEDIN-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=0A1628"/></a>
  <a href="mailto:amaankhan172595@gmail.com"><img src="https://img.shields.io/badge/◈_GMAIL-D14836?style=for-the-badge&logo=gmail&logoColor=white&labelColor=1A0810"/></a>
  <a href="https://leetcode.com/Amaan_Khan1"><img src="https://img.shields.io/badge/◈_LEETCODE-FFA116?style=for-the-badge&logo=leetcode&logoColor=black&labelColor=1A1200"/></a>
  <img src="https://komarev.com/ghpvc/?username=amaan-khan&label=◈+PROFILE+SCANS&color=00f5ff&style=for-the-badge"/>
</p>

</div>

<!-- ══════════════════════════════════════════════════════ -->
<!--   SECTOR 04 — ABOUT: ENGINEERING BRIEFING             -->
<!-- ══════════════════════════════════════════════════════ -->

<br/>

<table align="center" width="98%">
<tr>
<td width="58%" valign="top">

```
╔═══════════════════════════════════════════╗
║    ◈ ENGINEER PROFILE  //  AMAAN KHAN     ║
╠═══════════════════════════════════════════╣
║                                           ║
║  CALLSIGN    : AMAAN-01                   ║
║  CLEARANCE   : AWS CLOUD PRACTITIONER     ║
║  UNIT        : WOTPAN ENGINEERING CORPS   ║
║  LOCATION    : KASHIPUR, UTTARAKHAND, IN  ║
║  SPECIALITY  : FULL-STACK + CLOUD/DEVOPS  ║
║  DSA KILLS   : 1000+ PROBLEMS SOLVED      ║
║  ACCOLADE    : NASA SPACE APPS CHALLENGER ║
║  STATUS      : ■ ACTIVE — BUILDING        ║
║                                           ║
╚═══════════════════════════════════════════╝
```

</td>
<td width="42%" align="center" valign="middle">
<img src="https://media.giphy.com/media/qgQUggAC3Pfv687qPC/giphy.gif" width="95%" style="border-radius:8px;"/>
</td>
</tr>
</table>

<!-- ══════════════════════════════════════════════════════ -->
<!--   SECTOR 05 — ENGINE COMPONENTS (TECH STACK)          -->
<!-- ══════════════════════════════════════════════════════ -->

<br/>

<div align="center">

<svg viewBox="0 0 900 32" width="100%" xmlns="http://www.w3.org/2000/svg">
  <rect width="900" height="32" fill="#050A10"/>
  <rect x="0" y="0" width="900" height="1" fill="#00F5FF" opacity="0.8"/>
  <rect x="0" y="31" width="900" height="1" fill="#00F5FF" opacity="0.8"/>
  <text x="450" y="21" text-anchor="middle" fill="#00F5FF" font-size="13" font-family="monospace" font-weight="bold" letter-spacing="6">◈ ENGINE COMPONENTS ◈</text>
</svg>

</div>

<br/>

<table align="center" width="98%">
<tr>
<td width="25%" valign="top">

```
┌──────────────────┐
│  FRONTEND ENGINE │
├──────────────────┤
│  ◈ React         │
│  ◈ Flutter       │
│  ◈ TypeScript    │
│  ◈ Tailwind CSS  │
└──────────────────┘
```

</td>
<td width="25%" valign="top">

```
┌──────────────────┐
│  BACKEND ENGINE  │
├──────────────────┤
│  ◈ NestJS        │
│  ◈ Node.js       │
│  ◈ Express.js    │
│  ◈ REST APIs     │
└──────────────────┘
```

</td>
<td width="25%" valign="top">

```
┌──────────────────┐
│  INFRASTRUCTURE  │
├──────────────────┤
│  ◈ AWS           │
│  ◈ Docker        │
│  ◈ Kubernetes    │
│  ◈ Nginx / PM2   │
└──────────────────┘
```

</td>
<td width="25%" valign="top">

```
┌──────────────────┐
│  DATABASE CORE   │
├──────────────────┤
│  ◈ MongoDB       │
│  ◈ MySQL         │
│  ◈ Redis         │
│  ◈ Cloudinary    │
└──────────────────┘
```

</td>
</tr>
</table>

<div align="center">

**Languages:**
<img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white"/>
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"/>
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black"/>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white"/>
<img src="https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=white"/>
<img src="https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=dart&logoColor=white"/>

</div>

<!-- ══════════════════════════════════════════════════════ -->
<!--   SECTOR 06 — EXPERIENCE AT WOTPAN                    -->
<!-- ══════════════════════════════════════════════════════ -->

<br/>

<div align="center">

<svg viewBox="0 0 900 32" width="100%" xmlns="http://www.w3.org/2000/svg">
  <rect width="900" height="32" fill="#050A10"/>
  <rect x="0" y="0" width="900" height="1" fill="#FF1744" opacity="0.8"/>
  <rect x="0" y="31" width="900" height="1" fill="#FF1744" opacity="0.8"/>
  <text x="450" y="21" text-anchor="middle" fill="#FF1744" font-size="13" font-family="monospace" font-weight="bold" letter-spacing="6">◈ DEPLOYMENT LOG ◈</text>
</svg>

</div>

<br/>

<table align="center" width="98%">
<tr>
<td>

```
╔══════════════════════════════════════════════════════════════════════╗
║  🚀 SOFTWARE ENGINEER @ WOTPAN                                       ║
║  ─────────────────────────────────────────────────────────────────  ║
║  PERIOD   : NOV 2025 – PRESENT  //  KASHIPUR, UK, INDIA              ║
╠══════════════════════════════════════════════════════════════════════╣
║                                                                      ║
║  [1] CROSS-PLATFORM MOBILE (FLUTTER)                                 ║
║      └─ Architected reusable UI components for Android & iOS.        ║
║                                                                      ║
║  [2] MODULAR BACKEND SYSTEMS (NESTJS)                                ║
║      └─ REST APIs with JWT auth, custom guards, & DTO validation.    ║
║                                                                      ║
║  [3] DEVOPS & INFRASTRUCTURE (DOCKER + NGINX + PM2)                  ║
║      └─ Containerized deployments, reverse proxy, SSL, zero-downtime.║
║                                                                      ║
║  [4] CI/CD PIPELINE AUTOMATION                                       ║
║      └─ End-to-end automated build & deploy workflows.               ║
║                                                                      ║
╚══════════════════════════════════════════════════════════════════════╝
```

</td>
</tr>
</table>

<!-- ══════════════════════════════════════════════════════ -->
<!--   SECTOR 07 — HOLO PROJECT PANELS                     -->
<!-- ══════════════════════════════════════════════════════ -->

<br/>

<div align="center">

<svg viewBox="0 0 900 32" width="100%" xmlns="http://www.w3.org/2000/svg">
  <rect width="900" height="32" fill="#050A10"/>
  <rect x="0" y="0" width="900" height="1" fill="#1565FF" opacity="0.8"/>
  <rect x="0" y="31" width="900" height="1" fill="#1565FF" opacity="0.8"/>
  <text x="450" y="21" text-anchor="middle" fill="#1565FF" font-size="13" font-family="monospace" font-weight="bold" letter-spacing="6">◈ PROJECT SYSTEMS ◈</text>
</svg>

</div>

<br/>

<table align="center" width="98%">
<tr>
<td width="50%" valign="top">

```
╔════════════════════════════════════╗
║  🤖 AI CONVERSATIONAL ASSISTANT    ║
╠════════════════════════════════════╣
║  STATUS   : ■ ACTIVE               ║
║  FRONTEND : React + Axios          ║
║  BACKEND  : Express.js + REST APIs ║
║  DATABASE : MongoDB                ║
║  SECURITY : JWT + HttpOnly Cookies ║
║  MEDIA    : Cloudinary CDN         ║
╚════════════════════════════════════╝
```

</td>
<td width="50%" valign="top">

```
╔════════════════════════════════════╗
║  🚀 LAUNCHPAD SAAS ENGINE          ║
╠════════════════════════════════════╣
║  STATUS   : ■ LIVE                 ║
║  FRONTEND : React + Tailwind CSS   ║
║  DEPLOY   : Vercel Edge Network    ║
║  PERF     : 95+ Lighthouse Score   ║
║  REACH    : Global CDN Delivery    ║
║  PATTERN  : Mobile-First Design    ║
╚════════════════════════════════════╝
```

</td>
</tr>
</table>

<!-- ══════════════════════════════════════════════════════ -->
<!--   SECTOR 08 — SYSTEM ARCHITECTURE (ANIMATED FLOW)     -->
<!-- ══════════════════════════════════════════════════════ -->

<br/>

<div align="center">

<svg viewBox="0 0 900 32" width="100%" xmlns="http://www.w3.org/2000/svg">
  <rect width="900" height="32" fill="#050A10"/>
  <rect x="0" y="0" width="900" height="1" fill="#00F5FF" opacity="0.5"/>
  <rect x="0" y="31" width="900" height="1" fill="#00F5FF" opacity="0.5"/>
  <text x="450" y="21" text-anchor="middle" fill="#00F5FF" font-size="13" font-family="monospace" font-weight="bold" letter-spacing="6">◈ SYSTEM ARCHITECTURE ◈</text>
</svg>

<br/>

<svg viewBox="0 0 900 380" width="80%" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="archBg" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#050A10"/>
      <stop offset="100%" stop-color="#0A1220"/>
    </linearGradient>
    <filter id="boxGlow">
      <feGaussianBlur stdDeviation="3" result="blur"/>
      <feFlood flood-color="#00F5FF" flood-opacity="0.4" result="color"/>
      <feComposite in="color" in2="blur" operator="in" result="g"/>
      <feMerge><feMergeNode in="g"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <filter id="redBoxGlow">
      <feGaussianBlur stdDeviation="3" result="blur"/>
      <feFlood flood-color="#FF1744" flood-opacity="0.5" result="color"/>
      <feComposite in="color" in2="blur" operator="in" result="g"/>
      <feMerge><feMergeNode in="g"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>
  <rect width="900" height="380" fill="url(#archBg)" rx="6"/>
  <rect x="1" y="1" width="898" height="378" fill="none" stroke="#00F5FF" stroke-width="0.6" rx="6" opacity="0.3"/>

  <!-- BOXES: top to bottom -->
  <!-- USER -->
  <rect x="350" y="20" width="200" height="44" rx="4" fill="#0A1628" stroke="#00F5FF" stroke-width="1.5" filter="url(#boxGlow)"/>
  <text x="450" y="37" text-anchor="middle" fill="#00F5FF" font-size="10" font-family="monospace" letter-spacing="2">◈ USER</text>
  <text x="450" y="54" text-anchor="middle" fill="#C0C0C0" font-size="8" font-family="monospace">MOBILE / BROWSER CLIENT</text>

  <!-- ARROW 1 -->
  <line x1="450" y1="64" x2="450" y2="82" stroke="#00F5FF" stroke-width="1.5" stroke-dasharray="4,2"/>
  <circle cx="450" cy="73" r="3" fill="#00F5FF">
    <animate attributeName="cy" values="64;82;64" dur="1.5s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="1;0.3;1" dur="1.5s" repeatCount="indefinite"/>
  </circle>
  <polygon points="442,80 450,90 458,80" fill="#00F5FF"/>

  <!-- MOBILE INTERFACE -->
  <rect x="300" y="90" width="300" height="44" rx="4" fill="#0A1628" stroke="#00F5FF" stroke-width="1.5" filter="url(#boxGlow)"/>
  <text x="450" y="108" text-anchor="middle" fill="#00F5FF" font-size="10" font-family="monospace" letter-spacing="2">◈ MOBILE INTERFACE</text>
  <text x="450" y="124" text-anchor="middle" fill="#C0C0C0" font-size="8" font-family="monospace">FLUTTER // REACT // TAILWIND CSS</text>

  <!-- ARROW 2 -->
  <line x1="450" y1="134" x2="450" y2="152" stroke="#1565FF" stroke-width="1.5" stroke-dasharray="4,2"/>
  <circle cx="450" cy="143" r="3" fill="#1565FF">
    <animate attributeName="cy" values="134;152;134" dur="1.5s" begin="0.3s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="1;0.3;1" dur="1.5s" repeatCount="indefinite"/>
  </circle>
  <polygon points="442,150 450,160 458,150" fill="#1565FF"/>

  <!-- API GATEWAY -->
  <rect x="275" y="160" width="350" height="44" rx="4" fill="#0A1628" stroke="#1565FF" stroke-width="1.5"/>
  <text x="450" y="178" text-anchor="middle" fill="#1565FF" font-size="10" font-family="monospace" letter-spacing="2">◈ API GATEWAY</text>
  <text x="450" y="194" text-anchor="middle" fill="#C0C0C0" font-size="8" font-family="monospace">NESTJS // JWT AUTH // REST</text>

  <!-- ARROW 3 -->
  <line x1="450" y1="204" x2="450" y2="222" stroke="#FF1744" stroke-width="1.5" stroke-dasharray="4,2"/>
  <circle cx="450" cy="213" r="3" fill="#FF1744">
    <animate attributeName="cy" values="204;222;204" dur="1.5s" begin="0.6s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="1;0.3;1" dur="1.5s" repeatCount="indefinite"/>
  </circle>
  <polygon points="442,220 450,230 458,220" fill="#FF1744"/>

  <!-- MICROSERVICES -->
  <rect x="250" y="230" width="400" height="44" rx="4" fill="#0A1628" stroke="#FF1744" stroke-width="1.5" filter="url(#redBoxGlow)"/>
  <text x="450" y="248" text-anchor="middle" fill="#FF1744" font-size="10" font-family="monospace" letter-spacing="2">◈ MICROSERVICES</text>
  <text x="450" y="264" text-anchor="middle" fill="#C0C0C0" font-size="8" font-family="monospace">NODE.JS // EXPRESS // BUSINESS LOGIC</text>

  <!-- ARROW 4 -->
  <line x1="450" y1="274" x2="450" y2="292" stroke="#C0C0C0" stroke-width="1.5" stroke-dasharray="4,2"/>
  <circle cx="450" cy="283" r="3" fill="#C0C0C0">
    <animate attributeName="cy" values="274;292;274" dur="1.5s" begin="0.9s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="1;0.3;1" dur="1.5s" repeatCount="indefinite"/>
  </circle>
  <polygon points="442,290 450,300 458,290" fill="#C0C0C0"/>

  <!-- DATABASE -->
  <rect x="275" y="300" width="350" height="44" rx="4" fill="#0A1628" stroke="#C0C0C0" stroke-width="1.5"/>
  <text x="450" y="318" text-anchor="middle" fill="#C0C0C0" font-size="10" font-family="monospace" letter-spacing="2">◈ DATABASE CORE</text>
  <text x="450" y="334" text-anchor="middle" fill="#C0C0C0" font-size="8" font-family="monospace">MONGODB // MYSQL // REDIS // CLOUDINARY</text>

  <!-- CLOUD INFRA (side) -->
  <rect x="680" y="230" width="200" height="44" rx="4" fill="#0A1628" stroke="#00F5FF" stroke-width="1" opacity="0.8"/>
  <text x="780" y="248" text-anchor="middle" fill="#00F5FF" font-size="9" font-family="monospace">◈ CLOUD INFRA</text>
  <text x="780" y="264" text-anchor="middle" fill="#C0C0C0" font-size="7" font-family="monospace">AWS // DOCKER // K8S // NGINX</text>
  <!-- side arrow -->
  <line x1="650" y1="252" x2="680" y2="252" stroke="#00F5FF" stroke-width="1" stroke-dasharray="3,2" opacity="0.7"/>
  <circle cx="665" cy="252" r="2.5" fill="#00F5FF" opacity="0.7">
    <animate attributeName="cx" values="650;678;650" dur="1.5s" repeatCount="indefinite"/>
  </circle>
</svg>

</div>

<!-- ══════════════════════════════════════════════════════ -->
<!--   SECTOR 09 — GITHUB ANALYTICS (MISSION CONTROL)      -->
<!-- ══════════════════════════════════════════════════════ -->

<br/>

<div align="center">

<svg viewBox="0 0 900 32" width="100%" xmlns="http://www.w3.org/2000/svg">
  <rect width="900" height="32" fill="#050A10"/>
  <rect x="0" y="0" width="900" height="1" fill="#00F5FF" opacity="0.8"/>
  <rect x="0" y="31" width="900" height="1" fill="#00F5FF" opacity="0.8"/>
  <text x="450" y="21" text-anchor="middle" fill="#00F5FF" font-size="13" font-family="monospace" font-weight="bold" letter-spacing="4">◈ MISSION CONTROL — GITHUB ANALYTICS ◈</text>
</svg>

<br/>

<img width="48%" src="https://github-readme-stats.vercel.app/api?username=amaan-khan&show_icons=true&theme=radical&hide_border=true&count_private=true&bg_color=050A10&title_color=00F5FF&icon_color=1565FF&text_color=C0C0C0" alt="GitHub Stats"/>
<img width="48%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=amaan-khan&layout=compact&theme=radical&hide_border=true&langs_count=8&bg_color=050A10&title_color=00F5FF&text_color=C0C0C0" alt="Top Languages"/>

<br/><br/>

<img width="98%" src="https://github-readme-activity-graph.vercel.app/graph?username=amaan-khan&theme=react-dark&bg_color=050A10&color=00F5FF&line=1565FF&point=FF1744&hide_border=true" alt="Activity Graph"/>

<br/>

<img src="https://raw.githubusercontent.com/amaan-khan/amaan-khan/output/github-contribution-grid-snake.svg" width="98%" alt="Contribution Snake"/>

</div>

<!-- ══════════════════════════════════════════════════════ -->
<!--   SECTOR 10 — DSA COMBAT RECORD                       -->
<!-- ══════════════════════════════════════════════════════ -->

<br/>

<div align="center">

<svg viewBox="0 0 900 32" width="100%" xmlns="http://www.w3.org/2000/svg">
  <rect width="900" height="32" fill="#050A10"/>
  <rect x="0" y="0" width="900" height="1" fill="#FFA116" opacity="0.8"/>
  <rect x="0" y="31" width="900" height="1" fill="#FFA116" opacity="0.8"/>
  <text x="450" y="21" text-anchor="middle" fill="#FFA116" font-size="13" font-family="monospace" font-weight="bold" letter-spacing="6">◈ DSA COMBAT RECORD ◈</text>
</svg>

<br/>

<p>
  <a href="https://leetcode.com/Amaan_Khan1"><img src="https://img.shields.io/badge/LeetCode-1000%2B_Problems_Conquered-FFA116?style=for-the-badge&logo=leetcode&logoColor=black"/></a>
  <img src="https://img.shields.io/badge/CodeChef-Active_Gladiator-5B4638?style=for-the-badge&logo=codechef&logoColor=white"/>
  <img src="https://img.shields.io/badge/HackerRank-5_Stars_Gold-2EC866?style=for-the-badge&logo=hackerrank&logoColor=white"/>
</p>

</div>

<!-- ══════════════════════════════════════════════════════ -->
<!--   SECTOR 11 — DEV QUOTE                               -->
<!-- ══════════════════════════════════════════════════════ -->

<br/>

<div align="center">

<img src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=radical" alt="Dev Quote"/>

</div>

<!-- ══════════════════════════════════════════════════════ -->
<!--   SECTOR 12 — CLOSING SEQUENCE / FOOTER               -->
<!-- ══════════════════════════════════════════════════════ -->

<br/>

<div align="center">

<svg viewBox="0 0 900 90" width="100%" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="footerBg" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%" stop-color="#1565FF" stop-opacity="0"/>
      <stop offset="20%" stop-color="#050A10"/>
      <stop offset="50%" stop-color="#0A1628"/>
      <stop offset="80%" stop-color="#050A10"/>
      <stop offset="100%" stop-color="#FF1744" stop-opacity="0"/>
    </linearGradient>
  </defs>
  <rect width="900" height="90" fill="url(#footerBg)"/>
  <rect x="0" y="0" width="900" height="1" fill="#00F5FF" opacity="0.4"/>
  <!-- M Stripe -->
  <rect x="330" y="8" width="80" height="3" fill="#1565FF" rx="1"/>
  <rect x="410" y="8" width="30" height="3" fill="#FF1744" rx="1"/>
  <rect x="440" y="8" width="130" height="3" fill="#C0C0C0" rx="1"/>
  <text x="450" y="42" text-anchor="middle" fill="#FFFFFF" font-size="16" font-family="monospace" font-weight="bold" letter-spacing="3">AMAAN KHAN</text>
  <text x="450" y="60" text-anchor="middle" fill="#C0C0C0" font-size="9" font-family="monospace">"Code is not just logic. It is precision engineering."</text>
  <text x="450" y="78" text-anchor="middle" fill="#1565FF" font-size="8" font-family="monospace" opacity="0.7">© 2025 AMAAN KHAN — github.com/amaan-khan</text>
</svg>

</div>
