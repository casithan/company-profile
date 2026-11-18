<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>TKJ — Teknik Komputer & Jaringan | Profil Jurusan</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            navy: {
              950: '#040814',
              900: '#091126',
              800: '#0f1c3f',
              700: '#16295c',
            },
            cyan: {
              400: '#22d3ee',
              500: '#06b6d4',
            }
          },
          fontFamily: {
            sans: ['Inter', 'system-ui', 'sans-serif'],
            mono: ['JetBrains Mono', 'monospace'],
          }
        }
      }
    }
  </script>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=JetBrains+Mono:wght@400;600&display=swap" rel="stylesheet">
  <style>
    body {
      background-color: #040814;
      color: #f8fafc;
    }
    .glass {
      background: rgba(15, 28, 63, 0.45);
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      border: 1px solid rgba(34, 211, 238, 0.15);
    }
    .glass-card {
      background: linear-gradient(145deg, rgba(15, 28, 63, 0.65), rgba(9, 17, 38, 0.85));
      backdrop-filter: blur(10px);
      border: 1px solid rgba(255, 255, 255, 0.08);
      transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
    }
    .glass-card:hover {
      border-color: rgba(34, 211, 238, 0.45);
      transform: translateY(-4px);
      box-shadow: 0 12px 30px -10px rgba(6, 182, 212, 0.25);
    }
    .grid-bg {
      background-size: 40px 40px;
      background-image: 
        linear-gradient(to right, rgba(34, 211, 238, 0.05) 1px, transparent 1px),
        linear-gradient(to bottom, rgba(34, 211, 238, 0.05) 1px, transparent 1px);
    }
    .glow-orb {
      background: radial-gradient(circle, rgba(6, 182, 212, 0.22) 0%, rgba(4, 8, 20, 0) 70%);
    }
  </style>
</head>
<body class="antialiased selection:bg-cyan-500 selection:text-navy-950">

  <!-- Navbar -->
  <header class="fixed top-0 left-0 right-0 z-50 glass border-b border-white/10">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-16">
        <a href="#" class="flex items-center gap-3 group">
          <div class="w-9 h-9 rounded-lg bg-gradient-to-br from-cyan-400 to-blue-600 flex items-center justify-center font-mono font-bold text-navy-950 shadow-lg shadow-cyan-500/30">
            &lt;/&gt;
          </div>
          <div>
            <span class="font-bold text-lg tracking-tight text-white">TKJ<span class="text-cyan-400">.NET</span></span>
            <span class="hidden sm:inline-block text-xs text-slate-400 ml-2 border-l border-slate-700 pl-2">Teknik Komputer & Jaringan</span>
          </div>
        </a>

        <!-- Desktop Nav -->
        <nav class="hidden md:flex items-center gap-8 text-sm font-medium text-slate-300">
          <a href="#tentang" class="hover:text-cyan-400 transition">Tentang</a>
          <a href="#kompetensi" class="hover:text-cyan-400 transition">Kompetensi</a>
          <a href="#fasilitas" class="hover:text-cyan-400 transition">Fasilitas Lab</a>
          <a href="#proyek" class="hover:text-cyan-400 transition">Karya Siswa</a>
          <a href="#karir" class="hover:text-cyan-400 transition">Prospek Karir</a>
        </nav>

        <div class="hidden md:flex items-center gap-3">
          <a href="#daftar" class="px-4 py-2 rounded-lg bg-cyan-500 hover:bg-cyan-400 text-navy-950 font-semibold text-sm transition shadow-lg shadow-cyan-500/20">
            Info PPDB
          </a>
        </div>

        <!-- Mobile Menu Button -->
        <button id="mobile-menu-btn" class="md:hidden p-2 rounded-lg text-slate-300 hover:text-white hover:bg-white/5">
          <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"/>
          </svg>
        </button>
      </div>
    </div>

    <!-- Mobile Menu -->
    <div id="mobile-menu" class="hidden md:hidden bg-navy-900/95 border-b border-white/10 px-4 pt-2 pb-5 space-y-2">
      <a href="#tentang" class="block px-3 py-2 rounded-lg text-slate-300 hover:bg-white/5 hover:text-cyan-400">Tentang</a>
      <a href="#kompetensi" class="block px-3 py-2 rounded-lg text-slate-300 hover:bg-white/5 hover:text-cyan-400">Kompetensi</a>
      <a href="#fasilitas" class="block px-3 py-2 rounded-lg text-slate-300 hover:bg-white/5 hover:text-cyan-400">Fasilitas Lab</a>
      <a href="#proyek" class="block px-3 py-2 rounded-lg text-slate-300 hover:bg-white/5 hover:text-cyan-400">Karya Siswa</a>
      <a href="#karir" class="block px-3 py-2 rounded-lg text-slate-300 hover:bg-white/5 hover:text-cyan-400">Prospek Karir</a>
      <a href="#daftar" class="block mt-2 text-center px-4 py-2.5 rounded-lg bg-cyan-500 text-navy-950 font-semibold">Info PPDB</a>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="relative pt-28 pb-20 lg:pt-36 lg:pb-28 overflow-hidden grid-bg">
    <div class="glow-orb absolute top-10 left-1/2 -translate-x-1/2 w-[700px] h-[500px] pointer-events-none"></div>
    
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
      <div class="grid lg:grid-cols-12 gap-12 items-center">
        <div class="lg:col-span-7 space-y-6">
          <div class="inline-flex items-center gap-2 px-3 py-1.5 rounded-full bg-cyan-500/10 border border-cyan-500/30 text-cyan-400 text-xs font-mono">
            <span class="w-2 h-2 rounded-full bg-cyan-400 animate-ping"></span>
            AKREDITASI A • KURIKULUM STANDAR INDUSTRI
          </div>
          
          <h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold tracking-tight leading-tight">
            Membangun Infrastruktur <span class="text-transparent bg-clip-text bg-gradient-to-r from-cyan-400 to-blue-500">Digital Masa Depan</span>
          </h1>
          
          <p class="text-slate-300 text-lg leading-relaxed max-w-2xl">
            Program Keahlian <strong>Teknik Komputer dan Jaringan (TKJ)</strong> mencetak teknisi jaringan, administrator server, spesialis keamanan siber, dan engineer cloud yang siap terjun langsung ke dunia industri modern.
          </p>

          <div class="flex flex-wrap gap-4 pt-2">
            <a href="#kompetensi" class="px-6 py-3.5 rounded-xl bg-cyan-500 hover:bg-cyan-400 text-navy-950 font-bold transition shadow-lg shadow-cyan-500/25 flex items-center gap-2">
              Eksplorasi Kompetensi
              <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 7l5 5m0 0l-5 5m5-5H6"/></svg>
            </a>
            <a href="#proyek" class="px-6 py-3.5 rounded-xl glass hover:bg-white/10 text-white font-semibold transition">
              Lihat Karya Siswa
            </a>
          </div>

          <!-- Stats -->
          <div class="grid grid-cols-3 gap-6 pt-8 border-t border-white/10">
            <div>
              <div class="text-2xl sm:text-3xl font-extrabold text-white">95%</div>
              <div class="text-xs sm:text-sm text-slate-400">Serapan Kerja & Kuliah</div>
            </div>
            <div>
              <div class="text-2xl sm:text-3
              
