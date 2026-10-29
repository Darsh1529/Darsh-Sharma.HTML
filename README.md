<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Darsh Sharma | Class 9 Student Portfolio</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts: Inter & Outfit -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Outfit:wght@500;600;700;800&display=swap" rel="stylesheet">
    <!-- Canvas Confetti -->
    <script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.6.0/dist/confetti.browser.min.js"></script>
    
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        brand: {
                            navy: '#0b132b',
                            blue: '#1c2541',
                            cyan: '#00f5d4',
                            electric: '#3a86ff',
                            gold: '#ffb703',
                            orange: '#fb8500'
                        }
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        heading: ['Outfit', 'sans-serif']
                    }
                }
            }
        }
    </script>
    <style>
        .glow-cyan {
            box-shadow: 0 0 20px rgba(0, 245, 212, 0.35);
        }
        .glow-electric {
            box-shadow: 0 0 20px rgba(58, 134, 255, 0.35);
        }
        .bg-grid-pattern {
            background-image: radial-gradient(rgba(255, 255, 255, 0.1) 1px, transparent 1px);
            background-size: 24px 24px;
        }
        .glass-card {
            background: rgba(28, 37, 65, 0.7);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
    </style>
</head>
<body class="bg-brand-navy text-slate-100 font-sans min-h-screen selection:bg-brand-cyan selection:text-brand-navy">

    <!-- Navigation Bar -->
    <nav class="fixed top-0 left-0 right-0 z-50 bg-brand-navy/80 backdrop-blur-md border-b border-white/10">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-16">
                <!-- Logo & Name -->
                <div class="flex items-center space-x-3">
                    <div class="w-10 h-10 rounded-xl bg-gradient-to-tr from-brand-cyan to-brand-electric flex items-center justify-center text-brand-navy font-heading font-extrabold text-xl shadow-lg">
                        DS
                    </div>
                    <div>
                        <span class="font-heading font-bold text-lg text-white block leading-tight">Darsh Sharma</span>
                        <span class="text-xs text-brand-cyan font-medium block">Narayana E-Techno, Vidisha</span>
                    </div>
                </div>

                <!-- Desktop Nav Links -->
                <div class="hidden md:flex items-center space-x-6 text-sm font-medium">
                    <a href="#about" class="text-slate-300 hover:text-brand-cyan transition-colors">About</a>
                    <a href="#projects" class="text-slate-300 hover:text-brand-cyan transition-colors">Projects</a>
                    <a href="#achievements" class="text-slate-300 hover:text-brand-cyan transition-colors">Achievements</a>
                    <a href="#skills" class="text-slate-300 hover:text-brand-cyan transition-colors">Skills</a>
                    <a href="#timeline" class="text-slate-300 hover:text-brand-cyan transition-colors">Timeline</a>
                    <a href="#interactive" class="text-slate-300 hover:text-brand-cyan transition-colors">STEM Quiz</a>
                    <a href="#guestbook" class="px-4 py-2 rounded-lg bg-gradient-to-r from-brand-cyan to-brand-electric text-brand-navy font-bold hover:shadow-lg hover:shadow-brand-cyan/20 transition-all">
                        Guestbook
                    </a>
                </div>

                <!-- Mobile Menu Button -->
                <button id="mobile-menu-btn" class="md:hidden text-slate-300 hover:text-white p-2">
                    <i class="fa-solid fa-bars text-xl"></i>
                </button>
            </div>
        </div>

        <!-- Mobile Navigation Drawer -->
        <div id="mobile-menu" class="hidden md:hidden bg-brand-blue border-b border-white/10 px-4 pt-2 pb-4 space-y-2">
            <a href="#about" class="mobile-nav-link block px-3 py-2 rounded-md text-slate-300 hover:text-brand-cyan">About</a>
            <a href="#projects" class="mobile-nav-link block px-3 py-2 rounded-md text-slate-300 hover:text-brand-cyan">Projects</a>
            <a href="#achievements" class="mobile-nav-link block px-3 py-2 rounded-md text-slate-300 hover:text-brand-cyan">Achievements</a>
            <a href="#skills" class="mobile-nav-link block px-3 py-2 rounded-md text-slate-300 hover:text-brand-cyan">Skills</a>
            <a href="#timeline" class="mobile-nav-link block px-3 py-2 rounded-md text-slate-300 hover:text-brand-cyan">Timeline</a>
            <a href="#interactive" class="mobile-nav-link block px-3 py-2 rounded-md text-slate-300 hover:text-brand-cyan">STEM Quiz</a>
            <a href="#guestbook" class="mobile-nav-link block px-3 py-2 rounded-md text-brand-cyan font-bold">Guestbook</a>
        </div>
    </nav>

    <!-- Hero Header -->
    <header class="pt-28 pb-20 relative overflow-hidden bg-grid-pattern">
        <!-- Radial gradient background highlight -->
        <div class="absolute top-1/4 left-1/2 -translate-x-1/2 -translate-y-1/2 w-96 h-96 bg-brand-electric/20 rounded-full blur-3xl pointer-events-none"></div>
        <div class="absolute bottom-10 right-10 w-80 h-80 bg-brand-cyan/10 rounded-full blur-3xl pointer-events-none"></div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="flex flex-col lg:flex-row items-center justify-between gap-12">
                <!-- Left Text Content -->
                <div class="flex-1 text-center lg:text-left">
                    <div class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full bg-brand-blue border border-brand-cyan/30 text-brand-cyan text-sm font-semibold mb-6">
                        <i class="fa-solid fa-atom animate-spin-slow"></i>
                        <span>Narayana STEM & Innovation Club</span>
                    </div>
                    <h1 class="font-heading text-4xl sm:text-5xl lg:text-6xl font-extrabold tracking-tight text-white leading-tight">
                        Hello, I'm <br class="hidden sm:inline">
                        <span class="bg-gradient-to-r from-brand-cyan via-brand-electric to-brand-gold bg-clip-text text-transparent">
                            Darsh Sharma
                        </span>
                    </h1>
                    <p class="mt-4 text-lg text-slate-300 font-medium">
                        Class 9 Student & Young Innovator at <span class="text-white font-semibold">Narayana E-Techno School, Vidisha (M.P.)</span>
                    </p>
                    <p class="mt-2 text-slate-400 max-w-xl mx-auto lg:mx-0 text-sm sm:text-base">
                        Passionate about Robotics, Coding, and Eco-Tech solutions. Driven by curiosity and dedicated to building creative STEM projects for school and community impact.
                    </p>

                    <!-- Motto Badges -->
                    <div class="mt-6 flex flex-wrap justify-center lg:justify-start gap-3">
                        <span class="px-3 py-1 rounded-md bg-brand-blue/80 border border-white/10 text-xs font-mono text-brand-cyan flex items-center gap-1.5">
                            <i class="fa-solid fa-magnifying-glass"></i> INQUIRE
                        </span>
                        <span class="px-3 py-1 rounded-md bg-brand-blue/80 border border-white/10 text-xs font-mono text-brand-gold flex items-center gap-1.5">
                            <i class="fa-solid fa-lightbulb"></i> INNOVATE
                        </span>
                        <span class="px-3 py-1 rounded-md bg-brand-blue/80 border border-white/10 text-xs font-mono text-brand-electric flex items-center gap-1.5">
                            <i class="fa-solid fa-rocket"></i> INSPIRE
                        </span>
                    </div>

                    <!-- Call to Actions -->
                    <div class="mt-8 flex flex-wrap justify-center lg:justify-start gap-4">
                        <a href="#projects" class="px-6 py-3 rounded-xl bg-gradient-to-r from-brand-cyan to-brand-electric text-brand-navy font-bold text-sm shadow-lg hover:shadow-brand-cyan/25 hover:-translate-y-0.5 transition-all flex items-center gap-2">
                            <i class="fa-solid fa-diagram-project"></i> View Club Projects
                        </a>
                        <a href="#guestbook" class="px-6 py-3 rounded-xl bg-brand-blue hover:bg-brand-blue/80 border border-white/10 text-slate-200 font-semibold text-sm transition-all flex items-center gap-2">
                            <i class="fa-solid fa-pen-to-square"></i> Leave Message
                        </a>
                    </div>
                </div>

                <!-- Right Avatar & Interactive Card Placeholder -->
                <div class="flex-1 max-w-md w-full">
                    <div class="relative glass-card rounded-3xl p-6 glow-cyan transition-all duration-500 hover:scale-[1.02]">
                        <div class="absolute -top-3 -right-3 bg-brand-gold text-brand-navy font-extrabold text-xs px-3 py-1 rounded-full shadow-lg">
                            CLASS 9th
                        </div>
                        
                        <!-- Avatar Container -->
                        <div class="relative w-40 h-40 mx-auto mb-6 rounded-2xl overflow-hidden bg-gradient-to-tr from-brand-electric to-brand-cyan p-1">
                            <div class="w-full h-full bg-brand-blue rounded-xl flex items-center justify-center relative overflow-hidden">
                                <!-- SVG Student Avatar -->
                                <svg class="w-32 h-32 text-slate-300" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 3c1.66 0 3 1.34 3 3s-1.34 3-3 3-3-1.34-3-3 1.34-3 3-3zm0 14.2c-2.5 0-4.71-1.28-6-3.22.03-1.99 4-3.08 6-3.08 1.99 0 5.97 1.09 6 3.08-1.29 1.94-3.5 3.22-6 3.22z"/>
                                </svg>
                                <div class="absolute bottom-2 bg-brand-navy/90 text-brand-cyan text-[10px] font-mono px-2 py-0.5 rounded">
                                    VIDISHA (M.P.)
                                </div>
                            </div>
                        </div>

                        <!-- Card Info -->
                        <div class="text-center space-y-2">
                            <h2 class="font-heading font-bold text-xl text-white">Darsh Sharma</h2>
                            <p class="text-xs text-slate-400 font-mono">School ID: NETS-VID-2026-9A</p>
                            
                            <div class="pt-3 border-t border-white/10 grid grid-cols-3 gap-2 text-center text-xs">
                                <div class="p-2 rounded-lg bg-brand-navy/50">
                                    <span class="block font-bold text-brand-cyan text-base">4+</span>
                                    <span class="text-slate-400">Projects</span>
                                </div>
                                <div class="p-2 rounded-lg bg-brand-navy/50">
                                    <span class="block font-bold text-brand-gold text-base">3</span>
                                    <span class="text-slate-400">Awards</span>
                                </div>
                                <div class="p-2 rounded-lg bg-brand-navy/50">
                                    <span class="block font-bold text-brand-electric text-base">95%</span>
                                    <span class="text-slate-400">STEM Score</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </header>

    <!-- About Me Section -->
    <section id="about" class="py-16 bg-brand-blue/40 border-y border-white/5">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-12">
                <h2 class="text-xs font-mono text-brand-cyan uppercase tracking-widest mb-2">Student Profile</h2>
                <h3 class="font-heading text-3xl font-bold text-white">About Darsh Sharma</h3>
                <div class="w-16 h-1 bg-brand-cyan mx-auto mt-3 rounded-full"></div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Academic Focus -->
                <div class="glass-card p-6 rounded-2xl hover:border-brand-cyan/50 transition-all">
                    <div class="w-12 h-12 rounded-xl bg-brand-cyan/10 text-brand-cyan flex items-center justify-center text-xl mb-4">
                        <i class="fa-solid fa-graduation-cap"></i>
                    </div>
                    <h4 class="font-heading font-bold text-lg text-white mb-2">Academic Drive</h4>
                    <p class="text-slate-300 text-sm leading-relaxed">
                        Currently studying in Class 9 at Narayana E-Techno School, Vidisha. Deeply interested in Physics, Applied Mathematics, and Computer Science concepts.
                    </p>
                </div>

                <!-- Club Participation -->
                <div class="glass-card p-6 rounded-2xl hover:border-brand-electric/50 transition-all">
                    <div class="w-12 h-12 rounded-xl bg-brand-electric/10 text-brand-electric flex items-center justify-center text-xl mb-4">
                        <i class="fa-solid fa-users-gear"></i>
                    </div>
                    <h4 class="font-heading font-bold text-lg text-white mb-2">Club Role</h4>
                    <p class="text-slate-300 text-sm leading-relaxed">
                        Active student lead in the School Science & Robotics Club. I enjoy collaborating on team prototypes, organizing tech demos, and presenting at school expos.
                    </p>
                </div>

                <!-- Future Aspirations -->
                <div class="glass-card p-6 rounded-2xl hover:border-brand-gold/50 transition-all">
                    <div class="w-12 h-12 rounded-xl bg-brand-gold/10 text-brand-gold flex items-center justify-center text-xl mb-4">
                        <i class="fa-solid fa-microchip"></i>
                    </div>
                    <h4 class="font-heading font-bold text-lg text-white mb-2">Tech Vision</h4>
                    <p class="text-slate-300 text-sm leading-relaxed">
                        Aiming to build smart eco-friendly IoT devices that solve local agricultural and urban challenges in Madhya Pradesh using modern hardware and web tools.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Club & Projects Section -->
    <section id="projects" class="py-20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col md:flex-row md:items-end justify-between mb-10">
                <div>
                    <h2 class="text-xs font-mono text-brand-cyan uppercase tracking-widest mb-2">Portfolio Showcase</h2>
                    <h3 class="font-heading text-3xl font-bold text-white">Featured Club Projects</h3>
                </div>

                <!-- Filter Buttons -->
                <div class="mt-4 md:mt-0 flex flex-wrap gap-2" id="project-filters">
                    <button class="filter-btn active px-4 py-2 rounded-lg text-xs font-bold transition-all bg-brand-cyan text-brand-navy" data-filter="all">All Projects</button>
                    <button class="filter-btn px-4 py-2 rounded-lg text-xs font-bold transition-all bg-brand-blue text-slate-300 hover:text-white" data-filter="robotics">Robotics</button>
                    <button class="filter-btn px-4 py-2 rounded-lg text-xs font-bold transition-all bg-brand-blue text-slate-300 hover:text-white" data-filter="ecotech">Eco-Tech</button>
                    <button class="filter-btn px-4 py-2 rounded-lg text-xs font-bold transition-all bg-brand-blue text-slate-300 hover:text-white" data-filter="math">Math & Science</button>
                </div>
            </div>

            <!-- Project Cards Grid -->
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8" id="projects-grid">
                
                <!-- Project 1 -->
                <div class="project-card glass-card rounded-2xl p-6 border border-white/10 hover:border-brand-cyan/50 transition-all flex flex-col justify-between" data-category="robotics">
                    <div>
                        <div class="flex justify-between items-start mb-4">
                            <span class="px-2.5 py-1 rounded bg-brand-cyan/10 text-brand-cyan text-xs font-semibold">Robotics Bot</span>
                            <span class="text-xs font-mono text-slate-400">Class Expo 2026</span>
                        </div>
                        <h4 class="font-heading font-bold text-xl text-white mb-2">Obstacle-Avoiding Rover (RoboVid)</h4>
                        <p class="text-slate-300 text-sm mb-4">
                            Designed and programmed a mini ultrasonic sensor-powered vehicle capable of detecting obstacles and dynamically recalculating its pathway.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-6">
                            <span class="text-[11px] font-mono px-2 py-0.5 rounded bg-brand-navy text-slate-300">Arduino Uno</span>
                            <span class="text-[11px] font-mono px-2 py-0.5 rounded bg-brand-navy text-slate-300">HC-SR04 Sensor</span>
                            <span class="text-[11px] font-mono px-2 py-0.5 rounded bg-brand-navy text-slate-300">C++ Programming</span>
                        </div>
                    </div>
                    <div>
                        <div class="mb-2 flex justify-between text-xs">
                            <span class="text-slate-400">Completion Status</span>
                            <span class="text-brand-cyan font-bold">100% (Completed)</span>
                        </div>
                        <div class="w-full bg-brand-navy h-2 rounded-full overflow-hidden">
                            <div class="bg-brand-cyan h-full rounded-full w-full"></div>
                        </div>
                    </div>
                </div>

                <!-- Project 2 -->
                <div class="project-card glass-card rounded-2xl p-6 border border-white/10 hover:border-brand-electric/50 transition-all flex flex-col justify-between" data-category="ecotech">
                    <div>
                        <div class="flex justify-between items-start mb-4">
                            <span class="px-2.5 py-1 rounded bg-brand-electric/10 text-brand-electric text-xs font-semibold">Eco-Tech</span>
                            <span class="text-xs font-mono text-slate-400">Green Club Initiative</span>
                        </div>
                        <h4 class="font-heading font-bold text-xl text-white mb-2">Smart Drip Irrigation Prototype</h4>
                        <p class="text-slate-300 text-sm mb-4">
                            An automated soil-moisture sensing system engineered to conserve water in home garden setups for Vidisha's local climate conditions.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-6">
                            <span class="text-[11px] font-mono px-2 py-0.5 rounded bg-brand-navy text-slate-300">Soil Probe</span>
                            <span class="text-[11px] font-mono px-2 py-0.5 rounded bg-brand-navy text-slate-300">Relay Switch</span>
                            <span class="text-[11px] font-mono px-2 py-0.5 rounded bg-brand-navy text-slate-300">Solar Power</span>
                        </div>
                    </div>
                    <div>
                        <div class="mb-2 flex justify-between text-xs">
                            <span class="text-slate-400">Completion Status</span>
                            <span class="text-brand-electric font-bold">85% (In Testing)</span>
                        </div>
                        <div class="w-full bg-brand-navy h-2 rounded-full overflow-hidden">
                            <div class="bg-brand-electric h-full rounded-full w-[85%]"></div>
                        </div>
                    </div>
                </div>

                <!-- Project 3 -->
                <div class="project-card glass-card rounded-2xl p-6 border border-white/10 hover:border-brand-gold/50 transition-all flex flex-col justify-between" data-category="math">
                    <div>
                        <div class="flex justify-between items-start mb-4">
                            <span class="px-2.5 py-1 rounded bg-brand-gold/10 text-brand-gold text-xs font-semibold">Math Club Challenge</span>
                            <span class="text-xs font-mono text-slate-400">Math Olympiad Activity</span>
                        </div>
                        <h4 class="font-heading font-bold text-xl text-white mb-2">Pythagorean Geometry Modeler</h4>
                        <p class="text-slate-300 text-sm mb-4">
                            An interactive visual aid created using cardboard, light sensors, and web code to demonstrate trigonometric ratios and Pythagorean theorems to junior students.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-6">
                            <span class="text-[11px] font-mono px-2 py-0.5 rounded bg-brand-navy text-slate-300">HTML/CSS</span>
                            <span class="text-[11px] font-mono px-2 py-0.5 rounded bg-brand-navy text-slate-300">Geometry Kit</span>
                            <span class="text-[11px] font-mono px-2 py-0.5 rounded bg-brand-navy text-slate-300">Logic Design</span>
                        </div>
                    </div>
                    <div>
                        <div class="mb-2 flex justify-between text-xs">
                            <span class="text-slate-400">Completion Status</span>
                            <span class="text-brand-gold font-bold">100% (Presented)</span>
                        </div>
                        <div class="w-full bg-brand-navy h-2 rounded-full overflow-hidden">
                            <div class="bg-brand-gold h-full rounded-full w-full"></div>
                        </div>
                    </div>
                </div>

                <!-- Project 4 -->
                <div class="project-card glass-card rounded-2xl p-6 border border-white/10 hover:border-brand-cyan/50 transition-all flex flex-col justify-between" data-category="robotics">
                    <div>
                        <div class="flex justify-between items-start mb-4">
                            <span class="px-2.5 py-1 rounded bg-brand-cyan/10 text-brand-cyan text-xs font-semibold">Coding & AI</span>
                            <span class="text-xs font-mono text-slate-400">Class 9 Web Project</span>
                        </div>
                        <h4 class="font-heading font-bold text-xl text-white mb-2">Student Club Interactive Portal</h4>
                        <p class="text-slate-300 text-sm mb-4">
                            This responsive web portfolio platform designed to showcase club activities, student projects, and interactive quizzes for Narayana E-Techno School.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-6">
                            <span class="text-[11px] font-mono px-2 py-0.5 rounded bg-brand-navy text-slate-300">Tailwind CSS</span>
                            <span class="text-[11px] font-mono px-2 py-0.5 rounded bg-brand-navy text-slate-300">JavaScript</span>
                            <span class="text-[11px] font-mono px-2 py-0.5 rounded bg-brand-navy text-slate-300">UI/UX</span>
                        </div>
                    </div>
                    <div>
                        <div class="mb-2 flex justify-between text-xs">
                            <span class="text-slate-400">Completion Status</span>
                            <span class="text-brand-cyan font-bold">90% (Live Demo)</span>
                        </div>
                        <div class="w-full bg-brand-navy h-2 rounded-full overflow-hidden">
                            <div class="bg-brand-cyan h-full rounded-full w-[90%]"></div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- Achievements Section -->
    <section id="achievements" class="py-16 bg-brand-blue/30 border-y border-white/5">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-12">
                <h2 class="text-xs font-mono text-brand-cyan uppercase tracking-widest mb-2">Recognitions</h2>
                <h3 class="font-heading text-3xl font-bold text-white">Academic & Co-Curricular Badges</h3>
                <div class="w-16 h-1 bg-brand-gold mx-auto mt-3 rounded-full"></div>
            </div>

            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6">
                <!-- Badge 1 -->
                <div class="glass-card p-6 rounded-2xl text-center border border-white/10 hover:border-brand-gold transition-all group">
                    <div class="w-16 h-16 mx-auto rounded-2xl bg-brand-gold/10 text-brand-gold flex items-center justify-center text-3xl mb-4 group-hover:scale-110 transition-transform">
                        <i class="fa-solid fa-trophy"></i>
                    </div>
                    <h4 class="font-heading font-bold text-white mb-1">Science Expo Winner</h4>
                    <p class="text-xs text-brand-gold font-medium mb-2">1st Rank - Inter-Class 2025</p>
                    <p class="text-slate-400 text-xs">Awarded for the Obstacle-Avoiding Rover prototype model presentation.</p>
                </div>

                <!-- Badge 2 -->
                <div class="glass-card p-6 rounded-2xl text-center border border-white/10 hover:border-brand-cyan transition-all group">
                    <div class="w-16 h-16 mx-auto rounded-2xl bg-brand-cyan/10 text-brand-cyan flex items-center justify-center text-3xl mb-4 group-hover:scale-110 transition-transform">
                        <i class="fa-solid fa-award"></i>
                    </div>
                    <h4 class="font-heading font-bold text-white mb-1">Math Olympiad Medalist</h4>
                    <p class="text-xs text-brand-cyan font-medium mb-2">School Level Distinction</p>
                    <p class="text-slate-400 text-xs">Recognized for top problem-solving percentile in Class 8/9 competitive math.</p>
                </div>

                <!-- Badge 3 -->
                <div class="glass-card p-6 rounded-2xl text-center border border-white/10 hover:border-brand-electric transition-all group">
                    <div class="w-16 h-16 mx-auto rounded-2xl bg-brand-electric/10 text-brand-electric flex items-center justify-center text-3xl mb-4 group-hover:scale-110 transition-transform">
                        <i class="fa-solid fa-star"></i>
                    </div>
                    <h4 class="font-heading font-bold text-white mb-1">Best Club Presenter</h4>
                    <p class="text-xs text-brand-electric font-medium mb-2">Narayana E-Techno Club</p>
                    <p class="text-slate-400 text-xs">Awarded by club mentor for clear technical demonstration and peer engagement.</p>
                </div>

                <!-- Badge 4 -->
                <div class="glass-card p-6 rounded-2xl text-center border border-white/10 hover:border-brand-orange transition-all group">
                    <div class="w-16 h-16 mx-auto rounded-2xl bg-brand-orange/10 text-brand-orange flex items-center justify-center text-3xl mb-4 group-hover:scale-110 transition-transform">
                        <i class="fa-solid fa-seedling"></i>
                    </div>
                    <h4 class="font-heading font-bold text-white mb-1">Eco Innovator Cert</h4>
                    <p class="text-xs text-brand-orange font-medium mb-2">District Green School Activity</p>
                    <p class="text-slate-400 text-xs">Honored for contributing smart irrigation design concepts for water conservation.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Interactive Skills Section -->
    <section id="skills" class="py-20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                
                <div>
                    <h2 class="text-xs font-mono text-brand-cyan uppercase tracking-widest mb-2">Capabilities</h2>
                    <h3 class="font-heading text-3xl font-bold text-white mb-4">Skills & Technical Proficiency</h3>
                    <p class="text-slate-300 text-sm leading-relaxed mb-6">
                        Combining academic core subjects with practical hands-on technology skills to create balanced STEM projects.
                    </p>

                    <!-- Skill Progress Bars -->
                    <div class="space-y-5">
                        <!-- Skill 1 -->
                        <div>
                            <div class="flex justify-between text-xs font-semibold mb-1">
                                <span class="text-white flex items-center gap-2"><i class="fa-solid fa-code text-brand-cyan"></i> Robotics & Arduino C++</span>
                                <span class="text-brand-cyan">88%</span>
                            </div>
                            <div class="w-full bg-brand-blue h-2.5 rounded-full overflow-hidden p-0.5 border border-white/10">
                                <div class="bg-gradient-to-r from-brand-cyan to-brand-electric h-full rounded-full w-[88%]"></div>
                            </div>
                        </div>

                        <!-- Skill 2 -->
                        <div>
                            <div class="flex justify-between text-xs font-semibold mb-1">
                                <span class="text-white flex items-center gap-2"><i class="fa-solid fa-cubes text-brand-electric"></i> Web Basics (HTML/Tailwind CSS)</span>
                                <span class="text-brand-electric">80%</span>
                            </div>
                            <div class="w-full bg-brand-blue h-2.5 rounded-full overflow-hidden p-0.5 border border-white/10">
                                <div class="bg-gradient-to-r from-brand-electric to-brand-cyan h-full rounded-full w-[80%]"></div>
                            </div>
                        </div>

                        <!-- Skill 3 -->
                        <div>
                            <div class="flex justify-between text-xs font-semibold mb-1">
                                <span class="text-white flex items-center gap-2"><i class="fa-solid fa-brain text-brand-gold"></i> Problem Solving & Logic</span>
                                <span class="text-brand-gold">92%</span>
                            </div>
                            <div class="w-full bg-brand-blue h-2.5 rounded-full overflow-hidden p-0.5 border border-white/10">
                                <div class="bg-gradient-to-r from-brand-gold to-brand-orange h-full rounded-full w-[92%]"></div>
                            </div>
                        </div>

                        <!-- Skill 4 -->
                        <div>
                            <div class="flex justify-between text-xs font-semibold mb-1">
                                <span class="text-white flex items-center gap-2"><i class="fa-solid fa-comments text-brand-orange"></i> Public Speaking & Demo</span>
                                <span class="text-brand-orange">85%</span>
                            </div>
                            <div class="w-full bg-brand-blue h-2.5 rounded-full overflow-hidden p-0.5 border border-white/10">
                                <div class="bg-gradient-to-r from-brand-orange to-brand-gold h-full rounded-full w-[85%]"></div>
                            </div>
                        </div>

                        <!-- Skill 5 -->
                        <div>
                            <div class="flex justify-between text-xs font-semibold mb-1">
                                <span class="text-white flex items-center gap-2"><i class="fa-solid fa-users text-brand-cyan"></i> Team Collaboration</span>
                                <span class="text-brand-cyan">90%</span>
                            </div>
                            <div class="w-full bg-brand-blue h-2.5 rounded-full overflow-hidden p-0.5 border border-white/10">
                                <div class="bg-gradient-to-r from-brand-cyan to-brand-electric h-full rounded-full w-[90%]"></div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- STEM Radar / Focus Matrix Cards -->
                <div class="glass-card p-8 rounded-3xl border border-white/10 relative">
                    <h4 class="font-heading font-bold text-lg text-white mb-6 text-center">STEM Focus Radar</h4>
                    
                    <div class="grid grid-cols-2 gap-4">
                        <div class="p-4 rounded-xl bg-brand-navy/60 border border-brand-cyan/20 text-center hover:bg-brand-navy/80 transition-all">
                            <i class="fa-solid fa-flask text-2xl text-brand-cyan mb-2"></i>
                            <h5 class="font-bold text-sm text-white">Science</h5>
                            <p class="text-slate-400 text-xs mt-1">Physics & Circuit Kinematics</p>
                        </div>
                        <div class="p-4 rounded-xl bg-brand-navy/60 border border-brand-electric/20 text-center hover:bg-brand-navy/80 transition-all">
                            <i class="fa-solid fa-laptop-code text-2xl text-brand-electric mb-2"></i>
                            <h5 class="font-bold text-sm text-white">Technology</h5>
                            <p class="text-slate-400 text-xs mt-1">Sensors, Microcontrollers & Web</p>
                        </div>
                        <div class="p-4 rounded-xl bg-brand-navy/60 border border-brand-gold/20 text-center hover:bg-brand-navy/80 transition-all">
                            <i class="fa-solid fa-gears text-2xl text-brand-gold mb-2"></i>
                            <h5 class="font-bold text-sm text-white">Engineering</h5>
                            <p class="text-slate-400 text-xs mt-1">3D Models & Hardware Craft</p>
                        </div>
                        <div class="p-4 rounded-xl bg-brand-navy/60 border border-brand-orange/20 text-center hover:bg-brand-navy/80 transition-all">
                            <i class="fa-solid fa-calculator text-2xl text-brand-orange mb-2"></i>
                            <h5 class="font-bold text-sm text-white">Mathematics</h5>
                            <p class="text-slate-400 text-xs mt-1">Algebra & Spatial Geometry</p>
                        </div>
                    </div>

                    <div class="mt-6 p-3 rounded-xl bg-brand-cyan/10 border border-brand-cyan/30 text-center text-xs text-brand-cyan font-medium">
                        <i class="fa-solid fa-circle-check mr-1"></i> Continuously expanding STEM skills through Narayana School workshops!
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- Timeline & Journal Section -->
    <section id="timeline" class="py-16 bg-brand-blue/30 border-y border-white/5">
        <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-12">
                <h2 class="text-xs font-mono text-brand-cyan uppercase tracking-widest mb-2">Activity Journal</h2>
                <h3 class="font-heading text-3xl font-bold text-white">Club Milestones & Roadmap</h3>
                <div class="w-16 h-1 bg-brand-electric mx-auto mt-3 rounded-full"></div>
            </div>

            <div class="relative border-l-2 border-brand-electric/30 ml-4 md:ml-32 space-y-8">
                
                <!-- Event 1 -->
                <div class="relative pl-6 md:pl-8 group">
                    <div class="absolute -left-[9px] top-1.5 w-4 h-4 rounded-full bg-brand-cyan border-4 border-brand-navy"></div>
                    <div class="hidden md:block absolute -left-32 top-1 w-24 text-right font-mono text-xs text-brand-cyan font-bold">FEB 2026</div>
                    <div class="glass-card p-5 rounded-2xl border border-white/10 group-hover:border-brand-cyan transition-all">
                        <span class="md:hidden text-xs font-mono text-brand-cyan font-bold block mb-1">FEB 2026</span>
                        <h4 class="font-heading font-bold text-white text-base">Club Portfolio Presentation</h4>
                        <p class="text-slate-300 text-xs mt-1">
                            Presenting the interactive student website and projects live at the Narayana E-Techno School Club Meet in Vidisha.
                        </p>
                    </div>
                </div>

                <!-- Event 2 -->
                <div class="relative pl-6 md:pl-8 group">
                    <div class="absolute -left-[9px] top-1.5 w-4 h-4 rounded-full bg-brand-gold border-4 border-brand-navy"></div>
                    <div class="hidden md:block absolute -left-32 top-1 w-24 text-right font-mono text-xs text-brand-gold font-bold">DEC 2025</div>
                    <div class="glass-card p-5 rounded-2xl border border-white/10 group-hover:border-brand-gold transition-all">
                        <span class="md:hidden text-xs font-mono text-brand-gold font-bold block mb-1">DEC 2025</span>
                        <h4 class="font-heading font-bold text-white text-base">Annual Science Exhibition Showcase</h4>
                        <p class="text-slate-300 text-xs mt-1">
                            Demonstrated the Ultrasonic Obstacle-Avoiding Bot to school leadership, parents, and visiting faculty.
                        </p>
                    </div>
                </div>

                <!-- Event 3 -->
                <div class="relative pl-6 md:pl-8 group">
                    <div class="absolute -left-[9px] top-1.5 w-4 h-4 rounded-full bg-brand-electric border-4 border-brand-navy"></div>
                    <div class="hidden md:block absolute -left-32 top-1 w-24 text-right font-mono text-xs text-brand-electric font-bold">OCT 2025</div>
                    <div class="glass-card p-5 rounded-2xl border border-white/10 group-hover:border-brand-electric transition-all">
                        <span class="md:hidden text-xs font-mono text-brand-electric font-bold block mb-1">OCT 2025</span>
                        <h4 class="font-heading font-bold text-white text-base">Inter-School Math & Robotics Workshop</h4>
                        <p class="text-slate-300 text-xs mt-1">
                            Participated in hands-on sensor programming and logic circuit design sessions at school.
                        </p>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- STEM Quiz Interactive Section -->
    <section id="interactive" class="py-20">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-10">
                <h2 class="text-xs font-mono text-brand-cyan uppercase tracking-widest mb-2">Interactive Challenge</h2>
                <h3 class="font-heading text-3xl font-bold text-white">Quick STEM Quiz Widget</h3>
                <p class="text-slate-400 text-sm mt-2">Test your science & tech trivia alongside Darsh!</p>
            </div>

            <div class="glass-card rounded-3xl p-6 sm:p-8 border border-white/10 glow-electric relative overflow-hidden" id="quiz-container">
                <div class="flex justify-between items-center mb-6 border-b border-white/10 pb-4">
                    <span class="text-xs font-mono text-brand-cyan font-bold" id="quiz-progress">Question 1 of 3</span>
                    <span class="text-xs font-mono bg-brand-blue px-3 py-1 rounded-full text-brand-gold" id="quiz-score">Score: 0</span>
                </div>

                <!-- Question Area -->
                <div id="quiz-card">
                    <h4 class="font-heading font-bold text-lg text-white mb-6" id="quiz-question">
                        Loading question...
                    </h4>

                    <div class="space-y-3" id="quiz-options">
                        <!-- Options will be injected by JavaScript -->
                    </div>
                </div>

                <!-- Quiz Completion Message (Hidden by default) -->
                <div id="quiz-result" class="hidden text-center py-8">
                    <div class="w-16 h-16 rounded-full bg-brand-cyan/20 text-brand-cyan flex items-center justify-center text-3xl mx-auto mb-4">
                        <i class="fa-solid fa-trophy"></i>
                    </div>
                    <h4 class="font-heading font-bold text-2xl text-white mb-2">Quiz Completed!</h4>
                    <p class="text-slate-300 text-sm mb-6" id="quiz-final-text">Great effort!</p>
                    <button onclick="resetQuiz()" class="px-6 py-2.5 rounded-xl bg-brand-cyan text-brand-navy font-bold text-xs hover:shadow-lg transition-all">
                        Try Again
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- Guestbook / Encouragement Box Section -->
    <section id="guestbook" class="py-16 bg-brand-blue/40 border-t border-white/5">
        <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-10">
                <h2 class="text-xs font-mono text-brand-cyan uppercase tracking-widest mb-2">Club Interactions</h2>
                <h3 class="font-heading text-3xl font-bold text-white">Student & Teacher Guestbook</h3>
                <p class="text-slate-400 text-sm mt-2">Leave an encouraging message or club note for Darsh Sharma!</p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-5 gap-8">
                <!-- Form Column -->
                <div class="lg:col-span-2 glass-card p-6 rounded-2xl border border-white/10">
                    <h4 class="font-heading font-bold text-white text-base mb-4">Leave a Note</h4>
                    <form id="guestbook-form" class="space-y-4">
                        <div>
                            <label class="block text-xs font-semibold text-slate-300 mb-1">Your Name / Designation</label>
                            <input type="text" id="guest-name" required placeholder="e.g. Teacher, Club Member" class="w-full bg-brand-navy border border-white/10 rounded-xl px-3.5 py-2.5 text-xs text-white placeholder-slate-500 focus:outline-none focus:border-brand-cyan transition-colors">
                        </div>
                        <div>
                            <label class="block text-xs font-semibold text-slate-300 mb-1">Encouraging Message</label>
                            <textarea id="guest-message" required rows="3" placeholder="Great STEM work Darsh! Keep innovating..." class="w-full bg-brand-navy border border-white/10 rounded-xl px-3.5 py-2.5 text-xs text-white placeholder-slate-500 focus:outline-none focus:border-brand-cyan transition-colors resize-none"></textarea>
                        </div>
                        <button type="submit" class="w-full py-2.5 rounded-xl bg-gradient-to-r from-brand-cyan to-brand-electric text-brand-navy font-bold text-xs hover:shadow-lg hover:shadow-brand-cyan/20 transition-all">
                            Post Message
                        </button>
                    </form>
                </div>

                <!-- Messages Display Column -->
                <div class="lg:col-span-3 space-y-4 max-h-[380px] overflow-y-auto pr-2" id="guestbook-list">
                    <!-- Pre-populated Messages -->
                    <div class="glass-card p-4 rounded-xl border border-white/10">
                        <div class="flex justify-between items-center mb-1">
                            <span class="font-bold text-xs text-brand-cyan">Science Club Mentor</span>
                            <span class="text-[10px] text-slate-500 font-mono">Today</span>
                        </div>
                        <p class="text-slate-300 text-xs">
                            "Impressive dedication to your robotics model, Darsh! The obstacle avoidance logic shows great computational thinking for Class 9."
                        </p>
                    </div>

                    <div class="glass-card p-4 rounded-xl border border-white/10">
                        <div class="flex justify-between items-center mb-1">
                            <span class="font-bold text-xs text-brand-gold">Aarav (Classmate)</span>
                            <span class="text-[10px] text-slate-500 font-mono">Yesterday</span>
                        </div>
                        <p class="text-slate-300 text-xs">
                            "Awesome portfolio presentation for our Vidisha club meet! Love the smart irrigation prototype setup."
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-brand-navy border-t border-white/10 py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col md:flex-row items-center justify-between gap-6 text-center md:text-left">
                <div>
                    <div class="font-heading font-extrabold text-xl text-white">DARSH SHARMA</div>
                    <p class="text-xs text-brand-cyan font-medium mt-1">
                        Class 9 Student • Narayana E-Techno School, Vidisha (M.P.)
                    </p>
                </div>

                <div class="text-slate-400 text-xs max-w-md">
                    <p>Designed for School Science & Technology Club Presentations.</p>
                    <p class="text-slate-500 mt-1">© 2026 Darsh Sharma. Narayana E-Techno Student Showcase.</p>
                </div>

                <!-- Social/Contact Placeholder Badges -->
                <div class="flex gap-3 text-slate-300">
                    <a href="#about" class="w-9 h-9 rounded-lg bg-brand-blue border border-white/10 flex items-center justify-center hover:text-brand-cyan hover:border-brand-cyan transition-all">
                        <i class="fa-solid fa-graduation-cap"></i>
                    </a>
                    <a href="#projects" class="w-9 h-9 rounded-lg bg-brand-blue border border-white/10 flex items-center justify-center hover:text-brand-cyan hover:border-brand-cyan transition-all">
                        <i class="fa-solid fa-code"></i>
                    </a>
                    <a href="#guestbook" class="w-9 h-9 rounded-lg bg-brand-blue border border-white/10 flex items-center justify-center hover:text-brand-cyan hover:border-brand-cyan transition-all">
                        <i class="fa-solid fa-envelope"></i>
                    </a>
                </div>
            </div>
        </div>
    </footer>

    <!-- JavaScript Logic -->
    <script>
        // Mobile Navigation Toggle
        const mobileBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        const mobileLinks = document.querySelectorAll('.mobile-nav-link');

        mobileBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        mobileLinks.forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });

        // Project Filtering Logic
        const filterBtns = document.querySelectorAll('.filter-btn');
        const projectCards = document.querySelectorAll('.project-card');

        filterBtns.forEach(btn => {
            btn.addEventListener('click', () => {
                filterBtns.forEach(b => {
                    b.classList.remove('active', 'bg-brand-cyan', 'text-brand-navy');
                    b.classList.add('bg-brand-blue', 'text-slate-300');
                });
                btn.classList.add('active', 'bg-brand-cyan', 'text-brand-navy');
                btn.classList.remove('bg-brand-blue', 'text-slate-300');

                const filter = btn.getAttribute('data-filter');

                projectCards.forEach(card => {
                    if (filter === 'all' || card.getAttribute('data-category') === filter) {
                        card.style.display = 'flex';
                    } else {
                        card.style.display = 'none';
                    }
                });
            });
        });

        // STEM Quiz Interactive Data & Logic
        const quizData = [
            {
                question: "Which component is primarily used in robotics to measure distances using sound waves?",
                options: ["Infrared Sensor", "Ultrasonic Sensor", "Gyroscope Sensor", "LDR Sensor"],
                correct: 1
            },
            {
                question: "What is the primary power source utilized in Darsh's Eco-Tech Irrigation prototype?",
                options: ["Wind Power", "Hydro Energy", "Solar Energy", "Geothermal Energy"],
                correct: 2
            },
            {
                question: "In computer programming, which language is standard for programming Arduino hardware models?",
                options: ["C / C++", "Python", "HTML", "SQL"],
                correct: 0
            }
        ];

        let currentQuizIndex = 0;
        let score = 0;

        function loadQuizQuestion() {
            const current = quizData[currentQuizIndex];
            document.getElementById('quiz-progress').innerText = `Question ${currentQuizIndex + 1} of ${quizData.length}`;
            document.getElementById('quiz-score').innerText = `Score: ${score}`;
            document.getElementById('quiz-question').innerText = current.question;

            const optionsContainer = document.getElementById('quiz-options');
            optionsContainer.innerHTML = '';

            current.options.forEach((opt, index) => {
                const button = document.createElement('button');
                button.className = "w-full text-left p-3.5 rounded-xl bg-brand-navy/80 border border-white/10 hover:border-brand-cyan/60 hover:bg-brand-blue transition-all text-xs font-medium text-slate-200 flex items-center justify-between";
                button.innerHTML = `<span>${opt}</span> <i class="fa-regular fa-circle text-slate-500"></i>`;
                button.onclick = () => checkQuizAnswer(index);
                optionsContainer.appendChild(button);
            });
        }

        function checkQuizAnswer(selectedIndex) {
            const current = quizData[currentQuizIndex];
            if (selectedIndex === current.correct) {
                score += 10;
                // Trigger celebratory confetti effect
                confetti({
                    particleCount: 40,
                    spread: 60,
                    origin: { y: 0.8 }
                });
            }

            currentQuizIndex++;
            if (currentQuizIndex < quizData.length) {
                loadQuizQuestion();
            } else {
                showQuizResults();
            }
        }

        function showQuizResults() {
            document.getElementById('quiz-card').classList.add('hidden');
            document.getElementById('quiz-result').classList.remove('hidden');
            document.getElementById('quiz-score').innerText = `Score: ${score}`;
            document.getElementById('quiz-final-text').innerText = `You scored ${score} out of ${quizData.length * 10} points! Excellent STEM knowledge!`;
        }

        function resetQuiz() {
            currentQuizIndex = 0;
            score = 0;
            document.getElementById('quiz-card').classList.remove('hidden');
            document.getElementById('quiz-result').classList.add('hidden');
            loadQuizQuestion();
        }

        // Initialize Quiz
        loadQuizQuestion();

        // Guestbook Form Submission Handler
        const guestbookForm = document.getElementById('guestbook-form');
        const guestbookList = document.getElementById('guestbook-list');

        guestbookForm.addEventListener('submit', (e) => {
            e.preventDefault();
            const name = document.getElementById('guest-name').value.trim();
            const message = document.getElementById('guest-message').value.trim();

            if (name && message) {
                const newCard = document.createElement('div');
                newCard.className = 'glass-card p-4 rounded-xl border border-brand-cyan/40 bg-brand-cyan/5 transition-all animate-fade-in';
                newCard.innerHTML = `
                    <div class="flex justify-between items-center mb-1">
                        <span class="font-bold text-xs text-brand-cyan">${escapeHtml(name)}</span>
                        <span class="text-[10px] text-slate-400 font-mono">Just Now</span>
                    </div>
                    <p class="text-slate-200 text-xs">
                        "${escapeHtml(message)}"
                    </p>
                `;

                guestbookList.prepend(newCard);
                guestbookForm.reset();

                // Trigger confetti for leaving a message
                confetti({
                    particleCount: 30,
                    spread: 50,
                    origin: { y: 0.8 }
                });
            }
        });

        // Helper function to escape HTML string inputs
        function escapeHtml(str) {
            return str.replace(/[&<>"']/g, function(m) {
                return {
                    '&': '&amp;',
                    '<': '&lt;',
                    '>': '&gt;',
                    '"': '&quot;',
                    "'": '&#039;'
                }[m];
            });
        }
    </script>
</body>
</html>
