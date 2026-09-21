<div align="center">
  <!-- The Animated Scan Terminal Wrapper -->
  <svg width="100%" max-width="850px" height="340" viewBox="0 0 850 340" fill="none" xmlns="http://w3.org">
    <style>
      /* Terminal Styling */
      .bg { fill: #0d1117; rx: 8px; }
      .bar { fill: #161b22; }
      .dot { fill: #ff5f56; }
      .dot:nth-child(2) { fill: #ffbd2e; }
      .dot:nth-child(3) { fill: #27c93f; }
      
      /* Glowing Green Matrix Text */
      .ascii-text {
        font-family: 'Courier New', Courier, monospace;
        font-weight: bold;
        fill: #39ff14;
        font-size: 14px;
        white-space: pre;
      }
      .stats-text {
        font-family: 'Courier New', Courier, monospace;
        fill: #8b949e;
        font-size: 15px;
      }
      .highlight { fill: #58a6ff; font-weight: bold; }

      /* Scanning Card Overlay Line Animation */
      @keyframes scan {
        0% { transform: translateY(-10px); opacity: 0.3; }
        50% { opacity: 0.8; }
        100% { transform: translateY(330px); opacity: 0.3; }
      }
      .scan-line {
        stroke: #39ff14;
        stroke-width: 2;
        opacity: 0.5;
        filter: drop-shadow(0px 0px 6px #39ff14);
        animation: scan 4s linear infinite;
      }
    </style>

    <!-- Terminal Window Frame -->
    <rect class="bg" width="850" height="340" />
    <rect class="bar" width="850" height="30" />
    <circle class="dot" cx="20" cy="15" r="6" />
    <circle class="dot" cx="40" cy="15" r="6" />
    <circle class="dot" cx="60" cy="15" r="6" />

    <!-- REPLACE THIS TEXT BUFFER WITH YOUR ASCII LOGO FROM STEP 1 -->
    <text x="30" y="70" class="ascii-text">
    __  ___      _          _          ____  ___    ____  __  ___
   /  |/  /___ _/ /_  __  _/ /__  ____/ / / / / |  / __ \/  |/  /
  / /|_/ / __ `/ __ \/ / / / / _ \/ __  / /_/ /| | / /_/ / /|_/ / 
 / /  / / /_/ / / / / /_/ / /  __/ /_/ / __  /_| |/ _, _/ /  / /  
/_/  /_/\__,_/_/ /_/\__,_/_/\___/\__,_/_/ /_(_)[_/_/ |_/_/  /_/   
    </text>

    <!-- Terminal Information Details -->
    <g transform="translate(30, 180)" class="stats-text">
      <text x="0" y="20">> USERNAME:   <tspan class="highlight">your-github-handle</tspan></text>
      <text x="0" y="50">> OS:         <tspan class="highlight">Arch Linux x86_64</tspan></text>
      <text x="0" y="80">> CORE STACK: <tspan class="highlight">TypeScript, React, Python, Docker</tspan></text>
      <text x="0" y="110">> STATUS:     <tspan class="highlight">Building interactive terminal interfaces...</tspan></text>
    </g>

    <!-- The Active Scanning Line Visual -->
    <line x1="0" y1="0" x2="850" y2="0" class="scan-line" />
  </svg>
</div>
