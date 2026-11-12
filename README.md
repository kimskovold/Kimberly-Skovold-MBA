# Kimberly-Skovold-MBA
<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kimberly Skovold | Enterprise Customer Success & Technical Support Leader</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Plus+Jakarta+Sans:wght@600;700;800&display=swap" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        display: ['Plus Jakarta Sans', 'sans-serif'],
                    },
                    colors: {
                        navy: {
                            950: '#080D1A',
                            900: '#0F172A',
                            800: '#1E293B',
                            700: '#334155',
                        },
                        brand: {
                            teal: '#0D9488',
                            tealLight: '#CCFBF1',
                            blue: '#2563EB',
                            blueLight: '#DBEAFE',
                        }
                    }
                }
            }
        }
    </script>
    <style>
        body {
            background-color: #F8FAFC;
            color: #0F172A;
            -webkit-font-smoothing: antialiased;
        }
        .glass-nav {
            background: rgba(255, 255, 255, 0.92);
            backdrop-filter: blur(12px);
            border-bottom: 1px solid rgba(226, 232, 240, 0.8);
        }
        .card-elevated {
            background: #FFFFFF;
            border: 1px solid #E2E8F0;
            box-shadow: 0 4px 20px -2px rgba(15, 23, 42, 0.04), 0 1px 3px -1px rgba(15, 23, 42, 0.03);
            transition: transform 0.25s cubic-bezier(0.16, 1, 0.3, 1), box-shadow 0.25s cubic-bezier(0.16, 1, 0.3, 1), border-color 0.25s ease;
        }
        .card-elevated:hover {
            transform: translateY(-2px);
            box-shadow: 0 12px 28px -4px rgba(15, 23, 42, 0.08), 0 4px 10px -2px rgba(15, 23, 42, 0.04);
            border-color: #CBD5E1;
        }
        .fade-in-up {
            animation: fadeInUp 0.4s cubic-bezier(0.16, 1, 0.3, 1) forwards;
        }
        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .progress-bar-fill {
            transition: width 0.8s cubic-bezier(0.16, 1, 0.3, 1);
        }
        @media print {
            .no-print { display: none !important; }
            body { background: #FFFFFF !important; }
            .card-elevated { box-shadow: none !important; border: 1px solid #CBD5E1 !important; break-inside: avoid; }
            header, section { padding-top: 1.5rem !important; padding-bottom: 1.5rem !important; }
        }
    </style>
</head>
<body class="selection:bg-brand-blue/15 selection:text-brand-blue">

    <!-- Toast Notification for Copy-to-Clipboard -->
    <div id="toast" class="fixed bottom-6 right-6 z-50 transform translate-y-20 opacity-0 transition-all duration-300 pointer-events-none no-print">
        <div class="bg-navy-900 text-white px-5 py-3.5 rounded-xl shadow-xl border border-slate-700 flex items-center gap-3">
            <span class="w-6 h-6 rounded-full bg-brand-teal/20 text-brand-teal flex items-center justify-center">
                <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7"/></svg>
            </span>
            <span id="toast-message" class="text-sm font-medium">Copied to clipboard</span>
        </div>
    </div>

    <!-- Top Navigation Bar -->
    <nav class="glass-nav sticky top-0 z-40 no-print">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <div class="flex items-center gap-3">
                    <div class="w-9 h-9 rounded-xl bg-navy-900 text-white font-display font-bold flex items-center justify-center text-sm tracking-tight shadow-sm">
                        KS
                    </div>
                    <div>
                        <span class="font-display font-bold text-navy-900 text-base tracking-tight block leading-none">Kimberly Skovold</span>
                        <span class="text-xs text-slate-500 font-medium">MBA, Summa Cum Laude</span>
                    </div>
                </div>

                <!-- Desktop Nav Links -->
                <div class="hidden md:flex items-center gap-7 text-sm font-medium text-slate-600">
                    <a href="#role-lens" class="hover:text-navy-900 transition-colors">Role Alignment</a>
                    <a href="#impact-showcase" class="hover:text-navy-900 transition-colors">ROI &amp; Metrics</a>
                    <a href="#experience" class="hover:text-navy-900 transition-colors">Experience</a>
                    <a href="#playbook" class="hover:text-navy-900 transition-colors">90/180/365 Playbook</a>
                </div>

                <!-- Action Buttons -->
                <div class="flex items-center gap-2.5">
                    <button onclick="window.print()" class="hidden sm:inline-flex items-center gap-2 px-3.5 py-2 rounded-xl text-xs font-semibold text-slate-700 bg-slate-100 hover:bg-slate-200 transition-colors" title="Print or Save as PDF">
                        <svg class="w-4 h-4 text-slate-600" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M17 17h2a2 2 0 002-2v-4a2 2 0 00-2-2H5a2 2 0 00-2 2v4a2 2 0 002 2h2m2 4h6a2 2 0 002-2v-4a2 2 0 00-2-2H9a2 2 0 00-2 2v4a2 2 0 002 2zm8-12V5a2 2 0 00-2-2H9a2 2 0 00-2 2v4h10z"/></svg>
                        <span>Print Brief</span>
                    </button>
                    <a href="#recruiter-hub" class="inline-flex items-center gap-2 px-4 py-2 rounded-xl text-xs sm:text-sm font-semibold text-white bg-navy-900 hover:bg-navy-800 shadow-sm transition-all">
                        <span>Hire / Connect</span>
                        <svg class="w-4 h-4 text-brand-teal" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M14 5l7 7m0 0l-7 7m7-7H3"/></svg>
                    </a>
                </div>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <header class="relative overflow-hidden bg-navy-900 text-white pt-12 pb-24 sm:pt-16 sm:pb-28">
        <!-- Subtle Background Accent Grid -->
        <div class="absolute inset-0 opacity-10 pointer-events-none" style="background-image: radial-gradient(#94A3B8 1px, transparent 1px); background-size: 24px 24px;"></div>
        <div class="absolute -top-24 -right-24 w-96 h-96 bg-brand-blue/20 rounded-full blur-3xl pointer-events-none"></div>
        <div class="absolute -bottom-24 -left-24 w-96 h-96 bg-brand-teal/20 rounded-full blur-3xl pointer-events-none"></div>

        <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="max-w-4xl">
                <div class="inline-flex flex-wrap items-center gap-2 px-3.5 py-1.5 rounded-full bg-white/10 border border-white/15 text-xs font-medium text-teal-300 mb-6">
                    <span class="w-2 h-2 rounded-full bg-brand-teal animate-pulse"></span>
                    <span>Available for Senior/Enterprise CSM, Director of CS &amp; Client Operations Roles</span>
                </div>

                <h1 class="font-display text-3xl sm:text-5xl lg:text-[3.35rem] font-extrabold tracking-tight leading-[1.12] mb-5">
                    Turning Complex Enterprise SaaS Into Predictable <span class="text-transparent bg-clip-text bg-gradient-to-r from-teal-300 via-emerald-300 to-blue-300">Retention &amp; Revenue Growth.</span>
                </h1>

                <p class="text-base sm:text-lg text-slate-300 leading-relaxed max-w-3xl mb-8">
                    I’m <strong class="text-white font-semibold">Kimberly Skovold</strong>—a Customer Success &amp; Technical Support Leader with 10+ years of experience scaling North American service teams, managing 70+ enterprise SaaS portfolios, and engineering AI-driven operational workflows that accelerate time-to-value and protect ARR.
                </p>

                <!-- Quick Contact & Metadata Bar -->
                <div class="flex flex-wrap items-center gap-y-3 gap-x-6 text-sm text-slate-300 mb-8">
                    <div class="flex items-center gap-2">
                        <svg class="w-4 h-4 text-teal-400" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"/><path stroke-linecap="round" stroke-linejoin="round" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"/></svg>
                        <span>Chino, CA (Open to Remote &amp; Hybrid)</span>
                    </div>
                    <div class="flex items-center gap-2">
                        <svg class="w-4 h-4 text-blue-400" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M12 14l9-5-9-5-9 5 9 5z"/><path stroke-linecap="round" stroke-linejoin="round" d="M12 14l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-2.998 12.078 12.078 0 01.665-6.479L12 14z"/></svg>
                        <span>MBA, Summa Cum Laude — Grand Canyon University</span>
                    </div>
                </div>

                <!-- Primary CTAs -->
                <div class="flex flex-wrap items-center gap-3 no-print">
                    <button onclick="copyText('kimberlyveronica@me.com', 'Email address copied: kimberlyveronica@me.com')" class="inline-flex items-center gap-2.5 px-5 py-3 rounded-xl bg-brand-teal hover:bg-teal-500 text-white font-semibold text-sm shadow-lg shadow-teal-950/30 transition-all cursor-pointer">
                        <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"/></svg>
                        <span>Copy Email: kimberlyveronica@me.com</span>
                    </button>
                    <button onclick="copyText('+1 714 492 4359', 'Phone number copied: +1 714 492 4359')" class="inline-flex items-center gap-2.5 px-5 py-3 rounded-xl bg-white/10 hover:bg-white/15 text-white border border-white/15 font-semibold text-sm transition-all cursor-pointer">
                        <svg class="w-4 h-4 text-slate-300" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"/></svg>
                        <span>+1 714 492 4359</span>
                    </button>
                    <a href="#role-lens" class="inline-flex items-center gap-2 px-5 py-3 rounded-xl bg-brand-blue hover:bg-blue-500 text-white font-semibold text-sm transition-all">
                        <span>Tailor Portfolio to Your Role</span>
                        <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7"/></svg>
                    </a>
                </div>
            </div>
        </div>
    </header>

    <!-- Executive KPI Banner (Overlapping Hero) -->
    <section class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 -mt-12 sm:-mt-14 relative z-10">
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4 sm:gap-5">
            <!-- KPI 1 -->
            <div class="card-elevated rounded-2xl p-6 border-t-4 border-t-brand-blue">
                <div class="flex items-center justify-between mb-2">
                    <span class="text-xs font-bold uppercase tracking-wider text-slate-500">Enterprise Portfolio</span>
                    <span class="w-8 h-8 rounded-lg bg-blue-50 text-brand-blue flex items-center justify-center">
                        <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M19 21V5a2 2 0 00-2-2H7a2 2 0 00-2 2v16m14 0h2m-2 0h-5m-9 0H3m2 0h5M9 7h1m-1 4h1m4-4h1m-1 4h1m-5 10v-5a1 1 0 011-1h2a1 1 0 011 1v5m-4 0h4"/></svg>
                    </span>
                </div>
                <div class="font-display text-3xl sm:text-4xl font-extrabold text-navy-900 tracking-tight">70+</div>
                <p class="text-sm font-medium text-slate-700 mt-1">Enterprise Accounts Managed</p>
                <p class="text-xs text-slate-500 mt-1">C-suite advisory, ARR retention &amp; expansion</p>
            </div>

            <!-- KPI 2 -->
            <div class="card-elevated rounded-2xl p-6 border-t-4 border-t-brand-teal">
                <div class="flex items-center justify-between mb-2">
                    <span class="text-xs font-bold uppercase tracking-wider text-slate-500">Client Satisfaction</span>
                    <span class="w-8 h-8 rounded-lg bg-teal-50 text-brand-teal flex items-center justify-center">
                        <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
                    </span>
                </div>
                <div class="font-display text-3xl sm:text-4xl font-extrabold text-navy-900 tracking-tight">98%+</div>
                <p class="text-sm font-medium text-slate-700 mt-1">Client CSAT Rating</p>
                <p class="text-xs text-slate-500 mt-1">Sustained across SaaS &amp; luxury service ops</p>
            </div>

            <!-- KPI 3 -->
            <div class="card-elevated rounded-2xl p-6 border-t-4 border-t-indigo-600">
                <div class="flex items-center justify-between mb-2">
                    <span class="text-xs font-bold uppercase tracking-wider text-slate-500">Team Scaling</span>
                    <span class="w-8 h-8 rounded-lg bg-indigo-50 text-indigo-600 flex items-center justify-center">
                        <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M13 7h8m0 0v8m0-8l-8 8-4-4-6 6"/></svg>
                    </span>
                </div>
                <div class="font-display text-3xl sm:text-4xl font-extrabold text-navy-900 tracking-tight">200%</div>
                <p class="text-sm font-medium text-slate-700 mt-1">Support Division Growth</p>
                <p class="text-xs text-slate-500 mt-1">Scaled North American team from 3 to 9</p>
            </div>

            <!-- KPI 4 -->
            <div class="card-elevated rounded-2xl p-6 border-t-4 border-t-emerald-600">
                <div class="flex items-center justify-between mb-2">
                    <span class="text-xs font-bold uppercase tracking-wider text-slate-500">AI Enablement</span>
                    <span class="w-8 h-8 rounded-lg bg-emerald-50 text-emerald-600 flex items-center justify-center">
                        <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M13 10V3L4 14h7v7l9-11h-7z"/></svg>
                    </span>
                </div>
                <div class="font-display text-3xl sm:text-4xl font-extrabold text-navy-900 tracking-tight">60%</div>
                <p class="text-sm font-medium text-slate-700 mt-1">Prep Time Reduction</p>
                <p class="text-xs text-slate-500 mt-1">Via structured Gemini &amp; ChatGPT workflows</p>
            </div>
        </div>
    </section>

    <!-- Interactive Feature 1: Role-Fit Lens Switcher -->
    <section id="role-lens" class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 pt-16 sm:pt-24">
        <div class="flex flex-col lg:flex-row lg:items-end justify-between gap-6 mb-8">
            <div>
                <span class="inline-block text-xs font-bold uppercase tracking-widest text-brand-teal mb-2">Interactive Recruiter Filter</span>
                <h2 class="font-display text-2xl sm:text-3xl font-bold text-navy-900 tracking-tight">Select the Role You’re Hiring For</h2>
                <p class="text-slate-600 text-sm sm:text-base mt-2 max-w-2xl">
                    Toggle between leadership lenses below to dynamically align Kimberly’s core value proposition, proven outcomes, and technical stack to your open requisition.
                </p>
            </div>

            <!-- Lens Switcher Buttons -->
            <div class="inline-flex flex-wrap p-1.5 rounded-2xl bg-slate-200/80 border border-slate-300/60 gap-1 no-print" role="tablist" aria-label="Role Focus Filter">
                <button onclick="switchLens('cs')" id="lens-btn-cs" class="lens-tab px-4 py-2.5 rounded-xl text-xs sm:text-sm font-semibold transition-all cursor-pointer bg-navy-900 text-white shadow-sm">
                    Enterprise Customer Success
                </button>
                <button onclick="switchLens('support')" id="lens-btn-support" class="lens-tab px-4 py-2.5 rounded-xl text-xs sm:text-sm font-semibold transition-all cursor-pointer text-slate-700 hover:text-navy-900">
                    Technical Support &amp; Escalations
                </button>
                <button onclick="switchLens('ops')" id="lens-btn-ops" class="lens-tab px-4 py-2.5 rounded-xl text-xs sm:text-sm font-semibold transition-all cursor-pointer text-slate-700 hover:text-navy-900">
                    AI &amp; Revenue Operations
                </button>
            </div>
        </div>

        <!-- Dynamic Lens Content Card -->
        <div id="lens-container" class="card-elevated rounded-3xl p-6 sm:p-10 bg-white">
            <!-- Populated dynamically via JS -->
        </div>
    </section>

    <!-- Interactive Feature 3: ROI & Retention Impact Showcase -->
    <section id="impact-showcase" class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 pt-16 sm:pt-24">
        <div class="mb-10">
            <span class="inline-block text-xs font-bold uppercase tracking-widest text-brand-blue mb-2">Measurable Business Outcomes</span>
            <h2 class="font-display text-2xl sm:text-3xl font-bold text-navy-900 tracking-tight">How Operational Rigor Drives Net Revenue Retention</h2>
            <p class="text-slate-600 text-sm sm:text-base mt-2 max-w-2xl">
                Connecting frontline customer enablement, SLA automation, and executive KPI consulting directly to ARR protection and account expansion.
            </p>
        </div>

        <div class="grid grid-cols-1 lg:grid-cols-3 gap-6">
            <!-- Impact Card 1: Time-to-Value & Early Churn Prevention -->
            <div class="card-elevated rounded-2xl p-6 sm:p-7 flex flex-col justify-between">
                <div>
                    <div class="flex items-center justify-between mb-4">
                        <span class="px-3 py-1 rounded-full text-xs font-semibold bg-teal-50 text-brand-teal">Onboarding &amp; Adoption</span>
                        <span class="text-xs font-bold text-slate-400">01</span>
                    </div>
                    <h3 class="font-display text-xl font-bold text-navy-900 mb-2">Accelerated Time-to-Value</h3>
                    <p class="text-sm text-slate-600 leading-relaxed mb-6">
                        Spearheaded structured onboarding and enablement frameworks for 70+ enterprise accounts at Dynatron Software, eliminating early-stage friction and establishing clear KPI baselines within the first 90 days.
                    </p>
                </div>

                <div class="bg-slate-50 rounded-xl p-4 border border-slate-200/80">
                    <div class="flex justify-between text-xs font-semibold text-slate-700 mb-1.5">
                        <span>Early-Stage Retention Health</span>
                        <span class="text-brand-teal">98% CSAT Benchmark</span>
                    </div>
                    <div class="w-full bg-slate-200 rounded-full h-2.5 overflow-hidden">
                        <div class="bg-brand-teal h-2.5 rounded-full progress-bar-fill" style="width: 98%"></div>
                    </div>
                    <p class="text-xs text-slate-500 mt-2.5">Result: Measurable drop in early churn &amp; faster analytics adoption.</p>
                </div>
            </div>

            <!-- Impact Card 2: High-Velocity Scale & SLA Stability -->
            <div class="card-elevated rounded-2xl p-6 sm:p-7 flex flex-col justify-between">
                <div>
                    <div class="flex items-center justify-between mb-4">
                        <span class="px-3 py-1 rounded-full text-xs font-semibold bg-blue-50 text-brand-blue">Escalation Architecture</span>
                        <span class="text-xs font-bold text-slate-400">02</span>
                    </div>
                    <h3 class="font-display text-xl font-bold text-navy-900 mb-2">3x Volume Resilience Without SLA Slip</h3>
                    <p class="text-sm text-slate-600 leading-relaxed mb-6">
                        Engineered automated escalation routing and real-time Power BI / Zendesk telemetry at myKaarma, preserving strict SLA compliance and cross-functional Engineering alignment during a 300% surge in ticket volume.
                    </p>
                </div>

                <div class="bg-slate-50 rounded-xl p-4 border border-slate-200/80">
                    <div class="flex justify-between text-xs font-semibold text-slate-700 mb-1.5">
                        <span>North American Team Capacity</span>
                        <span class="text-brand-blue">+200% Scaled (3 → 9)</span>
                    </div>
                    <div class="w-full bg-slate-200 rounded-full h-2.5 overflow-hidden">
                        <div class="bg-brand-blue h-2.5 rounded-full progress-bar-fill" style="width: 92%"></div>
                    </div>
                    <p class="text-xs text-slate-500 mt-2.5">Result: Lower team turnover alongside annual CSAT &amp; NPS gains.</p>
                </div>
            </div>

            <!-- Impact Card 3: AI Workflow Automation -->
            <div class="card-elevated rounded-2xl p-6 sm:p-7 flex flex-col justify-between">
                <div>
                    <div class="flex items-center justify-between mb-4">
                        <span class="px-3 py-1 rounded-full text-xs font-semibold bg-indigo-50 text-indigo-600">AI-Enabled CS Ops</span>
                        <span class="text-xs font-bold text-slate-400">03</span>
                    </div>
                    <h3 class="font-display text-xl font-bold text-navy-900 mb-2">60% Faster Executive QBR Prep</h3>
                    <p class="text-sm text-slate-600 leading-relaxed mb-6">
                        Designed repeatable prompt architectures in Gemini and ChatGPT to synthesize client performance metrics and surface expansion opportunities—reclaiming hours of strategic bandwidth per enterprise account.
                    </p>
                </div>

                <div class="bg-slate-50 rounded-xl p-4 border border-slate-200/80">
                    <div class="flex justify-between text-xs font-semibold text-slate-700 mb-1.5">
                        <span>Manual Prep Time Eliminated</span>
                        <span class="text-indigo-600">60% Efficiency Gain</span>
                    </div>
                    <div class="w-full bg-slate-200 rounded-full h-2.5 overflow-hidden">
                        <div class="bg-indigo-600 h-2.5 rounded-full progress-bar-fill" style="width: 60%"></div>
                    </div>
                    <p class="text-xs text-slate-500 mt-2.5">Result: Deeper C-suite profitability consulting &amp; higher expansion velocity.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Experience Timeline & Interactive Case Studies -->
    <section id="experience" class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 pt-16 sm:pt-24">
        <div class="mb-10">
            <span class="inline-block text-xs font-bold uppercase tracking-widest text-brand-teal mb-2">Career Track Record</span>
            <h2 class="font-display text-2xl sm:text-3xl font-bold text-navy-900 tracking-tight">Executive Experience &amp; Case Studies</h2>
            <p class="text-slate-600 text-sm sm:text-base mt-2 max-w-2xl">
                Over a decade of progressive leadership bridging enterprise customer success, SaaS technical support architecture, and high-volume service operations.
            </p>
        </div>

        <div class="space-y-6">
            <!-- Role 1: Dynatron Software -->
            <article class="card-elevated rounded-2xl p-6 sm:p-8 border-l-4 border-l-brand-teal">
                <div class="flex flex-col md:flex-row md:items-center justify-between gap-2 pb-5 border-b border-slate-100">
                    <div>
                        <div class="flex flex-wrap items-center gap-2.5">
                            <h3 class="font-display text-xl font-bold text-navy-900">Customer Success Manager / Client Performance Coach</h3>
                            <span class="px-2.5 py-0.5 rounded-full text-xs font-semibold bg-teal-50 text-brand-teal border border-teal-200/60">Current Role</span>
                        </div>
                        <p class="text-base font-semibold text-brand-blue mt-1">Dynatron Software <span class="text-slate-400 font-normal">• Dallas, TX / Remote</span></p>
                    </div>
                    <div class="text-sm font-semibold text-slate-600 bg-slate-100 px-3.5 py-1.5 rounded-xl self-start md:self-center">
                        July 2024 – Present
                    </div>
                </div>

                <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 pt-5">
                    <div class="lg:col-span-8 space-y-3">
                        <ul class="space-y-2.5 text-sm sm:text-[15px] text-slate-700 leading-relaxed">
                            <li class="flex items-start gap-3">
                                <span class="w-1.5 h-1.5 rounded-full bg-brand-teal mt-2 shrink-0"></span>
                                <span>Manage a strategic portfolio of <strong>70+ high-value enterprise accounts</strong>, acting as a trusted advisor to drive SaaS analytics adoption, ARR retention, and continuous account expansion.</span>
                            </li>
                            <li class="flex items-start gap-3">
                                <span class="w-1.5 h-1.5 rounded-full bg-brand-teal mt-2 shrink-0"></span>
                                <span>Deliver <strong>data-driven executive consultations</strong> analyzing critical operational KPIs and constructing customized growth frameworks that enhance client profitability and operational efficiency.</span>
                            </li>
                            <li class="flex items-start gap-3">
                                <span class="w-1.5 h-1.5 rounded-full bg-brand-teal mt-2 shrink-0"></span>
                                <span>Designed structured <strong>AI prompt workflows using Gemini and ChatGPT</strong> to automate client performance synthesis and meeting preparation, cutting consultation prep time by <strong>60%</strong>.</span>
                            </li>
                            <li class="flex items-start gap-3">
                                <span class="w-1.5 h-1.5 rounded-full bg-brand-teal mt-2 shrink-0"></span>
                                <span>Spearheaded proactive onboarding and customer enablement programs that measurably reduced early-stage account churn while accelerating client time-to-value.</span>
                            </li>
                        </ul>
                    </div>

                    <div class="lg:col-span-4 bg-slate-50 rounded-xl p-5 border border-slate-200/70 flex flex-col justify-between">
                        <div>
                            <span class="text-xs font-bold uppercase tracking-wider text-slate-500 block mb-3">Case Study Highlight</span>
                            <p class="text-sm font-semibold text-navy-900 mb-1.5">AI-Powered Executive Consultation Engine</p>
                            <p class="text-xs text-slate-600 leading-relaxed">
                                Standardized complex financial &amp; operational telemetry analysis using LLM workflows, enabling deeper C-suite strategic coaching across 70+ accounts without adding headcount.
                            </p>
                        </div>
                        <div class="flex flex-wrap gap-1.5 mt-4 pt-3 border-t border-slate-200/80">
                            <span class="px-2.5 py-1 rounded-md bg-white border border-slate-200 text-xs font-medium text-slate-700">Enterprise CS</span>
                            <span class="px-2.5 py-1 rounded-md bg-white border border-slate-200 text-xs font-medium text-slate-700">Gemini &amp; ChatGPT</span>
                            <span class="px-2.5 py-1 rounded-md bg-white border border-slate-200 text-xs font-medium text-slate-700">ARR Expansion</span>
                        </div>
                    </div>
                </div>
            </article>

            <!-- Role 2: myKaarma -->
            <article class="card-elevated rounded-2xl p-6 sm:p-8 border-l-4 border-l-brand-blue">
                <div class="flex flex-col md:flex-row md:items-center justify-between gap-2 pb-5 border-b border-slate-100">
                    <div>
                        <h3 class="font-display text-xl font-bold text-navy-900">Director of Technical Support</h3>
                        <p class="text-base font-semibold text-brand-blue mt-1">myKaarma <span class="text-slate-400 font-normal">• Long Beach, CA</span></p>
                    </div>
                    <div class="text-sm font-semibold text-slate-600 bg-slate-100 px-3.5 py-1.5 rounded-xl self-start md:self-center">
                        February 2016 – June 2024
                    </div>
                </div>

                <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 pt-5">
                    <div class="lg:col-span-8 space-y-3">
                        <ul class="space-y-2.5 text-sm sm:text-[15px] text-slate-700 leading-relaxed">
                            <li class="flex items-start gap-3">
                                <span class="w-1.5 h-1.5 rounded-full bg-brand-blue mt-2 shrink-0"></span>
                                <span>Built and scaled a high-performing <strong>North American technical support division by 200%</strong> (from 3 to 9 members across the US and Canada) to support rapid SaaS expansion and high-volume client accounts.</span>
                            </li>
                            <li class="flex items-start gap-3">
                                <span class="w-1.5 h-1.5 rounded-full bg-brand-blue mt-2 shrink-0"></span>
                                <span>Engineered automated support workflows, escalation protocols, and <strong>Power BI and Zendesk dashboards</strong> that elevated response efficiency and SLA compliance during a <strong>3x increase in ticket volume</strong>.</span>
                            </li>
                            <li class="flex items-start gap-3">
                                <span class="w-1.5 h-1.5 rounded-full bg-brand-blue mt-2 shrink-0"></span>
                                <span>Orchestrated cross-functional collaboration with <strong>Engineering, Sales, and Product</strong> to streamline complex technical escalation management, improving platform stability and eliminating customer friction.</span>
                            </li>
                            <li class="flex items-start gap-3">
                                <span class="w-1.5 h-1.5 rounded-full bg-brand-blue mt-2 shrink-0"></span>
                                <span>Mentored support team members in advanced technical troubleshooting and customer communication, reducing departmental turnover while consistently driving annual CSAT and NPS increases.</span>
                            </li>
                        </ul>
                    </div>

                    <div class="lg:col-span-4 bg-slate-50 rounded-xl p-5 border border-slate-200/70 flex flex-col justify-between">
                        <div>
                            <span class="text-xs font-bold uppercase tracking-wider text-slate-500 block mb-3">Case Study Highlight</span>
                            <p class="text-sm font-semibold text-navy-900 mb-1.5">Automated Escalation &amp; Telemetry Architecture</p>
                            <p class="text-xs text-slate-600 leading-relaxed">
                                Replaced ad-hoc issue triage with automated Zendesk routing, Jira engineering handoffs, and executive Power BI SLA reporting—turning support into a proactive retention engine.
                            </p>
                        </div>
                        <div class="flex flex-wrap gap-1.5 mt-4 pt-3 border-t border-slate-200/80">
                            <span class="px-2.5 py-1 rounded-md bg-white border border-slate-200 text-xs font-medium text-slate-700">Zendesk</span>
                            <span class="px-2.5 py-1 rounded-md bg-white border border-slate-200 text-xs font-medium text-slate-700">Power BI</span>
                            <span class="px-2.5 py-1 rounded-md bg-white border border-slate-200 text-xs font-medium text-slate-700">Jira &amp; Product Ops</span>
                        </div>
                    </div>
                </div>
            </article>

            <!-- Role 3: South Bay BMW & MINI -->
            <article class="card-elevated rounded-2xl p-6 sm:p-8 border-l-4 border-l-slate-700">
                <div class="flex flex-col md:flex-row md:items-center justify-between gap-2 pb-4 border-b border-slate-100">
                    <div>
                        <h3 class="font-display text-xl font-bold text-navy-900">Service Operations Manager</h3>
                        <p class="text-base font-semibold text-slate-700 mt-1">South Bay BMW &amp; MINI <span class="text-slate-400 font-normal">• Torrance, CA</span></p>
                    </div>
                    <div class="text-sm font-semibold text-slate-600 bg-slate-100 px-3.5 py-1.5 rounded-xl self-start md:self-center">
                        January 2013 – November 2015
                    </div>
                </div>

                <div class="pt-4">
                    <ul class="space-y-2.5 text-sm sm:text-[15px] text-slate-700 leading-relaxed">
                        <li class="flex items-start gap-3">
                            <span class="w-1.5 h-1.5 rounded-full bg-slate-700 mt-2 shrink-0"></span>
                            <span>Directed daily service operations for a premier luxury dealership, leading <strong>25+ cross-functional team members</strong> across service, parts, and technical departments.</span>
                        </li>
                        <li class="flex items-start gap-3">
                            <span class="w-1.5 h-1.5 rounded-full bg-slate-700 mt-2 shrink-0"></span>
                            <span>Achieved <strong>98%+ customer satisfaction</strong> while consistently exceeding monthly revenue targets through workflow optimization and white-glove client relationship initiatives.</span>
                        </li>
                    </ul>
                </div>
            </article>
        </div>
    </section>

    <!-- Interactive Feature 2: Interactive 90 / 180 / 365 Day CS Playbook Preview -->
    <section id="playbook" class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 pt-16 sm:pt-24">
        <div class="bg-navy-900 rounded-3xl p-6 sm:p-10 lg:p-12 text-white shadow-xl relative overflow-hidden">
            <div class="absolute top-0 right-0 w-80 h-80 bg-brand-teal/15 rounded-full blur-3xl pointer-events-none"></div>

            <div class="relative z-10">
                <div class="flex flex-col lg:flex-row lg:items-end justify-between gap-6 mb-8">
                    <div>
                        <span class="inline-block text-xs font-bold uppercase tracking-widest text-teal-400 mb-2">Strategic Execution Roadmap</span>
                        <h2 class="font-display text-2xl sm:text-3xl font-bold tracking-tight">How I Deliver Impact: First 90, 180 &amp; 365 Days</h2>
                        <p class="text-slate-300 text-sm sm:text-base mt-2 max-w-2xl">
                            A proven leadership blueprint for ramping rapidly on complex SaaS platforms, de-risking enterprise accounts, and scaling Customer Experience operations.
                        </p>
                    </div>

                    <!-- Playbook Horizon Tabs -->
                    <div class="inline-flex p-1.5 rounded-2xl bg-white/10 border border-white/15 gap-1 no-print" role="tablist">
                        <button onclick="switchPlaybook('90')" id="pb-btn-90" class="pb-tab px-4 py-2.5 rounded-xl text-xs sm:text-sm font-semibold transition-all cursor-pointer bg-brand-teal text-white shadow">
                            Days 1–90: Ramp &amp; Align
                        </button>
                        <button onclick="switchPlaybook('180')" id="pb-btn-180" class="pb-tab px-4 py-2.5 rounded-xl text-xs sm:text-sm font-semibold transition-all cursor-pointer text-slate-300 hover:text-white">
                            Days 91–180: Scale &amp; Optimize
                        </button>
                        <button onclick="switchPlaybook('365')" id="pb-btn-365" class="pb-tab px-4 py-2.5 rounded-xl text-xs sm:text-sm font-semibold transition-all cursor-pointer text-slate-300 hover:text-white">
                            Days 181–365: Lead &amp; Expand
                        </button>
                    </div>
                </div>

                <!-- Dynamic Playbook Content -->
                <div id="playbook-container" class="grid grid-cols-1 md:grid-cols-3 gap-5">
                    <!-- Populated via JS -->
                </div>
            </div>
        </div>
    </section>

    <!-- Education & Core Tech Stack Section -->
    <section class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 pt-16 sm:pt-24">
        <div class="grid grid-cols-1 lg:grid-cols-12 gap-8">
            <!-- Education Column -->
            <div class="lg:col-span-5">
                <span class="inline-block text-xs font-bold uppercase tracking-widest text-brand-blue mb-2">Academic Credentials</span>
                <h2 class="font-display text-2xl font-bold text-navy-900 tracking-tight mb-6">Education</h2>

                <div class="space-y-4">
                    <div class="card-elevated rounded-2xl p-6 border-l-4 border-l-brand-teal">
                        <div class="flex items-start justify-between gap-3">
                            <div>
                                <h3 class="font-display font-bold text-lg text-navy-900">Master of Business Administration (MBA)</h3>
                                <p class="text-sm font-semibold text-slate-700 mt-0.5">Grand Canyon University</p>
                            </div>
                            <span class="px-3 py-1 rounded-lg bg-slate-100 text-xs font-bold text-navy-900">2026</span>
                        </div>
                        <div class="mt-3 inline-flex items-center gap-1.5 px-3 py-1 rounded-full bg-teal-50 text-brand-teal text-xs font-bold">
                            <svg class="w-3.5 h-3.5" fill="currentColor" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/></svg>
                            <span>Summa Cum Laude</span>
                        </div>
                    </div>

                    <div class="card-elevated rounded-2xl p-6 border-l-4 border-l-brand-blue">
                        <div class="flex items-start justify-between gap-3">
                            <div>
                                <h3 class="font-display font-bold text-lg text-navy-900">Bachelor of Arts (BA), Arts</h3>
                                <p class="text-sm font-semibold text-slate-700 mt-0.5">Grand Canyon University</p>
                            </div>
                            <span class="px-3 py-1 rounded-lg bg-slate-100 text-xs font-bold text-navy-900">2020</span>
                        </div>
                        <div class="mt-3 inline-flex items-center gap-1.5 px-3 py-1 rounded-full bg-blue-50 text-brand-blue text-xs font-bold">
                            <span>Magna Cum Laude</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Systems, Analytics & Competencies Column -->
            <div class="lg:col-span-7">
                <span class="inline-block text-xs font-bold uppercase tracking-widest text-brand-teal mb-2">Operational Ecosystem</span>
                <h2 class="font-display text-2xl font-bold text-navy-900 tracking-tight mb-6">Enterprise Tech Stack &amp; Core Competencies</h2>

                <div class="card-elevated rounded-2xl p-6 sm:p-7 space-y-6">
                    <div>
                        <h3 class="text-xs font-bold uppercase tracking-wider text-slate-500 mb-3">CRM, Service Delivery &amp; Product Collaboration</h3>
                        <div class="flex flex-wrap gap-2">
                            <span class="px-3.5 py-2 rounded-xl bg-slate-900 text-white text-xs font-semibold">Salesforce</span>
                            <span class="px-3.5 py-2 rounded-xl bg-slate-900 text-white text-xs font-semibold">Zendesk</span>
                            <span class="px-3.5 py-2 rounded-xl bg-slate-100 text-navy-900 border border-slate-200 text-xs font-semibold">Jira</span>
                            <span class="px-3.5 py-2 rounded-xl bg-slate-100 text-navy-900 border border-slate-200 text-xs font-semibold">HubSpot</span>
                            <span class="px-3.5 py-2 rounded-xl bg-slate-100 text-navy-900 border border-slate-200 text-xs font-semibold">Freshdesk</span>
                            <span class="px-3.5 py-2 rounded-xl bg-slate-100 text-navy-900 border border-slate-200 text-xs font-semibold">Confluence</span>
                        </div>
                    </div>

                    <div>
                        <h3 class="text-xs font-bold uppercase tracking-wider text-slate-500 mb-3">Analytics, Reporting &amp; AI Automation</h3>
                        <div class="flex flex-wrap gap-2">
                            <span class="px-3.5 py-2 rounded-xl bg-blue-50 text-brand-blue border border-blue-200/70 text-xs font-semibold">Microsoft Power BI</span>
                            <span class="px-3.5 py-2 rounded-xl bg-teal-50 text-brand-teal border border-teal-200/70 text-xs font-semibold">AI Prompt Workflows (Gemini &amp; ChatGPT)</span>
                            <span class="px-3.5 py-2 rounded-xl bg-slate-100 text-navy-900 border border-slate-200 text-xs font-semibold">Advanced Excel</span>
                            <span class="px-3.5 py-2 rounded-xl bg-slate-100 text-navy-900 border border-slate-200 text-xs font-semibold">Basic SQL</span>
                            <span class="px-3.5 py-2 rounded-xl bg-slate-100 text-navy-900 border border-slate-200 text-xs font-semibold">Operational KPI &amp; SLA Dashboards</span>
                        </div>
                    </div>

                    <div>
                        <h3 class="text-xs font-bold uppercase tracking-wider text-slate-500 mb-3">Executive Leadership &amp; CS Domains</h3>
                        <div class="flex flex-wrap gap-2">
                            <span class="px-3 py-1.5 rounded-lg bg-slate-50 text-slate-700 border border-slate-200/80 text-xs font-medium">Enterprise Account Strategy</span>
                            <span class="px-3 py-1.5 rounded-lg bg-slate-50 text-slate-700 border border-slate-200/80 text-xs font-medium">C-Suite Consulting</span>
                            <span class="px-3 py-1.5 rounded-lg bg-slate-50 text-slate-700 border border-slate-200/80 text-xs font-medium">SaaS Onboarding &amp; Enablement</span>
                            <span class="px-3 py-1.5 rounded-lg bg-slate-50 text-slate-700 border border-slate-200/80 text-xs font-medium">Escalation Management</span>
                            <span class="px-3 py-1.5 rounded-lg bg-slate-50 text-slate-700 border border-slate-200/80 text-xs font-medium">Churn Mitigation &amp; ARR Expansion</span>
                            <span class="px-3 py-1.5 rounded-lg bg-slate-50 text-slate-700 border border-slate-200/80 text-xs font-medium">Cross-Functional Product Advocacy</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Interactive Feature 4: Quick-Copy Recruiter Brief & Contact Hub -->
    <section id="recruiter-hub" class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 pt-16 sm:pt-24 pb-20">
        <div class="card-elevated rounded-3xl p-6 sm:p-10 bg-white border-2 border-slate-200">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-start">
                <!-- Left: Direct Contact & Quick Copy -->
                <div class="lg:col-span-5 space-y-5">
                    <div>
                        <span class="inline-block text-xs font-bold uppercase tracking-widest text-brand-teal mb-2">Recruiter &amp; Hiring Manager Hub</span>
                        <h2 class="font-display text-2xl sm:text-3xl font-bold text-navy-900 tracking-tight">Ready to Scale Your Customer Organization?</h2>
                        <p class="text-sm text-slate-600 mt-2 leading-relaxed">
                            Use the one-click copy tools below to grab Kimberly’s contact information or paste her executive summary directly into your ATS or hiring committee notes.
                        </p>
                    </div>

                    <div class="space-y-3 pt-2">
                        <!-- Email Copy Card -->
                        <div class="flex items-center justify-between p-4 rounded-2xl bg-slate-50 border border-slate-200">
                            <div class="min-w-0 pr-3">
                                <span class="text-xs font-bold uppercase tracking-wider text-slate-400 block">Direct Email</span>
                                <span class="text-sm font-semibold text-navy-900 truncate block">kimberlyveronica@me.com</span>
                            </div>
                            <button onclick="copyText('kimberlyveronica@me.com', 'Email copied to clipboard!')" class="shrink-0 px-3.5 py-2 rounded-xl bg-white hover:bg-slate-100 text-navy-900 border border-slate-300 text-xs font-semibold shadow-2xs transition-colors cursor-pointer no-print">
                                Copy
                            </button>
                        </div>

                        <!-- Phone Copy Card -->
                        <div class="flex items-center justify-between p-4 rounded-2xl bg-slate-50 border border-slate-200">
                            <div>
                                <span class="text-xs font-bold uppercase tracking-wider text-slate-400 block">Direct Phone</span>
                                <span class="text-sm font-semibold text-navy-900">+1 714 492 4359</span>
                            </div>
                            <button onclick="copyText('+1 714 492 4359', 'Phone number copied to clipboard!')" class="shrink-0 px-3.5 py-2 rounded-xl bg-white hover:bg-slate-100 text-navy-900 border border-slate-300 text-xs font-semibold shadow-2xs transition-colors cursor-pointer no-print">
                                Copy
                            </button>
                        </div>

                        <!-- Location Card -->
                        <div class="flex items-center justify-between p-4 rounded-2xl bg-slate-50 border border-slate-200">
                            <div>
                                <span class="text-xs font-bold uppercase tracking-wider text-slate-400 block">Location &amp; Work Style</span>
                                <span class="text-sm font-semibold text-navy-900">Chino, CA • Remote / Hybrid</span>
                            </div>
                            <a href="mailto:kimberlyveronica@me.com?subject=Interview%20Invitation%20%E2%80%94%20Customer%20Success%20Leadership" class="shrink-0 px-3.5 py-2 rounded-xl bg-brand-blue hover:bg-blue-600 text-white text-xs font-semibold transition-colors no-print">
                                Email Now
                            </a>
                        </div>
                    </div>
                </div>

                <!-- Right: One-Click Recruiter Summary Brief -->
                <div class="lg:col-span-7 bg-slate-900 text-white rounded-2xl p-6 sm:p-8 flex flex-col justify-between">
                    <div>
                        <div class="flex flex-wrap items-center justify-between gap-3 mb-4">
                            <div class="flex items-center gap-2">
                                <span class="w-2.5 h-2.5 rounded-full bg-brand-teal"></span>
                                <h3 class="font-display font-bold text-base sm:text-lg">Executive Recruiter Brief (Ready to Paste)</h3>
                            </div>
                            <button onclick="copyRecruiterBrief()" class="inline-flex items-center gap-2 px-4 py-2 rounded-xl bg-brand-teal hover:bg-teal-500 text-white text-xs font-semibold transition-all cursor-pointer no-print">
                                <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M8 5H6a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2v-1M8 5a2 2 0 002 2h2a2 2 0 002-2M8 5a2 2 0 012-2h2a2 2 0 012 2m0 0h2a2 2 0 012 2v3m2 4H10m0 0l3-3m-3 3l3 3"/></svg>
                                <span>Copy Full Candidate Brief</span>
                            </button>
                        </div>

                        <div id="recruiter-brief-text" class="bg-white/5 border border-white/10 rounded-xl p-5 text-xs sm:text-sm text-slate-300 leading-relaxed space-y-3 font-normal">
                            <p><strong class="text-white">Candidate:</strong> Kimberly Skovold | Customer Success &amp; Technical Support Leader (MBA, Summa Cum Laude)</p>
                            <p><strong class="text-white">Core Value Proposition:</strong> Customer Success leader and former Director of Technical Support with 10+ years of experience scaling enterprise account management frameworks, North American technical service teams, and SaaS operations.</p>
                            <p><strong class="text-white">Key Quantified Wins:</strong><br>
                            • Manages a portfolio of 70+ enterprise accounts at Dynatron Software, driving analytics adoption, ARR retention, and C-suite KPI consulting.<br>
                            • Engineered AI prompt workflows (Gemini &amp; ChatGPT) that cut executive consultation preparation time by 60%.<br>
                            • Scaled myKaarma’s North American technical support team by 200% (3 to 9 members) and maintained SLA compliance across a 3x ticket volume surge.<br>
                            • Sustained a 98%+ client CSAT rating while partnering cross-functionally with Product, Engineering, and Sales.</p>
                            <p><strong class="text-white">Contact:</strong> Chino, CA | +1 714 492 4359 | kimberlyveronica@me.com</p>
                        </div>
                    </div>

                    <div class="mt-5 pt-4 border-t border-white/10 flex flex-wrap items-center justify-between gap-2 text-xs text-slate-400">
                        <span>Target Roles: Senior / Enterprise CSM, Director of CS, Client Operations</span>
                        <button onclick="window.print()" class="text-teal-300 hover:text-teal-200 font-semibold underline underline-offset-4 cursor-pointer no-print">
                            Save Page as PDF
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="border-t border-slate-200 bg-white py-8">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col sm:flex-row items-center justify-between gap-4 text-xs text-slate-500">
            <p class="font-medium text-slate-700">© 2026 Kimberly Skovold. Customer Success &amp; Technical Support Leader.</p>
            <div class="flex items-center gap-5">
                <span>Chino, CA</span>
                <span>•</span>
                <span>kimberlyveronica@me.com</span>
                <span>•</span>
                <span>+1 714 492 4359</span>
            </div>
        </div>
    </footer>

    <!-- Interactive JavaScript Logic -->
    <script>
        // Data for Role-Fit Lens Switcher
        const roleLenses = {
            cs: {
                badge: 'Senior & Enterprise Customer Success Lens',
                badgeColor: 'bg-teal-50 text-brand-teal border-teal-200',
                headline: 'Trusted C-Suite Advisor Driving Adoption, Retention & Enterprise ARR Expansion',
                summary: 'Combines executive-level KPI consulting with proactive onboarding frameworks to turn complex enterprise SaaS deployments into measurable profitability and long-term net dollar retention.',
                highlights: [
                    {
                        title: '70+ Enterprise Account Portfolio Ownership',
                        detail: 'Direct strategic advisor at Dynatron Software, guiding C-suite and operational stakeholders through data-driven growth frameworks that strengthen ARR retention and expansion.'
                    },
                    {
                        title: 'Proactive Onboarding & Early Churn Reduction',
                        detail: 'Spearheaded structured onboarding and customer enablement programs that accelerated client time-to-value and measurably reduced early-stage account churn.'
                    },
                    {
                        title: 'Executive QBR & KPI Consulting',
                        detail: 'Translates complex platform analytics into clear operational and financial outcomes, partnering across Sales, Product, and Solutions teams to champion customer advocacy.'
                    }
                ],
                tools: ['Salesforce', 'HubSpot', 'Power BI', 'Gemini & ChatGPT Workflows', 'Executive QBR Frameworks', 'Confluence'],
                keyMetric: { value: '70+', label: 'Enterprise Accounts Advised', sub: 'With 98%+ sustained client CSAT' }
            },
            support: {
                badge: 'Director of Technical Support & Escalations Lens',
                badgeColor: 'bg-blue-50 text-brand-blue border-blue-200',
                headline: 'High-Velocity Support Architecture & Cross-Functional Escalation Leadership',
                summary: 'Proven track record building North American technical support organizations from the ground up, engineering automated SLA routing, and partnering with Engineering to eliminate product friction.',
                highlights: [
                    {
                        title: '200% North American Team Expansion',
                        detail: 'Built and scaled myKaarma’s technical support division from 3 to 9 specialists across the US and Canada while reducing turnover through structured technical mentorship.'
                    },
                    {
                        title: '3x Ticket Surge SLA Resilience',
                        detail: 'Engineered automated support workflows, tiered escalation protocols, and Power BI / Zendesk dashboards that elevated response efficiency during a 300% volume increase.'
                    },
                    {
                        title: 'Engineering & Product Feedback Loop',
                        detail: 'Orchestrated seamless escalation management between Support, Engineering, and Product to improve platform stability and boost annual CSAT and NPS scores.'
                    }
                ],
                tools: ['Zendesk', 'Jira', 'Freshdesk', 'Power BI', 'Basic SQL', 'Confluence', 'SLA & Escalation Protocols'],
                keyMetric: { value: '200%', label: 'Support Division Growth', sub: 'Maintained SLAs through 3x ticket surge' }
            },
            ops: {
                badge: 'AI Enablement & Client Operations Lens',
                badgeColor: 'bg-indigo-50 text-indigo-600 border-indigo-200',
                headline: 'MBA-Backed Operational Rigor & AI-Powered Customer Workflow Automation',
                summary: 'Bridges business strategy (MBA, Summa Cum Laude) with hands-on AI workflow engineering and BI telemetry to eliminate manual bottlenecks and scale customer operations efficiently.',
                highlights: [
                    {
                        title: '60% Reduction in Consultation Prep Time',
                        detail: 'Designed structured AI prompt workflows in Gemini and ChatGPT to automate client performance synthesis and executive meeting preparation across 70+ accounts.'
                    },
                    {
                        title: 'Automated Telemetry & KPI Dashboards',
                        detail: 'Built real-time operational reporting across Salesforce, Zendesk, Power BI, and Excel to surface churn risks early and standardize team performance metrics.'
                    },
                    {
                        title: 'Multi-Department Operational Leadership',
                        detail: 'Directed 25+ cross-functional team members across service, technical, and parts operations at South Bay BMW & MINI, consistently exceeding monthly revenue targets.'
                    }
                ],
                tools: ['Gemini & ChatGPT', 'Microsoft Power BI', 'Salesforce', 'Advanced Excel', 'Basic SQL', 'Zendesk', 'Jira'],
                keyMetric: { value: '60%', label: 'Consultation Prep Saved', sub: 'Via structured LLM prompt workflows' }
            }
        };

        // Data for 90 / 180 / 365 Day Playbook
        const playbookHorizons = {
            '90': [
                {
                    step: '01 • Platform & Domain Mastery',
                    title: 'Deep-Dive Product & Workflow Immersion',
                    desc: 'Rapidly master core platform architecture, customer use cases, and compliance/operational workflows. Shadow active onboarding and executive calls to map existing friction points.'
                },
                {
                    step: '02 • Cross-Functional Alignment',
                    title: 'Internal Stakeholder & Escalation Sync',
                    desc: 'Establish tight operating rhythms with Solutions Architecture, Product, Engineering, and Support to ensure seamless handoffs from pre-sales through technical implementation.'
                },
                {
                    step: '03 • Early Portfolio Execution',
                    title: 'Lead Initial Onboardings & Risk Audits',
                    desc: 'Take ownership of initial customer onboarding milestones, conduct proactive health checks, and begin capturing structured product feedback from frontline stakeholders.'
                }
            ],
            '180': [
                {
                    step: '04 • Autonomous Portfolio Management',
                    title: 'Full Lifecycle Ownership & Adoption',
                    desc: 'Independently drive onboarding, technical enablement, and executive QBRs across the assigned enterprise portfolio—aligning platform usage directly to client KPIs.'
                },
                {
                    step: '05 • Scalable Playbooks & AI Workflows',
                    title: 'Standardize Onboarding & Prep Automation',
                    desc: 'Contribute repeatable onboarding playbooks, health-scoring telemetry, and AI-assisted QBR synthesis workflows to elevate team-wide efficiency and reduce time-to-value.'
                },
                {
                    step: '06 • Proactive Churn Mitigation',
                    title: 'Early Risk Detection & Get-Well Plans',
                    desc: 'Leverage operational usage signals to identify adoption gaps early, executing cross-functional mitigation plans that protect renewals and strengthen stakeholder trust.'
                }
            ],
            '365': [
                {
                    step: '07 • Executive Advisory & Expansion',
                    title: 'Drive Net Revenue Retention & Advocacy',
                    desc: 'Operate as a trusted C-suite partner across key enterprise accounts—uncovering expansion opportunities, securing referenceable advocates, and sustaining 98%+ CSAT.'
                },
                {
                    step: '08 • Team Mentorship & Enablement',
                    title: 'Elevate Customer Experience Capabilities',
                    desc: 'Mentor incoming CSMs and support specialists in executive communication, escalation management, and data-driven client coaching to scale organizational maturity.'
                },
                {
                    step: '09 • Product & Strategic Influence',
                    title: 'Shape Roadmap & Operational Evolution',
                    desc: 'Synthesize enterprise trends into actionable product insights for leadership, demonstrating measurable impact on retention, operational efficiency, and platform evolution.'
                }
            ]
        };

        // Render Role Lens
        function switchLens(lensKey) {
            const data = roleLenses[lensKey];
            if (!data) return;

            // Update active tab styling
            document.querySelectorAll('.lens-tab').forEach(btn => {
                btn.classList.remove('bg-navy-900', 'text-white', 'shadow-sm');
                btn.classList.add('text-slate-700', 'hover:text-navy-900');
            });
            const activeBtn = document.getElementById(`lens-btn-${lensKey}`);
            activeBtn.classList.remove('text-slate-700', 'hover:text-navy-900');
            activeBtn.classList.add('bg-navy-900', 'text-white', 'shadow-sm');

            const container = document.getElementById('lens-container');
            container.innerHTML = `
                <div class="fade-in-up grid grid-cols-1 lg:grid-cols-12 gap-8 items-start">
                    <div class="lg:col-span-8 space-y-6">
                        <div>
                            <span class="inline-flex items-center px-3 py-1 rounded-full text-xs font-bold border ${data.badgeColor} mb-3">
                                ${data.badge}
                            </span>
                            <h3 class="font-display text-2xl sm:text-3xl font-bold text-navy-900 leading-tight">
                                ${data.headline}
                            </h3>
                            <p class="text-slate-600 text-sm sm:text-base mt-3 leading-relaxed">
                                ${data.summary}
                            </p>
                        </div>

                        <div class="grid grid-cols-1 md:grid-cols-3 gap-4 pt-2">
                            ${data.highlights.map(item => `
                                <div class="p-4 rounded-2xl bg-slate-50 border border-slate-200/80">
                                    <h4 class="font-display font-bold text-sm text-navy-900 mb-1.5">${item.title}</h4>
                                    <p class="text-xs text-slate-600 leading-relaxed">${item.detail}</p>
                                </div>
                            `).join('')}
                        </div>
                    </div>

                    <div class="lg:col-span-4 bg-slate-900 text-white rounded-2xl p-6 flex flex-col justify-between h-full">
                        <div>
                            <span class="text-xs font-bold uppercase tracking-wider text-teal-400 block mb-2">Anchor Proof Point</span>
                            <div class="font-display text-4xl font-extrabold text-white">${data.keyMetric.value}</div>
                            <p class="text-sm font-semibold text-slate-200 mt-1">${data.keyMetric.label}</p>
                            <p class="text-xs text-slate-400 mt-0.5">${data.keyMetric.sub}</p>

                            <div class="mt-6 pt-5 border-t border-white/10">
                                <span class="text-xs font-bold uppercase tracking-wider text-slate-400 block mb-3">Priority Tech Stack for Role</span>
                                <div class="flex flex-wrap gap-1.5">
                                    ${data.tools.map(tool => `
                                        <span class="px-2.5 py-1 rounded-lg bg-white/10 text-xs font-medium text-slate-200 border border-white/10">${tool}</span>
                                    `).join('')}
                                </div>
                            </div>
                        </div>

                        <div class="mt-6 pt-4 border-t border-white/10">
                            <a href="#recruiter-hub" class="w-full inline-flex items-center justify-center gap-2 px-4 py-2.5 rounded-xl bg-brand-teal hover:bg-teal-500 text-white text-xs font-semibold transition-colors">
                                <span>Connect Regarding This Role</span>
                                <svg class="w-3.5 h-3.5" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M14 5l7 7m0 0l-7 7m7-7H3"/></svg>
                            </a>
                        </div>
                    </div>
                </div>
            `;
        }

        // Render Playbook Horizon
        function switchPlaybook(horizon) {
            const items = playbookHorizons[horizon];
            if (!items) return;

            document.querySelectorAll('.pb-tab').forEach(btn => {
                btn.classList.remove('bg-brand-teal', 'text-white', 'shadow');
                btn.classList.add('text-slate-300', 'hover:text-white');
            });
            const activeBtn = document.getElementById(`pb-btn-${horizon}`);
            activeBtn.classList.remove('text-slate-300', 'hover:text-white');
            activeBtn.classList.add('bg-brand-teal', 'text-white', 'shadow');

            const container = document.getElementById('playbook-container');
            container.innerHTML = items.map(card => `
                <div class="fade-in-up bg-white/5 border border-white/10 rounded-2xl p-6 hover:bg-white/[0.08] transition-colors">
                    <span class="text-xs font-bold uppercase tracking-wider text-teal-300 block mb-2">${card.step}</span>
                    <h3 class="font-display text-lg font-bold text-white mb-2.5">${card.title}</h3>
                    <p class="text-sm text-slate-300 leading-relaxed">${card.desc}</p>
                </div>
            `).join('');
        }

        // Copy-to-Clipboard with Fallback
        function copyText(text, successMsg) {
            const tempInput = document.createElement('textarea');
            tempInput.value = text;
            tempInput.style.position = 'fixed';
            tempInput.style.left = '-9999px';
            document.body.appendChild(tempInput);
            tempInput.select();
            try {
                document.execCommand('copy');
                showToast(successMsg || 'Copied to clipboard!');
            } catch (err) {
                showToast('Unable to copy automatically. Please select and copy manually.');
            }
            document.body.removeChild(tempInput);
        }

        function copyRecruiterBrief() {
            const brief = `Candidate: Kimberly Skovold | Customer Success & Technical Support Leader (MBA, Summa Cum Laude)
Core Value Proposition: Customer Success leader and former Director of Technical Support with 10+ years of experience scaling enterprise account management frameworks, North American technical service teams, and SaaS operations.
Key Quantified Wins:
• Manages a portfolio of 70+ enterprise accounts at Dynatron Software, driving analytics adoption, ARR retention, and C-suite KPI consulting.
• Engineered AI prompt workflows (Gemini & ChatGPT) that cut executive consultation preparation time by 60%.
• Scaled myKaarma’s North American technical support team by 200% (3 to 9 members) and maintained SLA compliance across a 3x ticket volume surge.
• Sustained a 98%+ client CSAT rating while partnering cross-functionally with Product, Engineering, and Sales.
Contact: Chino, CA | +1 714 492 4359 | kimberlyveronica@me.com`;
            copyText(brief, 'Full recruiter brief copied to clipboard!');
        }

        let toastTimeout;
        function showToast(message) {
            const toast = document.getElementById('toast');
            const msgEl = document.getElementById('toast-message');
            msgEl.textContent = message;
            toast.classList.remove('translate-y-20', 'opacity-0');
            clearTimeout(toastTimeout);
            toastTimeout = setTimeout(() => {
                toast.classList.add('translate-y-20', 'opacity-0');
            }, 3200);
        }

        // Initialize Default Interactive Views on Load
        document.addEventListener('DOMContentLoaded', () => {
            switchLens('cs');
            switchPlaybook('90');
        });
    </script>
</body>
</html>