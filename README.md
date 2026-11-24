<!DOCTYPE html>

<html lang="en"><head>
<meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>Climatic GitHub Profile README - Jegath</title>
<script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
<link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css" rel="stylesheet"/>
<link href="https://fonts.googleapis.com" rel="preconnect"/>
<link crossorigin="" href="https://fonts.gstatic.com" rel="preconnect"/>
<link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;500;600&amp;family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&amp;display=swap" rel="stylesheet"/>
<script>
    tailwind.config = {
      darkMode: 'class',
      theme: {
        extend: {
          fontFamily: {
            sans: ['"Plus Jakarta Sans"', 'sans-serif'],
            mono: ['"Fira Code"', 'monospace']
          },
          colors: {
            twilight: {
              base: '#040711',
              card: '#080e1e',
              deep: '#060a16',
              border: '#16233b'
            }
          }
        }
      }
    }
  </script>
<style>
    @keyframes rain-fall {
      0% { transform: translateY(-120%); opacity: 0; }
      20% { opacity: 0.75; }
      85% { opacity: 0.7; }
      100% { transform: translateY(110vh); opacity: 0; }
    }
    @keyframes mist-drift {
      0% { transform: translateX(-3%) translateY(0); opacity: 0.35; }
      50% { transform: translateX(3%) translateY(-15px); opacity: 0.55; }
      100% { transform: translateX(-3%) translateY(0); opacity: 0.35; }
    }
    @keyframes lightning-glow {
      0%, 100% {
        transform: scale(1) rotate(0deg);
        filter: drop-shadow(0 0 10px rgba(251, 191, 36, 0.7)) drop-shadow(0 0 24px rgba(34, 211, 238, 0.8));
      }
      50% {
        transform: scale(1.15) rotate(4deg);
        filter: drop-shadow(0 0 18px rgba(251, 191, 36, 1)) drop-shadow(0 0 35px rgba(56, 189, 248, 1));
      }
    }
    @keyframes cursor-blink {
      0%, 49% { opacity: 1; }
      50%, 100% { opacity: 0; }
    }
    @keyframes subtle-badge-pulse {
      0%, 100% {
        box-shadow: 0 0 12px rgba(6, 182, 212, 0.25), inset 0 0 8px rgba(6, 182, 212, 0.15);
        border-color: rgba(34, 211, 238, 0.45);
      }
      50% {
        box-shadow: 0 0 22px rgba(168, 85, 247, 0.35), inset 0 0 12px rgba(34, 211, 238, 0.25);
        border-color: rgba(168, 85, 247, 0.6);
      }
    }

    .rain-drop {
      position: absolute;
      background: linear-gradient(to bottom, rgba(56, 189, 248, 0), rgba(56, 189, 248, 0.85) 65%, rgba(168, 85, 247, 0.9));
      height: 64px;
      width: 1.5px;
      animation: rain-fall linear infinite;
      pointer-events: none;
    }
    .rain-drop-fast {
      position: absolute;
      background: linear-gradient(to bottom, rgba(147, 197, 253, 0), rgba(125, 211, 252, 0.95));
      height: 48px;
      width: 1px;
      animation: rain-fall linear infinite;
      pointer-events: none;
    }
    .mist-layer {
      animation: mist-drift 18s ease-in-out infinite;
    }
    .lightning-spark {
      display: inline-block;
      animation: lightning-glow 2.4s ease-in-out infinite;
    }
    .cursor-shimmer {
      display: inline-block;
      width: 8px;
      height: 15px;
      background-color: #38bdf8;
      box-shadow: 0 0 10px #38bdf8;
      vertical-align: middle;
      animation: cursor-blink 1s step-start infinite;
    }
    .pulse-glow-badge {
      animation: subtle-badge-pulse 3.5s ease-in-out infinite;
    }
    
    .glass-panel {
      background: linear-gradient(135deg, rgba(8, 14, 30, 0.92) 0%, rgba(6, 10, 22, 0.95) 100%);
      backdrop-filter: blur(24px);
      -webkit-backdrop-filter: blur(24px);
      border: 1px solid rgba(56, 189, 248, 0.28);
      box-shadow: 0 25px 50px -12px rgba(2, 6, 23, 0.9), 0 0 40px rgba(56, 189, 248, 0.12), inset 0 1px 1px rgba(255, 255, 255, 0.1);
    }
    
    .glass-card {
      background: linear-gradient(145deg, rgba(11, 21, 40, 0.78) 0%, rgba(7, 13, 26, 0.88) 100%);
      backdrop-filter: blur(16px);
      -webkit-backdrop-filter: blur(16px);
      border: 1px solid rgba(56, 189, 248, 0.14);
      transition: all 0.35s cubic-bezier(0.4, 0, 0.2, 1);
    }
    
    .tech-card {
      transition: all 0.3s cubic-bezier(0.34, 1.56, 0.64, 1);
    }
    .tech-card:hover {
      transform: translateY(-4px) scale(1.03);
      border-color: rgba(56, 189, 248, 0.65);
      background: linear-gradient(145deg, rgba(14, 27, 54, 0.92) 0%, rgba(10, 18, 38, 0.95) 100%);
      box-shadow: 0 10px 25px -4px rgba(6, 182, 212, 0.35), 0 0 20px rgba(34, 211, 238, 0.25);
    }

    .glow-text {
      text-shadow: 0 0 25px rgba(56, 189, 248, 0.7), 0 0 50px rgba(14, 165, 233, 0.4), 0 0 75px rgba(168, 85, 247, 0.25);
    }

    @media (prefers-reduced-motion: reduce) {
      .rain-drop, .rain-drop-fast, .mist-layer, .lightning-spark, .cursor-shimmer, .pulse-glow-badge {
        animation: none !important;
      }
      .tech-card:hover {
        transform: none !important;
      }
    }
  </style>
</head>
<body class="bg-[#03060f] text-slate-200 font-sans min-h-screen selection:bg-cyan-500/35 selection:text-cyan-100 relative overflow-x-hidden p-4 md:p-8 flex justify-center items-start">
<!-- Atmospheric Background Ambient Rain & Glow -->
<div class="fixed inset-0 pointer-events-none overflow-hidden z-0">
<!-- Gentle Ambient Raindroplets -->
<div class="rain-drop" style="left: 6%; animation-duration: 1.3s; animation-delay: 0.1s;"></div>
<div class="rain-drop-fast" style="left: 14%; animation-duration: 1.05s; animation-delay: 0.5s;"></div>
<div class="rain-drop" style="left: 23%; animation-duration: 1.55s; animation-delay: 0.7s;"></div>
<div class="rain-drop-fast" style="left: 33%; animation-duration: 1.15s; animation-delay: 0.25s;"></div>
<div class="rain-drop" style="left: 45%; animation-duration: 1.25s; animation-delay: 0.9s;"></div>
<div class="rain-drop-fast" style="left: 56%; animation-duration: 1.35s; animation-delay: 0.4s;"></div>
<div class="rain-drop" style="left: 68%; animation-duration: 1.45s; animation-delay: 0.85s;"></div>
<div class="rain-drop-fast" style="left: 77%; animation-duration: 1.1s; animation-delay: 0.15s;"></div>
<div class="rain-drop" style="left: 88%; animation-duration: 1.6s; animation-delay: 0.3s;"></div>
<div class="rain-drop-fast" style="left: 95%; animation-duration: 1.2s; animation-delay: 0.65s;"></div>
<!-- Atmospheric Twilight Gradients & Soft Mist Clouds -->
<div class="mist-layer absolute -top-40 left-1/4 w-[580px] h-[580px] rounded-full bg-gradient-to-tr from-cyan-600/20 via-sky-500/15 to-violet-600/20 blur-[140px]"></div>
<div class="mist-layer absolute top-1/3 -right-36 w-[620px] h-[620px] rounded-full bg-gradient-to-br from-violet-600/20 via-indigo-600/20 to-cyan-500/10 blur-[150px]" style="animation-delay: -5s;"></div>
<div class="mist-layer absolute bottom-12 -left-20 w-[520px] h-[520px] rounded-full bg-gradient-to-tr from-teal-500/15 via-cyan-600/15 to-amber-500/10 blur-[130px]" style="animation-delay: -9s;"></div>
<div class="absolute top-2/3 left-1/2 -translate-x-1/2 w-[700px] h-[350px] bg-sky-950/25 blur-[120px] pointer-events-none"></div>
</div>
<!-- Main GitHub README Shell -->
<main class="w-full max-w-4xl glass-panel rounded-3xl overflow-hidden shadow-2xl relative z-10 my-4 border border-cyan-500/30">
<!-- GitHub README Header / Status Bar -->
<div class="px-6 py-4 bg-gradient-to-r from-[#060b18]/95 via-[#081022]/95 to-[#060b18]/95 border-b border-cyan-500/20 flex items-center justify-between">
<div class="flex items-center space-x-3">
<div class="flex space-x-2">
<span class="w-3 h-3 rounded-full bg-rose-500/90 inline-block shadow-md shadow-rose-500/40"></span>
<span class="w-3 h-3 rounded-full bg-amber-400/90 inline-block shadow-md shadow-amber-500/40"></span>
<span class="w-3 h-3 rounded-full bg-emerald-400/90 inline-block shadow-md shadow-emerald-500/40"></span>
</div>
<span class="text-xs font-mono text-cyan-300 tracking-wider flex items-center gap-2 ml-2">
<i class="fa-solid fa-cloud-showers-heavy text-cyan-400 animate-pulse"></i> README.md — Climatic Profile Workspace
        </span>
</div>
<div class="flex items-center space-x-3">
<span class="inline-flex items-center gap-2 px-3 py-1.5 rounded-full text-xs font-medium bg-[#0a152d]/90 text-cyan-200 border border-cyan-400/40 shadow-[0_0_15px_rgba(6,182,212,0.25)] pulse-glow-badge">
<span class="relative flex h-2 w-2">
<span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-cyan-400 opacity-80"></span>
<span class="relative inline-flex rounded-full h-2 w-2 bg-cyan-300 shadow-[0_0_8px_#22d3ee]"></span>
</span>
          Atmosphere: Rainy Twilight
        </span>
</div>
</div>
<!-- Aesthetic Climatic Hero Banner Section -->
<div class="relative w-full overflow-hidden group">
<!-- Framed Atmospheric Banner Image with inner depth shadow -->
<div class="relative w-full h-72 md:h-96 overflow-hidden">
<img alt="Climatic Skyline Twilight Banner" class="w-full h-full object-cover object-center filter brightness-[0.98] contrast-[1.08] transition-transform duration-1000 group-hover:scale-[1.03]" src="https://lh3.googleusercontent.com/aida/ALJJyrDBRYkQ7b4MNQZPQCoFK8p5vDsBml5kJkt6xvSSO0VcoyI4LhADZf_ijaJG0AjxsFlVIWwhECfq6ajzmOqjNNDGv6mOyZsYCWnDOFCJRLHJFvHMuuQQIMYnfrew23OpIYt8vNOzEvf9b3TE5xNi5BGWc5Zr_2FEM1iIhjdRsRWApmiW7_IctK6x9b7yimKC29iRFIJmsIZ6nFvfTMJdbmev2jqWGTIUJjuskloP_MQ63Q"/>
<!-- Atmospheric Mist & Twilight Gradient Overlays -->
<div class="absolute inset-0 bg-gradient-to-t from-[#040711] via-[#040711]/55 to-transparent"></div>
<div class="absolute inset-0 bg-gradient-to-r from-[#040711]/85 via-transparent to-[#040711]/60"></div>
<div class="absolute inset-0 bg-gradient-to-b from-[#060b18]/40 via-transparent to-transparent pointer-events-none"></div>
<!-- Subtle rain overlay sheen -->
<div class="absolute inset-0 bg-[radial-gradient(ellipse_at_top,_var(--tw-gradient-stops))] from-cyan-400/10 via-transparent to-violet-950/20 pointer-events-none"></div>
</div>
<!-- Climatic Name & Title Floating Elements -->
<div class="absolute bottom-6 left-6 right-6 flex flex-col md:flex-row md:items-end justify-between gap-4">
<div>
<div class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-lg bg-slate-950/80 border border-cyan-400/45 text-cyan-300 font-mono text-xs mb-2.5 backdrop-blur-md shadow-[0_0_15px_rgba(6,182,212,0.2)]">
<i class="fa-solid fa-terminal text-cyan-400"></i> developer &amp; software architect
          </div>
<h1 class="text-3xl md:text-5xl font-extrabold tracking-tight text-white glow-text font-sans flex items-center flex-wrap gap-2 md:gap-3">
<span>Hi, I'm</span>
<span class="bg-gradient-to-r from-cyan-300 via-sky-200 to-amber-200 bg-clip-text text-transparent drop-shadow-[0_0_25px_rgba(34,211,238,0.5)]">Jegath</span>
<span class="lightning-spark text-amber-300 text-2xl md:text-4xl" title="Electrified focus">⚡</span>
</h1>
<p class="text-sm md:text-base text-slate-300 mt-1 max-w-xl font-medium tracking-wide flex items-center gap-2">
<i class="fa-solid fa-cloud-rain text-cyan-400 animate-pulse"></i>
            Building high-performance software amidst twilight rain and cyber aesthetics.
          </p>
</div>
<!-- Quick Status Pill -->
<div class="glass-card px-4 py-2.5 rounded-2xl flex items-center gap-3 border border-cyan-400/35 shadow-[0_4px_20px_rgba(6,182,212,0.18)] hover:border-cyan-300/60 transition-colors">
<div class="w-9 h-9 rounded-xl bg-gradient-to-br from-cyan-500/20 to-violet-500/20 flex items-center justify-center text-cyan-300 border border-cyan-400/40 shadow-[0_0_12px_rgba(34,211,238,0.3)]">
<i class="fa-solid fa-code-fork text-sm"></i>
</div>
<div>
<div class="text-[10px] text-slate-400 uppercase tracking-widest font-mono">Current Status</div>
<div class="text-xs font-semibold text-cyan-200 flex items-center gap-1.5">
<span>Crafting next-gen systems</span>
</div>
</div>
</div>
</div>
</div>
<!-- Inner Content Body -->
<div class="p-6 md:p-8 space-y-8">
<!-- About Me / Climatic Bio Snippet -->
<section class="glass-card p-6 rounded-2xl relative overflow-hidden border border-slate-700/60 shadow-lg shadow-black/40">
<div class="absolute -right-10 -bottom-10 w-52 h-52 bg-gradient-to-br from-cyan-500/10 via-violet-500/10 to-transparent rounded-full blur-2xl pointer-events-none"></div>
<div class="flex items-center justify-between mb-4 border-b border-slate-700/60 pb-3">
<h2 class="text-lg font-bold text-white flex items-center gap-2.5 tracking-wide">
<span class="flex items-center justify-center w-7 h-7 rounded-lg bg-cyan-950/80 border border-cyan-500/30 text-cyan-300 shadow-[0_0_10px_rgba(6,182,212,0.2)]">
<i class="fa-solid fa-compass text-xs"></i>
</span>
            About Me
          </h2>
<span class="text-xs font-mono text-cyan-300/90 px-2.5 py-0.5 rounded-md bg-cyan-950/40 border border-cyan-500/20">whoami.sh</span>
</div>
<div class="grid grid-cols-1 md:grid-cols-3 gap-4 text-sm text-slate-300">
<div class="flex items-start gap-3 p-4 rounded-xl bg-slate-900/60 border border-slate-800/80 hover:border-cyan-500/35 hover:bg-slate-900/90 transition-all duration-300">
<div class="w-8 h-8 rounded-lg bg-cyan-500/15 border border-cyan-500/30 flex items-center justify-center text-cyan-400 shrink-0 mt-0.5">
<i class="fa-solid fa-code text-sm"></i>
</div>
<div>
<div class="text-white font-semibold text-xs font-mono">Full-Stack Architect</div>
<div class="text-xs text-slate-400 mt-1 leading-relaxed">Designing end-to-end resilient applications and scalable APIs</div>
</div>
</div>
<div class="flex items-start gap-3 p-4 rounded-xl bg-slate-900/60 border border-slate-800/80 hover:border-amber-500/35 hover:bg-slate-900/90 transition-all duration-300">
<div class="w-8 h-8 rounded-lg bg-amber-500/15 border border-amber-500/30 flex items-center justify-center text-amber-400 shrink-0 mt-0.5">
<i class="fa-solid fa-bolt text-sm"></i>
</div>
<div>
<div class="text-white font-semibold text-xs font-mono">Performance &amp; Craft</div>
<div class="text-xs text-slate-400 mt-1 leading-relaxed">Dedicated to ultra-fast UI rendering and clean modular codebase</div>
</div>
</div>
<div class="flex items-start gap-3 p-4 rounded-xl bg-slate-900/60 border border-slate-800/80 hover:border-teal-500/35 hover:bg-slate-900/90 transition-all duration-300">
<div class="w-8 h-8 rounded-lg bg-teal-500/15 border border-teal-500/30 flex items-center justify-center text-teal-400 shrink-0 mt-0.5">
<i class="fa-solid fa-diagram-project text-sm"></i>
</div>
<div>
<div class="text-white font-semibold text-xs font-mono">Open Source Explorer</div>
<div class="text-xs text-slate-400 mt-1 leading-relaxed">Building dev utilities, contributing code, and shipping continuously</div>
</div>
</div>
</div>
</section>
<!-- Coding Tools & Tech Ecosystem (Vector & Clean Badges - NO numbers, NO strength bars) -->
<section class="space-y-4">
<div class="flex items-center justify-between">
<div class="flex items-center gap-2.5">
<span class="p-2 rounded-xl bg-cyan-950/90 text-cyan-300 border border-cyan-500/40 shadow-[0_0_12px_rgba(6,182,212,0.25)]">
<i class="fa-solid fa-cubes-stacked"></i>
</span>
<div>
<h2 class="text-lg font-bold text-white tracking-wide">Coding Tools &amp; Ecosystem</h2>
<p class="text-xs text-slate-400">Languages, frameworks, and developer toolchain</p>
</div>
</div>
<span class="text-xs font-mono text-cyan-300 px-3 py-1 rounded-full bg-slate-900/90 border border-cyan-400/35 shadow-sm">
            tech stack
          </span>
</div>
<div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-6 gap-3.5">
<!-- VS Code -->
<div class="glass-card tech-card p-3.5 rounded-xl flex flex-col items-center justify-center gap-2.5 group cursor-pointer border border-slate-800/90">
<div class="w-10 h-10 rounded-xl bg-blue-500/15 border border-blue-500/30 flex items-center justify-center text-blue-400 text-xl group-hover:scale-110 group-hover:shadow-[0_0_15px_rgba(59,130,246,0.5)] transition-all">
<i class="fa-solid fa-code"></i>
</div>
<span class="text-xs font-medium text-slate-300 group-hover:text-cyan-300 transition-colors">VS Code</span>
</div>
<!-- JavaScript -->
<div class="glass-card tech-card p-3.5 rounded-xl flex flex-col items-center justify-center gap-2.5 group cursor-pointer border border-slate-800/90">
<div class="w-10 h-10 rounded-xl bg-yellow-500/15 border border-yellow-500/30 flex items-center justify-center text-yellow-400 text-xl group-hover:scale-110 group-hover:shadow-[0_0_15px_rgba(234,179,8,0.5)] transition-all">
<i class="fa-brands fa-js"></i>
</div>
<span class="text-xs font-medium text-slate-300 group-hover:text-yellow-300 transition-colors">JavaScript</span>
</div>
<!-- TypeScript -->
<div class="glass-card tech-card p-3.5 rounded-xl flex flex-col items-center justify-center gap-2.5 group cursor-pointer border border-slate-800/90">
<div class="w-10 h-10 rounded-xl bg-blue-600/15 border border-blue-600/30 flex items-center justify-center text-blue-400 text-sm font-mono font-bold group-hover:scale-110 group-hover:shadow-[0_0_15px_rgba(37,99,235,0.5)] transition-all">
              TS
            </div>
<span class="text-xs font-medium text-slate-300 group-hover:text-blue-300 transition-colors">TypeScript</span>
</div>
<!-- Python -->
<div class="glass-card tech-card p-3.5 rounded-xl flex flex-col items-center justify-center gap-2.5 group cursor-pointer border border-slate-800/90">
<div class="w-10 h-10 rounded-xl bg-amber-500/15 border border-amber-500/30 flex items-center justify-center text-amber-400 text-xl group-hover:scale-110 group-hover:shadow-[0_0_15px_rgba(245,158,11,0.5)] transition-all">
<i class="fa-brands fa-python"></i>
</div>
<span class="text-xs font-medium text-slate-300 group-hover:text-amber-300 transition-colors">Python</span>
</div>
<!-- React -->
<div class="glass-card tech-card p-3.5 rounded-xl flex flex-col items-center justify-center gap-2.5 group cursor-pointer border border-slate-800/90">
<div class="w-10 h-10 rounded-xl bg-cyan-500/15 border border-cyan-500/30 flex items-center justify-center text-cyan-400 text-xl group-hover:scale-110 group-hover:shadow-[0_0_15px_rgba(6,182,212,0.5)] transition-all">
<i class="fa-brands fa-react"></i>
</div>
<span class="text-xs font-medium text-slate-300 group-hover:text-cyan-300 transition-colors">React</span>
</div>
<!-- Next.js -->
<div class="glass-card tech-card p-3.5 rounded-xl flex flex-col items-center justify-center gap-2.5 group cursor-pointer border border-slate-800/90">
<div class="w-10 h-10 rounded-xl bg-slate-100/15 border border-slate-100/30 flex items-center justify-center text-slate-100 text-sm font-mono font-bold group-hover:scale-110 group-hover:shadow-[0_0_15px_rgba(248,250,252,0.4)] transition-all">
              N
            </div>
<span class="text-xs font-medium text-slate-300 group-hover:text-white transition-colors">Next.js</span>
</div>
<!-- Node.js -->
<div class="glass-card tech-card p-3.5 rounded-xl flex flex-col items-center justify-center gap-2.5 group cursor-pointer border border-slate-800/90">
<div class="w-10 h-10 rounded-xl bg-emerald-500/15 border border-emerald-500/30 flex items-center justify-center text-emerald-400 text-xl group-hover:scale-110 group-hover:shadow-[0_0_15px_rgba(16,185,129,0.5)] transition-all">
<i class="fa-brands fa-node-js"></i>
</div>
<span class="text-xs font-medium text-slate-300 group-hover:text-emerald-300 transition-colors">Node.js</span>
</div>
<!-- Tailwind CSS -->
<div class="glass-card tech-card p-3.5 rounded-xl flex flex-col items-center justify-center gap-2.5 group cursor-pointer border border-slate-800/90">
<div class="w-10 h-10 rounded-xl bg-sky-500/15 border border-sky-500/30 flex items-center justify-center text-sky-400 text-lg group-hover:scale-110 group-hover:shadow-[0_0_15px_rgba(14,165,233,0.5)] transition-all">
<i class="fa-solid fa-wind"></i>
</div>
<span class="text-xs font-medium text-slate-300 group-hover:text-sky-300 transition-colors">Tailwind</span>
</div>
<!-- HTML5 -->
<div class="glass-card tech-card p-3.5 rounded-xl flex flex-col items-center justify-center gap-2.5 group cursor-pointer border border-slate-800/90">
<div class="w-10 h-10 rounded-xl bg-orange-500/15 border border-orange-500/30 flex items-center justify-center text-orange-400 text-xl group-hover:scale-110 group-hover:shadow-[0_0_15px_rgba(249,115,22,0.5)] transition-all">
<i class="fa-brands fa-html5"></i>
</div>
<span class="text-xs font-medium text-slate-300 group-hover:text-orange-300 transition-colors">HTML5</span>
</div>
<!-- CSS3 -->
<div class="glass-card tech-card p-3.5 rounded-xl flex flex-col items-center justify-center gap-2.5 group cursor-pointer border border-slate-800/90">
<div class="w-10 h-10 rounded-xl bg-blue-500/15 border border-blue-500/30 flex items-center justify-center text-blue-400 text-xl group-hover:scale-110 group-hover:shadow-[0_0_15px_rgba(59,130,246,0.5)] transition-all">
<i class="fa-brands fa-css3-alt"></i>
</div>
<span class="text-xs font-medium text-slate-300 group-hover:text-blue-300 transition-colors">CSS3</span>
</div>
<!-- Git -->
<div class="glass-card tech-card p-3.5 rounded-xl flex flex-col items-center justify-center gap-2.5 group cursor-pointer border border-slate-800/90">
<div class="w-10 h-10 rounded-xl bg-rose-500/15 border border-rose-500/30 flex items-center justify-center text-rose-400 text-xl group-hover:scale-110 group-hover:shadow-[0_0_15px_rgba(244,63,94,0.5)] transition-all">
<i class="fa-brands fa-git-alt"></i>
</div>
<span class="text-xs font-medium text-slate-300 group-hover:text-rose-300 transition-colors">Git</span>
</div>
<!-- GitHub -->
<div class="glass-card tech-card p-3.5 rounded-xl flex flex-col items-center justify-center gap-2.5 group cursor-pointer border border-slate-800/90">
<div class="w-10 h-10 rounded-xl bg-slate-100/15 border border-slate-100/30 flex items-center justify-center text-slate-100 text-xl group-hover:scale-110 group-hover:shadow-[0_0_15px_rgba(241,245,249,0.5)] transition-all">
<i class="fa-brands fa-github"></i>
</div>
<span class="text-xs font-medium text-slate-300 group-hover:text-white transition-colors">GitHub</span>
</div>
<!-- Docker -->
<div class="glass-card tech-card p-3.5 rounded-xl flex flex-col items-center justify-center gap-2.5 group cursor-pointer border border-slate-800/90">
<div class="w-10 h-10 rounded-xl bg-sky-500/15 border border-sky-500/30 flex items-center justify-center text-sky-400 text-xl group-hover:scale-110 group-hover:shadow-[0_0_15px_rgba(14,165,233,0.5)] transition-all">
<i class="fa-brands fa-docker"></i>
</div>
<span class="text-xs font-medium text-slate-300 group-hover:text-sky-300 transition-colors">Docker</span>
</div>
<!-- PostgreSQL / Database -->
<div class="glass-card tech-card p-3.5 rounded-xl flex flex-col items-center justify-center gap-2.5 group cursor-pointer border border-slate-800/90">
<div class="w-10 h-10 rounded-xl bg-sky-600/15 border border-sky-600/30 flex items-center justify-center text-sky-400 text-lg group-hover:scale-110 group-hover:shadow-[0_0_15px_rgba(2,132,199,0.5)] transition-all">
<i class="fa-solid fa-database"></i>
</div>
<span class="text-xs font-medium text-slate-300 group-hover:text-sky-300 transition-colors">PostgreSQL</span>
</div>
<!-- MongoDB -->
<div class="glass-card tech-card p-3.5 rounded-xl flex flex-col items-center justify-center gap-2.5 group cursor-pointer border border-slate-800/90">
<div class="w-10 h-10 rounded-xl bg-emerald-600/15 border border-emerald-600/30 flex items-center justify-center text-emerald-400 text-lg group-hover:scale-110 group-hover:shadow-[0_0_15px_rgba(5,150,105,0.5)] transition-all">
<i class="fa-solid fa-leaf"></i>
</div>
<span class="text-xs font-medium text-slate-300 group-hover:text-emerald-300 transition-colors">MongoDB</span>
</div>
<!-- Terminal / Bash -->
<div class="glass-card tech-card p-3.5 rounded-xl flex flex-col items-center justify-center gap-2.5 group cursor-pointer border border-slate-800/90">
<div class="w-10 h-10 rounded-xl bg-teal-500/15 border border-teal-500/30 flex items-center justify-center text-teal-400 text-lg group-hover:scale-110 group-hover:shadow-[0_0_15px_rgba(20,184,166,0.5)] transition-all">
<i class="fa-solid fa-terminal"></i>
</div>
<span class="text-xs font-medium text-slate-300 group-hover:text-teal-300 transition-colors">Terminal</span>
</div>
<!-- Figma -->
<div class="glass-card tech-card p-3.5 rounded-xl flex flex-col items-center justify-center gap-2.5 group cursor-pointer border border-slate-800/90">
<div class="w-10 h-10 rounded-xl bg-purple-500/15 border border-purple-500/30 flex items-center justify-center text-purple-400 text-xl group-hover:scale-110 group-hover:shadow-[0_0_15px_rgba(168,85,247,0.5)] transition-all">
<i class="fa-brands fa-figma"></i>
</div>
<span class="text-xs font-medium text-slate-300 group-hover:text-purple-300 transition-colors">Figma</span>
</div>
<!-- Postman / API -->
<div class="glass-card tech-card p-3.5 rounded-xl flex flex-col items-center justify-center gap-2.5 group cursor-pointer border border-slate-800/90">
<div class="w-10 h-10 rounded-xl bg-orange-600/15 border border-orange-600/30 flex items-center justify-center text-orange-400 text-lg group-hover:scale-110 group-hover:shadow-[0_0_15px_rgba(234,88,12,0.5)] transition-all">
<i class="fa-solid fa-paper-plane"></i>
</div>
<span class="text-xs font-medium text-slate-300 group-hover:text-orange-300 transition-colors">Postman</span>
</div>
</div>
</section>
<!-- Featured Focus & Climatic Terminal Highlights -->
<section class="grid grid-cols-1 md:grid-cols-2 gap-4">
<!-- Current Trajectory / Highlights -->
<div class="glass-card p-5 rounded-2xl border border-slate-700/60 flex flex-col justify-between hover:border-cyan-500/40 transition-colors shadow-lg">
<div>
<div class="flex items-center gap-2 text-cyan-400 mb-3">
<i class="fa-solid fa-satellite-dish text-cyan-300 animate-pulse"></i>
<h3 class="font-bold text-white text-sm uppercase tracking-wider font-mono">Current Trajectory</h3>
</div>
<ul class="space-y-3 text-xs text-slate-300">
<li class="flex items-start gap-2.5">
<span class="w-1.5 h-1.5 rounded-full bg-cyan-400 mt-1.5 shrink-0 shadow-[0_0_8px_#22d3ee]"></span>
<span><strong class="text-slate-100">Architecture:</strong> Distributed systems &amp; low-latency microservices</span>
</li>
<li class="flex items-start gap-2.5">
<span class="w-1.5 h-1.5 rounded-full bg-teal-400 mt-1.5 shrink-0 shadow-[0_0_8px_#2dd4bf]"></span>
<span><strong class="text-slate-100">AI Tooling:</strong> Agentic workflows and LLM orchestration</span>
</li>
<li class="flex items-start gap-2.5">
<span class="w-1.5 h-1.5 rounded-full bg-amber-400 mt-1.5 shrink-0 shadow-[0_0_8px_#fbbf24]"></span>
<span><strong class="text-slate-100">Core Focus:</strong> Lightning-fast responsive web applications</span>
</li>
</ul>
</div>
<div class="mt-4 pt-3 border-t border-slate-800/80 flex items-center justify-between text-[11px] text-slate-400">
<span class="flex items-center gap-2">
<span class="relative flex h-2 w-2">
<span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-emerald-400 opacity-75"></span>
<span class="relative inline-flex rounded-full h-2 w-2 bg-emerald-400 shadow-[0_0_6px_#34d399]"></span>
</span>
              Collaboration Open
            </span>
<span class="text-cyan-300 font-mono font-medium">Available for projects</span>
</div>
</div>
<!-- Climatic Code Snippet & Aesthetic Terminal -->
<div class="glass-card p-5 rounded-2xl border border-slate-700/60 font-mono text-xs flex flex-col justify-between hover:border-cyan-500/40 transition-colors shadow-lg">
<div>
<div class="flex items-center justify-between text-slate-400 mb-2.5 border-b border-slate-800/80 pb-2">
<span class="flex items-center gap-1.5 text-cyan-300 font-medium">
<i class="fa-solid fa-terminal text-[10px]"></i> console.log
              </span>
<span class="text-[10px] text-slate-500">zsh --utf8</span>
</div>
<div class="text-slate-300 leading-relaxed space-y-1">
<p><span class="text-purple-400">const</span> <span class="text-cyan-300">jegathDev</span> = {</p>
<p class="pl-4">weather: <span class="text-amber-300">"rainy twilight"</span>,</p>
<p class="pl-4">focus: <span class="text-teal-300">"unbreakable"</span>,</p>
<p class="pl-4">coffeeLevel: <span class="text-emerald-300">"high"</span>,</p>
<p class="pl-4">motto: <span class="text-cyan-200">"Build things that feel alive."</span><span class="cursor-shimmer ml-1"></span></p>
<p>};</p>
</div>
</div>
<div class="mt-3 text-[11px] text-cyan-400/90 flex items-center gap-1.5">
<i class="fa-solid fa-circle-check text-emerald-400 text-[10px]"></i> Environment synced successfully
          </div>
</div>
</section>
<!-- Connect & Socials Section -->
<section class="glass-panel rounded-2xl p-6 border border-cyan-500/30 text-center relative overflow-hidden shadow-xl">
<div class="absolute inset-0 bg-gradient-to-r from-cyan-500/10 via-violet-600/10 to-teal-500/10 pointer-events-none"></div>
<h3 class="text-base font-bold text-white mb-2 tracking-wide flex items-center justify-center gap-2">
<i class="fa-solid fa-paper-plane text-cyan-400"></i>
          Connect With Me
        </h3>
<p class="text-xs text-slate-400 max-w-md mx-auto mb-5">
          Reach out for collaborations, discussions on tech, or open-source projects!
        </p>
<div class="flex flex-wrap items-center justify-center gap-3">
<a class="px-4 py-2 rounded-xl bg-slate-900/90 hover:bg-cyan-950 text-cyan-300 text-xs font-medium border border-cyan-500/30 transition-all flex items-center gap-2 shadow-sm hover:shadow-[0_0_18px_rgba(6,182,212,0.35)] hover:border-cyan-400 hover:-translate-y-0.5" href="#">
<i class="fa-brands fa-github text-sm"></i> GitHub
          </a>
<a class="px-4 py-2 rounded-xl bg-slate-900/90 hover:bg-blue-950 text-blue-300 text-xs font-medium border border-blue-500/30 transition-all flex items-center gap-2 shadow-sm hover:shadow-[0_0_18px_rgba(59,130,246,0.35)] hover:border-blue-400 hover:-translate-y-0.5" href="#">
<i class="fa-brands fa-linkedin text-sm"></i> LinkedIn
          </a>
<a class="px-4 py-2 rounded-xl bg-slate-900/90 hover:bg-sky-950 text-sky-300 text-xs font-medium border border-sky-500/30 transition-all flex items-center gap-2 shadow-sm hover:shadow-[0_0_18px_rgba(14,165,233,0.35)] hover:border-sky-400 hover:-translate-y-0.5" href="#">
<i class="fa-brands fa-x-twitter text-sm"></i> Twitter / X
          </a>
<a class="px-4 py-2 rounded-xl bg-slate-900/90 hover:bg-rose-950 text-rose-300 text-xs font-medium border border-rose-500/30 transition-all flex items-center gap-2 shadow-sm hover:shadow-[0_0_18px_rgba(244,63,94,0.35)] hover:border-rose-400 hover:-translate-y-0.5" href="#">
<i class="fa-solid fa-envelope text-sm"></i> Mail Me
          </a>
</div>
</section>
</div>
<!-- Footer Bar -->
<div class="px-6 py-3.5 bg-gradient-to-r from-[#060b18]/95 via-[#081022]/95 to-[#060b18]/95 border-t border-slate-800 flex items-center justify-between text-[11px] text-slate-400 font-mono">
<span>Crafted with climatic serenity &amp; modern code</span>
<span class="text-cyan-300 flex items-center gap-1.5">
<span class="w-1.5 h-1.5 rounded-full bg-cyan-400 animate-pulse"></span>
        ✦ aesthetic edition
      </span>
</div>
</main>
</body></html>
