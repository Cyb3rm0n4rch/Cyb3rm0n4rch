<svg xmlns="http://www.w3.org/2000/svg" width="900" height="260" viewBox="0 0 900 260">
  <style>
    .grid { stroke: #00FF41; stroke-opacity: 0.07; fill: none; }
    .scanline { animation: scan 4s linear infinite; }
    @keyframes scan { 0% { transform: translateY(0); } 100% { transform: translateY(260px); } }
    .slash { stroke-dasharray: 380; stroke-dashoffset: 380; animation: draw 4s ease-in-out infinite; }
    @keyframes draw { 0% { stroke-dashoffset: 380; opacity: 1; } 45%, 75% { stroke-dashoffset: 0; opacity: 0.55; } 100% { stroke-dashoffset: -380; opacity: 0; } }
    .title { font-family: 'Courier New', monospace; font-size: 46px; font-weight: bold; fill: #D4AF37; animation: glitch 6s infinite; }
    @keyframes glitch {
      0%, 90%, 100% { transform: translate(0, 0); fill: #D4AF37; }
      91% { transform: translate(-4px, 0); fill: #00FF41; }
      93% { transform: translate(4px, 0); fill: #D4AF37; }
      95% { transform: translate(-2px, 1px); fill: #ffffff; }
      97% { transform: translate(0, 0); fill: #D4AF37; }
    }
    .sub { font-family: 'Courier New', monospace; font-size: 18px; fill: #00FF41; }
    .cursor { animation: blink 1s steps(2, start) infinite; }
    @keyframes blink { to { visibility: hidden; } }
    .code { font-family: 'Courier New', monospace; font-size: 12px; fill: #00FF41; opacity: 0.45; animation: flicker 3s infinite; }
    @keyframes flicker { 0%, 100% { opacity: 0.45; } 50% { opacity: 0.2; } }
    .ring { stroke: #00FF41; stroke-opacity: 0.25; fill: none; }
    .radar { transform-box: view-box; transform-origin: 760px 130px; animation: spin 5s linear infinite; }
    @keyframes spin { to { transform: rotate(360deg); } }
    .blip { fill: #00FF41; animation: ping 2.5s ease-out infinite; }
    .b1 { animation-delay: 0s; }
    .b2 { animation-delay: 1s; }
    .b3 { animation-delay: 1.8s; }
    @keyframes ping { 0%, 100% { opacity: 0; } 10% { opacity: 1; } 60% { opacity: 0.1; } }
  </style>

  <rect width="900" height="260" fill="#0d1117"/>

  <path class="grid" d="M0 52H900 M0 104H900 M0 156H900 M0 208H900 M90 0V260 M180 0V260 M270 0V260 M360 0V260 M450 0V260 M540 0V260 M630 0V260 M720 0V260 M810 0V260"/>

  <path class="slash" d="M0 260 L900 0" stroke="#D4AF37" stroke-width="2" fill="none"/>

  <rect class="scanline" x="0" y="0" width="900" height="3" fill="#00FF41" opacity="0.5"/>

  <text class="title" x="60" y="128">侍 r4gn4rock</text>
  <text class="sub" x="60" y="168">&gt; pentester · ctf player · soc analyst<tspan class="cursor">_</tspan></text>
  <text class="code" x="60" y="222">0x4A 0x3F 0x17 0x9C 0xE2 0x11 0xD8 0x7B 0x30 0xFA</text>

  <circle class="ring" cx="760" cy="130" r="40"/>
  <circle class="ring" cx="760" cy="130" r="70"/>
  <circle class="ring" cx="760" cy="130" r="100"/>
  <line x1="660" y1="130" x2="860" y2="130" stroke="#00FF41" stroke-opacity="0.15"/>
  <line x1="760" y1="30" x2="760" y2="230" stroke="#00FF41" stroke-opacity="0.15"/>

  <g class="radar">
    <path d="M760 130 L760 30 A100 100 0 0 0 663 104 Z" fill="#00FF41" opacity="0.18"/>
    <line x1="760" y1="130" x2="760" y2="30" stroke="#00FF41" stroke-width="2"/>
  </g>

  <circle class="blip b1" cx="722" cy="96" r="4"/>
  <circle class="blip b2" cx="792" cy="162" r="4"/>
  <circle class="blip b3" cx="748" cy="174" r="3"/>
</svg>
