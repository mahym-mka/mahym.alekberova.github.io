<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mahym Alekberova | Portfolio & Writing Hub</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Inter Font -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        brand: {
                            dark: '#00264d',     // Deep Policy Blue
                            navy: '#003366',     // Primary Header Blue
                            accent: '#0066cc',   // Vibrant Action Blue
                            light: '#e6f0fa',    // Soft Highlight Blue
                            bg: '#f4f7fa',       // Clean Neutral Grey/Blue BG
                            card: '#ffffff'      // Pure White Card BG
                        }
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    <style>
        /* Custom scrollbar for line-limited containers */
        .custom-scrollbar::-webkit-scrollbar {
            width: 6px;
        }
        .custom-scrollbar::-webkit-scrollbar-track {
            background: #f1f5f9;
            border-radius: 4px;
        }
        .custom-scrollbar::-webkit-scrollbar-thumb {
            background: #cbd5e1;
            border-radius: 4px;
        }
        .custom-scrollbar::-webkit-scrollbar-thumb:hover {
            background: #94a3b8;
        }
    </style>
</head>
<body class="bg-brand-bg font-sans text-slate-800 antialiased min-h-screen flex flex-col justify-between">

    <div>
        <header class="bg-gradient-to-r from-brand-dark via-brand-navy to-brand-accent text-white shadow-lg border-b-4 border-brand-accent">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8 sm:py-10">
                <div class="flex flex-col md:flex-row items-center justify-between gap-6">
                    <div class="text-center md:text-left">
                        <div class="inline-flex items-center gap-2 bg-white/10 backdrop-blur-md px-3 py-1 rounded-full text-xs font-semibold uppercase tracking-wider text-blue-100 mb-3 border border-white/20">
                            <i class="fa-solid me-1 fa-globe"></i> Public Policy & Development Hub
                        </div>
                        <h1 class="text-3xl sm:text-4xl md:text-5xl font-bold tracking-tight text-white">
                            Mahym Alekberova
                        </h1>
                        <p class="mt-2 text-lg sm:text-xl text-blue-100 font-light max-w-2xl">
                            Portfolio & Writing Hub — Policy Analysis, Spatial Analytics & Global Governance
                        </p>
                    </div>
                    <!-- Quick Actions / Social Header Links -->
                    <div class="flex items-center gap-3 bg-white/10 backdrop-blur-sm p-3 rounded-xl border border-white/15 shadow-inner">
                        <a href="mailto:email@example.com" title="Email Contact" class="p-2.5 bg-white text-brand-navy hover:bg-brand-light hover:text-brand-accent rounded-lg transition-all duration-200 shadow-sm font-medium text-sm flex items-center gap-2">
                            <i class="fa-solid fa-envelope"></i>
                            <span class="hidden sm:inline">Contact</span>
                        </a>
                        <a href="https://linkedin.com" target="_blank" title="LinkedIn Profile" class="p-2.5 bg-white text-brand-navy hover:bg-brand-light hover:text-brand-accent rounded-lg transition-all duration-200 shadow-sm font-medium text-sm flex items-center gap-2">
                            <i class="fa-brands fa-linkedin"></i>
                            <span class="hidden sm:inline">LinkedIn</span>
                        </a>
                        <a href="https://github.com/mahym-mka" target="_blank" title="GitHub Repository" class="p-2.5 bg-white text-brand-navy hover:bg-brand-light hover:text-brand-accent rounded-lg transition-all duration-200 shadow-sm font-medium text-sm flex items-center gap-2">
                            <i class="fa-brands fa-github"></i>
                            <span class="hidden sm:inline">GitHub</span>
                        </a>
                    </div>
                </div>
            </div>
        </header>

        <main class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-8">
                
                <!-- LEFT SIDEBAR -->
                <aside class="lg:col-span-4 space-y-6">
                    <!-- Navigation Panel -->
                    <div class="bg-brand-card p-5 rounded-2xl shadow-sm border border-slate-200">
                        <h2 class="text-xs font-bold uppercase tracking-wider text-slate-400 mb-4 px-2">
                            Navigation
                        </h2>
                        <nav class="space-y-2.5" id="nav-container">
                            <button onclick="switchTab('cv')" id="btn-cv" class="nav-btn w-full flex items-center gap-3 px-4 py-3 rounded-xl font-medium text-left transition-all duration-200 bg-brand-navy text-white shadow-md">
                                <i class="fa-solid fa-file-lines w-5 text-center"></i>
                                <span>CV / Resume</span>
                            </button>
                            <button onclick="switchTab('about')" id="btn-about" class="nav-btn w-full flex items-center gap-3 px-4 py-3 rounded-xl font-medium text-left transition-all duration-200 text-slate-600 hover:bg-brand-light hover:text-brand-accent">
                                <i class="fa-solid fa-user-tie w-5 text-center"></i>
                                <span>About Me</span>
                            </button>
                            <button onclick="switchTab('research')" id="btn-research" class="nav-btn w-full flex items-center gap-3 px-4 py-3 rounded-xl font-medium text-left transition-all duration-200 text-slate-600 hover:bg-brand-light hover:text-brand-accent">
                                <i class="fa-solid fa-book-bookmark w-5 text-center"></i>
                                <span>Research & Policy Briefs</span>
                            </button>
                            <button onclick="switchTab('blog')" id="btn-blog" class="nav-btn w-full flex items-center gap-3 px-4 py-3 rounded-xl font-medium text-left transition-all duration-200 text-slate-600 hover:bg-brand-light hover:text-brand-accent">
                                <i class="fa-solid fa-pen-nib w-5 text-center"></i>
                                <span>Blog & Writing</span>
                            </button>
                        </nav>
                    </div>

                    <!-- Styled 20-Line Text Box Sidebar Container -->
                    <div class="bg-brand-card p-5 rounded-2xl shadow-sm border border-slate-200">
                        <div class="flex items-center justify-between mb-3 border-b border-slate-100 pb-3">
                            <h2 class="text-xs font-bold uppercase tracking-wider text-slate-400 flex items-center gap-2">
                                <i class="fa-solid fa-quote-left text-brand-accent"></i> Executive Briefing
                            </h2>
                            <span class="text-[10px] font-semibold bg-brand-light text-brand-accent px-2 py-0.5 rounded-full">20 Lines Summary</span>
                        </div>
                        <!-- Container constrained to exactly 20 lines (leading-relaxed line-height * 20) -->
                        <div class="text-xs leading-relaxed text-slate-600 space-y-2 overflow-y-auto max-h-[30rem] pr-1 custom-scrollbar">
                            <p><strong>Line 01:</strong> Policy practitioner specialized in economic development & governance.</p>
                            <p><strong>Line 02:</strong> Applied quantitative research methods and spatial analytics (GIS) to regional problems.</p>
                            <p><strong>Line 03:</strong> Focus on municipal efficiency, infrastructure routing, and trade frameworks.</p>
                            <p><strong>Line 04:</strong> Skilled in translating complex data into concise, actionable policy briefs.</p>
                            <p><strong>Line 05:</strong> Research interest spans firm informality and macroeconomic market dynamics.</p>
                            <p><strong>Line 06:</strong> Experienced in multi-stakeholder policy formulation and baseline evaluations.</p>
                            <p><strong>Line 07:</strong> Utilizing econometric models to assess structural reforms in emerging markets.</p>
                            <p><strong>Line 08:</strong> Proven track record in preparing executive-level memos and analytical notes.</p>
                            <p><strong>Line 09:</strong> Proficient in R, Python, Stata, and geospatial mapping tools.</p>
                            <p><strong>Line 10:</strong> Dedicated to evidence-based policy solutions and international growth.</p>
                            <p><strong>Line 11:</strong> Collaborated with international institutions and public sector working groups.</p>
                            <p><strong>Line 12:</strong> Integrating MEAL frameworks for robust program monitoring and feedback loops.</p>
                            <p><strong>Line 13:</strong> Focused on bridging high-level econometric theory with boots-on-the-ground reality.</p>
                            <p><strong>Line 14:</strong> Skilled in designing survey instruments for market and household data collection.</p>
                            <p><strong>Line 15:</strong> Published policy commentaries on regional economic integration and trade flows.</p>
                            <p><strong>Line 16:</strong> Experienced in organizing stakeholder roundtables and public consultations.</p>
                            <p><strong>Line 17:</strong> Adept at communicating findings to technical specialists and lay audiences alike.</p>
                            <p><strong>Line 18:</strong> Strong background in public finance management and institutional analysis.</p>
                            <p><strong>Line 19:</strong> Committed to open data standards, transparent methodologies, and continuous learning.</p>
                            <p><strong>Line 20:</strong> Open for research collaborations, policy consulting, and strategic advisory roles.</p>
                        </div>
                    </div>
                </aside>

                <!-- RIGHT MAIN CONTENT AREA -->
                <section class="lg:col-span-8">
                    
                    <!-- TAB 1: CV / RESUME (Default Visible) -->
                    <div id="tab-cv" class="tab-content space-y-6">
                        <div class="bg-brand-card p-6 sm:p-8 rounded-2xl shadow-sm border border-slate-200">
                            <div class="flex flex-wrap items-center justify-between gap-4 pb-6 border-b border-slate-100">
                                <div>
                                    <h2 class="text-2xl font-bold text-brand-navy">Curriculum Vitae</h2>
                                    <p class="text-sm text-slate-500">Public Policy Analysis & Research Profile</p>
                                </div>
                                <a href="sample1.pdf" download class="inline-flex items-center gap-2 bg-brand-accent hover:bg-brand-navy text-white px-4 py-2.5 rounded-xl font-medium text-sm transition-all shadow-md">
                                    <i class="fa-solid fa-file-arrow-down"></i> Download PDF Resume
                                </a>
                            </div>

                            <div class="mt-6 space-y-8">
                                <!-- Education -->
                                <div>
                                    <h3 class="text-lg font-semibold text-brand-navy mb-4 flex items-center gap-2">
                                        <i class="fa-solid fa-graduation-cap text-brand-accent"></i> Education
                                    </h3>
                                    <div class="border-l-2 border-brand-light pl-4 space-y-4">
                                        <div>
                                            <div class="flex justify-between items-baseline">
                                                <h4 class="font-semibold text-slate-800">Master of Public Policy (MPP)</h4>
                                                <span class="text-xs font-semibold text-brand-accent bg-brand-light px-2.5 py-1 rounded-md">2022 - 2024</span>
                                            </div>
                                            <p class="text-sm text-slate-600">Specialization in Quantitative Policy & International Development</p>
                                        </div>
                                    </div>
                                </div>

                                <!-- Professional Experience -->
                                <div>
                                    <h3 class="text-lg font-semibold text-brand-navy mb-4 flex items-center gap-2">
                                        <i class="fa-solid fa-briefcase text-brand-accent"></i> Experience Highlights
                                    </h3>
                                    <div class="border-l-2 border-brand-light pl-4 space-y-6">
                                        <div>
                                            <div class="flex justify-between items-baseline">
                                                <h4 class="font-semibold text-slate-800">Policy Analyst & Quantitative Researcher</h4>
                                                <span class="text-xs font-semibold text-slate-500">2024 - Present</span>
                                            </div>
                                            <p class="text-xs font-medium text-brand-accent">Development Policy Group</p>
                                            <ul class="mt-2 text-sm text-slate-600 list-disc list-inside space-y-1">
                                                <li>Authored policy memos on municipal resource allocation and spatial infrastructure efficiency.</li>
                                                <li>Applied econometric modeling to examine firm informality dynamics in regional markets.</li>
                                            </ul>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- TAB 2: ABOUT ME -->
                    <div id="tab-about" class="tab-content hidden space-y-6">
                        <div class="bg-brand-card p-6 sm:p-8 rounded-2xl shadow-sm border border-slate-200">
                            <h2 class="text-2xl font-bold text-brand-navy pb-4 border-b border-slate-100">About Me</h2>
                            <div class="mt-6 text-slate-600 space-y-4 leading-relaxed">
                                <p>
                                    Welcome to my policy portfolio and research repository. I am a public policy practitioner with a passion for data-driven economic development, spatial analytics, and governance research.
                                </p>
                                <p>
                                    My work focuses on bridging the gap between rigorous econometric methodologies and actionable policy formulation. I specialize in spatial route optimization, firm dynamics in developing markets, and structural economic analysis.
                                </p>
                                <div class="grid grid-cols-1 md:grid-cols-2 gap-4 mt-6">
                                    <div class="p-4 rounded-xl bg-brand-bg border border-slate-200">
                                        <h4 class="font-semibold text-brand-navy mb-1"><i class="fa-solid fa-chart-line text-brand-accent me-2"></i>Quantitative Methods</h4>
                                        <p class="text-xs text-slate-500">Econometrics, Stata, R, Python, and Survey Design</p>
                                    </div>
                                    <div class="p-4 rounded-xl bg-brand-bg border border-slate-200">
                                        <h4 class="font-semibold text-brand-navy mb-1"><i class="fa-solid fa-map-location-dot text-brand-accent me-2"></i>Spatial Analytics</h4>
                                        <p class="text-xs text-slate-500">GIS Mapping, Route Optimization & Spatial Hotspots</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- TAB 3: RESEARCH & POLICY BRIEFS -->
                    <div id="tab-research" class="tab-content hidden space-y-6">
                        <div class="bg-brand-card p-6 sm:p-8 rounded-2xl shadow-sm border border-slate-200">
                            <h2 class="text-2xl font-bold text-brand-navy pb-2">Research & Policy Briefs</h2>
                            <p class="text-sm text-slate-500 mb-6 pb-4 border-b border-slate-100">Peer-reviewed analytical notes, policy briefs, and spatial research projects.</p>

                            <!-- Sample Grid -->
                            <div class="grid grid-cols-1 gap-6">
                                
                                <!-- Card 1 -->
                                <div class="border border-slate-200 rounded-xl p-5 hover:shadow-md transition-shadow bg-white">
                                    <div class="flex flex-wrap gap-2 mb-3">
                                        <span class="text-xs font-semibold px-2.5 py-1 rounded-md bg-blue-50 text-brand-accent border border-blue-100">GIS Mapping</span>
                                        <span class="text-xs font-semibold px-2.5 py-1 rounded-md bg-blue-50 text-brand-accent border border-blue-100">Municipal Services</span>
                                    </div>
                                    <h3 class="text-lg font-bold text-slate-800 hover:text-brand-accent cursor-pointer">
                                        Spatial Route Optimization & Service Analysis
                                    </h3>
                                    <p class="text-xs font-semibold text-slate-500 mt-1">Context: Executive Municipal Infrastructure Brief</p>
                                    <p class="text-sm text-slate-600 mt-2 leading-relaxed">
                                        Evaluated municipal collection hotspot distributions to optimize spatial resource allocation, reducing transit bottlenecks and improving service coverage.
                                    </p>
                                    <div class="mt-4 pt-3 border-t border-slate-100 flex items-center justify-between">
                                        <span class="text-xs text-slate-400">Published 2024</span>
                                        <a href="sample1.pdf" download class="inline-flex items-center gap-1.5 text-xs font-semibold text-brand-accent hover:text-brand-navy">
                                            <i class="fa-solid fa-file-pdf"></i> Download Brief PDF
                                        </a>
                                    </div>
                                </div>

                                <!-- Card 2 -->
                                <div class="border border-slate-200 rounded-xl p-5 hover:shadow-md transition-shadow bg-white">
                                    <div class="flex flex-wrap gap-2 mb-3">
                                        <span class="text-xs font-semibold px-2.5 py-1 rounded-md bg-blue-50 text-brand-accent border border-blue-100">Trade Policy</span>
                                        <span class="text-xs font-semibold px-2.5 py-1 rounded-md bg-blue-50 text-brand-accent border border-blue-100">Regulatory Economics</span>
                                    </div>
                                    <h3 class="text-lg font-bold text-slate-800 hover:text-brand-accent cursor-pointer">
                                        Analytical Brief: Economic Policy & Firm Informality
                                    </h3>
                                    <p class="text-xs font-semibold text-slate-500 mt-1">Context: Developing Markets Trade Governance</p>
                                    <p class="text-sm text-slate-600 mt-2 leading-relaxed">
                                        Quantitative assessment of regulatory frameworks and informal firm behavior in response to cross-border trade policy adjustments.
                                    </p>
                                    <div class="mt-4 pt-3 border-t border-slate-100 flex items-center justify-between">
                                        <span class="text-xs text-slate-400">Published 2024</span>
                                        <a href="sample2.pdf" download class="inline-flex items-center gap-1.5 text-xs font-semibold text-brand-accent hover:text-brand-navy">
                                            <i class="fa-solid fa-file-pdf"></i> Download Brief PDF
                                        </a>
                                    </div>
                                </div>

                            </div>
                        </div>
                    </div>

                    <!-- TAB 4: BLOG & WRITING -->
                    <div id="tab-blog" class="tab-content hidden space-y-6">
                        <div class="bg-brand-card p-6 sm:p-8 rounded-2xl shadow-sm border border-slate-200">
                            <h2 class="text-2xl font-bold text-brand-navy pb-2">Blog & Policy Writing</h2>
                            <p class="text-sm text-slate-500 mb-6 pb-4 border-b border-slate-100">Commentaries, opinion pieces, and short analytical notes.</p>

                            <div class="space-y-6">
                                <article class="p-5 rounded-xl border border-slate-200 bg-white">
                                    <span class="text-xs text-slate-400">October 2024 • 5 min read</span>
                                    <h3 class="text-lg font-bold text-slate-800 mt-1">Translating Econometric Models into Policy Practice</h3>
                                    <p class="text-sm text-slate-600 mt-2">
                                        Why decision-makers often struggle with empirical findings and how researchers can better structure executive summaries for max impact.
                                    </p>
                                    <a href="#" class="inline-block mt-3 text-xs font-semibold text-brand-accent hover:underline">Read Article &rarr;</a>
                                </article>

                                <article class="p-5 rounded-xl border border-slate-200 bg-white">
                                    <span class="text-xs text-slate-400">September 2024 • 4 min read</span>
                                    <h3 class="text-lg font-bold text-slate-800 mt-1">The Role of Open Spatial Data in Local Governance</h3>
                                    <p class="text-sm text-slate-600 mt-2">
                                        How municipal planning departments leverage open-source GIS tools to optimize public service routing and infrastructure investment.
                                    </p>
                                    <a href="#" class="inline-block mt-3 text-xs font-semibold text-brand-accent hover:underline">Read Article &rarr;</a>
                                </article>
                            </div>
                        </div>
                    </div>

                </section>
            </div>
        </main>
    </div>

    <!-- FOOTER -->
    <footer class="bg-brand-dark text-slate-400 py-6 border-t border-slate-800 mt-12">
        <div class="max-w-7xl mx-auto px-4 text-center sm:flex sm:justify-between sm:items-center text-xs">
            <p>&copy; 2026 Mahym Alekberova. All rights reserved.</p>
            <p class="mt-2 sm:mt-0">Built with HTML & Tailwind CSS | Hosted on GitHub Pages</p>
        </div>
    </footer>

    <script>
        function switchTab(tabId) {
            // Hide all tab contents
            const contents = document.querySelectorAll('.tab-content');
            contents.forEach(el => el.classList.add('hidden'));

            // Reset all navigation button styles
            const buttons = document.querySelectorAll('.nav-btn');
            buttons.forEach(btn => {
                btn.classList.remove('bg-brand-navy', 'text-white', 'shadow-md');
                btn.classList.add('text-slate-600', 'hover:bg-brand-light', 'hover:text-brand-accent');
            });

            // Show target content
            const activeContent = document.getElementById('tab-' + tabId);
            if (activeContent) {
                activeContent.classList.remove('hidden');
            }

            // Highlight selected button
            const activeBtn = document.getElementById('btn-' + tabId);
            if (activeBtn) {
                activeBtn.classList.remove('text-slate-600', 'hover:bg-brand-light', 'hover:text-brand-accent');
                activeBtn.classList.add('bg-brand-navy', 'text-white', 'shadow-md');
            }
        }
    </script>
</body>
</html>
