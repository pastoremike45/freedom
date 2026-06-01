<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Michael • Freedomfighter News</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&amp;family=Space+Grotesk:wght@500;600&amp;display=swap');
        
        :root {
            --accent: #ef4444;
        }
        
        body {
            font-family: 'Inter', system_ui, sans-serif;
        }
        
        .font-display {
            font-family: 'Space Grotesk', 'Inter', system_ui, sans-serif;
            font-weight: 600;
            letter-spacing: -0.025em;
        }

        .section-header {
            font-size: 2.75rem;
            line-height: 1.05;
            font-weight: 700;
            letter-spacing: -0.04em;
        }

        .glass {
            background: rgba(255,255,255,0.06);
            backdrop-filter: blur(20px);
        }

        .nav-active {
            color: white;
            position: relative;
        }
        
        .nav-active:after {
            content: '';
            position: absolute;
            bottom: -2px;
            left: 0;
            width: 100%;
            height: 1px;
            background: linear-gradient(to right, #ef4444, transparent);
        }

        .content-card {
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }
        
        .content-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 20px 25px -5px rgb(0 0 0 / 0.1), 0 8px 10px -6px rgb(0 0 0 / 0.1);
            border-color: #ef4444;
        }

        .stat-number {
            font-variant-numeric: tabular-nums;
        }

        .red-accent {
            color: #ef4444;
        }

        .hero-bg {
            background: radial-gradient(circle at 50% 30%, rgba(239, 68, 68, 0.08) 0%, transparent 70%);
        }

        .link-btn {
            transition: all 0.2s ease;
        }
        
        .link-btn:hover {
            transform: translateX(4px);
        }

        .cocky-text {
            font-style: italic;
            color: #a1a1aa;
        }
    </style>
</head>
<body class="bg-zinc-950 text-white overflow-x-hidden">
    <!-- NAV -->
    <nav class="fixed top-0 left-0 right-0 z-50 border-b border-zinc-800 bg-zinc-950/95 backdrop-blur-lg">
        <div class="max-w-7xl mx-auto px-8 h-20 flex items-center justify-between">
            <div class="flex items-center gap-x-3">
                <div class="w-9 h-9 rounded-2xl bg-gradient-to-br from-red-500 to-rose-600 flex items-center justify-center">
                    <span class="font-display text-2xl font-black tracking-tighter">MF</span>
                </div>
                <div>
                    <span class="font-display text-3xl font-bold tracking-tighter">MICHAEL</span>
                </div>
            </div>
            
            <div class="hidden md:flex items-center gap-x-10 text-sm font-medium tracking-widest uppercase">
                <a href="#about" class="hover:text-red-400 transition-colors">About</a>
                <a href="#hubs" class="hover:text-red-400 transition-colors">Hubs</a>
                <a href="#live" class="hover:text-red-400 transition-colors">Live</a>
            </div>
            
            <div class="flex items-center gap-x-4">
                <a href="https://x.com/freedomfighter_news" target="_blank" 
                   class="px-5 py-2.5 text-sm font-semibold border border-zinc-700 hover:border-zinc-500 rounded-3xl flex items-center gap-x-2 transition-all hover:bg-zinc-900">
                    <i class="fa-brands fa-x-twitter"></i>
                    <span class="hidden sm:inline">X</span>
                </a>
                <button onclick="copyLink()" 
                        class="px-6 py-2.5 bg-white text-zinc-950 text-sm font-bold rounded-3xl flex items-center gap-x-2 hover:bg-zinc-100 active:scale-[0.985] transition-all">
                    <i class="fa-solid fa-link"></i>
                    <span>Copy Link</span>
                </button>
            </div>
        </div>
    </nav>

    <!-- HERO -->
    <div class="pt-20 min-h-[95vh] flex items-center hero-bg relative">
        <div class="max-w-5xl mx-auto px-6 md:px-8 pt-12 md:pt-0">
            <div class="grid md:grid-cols-12 gap-12 items-center">
                <!-- Text -->
                <div class="md:col-span-7 space-y-8">
                    <div class="inline-flex items-center gap-x-2 px-4 py-1.5 rounded-3xl border border-zinc-800 text-sm tracking-[2px] uppercase font-medium text-zinc-400">
                        <div class="w-2 h-2 bg-emerald-500 rounded-full animate-pulse"></div>
                        NOW LIVE ON TIKTOK
                    </div>
                    
                    <div>
                        <h1 class="font-display text-7xl md:text-8xl font-black tracking-tighter leading-none">
                            MICHAEL
                        </h1>
                        <p class="mt-4 text-3xl md:text-4xl font-medium text-zinc-300 tracking-tight">
                            25 • Intellectual • Unfiltered
                        </p>
                    </div>
                    
                    <p class="max-w-md text-xl text-zinc-400 leading-snug">
                        Intellectual pushback on trends, politics, and modern madness.<br>
                        No sacred cows. Comfort isn't the goal.
                    </p>
                    
                    <div class="flex flex-wrap gap-4 pt-4">
                        <a href="https://tiktok.com/@freedomfighter_news" target="_blank"
                           class="px-10 py-4 bg-red-500 hover:bg-red-600 active:bg-red-700 text-white font-bold rounded-3xl flex items-center justify-center gap-x-3 text-lg shadow-xl shadow-red-950/50 transition-all">
                            <i class="fa-brands fa-tiktok text-2xl"></i>
                            <span>Watch on TikTok</span>
                        </a>
                        
                        <a href="#hubs"
                           class="px-9 py-4 border border-zinc-700 hover:bg-zinc-900 text-lg font-semibold rounded-3xl flex items-center justify-center gap-x-2 transition-all">
                            Explore everything
                        </a>
                    </div>
                    
                    <div class="flex items-center gap-x-4 text-sm pt-3">
                        <div class="flex -space-x-2">
                            <div class="w-7 h-7 bg-zinc-700 rounded-full ring-2 ring-zinc-950 overflow-hidden"><img src="https://picsum.photos/id/64/28/28" class="object-cover"></div>
                            <div class="w-7 h-7 bg-zinc-700 rounded-full ring-2 ring-zinc-950 overflow-hidden"><img src="https://picsum.photos/id/65/28/28" class="object-cover"></div>
                            <div class="w-7 h-7 bg-zinc-700 rounded-full ring-2 ring-zinc-950 overflow-hidden"><img src="https://picsum.photos/id/66/28/28" class="object-cover"></div>
                        </div>
                        <span class="text-zinc-500 text-sm">Joined by <span class="font-semibold text-white">142k</span> truth-seekers this month</span>
                    </div>
                </div>
                
                <!-- Profile Image -->
                <div class="md:col-span-5 relative flex justify-center md:justify-end">
                    <div class="relative">
                        <div class="w-80 h-80 md:w-96 md:h-96 rounded-[3.5rem] overflow-hidden border-[12px] border-zinc-900 shadow-2xl shadow-black/70">
                            <img src="https://picsum.photos/id/1005/600/600" alt="Michael - 25-year-old intellectual delivering pushback on culture, politics, and modern madness" 
                                 class="w-full h-full object-cover grayscale-[0.15]">
                        </div>
                        <!-- Status badge -->
                        <div class="absolute -bottom-3 -right-3 bg-zinc-900 border border-zinc-700 px-5 py-2 rounded-3xl flex items-center gap-x-2 shadow-xl">
                            <div class="flex items-center gap-x-1.5">
                                <i class="fa-solid fa-microphone text-red-500"></i>
                                <span class="font-mono text-xs tracking-[1px] font-bold">LIVE IN 3H</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        
        <!-- Scroll indicator -->
        <div class="absolute bottom-12 left-1/2 hidden md:block">
            <div class="flex flex-col items-center text-xs tracking-[2px] text-zinc-500">
                SCROLL TO ENTER THE DISCOURSE
                <i class="fa-solid fa-chevron-down mt-1 animate-bounce"></i>
            </div>
        </div>
    </div>

    <!-- ABOUT -->
    <div id="about" class="max-w-4xl mx-auto px-6 py-24 border-b border-zinc-800">
        <div class="max-w-2xl">
            <div class="uppercase tracking-[3px] text-xs font-bold text-red-500 mb-4">THE MAN BEHIND THE MIC</div>
            
            <h2 class="section-header leading-none mb-8">Intellectual pushback.<br>No filters. No comfort.</h2>
            
            <div class="space-y-6 text-lg text-zinc-300 leading-relaxed">
                <p>I'm Michael — 25 years old, here for intellectual pushback on trends, politics, and modern madness. No sacred cows. Comfort isn't the goal. I call things as I see them because someone has to <span class="font-semibold text-white">wake up</span> to what's actually happening in culture, politics, and the institutions that shape your life.</p>
            </div>
            
            <!-- Stats removed per request - growing organically -->
        </div>
    </div>

    <!-- THE HUBS -->
    <div id="hubs" class="max-w-7xl mx-auto px-6 py-20">
        <div class="text-center mb-14">
            <div class="inline px-4 py-1 rounded-full border border-zinc-800 text-xs tracking-[2.5px] font-medium">PICK YOUR BATTLEFIELD</div>
            <h2 class="section-header mt-4">Where the real work happens</h2>
            <p class="mt-3 max-w-md mx-auto text-zinc-400">Short-form fire. Long-form depth. Visual proof. All in one place.</p>
        </div>
        
        <div class="grid md:grid-cols-3 gap-6">
            
            <!-- TikTok Card -->
            <div class="content-card group bg-zinc-900 border border-zinc-800 hover:border-red-500/70 rounded-3xl p-8 flex flex-col h-full">
                <div class="flex-1">
                    <div class="w-16 h-16 flex items-center justify-center text-6xl mb-8 group-hover:scale-110 transition-transform">🎥</div>
                    
                    <h3 class="font-display text-4xl font-bold tracking-tighter">TikTok</h3>
                    <p class="text-red-500 text-sm font-bold tracking-widest mt-1">SHORTS + LIVE DEBATES</p>
                    
                    <div class="mt-8 space-y-4 text-sm">
                        <div class="flex items-start gap-x-3">
                            <i class="fa-solid fa-check text-red-500 mt-1"></i>
                            <span class="text-zinc-300">Daily 60-second cultural takedowns</span>
                        </div>
                        <div class="flex items-start gap-x-3">
                            <i class="fa-solid fa-check text-red-500 mt-1"></i>
                            <span class="text-zinc-300">Live debates every Monday &amp; Thursday 8PM EST</span>
                        </div>
                        <div class="flex items-start gap-x-3">
                            <i class="fa-solid fa-check text-red-500 mt-1"></i>
                            <span class="text-zinc-300">Zero filter. Maximum receipts.</span>
                        </div>
                    </div>
                </div>
                
                <a href="https://tiktok.com/@freedomfighter_news" target="_blank"
                   class="mt-10 block w-full text-center py-4 border border-red-500 text-red-500 hover:bg-red-500 hover:text-white font-bold rounded-3xl transition-all link-btn">
                    ENTER THE ARENA →
                </a>
            </div>
            
            <!-- Instagram Card -->
            <div class="content-card group bg-zinc-900 border border-zinc-800 hover:border-red-500/70 rounded-3xl p-8 flex flex-col h-full">
                <div class="flex-1">
                    <div class="w-16 h-16 flex items-center justify-center text-6xl mb-8 group-hover:scale-110 transition-transform">📸</div>
                    
                    <h3 class="font-display text-4xl font-bold tracking-tighter">Instagram</h3>
                    <p class="text-red-500 text-sm font-bold tracking-widest mt-1">VISUAL COMMENTARY</p>
                    
                    <div class="mt-8 space-y-4 text-sm">
                        <div class="flex items-start gap-x-3">
                            <i class="fa-solid fa-check text-red-500 mt-1"></i>
                            <span class="text-zinc-300">Cinematic breakdowns of trends</span>
                        </div>
                        <div class="flex items-start gap-x-3">
                            <i class="fa-solid fa-check text-red-500 mt-1"></i>
                            <span class="text-zinc-300">Behind-the-scenes of the discourse</span>
                        </div>
                        <div class="flex items-start gap-x-3">
                            <i class="fa-solid fa-check text-red-500 mt-1"></i>
                            <span class="text-zinc-300">Stories that actually move the needle</span>
                        </div>
                    </div>
                </div>
                
                <a href="https://instagram.com/marcusvoss" target="_blank"
                   class="mt-10 block w-full text-center py-4 border border-red-500 text-red-500 hover:bg-red-500 hover:text-white font-bold rounded-3xl transition-all link-btn">
                    FOLLOW THE FEED →
                </a>
            </div>
            
            <!-- Podcast Card -->
            <div class="content-card group bg-zinc-900 border border-zinc-800 hover:border-red-500/70 rounded-3xl p-8 flex flex-col h-full">
                <div class="flex-1">
                    <div class="w-16 h-16 flex items-center justify-center text-6xl mb-8 group-hover:scale-110 transition-transform">🎙️</div>
                    
                    <h3 class="font-display text-4xl font-bold tracking-tighter">The Clear Lens</h3>
                    <p class="text-red-500 text-sm font-bold tracking-widest mt-1">WEEKLY LONG-FORM</p>
                    
                    <div class="mt-8 space-y-4 text-sm">
                        <div class="flex items-start gap-x-3">
                            <i class="fa-solid fa-check text-red-500 mt-1"></i>
                            <span class="text-zinc-300">Deep dives into politics &amp; culture</span>
                        </div>
                        <div class="flex items-start gap-x-3">
                            <i class="fa-solid fa-check text-red-500 mt-1"></i>
                            <span class="text-zinc-300">Guest debates that actually matter</span>
                        </div>
                        <div class="flex items-start gap-x-3">
                            <i class="fa-solid fa-check text-red-500 mt-1"></i>
                            <span class="text-zinc-300">Available on all platforms</span>
                        </div>
                    </div>
                </div>
                
                <div class="mt-10 space-y-3">
                    <a href="https://open.spotify.com/show/EXAMPLE" target="_blank"
                       class="block w-full text-center py-[17px] bg-zinc-800 hover:bg-zinc-700 font-bold rounded-3xl transition-all text-sm flex items-center justify-center gap-x-2 link-btn">
                        <i class="fa-brands fa-spotify"></i>
                        <span>SPOTIFY</span>
                    </a>
                    <div class="grid grid-cols-2 gap-3">
                        <a href="https://podcasts.apple.com/EXAMPLE" target="_blank"
                           class="block text-center py-3 border border-zinc-700 hover:bg-zinc-900 text-sm font-semibold rounded-3xl transition-all link-btn">Apple</a>
                        <a href="https://youtube.com/@freedomfighter_news" target="_blank"
                           class="block text-center py-3 border border-zinc-700 hover:bg-zinc-900 text-sm font-semibold rounded-3xl transition-all link-btn">YouTube</a>
                    </div>
                </div>
            </div>
            
        </div>
    </div>

    <!-- LIVE / CTA -->
    <div id="live" class="bg-zinc-900 py-20 border-y border-zinc-800">
        <div class="max-w-3xl mx-auto px-6 text-center">
            <div class="mx-auto w-20 h-20 rounded-2xl bg-red-500/10 flex items-center justify-center mb-8">
                <i class="fa-solid fa-broadcast-tower text-5xl text-red-500"></i>
            </div>
            
            <h2 class="font-display text-5xl font-bold tracking-tighter">The discourse doesn't wait.</h2>
            <p class="mt-4 text-xl text-zinc-400 max-w-md mx-auto">Catch me live on TikTok where I take on the hottest topics — and anyone brave enough to join.</p>
            
            <div class="mt-10 flex flex-col sm:flex-row gap-4 justify-center">
                <a href="https://tiktok.com/@freedomfighter_news/live" target="_blank"
                   class="px-14 py-4 bg-white text-zinc-950 font-extrabold text-lg rounded-3xl flex items-center justify-center gap-x-3 hover:bg-zinc-100 active:scale-[0.985]">
                    <span>JOIN THE NEXT LIVE</span>
                    <i class="fa-solid fa-arrow-right"></i>
                </a>
                
                <button onclick="showSchedule()"
                        class="px-10 py-4 border border-zinc-700 hover:bg-zinc-800 font-bold rounded-3xl text-lg flex items-center justify-center gap-x-2">
                    VIEW FULL SCHEDULE
                </button>
            </div>
            
            <p class="text-xs text-zinc-500 mt-8 tracking-widest">MONDAYS &amp; THURSDAYS • 8PM EST • NO HOLDS BARRED</p>
        </div>
    </div>

    <!-- FINAL CTA -->
    <div class="max-w-2xl mx-auto px-6 py-24 text-center">
        <div class="text-sm uppercase tracking-[2.5px] text-red-500 font-bold mb-3">ONE MORE THING</div>
        
        <h3 class="font-display text-5xl tracking-tighter font-bold leading-none mb-6">Stop consuming.<br>Start thinking.</h3>
        
        <p class="text-xl text-zinc-400 max-w-sm mx-auto">The algorithm wants you passive. Comfort isn't the goal.</p>
        
        <div class="mt-10">
            <a href="#" onclick="subscribeNewsletter(); return false"
               class="inline-flex items-center justify-center gap-x-3 px-12 py-5 border border-white text-lg font-bold rounded-3xl hover:bg-white hover:text-zinc-950 transition-all active:scale-[0.985]">
                <span>JOIN THE INNER CIRCLE</span>
                <i class="fa-solid fa-envelope"></i>
            </a>
        </div>
        
        <p class="text-[10px] text-zinc-500 mt-4">Weekly private briefings. No fluff. No noise.</p>
    </div>

    <!-- FOOTER -->
    <footer class="border-t border-zinc-800 bg-black py-12">
        <div class="max-w-7xl mx-auto px-8 text-sm">
            <div class="flex flex-col md:flex-row md:items-center justify-between gap-y-6">
                <div class="text-zinc-500">
                    © 2026 Michael. All rights reserved.<br>
                    <span class="text-xs">Built for those who still believe in reason.</span>
                </div>
                
                <div class="flex flex-wrap gap-x-6 gap-y-2 text-xs uppercase tracking-widest text-zinc-400">
                    <a href="#" class="hover:text-white">Privacy</a>
                    <a href="#" class="hover:text-white">Terms</a>
                    <a href="mailto:hello@freedomfighter_news.com" class="hover:text-white">Contact</a>
                    <a href="#" class="hover:text-white">Press Kit</a>
                </div>
                
                <div class="text-xs text-zinc-500 md:text-right">
                    Not affiliated with any party.<br>
                    Just aligned with reality.
                </div>
            </div>
        </div>
    </footer>

    <!-- Toast for copy -->
    <div id="toast" class="hidden fixed bottom-8 left-1/2 -translate-x-1/2 bg-zinc-800 border border-zinc-700 text-sm px-6 py-3 rounded-3xl flex items-center gap-x-2 shadow-2xl">
        <i class="fa-solid fa-check text-emerald-400"></i>
        <span>Link copied to clipboard</span>
    </div>

    <script>
        // Tailwind script
        function initializeTailwind() {
            document.documentElement.style.setProperty('--accent', '#ef4444');
        }
        
        function copyLink() {
            const link = window.location.href;
            navigator.clipboard.writeText(link).then(() => {
                const toast = document.getElementById('toast');
                toast.style.display = 'flex';
                toast.classList.remove('hidden');
                
                setTimeout(() => {
                    toast.style.transition = 'all 0.3s ease';
                    toast.style.opacity = '0';
                    
                    setTimeout(() => {
                        toast.style.display = 'none';
                        toast.style.opacity = '1';
                        toast.style.transition = '';
                    }, 300);
                }, 2200);
            });
        }
        
        function showSchedule() {
            const modal = document.createElement('div');
            modal.className = 'fixed inset-0 bg-black/90 z-[100] flex items-center justify-center p-6';
            modal.innerHTML = `
                <div class="bg-zinc-900 border border-zinc-700 rounded-3xl max-w-md w-full p-8 relative">
                    <button onclick="this.closest('.fixed').remove()" class="absolute top-6 right-6 text-zinc-400 hover:text-white">
                        <i class="fa-solid fa-times text-2xl"></i>
                    </button>
                    
                    <div class="text-center">
                        <i class="fa-solid fa-calendar text-red-500 text-5xl mb-6"></i>
                        <h3 class="font-display text-3xl font-bold tracking-tight">Live Schedule</h3>
                        <p class="text-sm text-zinc-400 mt-1">All times Eastern Standard</p>
                    </div>
                    
                    <div class="mt-8 space-y-5 text-sm">
                        <div class="flex justify-between items-center border-b border-zinc-800 pb-4">
                            <div>
                                <div class="font-semibold">Every Monday • 8:00 PM</div>
                                <div class="text-xs text-zinc-500">Deep-dive episode preview &amp; Q&amp;A</div>
                            </div>
                            <div class="px-4 py-1 bg-red-500 text-xs font-bold rounded-2xl">LIVE</div>
                        </div>
                        <div class="flex justify-between items-center">
                            <div>
                                <div class="font-semibold">Every Thursday • 8:00 PM</div>
                                <div class="text-xs text-zinc-500">Open Debate Night — Bring your best arguments</div>
                            </div>
                            <div class="text-emerald-400 text-xs font-bold">RECURRING</div>
                        </div>
                    </div>
                    
                    <div class="mt-8 pt-6 border-t border-zinc-800 text-center">
                        <p class="text-xs text-zinc-500">Set a reminder in your calendar.<br>Or just show up. I'll be there.</p>
                    </div>
                </div>
            `;
            document.body.appendChild(modal);
        }
        
        function subscribeNewsletter() {
            const modal = document.createElement('div');
            modal.className = 'fixed inset-0 bg-black/90 z-[100] flex items-center justify-center p-6';
            modal.innerHTML = `
                <div class="bg-zinc-900 border border-zinc-700 rounded-3xl max-w-sm w-full p-8">
                    <div class="text-center">
                        <i class="fa-solid fa-envelope-open text-red-500 text-5xl mb-5"></i>
                        <h4 class="font-display text-3xl font-bold tracking-tighter">The Inner Circle</h4>
                        <p class="text-sm text-zinc-400 mt-2">Private weekly briefings. Zero corporate media. Pure signal.</p>
                    </div>
                    
                    <div class="mt-8">
                        <input type="email" id="email-input" placeholder="your@email.com" 
                               class="w-full bg-zinc-800 border border-zinc-700 focus:border-red-500 rounded-3xl px-6 py-4 text-sm outline-none placeholder:text-zinc-500">
                        
                        <button onclick="submitNewsletter(this)" 
                                class="mt-3 w-full py-4 bg-red-500 hover:bg-red-600 active:bg-red-700 text-white font-extrabold rounded-3xl text-sm tracking-wider transition-all">
                            SUBSCRIBE — FREE
                        </button>
                        
                        <p class="text-center text-[10px] text-zinc-500 mt-4">We respect your inbox like we respect truth. Unsubscribe anytime.</p>
                    </div>
                </div>
            `;
            document.body.appendChild(modal);
            
            // Focus email
            setTimeout(() => {
                const input = document.getElementById('email-input');
                if (input) input.focus();
            }, 400);
        }
        
        function submitNewsletter(btn) {
            const input = document.getElementById('email-input');
            if (!input || !input.value.trim()) {
                input.style.borderColor = '#ef4444';
                setTimeout(() => input.style.borderColor = '', 1200);
                return;
            }
            
            btn.innerHTML = '<i class="fa-solid fa-check mr-2"></i> YOU\'RE IN';
            btn.style.background = '#16a34a';
            btn.disabled = true;
            
            setTimeout(() => {
                const modal = btn.closest('.fixed');
                if (modal) modal.remove();
                
                // Success toast
                const toast = document.createElement('div');
                toast.className = 'fixed bottom-8 left-1/2 -translate-x-1/2 bg-emerald-900 border border-emerald-700 text-emerald-300 px-8 py-4 rounded-3xl flex items-center gap-x-3 shadow-xl text-sm';
                toast.innerHTML = `
                    <i class="fa-solid fa-check-double"></i> 
                    <span>Welcome to the circle. First briefing drops Sunday.</span>
                `;
                document.body.appendChild(toast);
                
                setTimeout(() => {
                    toast.style.transition = 'all .4s ease';
                    toast.style.opacity = '0';
                    setTimeout(() => toast.remove(), 400);
                }, 2800);
            }, 1450);
        }
        
        // Keyboard shortcuts
        function setupKeyboard() {
            document.addEventListener('keydown', function(e) {
                if (e.key === '/' && document.activeElement.tagName === 'BODY') {
                    e.preventDefault();
                    const hubs = document.getElementById('hubs');
                    if (hubs) hubs.scrollIntoView({ behavior: 'smooth', block: 'start' });
                }
                
                if (e.metaKey && e.key === 'k') {
                    e.preventDefault();
                    copyLink();
                }
            });
            
            // Easter egg - konami code for fun
            let konami = '';
            document.addEventListener('keydown', function(e) {
                konami += e.key;
                if (konami.length > 10) konami = konami.slice(-10);
                if (konami.includes('ArrowUpArrowUpArrowDownArrowDownArrowLeftArrowRightArrowLeftArrowRightba')) {
                    const hero = document.querySelector('.hero-bg');
                    if (hero) {
                        hero.style.transition = 'all 1.2s cubic-bezier(0.23,1,0.32,1)';
                        hero.style.filter = 'hue-rotate(25deg) saturate(1.6)';
                        setTimeout(() => {
                            if (hero) hero.style.filter = '';
                        }, 2400);
                    }
                    konami = '';
                }
            });
        }
        
        // Boot everything
        function init() {
            initializeTailwind();
            setupKeyboard();
            
            // Smooth scroll for nav links
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function(e) {
                    const target = document.querySelector(this.getAttribute('href'));
                    if (target) {
                        e.preventDefault();
                        target.scrollIntoView({ behavior: 'smooth', block: 'start' });
                    }
                });
            });
            
            // Subtle entrance animation for cards
            const cards = document.querySelectorAll('.content-card');
            cards.forEach((card, i) => {
                card.style.opacity = '0';
                card.style.transform = 'translateY(30px)';
                setTimeout(() => {
                    card.style.transition = 'all 0.6s cubic-bezier(0.23, 1, 0.32, 1)';
                    card.style.transitionDelay = (i * 80) + 'ms';
                    card.style.opacity = '1';
                    card.style.transform = 'translateY(0)';
                }, 400);
            });
            
            // Console message for the curious
            console.log('%c[Marcus Voss] Bio hub initialized. Reality > narrative.', 'color:#3f3f46; font-size:9px');
        }
        
        window.onload = init;
    </script>
</body>
</html>
