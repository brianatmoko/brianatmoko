<div align="center">

<!-- 🪐 ZONA 1: LUAR ANGKASA ============================================= -->

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D0D2B,50:1A1A4E,100:2D4A7A&height=40&section=header&text=🪐&fontSize=30&fontAlignY=50" />

<br>

<!-- SVG SPACE BANNER -->
<svg width="100%" viewBox="0 0 800 420" xmlns="http://www.w3.org/2000/svg" style="max-width:800px;border-radius:16px;">
  <defs>
    <!-- Space gradient -->
    <linearGradient id="spaceGrad" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%"   stop-color="#0a0a2e"/>
      <stop offset="40%"  stop-color="#141452"/>
      <stop offset="70%"  stop-color="#1e2466"/>
      <stop offset="100%" stop-color="#2d3a7a"/>
    </linearGradient>

    <!-- Star glow filter -->
    <filter id="glow">
      <feGaussianBlur stdDeviation="2" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- Rocket flame gradient -->
    <linearGradient id="flameGrad" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%"   stop-color="#FFD700"/>
      <stop offset="50%"  stop-color="#FF6B35"/>
      <stop offset="100%" stop-color="#FF2222" stop-opacity="0"/>
    </linearGradient>

    <!-- Moon texture gradient -->
    <radialGradient id="moonGrad" cx="40%" cy="40%">
      <stop offset="0%"   stop-color="#FFFDE8"/>
      <stop offset="60%"  stop-color="#F5F0D0"/>
      <stop offset="100%" stop-color="#E8DCA0"/>
    </radialGradient>
  </defs>

  <!-- Background -->
  <rect width="800" height="420" fill="url(#spaceGrad)" rx="16"/>

  <!-- ===== STARS ===== -->
  <g fill="#ffffff">
    <circle cx="45"  cy="30"  r="1.8" opacity="0.9"/>
    <circle cx="120" cy="65"  r="1.2" opacity="0.6"/>
    <circle cx="200" cy="25"  r="2.0" opacity="0.8" filter="url(#glow)"/>
    <circle cx="310" cy="50"  r="1.0" opacity="0.5"/>
    <circle cx="400" cy="35"  r="1.5" opacity="0.7"/>
    <circle cx="500" cy="60"  r="2.2" opacity="0.9" filter="url(#glow)"/>
    <circle cx="580" cy="20"  r="1.0" opacity="0.4"/>
    <circle cx="650" cy="55"  r="1.8" opacity="0.8"/>
    <circle cx="720" cy="30"  r="1.3" opacity="0.6"/>
    <circle cx="760" cy="70"  r="2.0" opacity="0.7" filter="url(#glow)"/>

    <circle cx="80"  cy="100" r="1.0" opacity="0.4"/>
    <circle cx="160" cy="90"  r="1.5" opacity="0.7"/>
    <circle cx="250" cy="110" r="0.8" opacity="0.3"/>
    <circle cx="340" cy="85"  r="1.2" opacity="0.5"/>
    <circle cx="460" cy="100" r="1.8" opacity="0.8"/>
    <circle cx="550" cy="95"  r="1.0" opacity="0.4"/>
    <circle cx="670" cy="115" r="1.5" opacity="0.6"/>
    <circle cx="740" cy="90"  r="1.2" opacity="0.5"/>

    <!-- Cross stars ✦ -->
    <g stroke="#ffffff" stroke-width="1.2" opacity="0.7">
      <line x1="230" y1="48" x2="238" y2="56"/>
      <line x1="238" y1="48" x2="230" y2="56"/>
      <line x1="620" y1="40" x2="628" y2="48"/>
      <line x1="628" y1="40" x2="620" y2="48"/>
      <line x1="480" y1="128" x2="488" y2="136"/>
      <line x1="488" y1="128" x2="480" y2="136"/>
    </g>
  </g>

  <!-- ===== MINECRAFT MOON ===== -->
  <g transform="translate(620, 80)">
    <circle cx="0" cy="0" r="50" fill="url(#moonGrad)" stroke="#C8B878" stroke-width="1"/>
    <!-- Moon craters (pixel style) -->
    <rect x="-20" y="-25" width="12" height="10" rx="2" fill="#D8CCA0" opacity="0.6"/>
    <rect x="5"   y="-15" width="8"  height="8"  rx="2" fill="#D8CCA0" opacity="0.5"/>
    <rect x="-10" y="5"   width="14" height="10" rx="2" fill="#D8CCA0" opacity="0.4"/>
    <rect x="15"  y="10"  width="6"  height="6"  rx="2" fill="#D8CCA0" opacity="0.5"/>
    <rect x="-25" y="15"  width="8"  height="6"  rx="2" fill="#D8CCA0" opacity="0.3"/>
  </g>

  <!-- ===== SMALL PLANET ===== -->
  <g transform="translate(100, 130)">
    <circle cx="0" cy="0" r="18" fill="#8B5CF6" opacity="0.7"/>
    <circle cx="0" cy="0" r="18" fill="none" stroke="#A78BFA" stroke-width="1" opacity="0.5"/>
    <ellipse cx="0" cy="3" rx="20" ry="5" fill="none" stroke="#C4B5FD" stroke-width="0.8" opacity="0.4" transform="rotate(-15)"/>
  </g>

  <!-- ===== ROCKET ===== -->
  <g transform="translate(340, 160)">
    <!-- Rocket flame -->
    <path d="M 0,55 Q -12,75 -8,95 Q 0,105 8,95 Q 12,75 0,55" fill="url(#flameGrad)" opacity="0.9"/>
    <path d="M 0,55 Q -6,70 -4,85 Q 0,92 4,85 Q 6,70 0,55" fill="#FFE44D" opacity="0.6"/>

    <!-- Fins -->
    <polygon points="-18,40 -28,55 -18,50" fill="#CC3333" stroke="#991111" stroke-width="1"/>
    <polygon points="18,40 28,55 18,50" fill="#CC3333" stroke="#991111" stroke-width="1"/>
    <polygon points="0,45 0,58 -10,55" fill="#AA2222" stroke="#991111" stroke-width="0.5"/>
    <polygon points="0,45 0,58 10,55" fill="#AA2222" stroke="#991111" stroke-width="0.5"/>

    <!-- Rocket body -->
    <rect x="-14" y="5" width="28" height="45" rx="3" fill="#E8E8E8" stroke="#AAAAAA" stroke-width="1"/>
    <rect x="-14" y="5" width="28" height="45" rx="3" fill="url(#spaceGrad)" opacity="0.15"/>

    <!-- Rocket stripes -->
    <rect x="-14" y="35" width="28" height="6" fill="#DD4444"/>
    <rect x="-14" y="10" width="28" height="3" fill="#DD4444"/>

    <!-- Nose cone -->
    <polygon points="0,-30 -14,5 14,5" fill="#E8E8E8" stroke="#AAAAAA" stroke-width="1"/>
    <polygon points="0,-30 -14,5 14,5" fill="#FF4444" opacity="0.3"/>

    <!-- Window -->
    <circle cx="0" cy="18" r="6" fill="#4A90D9" stroke="#AAAAAA" stroke-width="1.5"/>
    <circle cx="-1" cy="17" r="2" fill="#87CEEB" opacity="0.6"/>

    <!-- Window reflection -->
    <circle cx="-2" cy="16" r="1" fill="white" opacity="0.7"/>
  </g>

  <!-- ===== MAIN TITLE ===== -->
  <text x="400" y="300" text-anchor="middle" dominant-baseline="middle"
        font-family="'Courier New', monospace" font-size="36" font-weight="bold"
        fill="#00D2FF" filter="url(#glow)">
    BRIAN ATMOKO
  </text>

  <!-- Subtitle with pixel feel -->
  <text x="400" y="330" text-anchor="middle" dominant-baseline="middle"
        font-family="'Courier New', monospace" font-size="16"
        fill="#87CEEB" opacity="0.9"
        letter-spacing="4">
    ★ DARI ANGKASA KE INTI BUMI ★
  </text>

  <!-- Tagline -->
  <text x="400" y="360" text-anchor="middle" dominant-baseline="middle"
        font-family="'Courier New', monospace" font-size="12"
        fill="#A0C0E0" opacity="0.7"
        letter-spacing="2">
    Embedded Systems  •  AI  •  Fullstack
  </text>

  <!-- Small decorative stars near title -->
  <g fill="#FFD700" opacity="0.6">
    <polygon points="150,290 153,296 160,296 155,300 157,307 150,303 143,307 145,300 140,296 147,296" transform="scale(0.6) translate(250,200)"/>
    <polygon points="150,290 153,296 160,296 155,300 157,307 150,303 143,307 145,300 140,296 147,296" transform="scale(0.4) translate(1400,480)"/>
  </g>
</svg>

<br>

<!-- TYPING ANIMATION -->
<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3000&pause=500&color=00D2FF&center=true&vCenter=true&multiline=true&width=700&height=80&lines=Halo%2C+dunia+bawah+tanah!;Saya+Brian+Atmoko+—+Embedded+Systems+Engineer;Mari+jelajah+dari+angkasa+ke+inti+bumi" alt="Typing SVG" />
</a>

<br>

<!-- FLOATING CLOUDS TRANSITION -->
<pre style="color:#87CEEB;font-size:10px;line-height:1.2;opacity:0.5;">
                .  ·  :  *  ¨  ¨  *  :  ·  .
            MASUK  ATMOSFER...
                ·  :  *  ¨  ¨  *  :  ·
</pre>

<br>

<!-- GLOWING SEPARATOR -->
<pre style="color:#00D2FF;font-size:14px;line-height:1;">
  ═══ ⋆★⋆  DARI BINTANG  ★  KE  RUMPUT  ⋆★⋆ ═══
</pre>

</div>

<!-- ================================================================== -->
<!-- 🪐 AKHIR ZONA 1 · BERSAMBUNG KE ZONA 2: ATMOSFER                  -->
<!-- ================================================================== -->
