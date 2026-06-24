<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>InternForge • AI Internship Program</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&amp;family=Space+Grotesk:wght@500;600;700&display=swap');
        
        :root {
            --primary: 59 130 246;
        }
        
        body {
            font-family: 'Inter', system-ui, sans-serif;
        }
        
        .heading-font {
            font-family: 'Space Grotesk', sans-serif;
        }

        .hero-bg {
            background: linear-gradient(135deg, #0f172a 0%, #1e2937 100%);
        }

        .card-hover {
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }
        
        .card-hover:hover {
            transform: translateY(-8px);
            box-shadow: 0 20px 25px -5px rgb(0 0 0 / 0.1), 0 8px 10px -6px rgb(0 0 0 / 0.1);
        }

        .nav-link {
            position: relative;
        }
        
        .nav-link:after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -2px;
            left: 0;
            background-color: rgb(59 130 246);
            transition: width 0.3s ease;
        }
        
        .nav-link:hover:after {
            width: 100%;
        }

        .timeline-dot {
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.6; }
        }
    </style>
</head>
<body class="bg-zinc-950 text-zinc-100">
    <!-- NAVBAR -->
    <nav class="bg-zinc-900 border-b border-zinc-800 sticky top-0 z-50">
        <div class="max-w-7xl mx-auto px-6 py-5 flex items-center justify-between">
            <div class="flex items-center gap-3">
                <div class="w-9 h-9 bg-blue-600 rounded-2xl flex items-center justify-center text-white font-bold text-2xl">IF</div>
                <div>
                    <span class="heading-font text-2xl font-semibold tracking-tighter">InternForge</span>
                </div>
            </div>
            
            <div class="hidden md:flex items-center gap-8 text-sm font-medium">
                <a href="#home" onclick="navigateToSection('home')" class="nav-link text-zinc-300 hover:text-white">Home</a>
                <a href="#program" onclick="navigateToSection('program')" class="nav-link text-zinc-300 hover:text-white">Program</a>
                <a href="#benefits" onclick="navigateToSection('benefits')" class="nav-link text-zinc-300 hover:text-white">Benefits</a>
                <a href="#stories" onclick="navigateToSection('stories')" class="nav-link text-zinc-300 hover:text-white">Stories</a>
                <a href="#enroll" onclick="navigateToSection('enroll')" class="nav-link text-zinc-300 hover:text-white">Enroll</a>
                <a href="#records" onclick="navigateToSection('records')" class="nav-link text-zinc-300 hover:text-white">Records</a>
            </div>
            
            <div class="flex items-center gap-4">
                <div class="bg-emerald-500 text-emerald-950 text-xs font-semibold px-3 py-1.5 rounded-full flex items-center gap-1">
                    <div class="w-2 h-2 bg-emerald-950 rounded-full animate-pulse"></div>
                    OPEN
                </div>
                <button onclick="navigateToSection('enroll')" 
                        class="bg-white text-zinc-900 hover:bg-zinc-100 px-5 py-2.5 rounded-2xl font-semibold text-sm transition-all active:scale-95">
                    Apply Now
                </button>
            </div>
        </div>
    </nav>

    <!-- HERO -->
    <section id="home" class="hero-bg pt-24 pb-20">
        <div class="max-w-5xl mx-auto px-6 text-center">
            <div class="inline-flex items-center gap-2 bg-zinc-800 border border-zinc-700 rounded-full px-4 py-2 text-sm mb-6">
                <span class="text-amber-400">✦</span>
                Summer 2026 Cohort
            </div>
            
            <h1 class="heading-font text-6xl md:text-7xl font-bold tracking-tighter leading-none mb-6">
                Build the Future.<br>
                <span class="bg-gradient-to-r from-blue-400 to-violet-400 bg-clip-text text-transparent">Master AI.</span>
            </h1>
            
            <p class="max-w-2xl mx-auto text-xl text-zinc-400 mb-10">
                12-week intensive AI &amp; Machine Learning internship. Real projects, expert mentorship, and a pathway to full-time roles.
            </p>
            
            <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
                <button onclick="navigateToSection('enroll')" 
                        class="bg-blue-600 hover:bg-blue-500 px-10 py-4 rounded-3xl font-semibold text-lg flex items-center gap-3 transition-all">
                    <i class="fas fa-rocket"></i>
                    Join the Program
                </button>
                <button onclick="navigateToSection('program')" 
                        class="border border-zinc-700 hover:bg-zinc-900 px-8 py-4 rounded-3xl font-medium text-lg transition-all">
                    Learn More
                </button>
            </div>
            
            <div class="mt-16 flex justify-center gap-12 text-sm">
                <div class="text-center">
                    <div class="text-3xl font-semibold text-emerald-400">June 15</div>
                    <div class="text-zinc-500">Start Date</div>
                </div>
                <div class="h-12 w-px bg-zinc-800"></div>
                <div class="text-center">
                    <div class="text-3xl font-semibold text-emerald-400">Sep 7</div>
                    <div class="text-zinc-500">End Date</div>
                </div>
                <div class="h-12 w-px bg-zinc-800"></div>
                <div class="text-center">
                    <div class="text-3xl font-semibold">12</div>
                    <div class="text-zinc-500">Weeks</div>
                </div>
            </div>
        </div>
    </section>

    <!-- PROGRAM DETAILS -->
    <section id="program" class="py-20 bg-zinc-950">
        <div class="max-w-6xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="heading-font text-5xl font-semibold tracking-tight mb-4">What the Internship Looks Like</h2>
                <p class="text-zinc-400 max-w-md mx-auto">Hands-on experience with cutting-edge AI technologies and real-world problem solving.</p>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8">
                <!-- Week Structure -->
                <div class="bg-zinc-900 border border-zinc-800 rounded-3xl p-8 card-hover">
                    <div class="w-12 h-12 bg-blue-500/10 rounded-2xl flex items-center justify-center text-blue-400 mb-6">
                        <i class="fas fa-calendar-alt text-2xl"></i>
                    </div>
                    <h3 class="text-2xl font-semibold mb-3">Program Timeline</h3>
                    <ul class="space-y-6 text-zinc-400">
                        <li class="flex gap-4">
                            <span class="text-emerald-400 font-mono">W1-3</span>
                            <div>Foundations of ML &amp; Python</div>
                        </li>
                        <li class="flex gap-4">
                            <span class="text-emerald-400 font-mono">W4-6</span>
                            <div>Deep Learning &amp; Neural Networks</div>
                        </li>
                        <li class="flex gap-4">
                            <span class="text-emerald-400 font-mono">W7-9</span>
                            <div>LLM Engineering &amp; RAG Systems</div>
                        </li>
                        <li class="flex gap-4">
                            <span class="text-emerald-400 font-mono">W10-12</span>
                            <div>Capstone Project + Portfolio</div>
                        </li>
                    </ul>
                </div>
                
                <!-- Activities -->
                <div class="bg-zinc-900 border border-zinc-800 rounded-3xl p-8 card-hover">
                    <div class="w-12 h-12 bg-violet-500/10 rounded-2xl flex items-center justify-center text-violet-400 mb-6">
                        <i class="fas fa-tools text-2xl"></i>
                    </div>
                    <h3 class="text-2xl font-semibold mb-3">What You'll Do</h3>
                    <div class="space-y-5">
                        <div class="flex items-start gap-4">
                            <i class="fas fa-brain text-amber-400 mt-1"></i>
                            <div>Train and fine-tune large language models</div>
                        </div>
                        <div class="flex items-start gap-4">
                            <i class="fas fa-chart-line text-amber-400 mt-1"></i>
                            <div>Build production-ready AI applications</div>
                        </div>
                        <div class="flex items-start gap-4">
                            <i class="fas fa-users text-amber-400 mt-1"></i>
                            <div>Collaborate with senior engineers</div>
                        </div>
                        <div class="flex items-start gap-4">
                            <i class="fas fa-laptop-code text-amber-400 mt-1"></i>
                            <div>Weekly code reviews &amp; tech talks</div>
                        </div>
                    </div>
                </div>
                
                <!-- Perks -->
                <div class="bg-zinc-900 border border-zinc-800 rounded-3xl p-8 card-hover">
                    <div class="w-12 h-12 bg-emerald-500/10 rounded-2xl flex items-center justify-center text-emerald-400 mb-6">
                        <i class="fas fa-gift text-2xl"></i>
                    </div>
                    <h3 class="text-2xl font-semibold mb-3">Perks &amp; Support</h3>
                    <ul class="space-y-4">
                        <li class="flex items-center gap-3">
                            <i class="fas fa-check text-emerald-400"></i>
                            <span>Stipend: $2,500 / month</span>
                        </li>
                        <li class="flex items-center gap-3">
                            <i class="fas fa-check text-emerald-400"></i>
                            <span>Remote-friendly (hybrid option)</span>
                        </li>
                        <li class="flex items-center gap-3">
                            <i class="fas fa-check text-emerald-400"></i>
                            <span>Laptop + tools provided</span>
                        </li>
                        <li class="flex items-center gap-3">
                            <i class="fas fa-check text-emerald-400"></i>
                            <span>Certificate + LinkedIn recommendation</span>
                        </li>
                        <li class="flex items-center gap-3">
                            <i class="fas fa-check text-emerald-400"></i>
                            <span>Full-time conversion opportunity</span>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- BENEFITS -->
    <section id="benefits" class="py-20 bg-zinc-900">
        <div class="max-w-6xl mx-auto px-6">
            <div class="grid md:grid-cols-2 gap-16 items-center">
                <div>
                    <h2 class="heading-font text-5xl font-semibold tracking-tight mb-8">What You'll Gain</h2>
                    
                    <div class="space-y-8">
                        <div class="flex gap-6">
                            <div class="flex-shrink-0 w-12 h-12 bg-blue-600/10 rounded-2xl flex items-center justify-center text-3xl">🚀</div>
                            <div>
                                <h4 class="text-xl font-semibold mb-2">Industry-Ready Skills</h4>
                                <p class="text-zinc-400">Master modern AI stack: PyTorch, LangChain, vector databases, and deployment pipelines.</p>
                            </div>
                        </div>
                        
                        <div class="flex gap-6">
                            <div class="flex-shrink-0 w-12 h-12 bg-blue-600/10 rounded-2xl flex items-center justify-center text-3xl">👥</div>
                            <div>
                                <h4 class="text-xl font-semibold mb-2">Strong Network</h4>
                                <p class="text-zinc-400">Connect with mentors from top AI labs and fellow passionate builders.</p>
                            </div>
                        </div>
                        
                        <div class="flex gap-6">
                            <div class="flex-shrink-0 w-12 h-12 bg-blue-600/10 rounded-2xl flex items-center justify-center text-3xl">📂</div>
                            <div>
                                <h4 class="text-xl font-semibold mb-2">Portfolio That Stands Out</h4>
                                <p class="text-zinc-400">Ship 3+ production-grade projects that you can showcase to recruiters.</p>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="bg-zinc-950 border border-zinc-800 rounded-3xl p-10">
                    <div class="text-emerald-400 text-sm font-medium mb-2 flex items-center gap-2">
                        <span>100% FREE</span> 
                        <span class="flex-1 h-px bg-gradient-to-r from-emerald-400/30 to-transparent"></span>
                    </div>
                    <h3 class="text-4xl font-semibold heading-font mb-8">Completely Free to Join</h3>
                    <p class="text-zinc-400 mb-8">No hidden fees. We believe talent should never be limited by finances. The only requirement is passion and commitment.</p>
                    
                    <div class="grid grid-cols-2 gap-6 text-sm">
                        <div class="bg-zinc-900 p-4 rounded-2xl">
                            <span class="block text-zinc-500">Application fee</span>
                            <span class="text-3xl font-semibold text-emerald-400">FREE</span>
                        </div>
                        <div class="bg-zinc-900 p-4 rounded-2xl">
                            <span class="block text-zinc-500">Program fee</span>
                            <span class="text-3xl font-semibold text-emerald-400">FREE</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- TESTIMONIALS -->
    <section id="stories" class="py-20 bg-zinc-950">
        <div class="max-w-6xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="heading-font text-5xl font-semibold tracking-tight">Previous Interns</h2>
                <p class="text-zinc-400 mt-3">Real stories from our alumni</p>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8">
                <!-- Testimonial 1 -->
                <div class="bg-zinc-900 border border-zinc-800 rounded-3xl p-8 card-hover">
                    <div class="flex items-center gap-4 mb-8">
                        <div class="w-12 h-12 bg-gradient-to-br from-pink-400 to-rose-400 rounded-2xl"></div>
                        <div>
                            <div class="font-semibold">Priya Sharma</div>
                            <div class="text-xs text-zinc-500">SDE @ Google • Batch '25</div>
                        </div>
                    </div>
                    <p class="text-zinc-300 italic">"The capstone project I built during the internship got me multiple interview calls. I joined Google directly after the program. Best decision of my college life."</p>
                </div>
                
                <!-- Testimonial 2 -->
                <div class="bg-zinc-900 border border-zinc-800 rounded-3xl p-8 card-hover">
                    <div class="flex items-center gap-4 mb-8">
                        <div class="w-12 h-12 bg-gradient-to-br from-cyan-400 to-blue-400 rounded-2xl"></div>
                        <div>
                            <div class="font-semibold">Rahul Verma</div>
                            <div class="text-xs text-zinc-500">AI Engineer @ OpenAI • Batch '25</div>
                        </div>
                    </div>
                    <p class="text-zinc-300 italic">"Working on real LLM infrastructure problems changed how I think about AI. The mentorship was world-class. I published my first research paper from this program."</p>
                </div>
                
                <!-- Testimonial 3 -->
                <div class="bg-zinc-900 border border-zinc-800 rounded-3xl p-8 card-hover">
                    <div class="flex items-center gap-4 mb-8">
                        <div class="w-12 h-12 bg-gradient-to-br from-amber-400 to-orange-400 rounded-2xl"></div>
                        <div>
                            <div class="font-semibold">Ayesha Khan</div>
                            <div class="text-xs text-zinc-500">Founding Engineer @ Perplexity • Batch '24</div>
                        </div>
                    </div>
                    <p class="text-zinc-300 italic">"InternForge helped me go from a confused CS sophomore to someone who shipped AI features used by millions. Highly recommended!"</p>
                </div>
            </div>
        </div>
    </section>

    <!-- ENROLLMENT FORM -->
    <section id="enroll" class="py-20 bg-zinc-900">
        <div class="max-w-2xl mx-auto px-6">
            <div class="bg-zinc-950 border border-zinc-800 rounded-3xl p-10">
                <h2 class="heading-font text-4xl font-semibold text-center mb-8">Apply for Summer 2026</h2>
                
                <form id="enrollForm" onsubmit="handleEnroll(event)" class="space-y-6">
                    <div class="grid grid-cols-2 gap-6">
                        <div>
                            <label class="block text-sm text-zinc-400 mb-2">Full Name</label>
                            <input type="text" id="name" required
                                   class="w-full bg-zinc-900 border border-zinc-700 rounded-2xl px-5 py-4 focus:outline-none focus:border-blue-600 transition-colors">
                        </div>
                        <div>
                            <label class="block text-sm text-zinc-400 mb-2">Email</label>
                            <input type="email" id="email" required
                                   class="w-full bg-zinc-900 border border-zinc-700 rounded-2xl px-5 py-4 focus:outline-none focus:border-blue-600 transition-colors">
                        </div>
                    </div>
                    
                    <div>
                        <label class="block text-sm text-zinc-400 mb-2">University / College</label>
                        <input type="text" id="college" required
                               class="w-full bg-zinc-900 border border-zinc-700 rounded-2xl px-5 py-4 focus:outline-none focus:border-blue-600 transition-colors">
                    </div>
                    
                    <div class="grid grid-cols-2 gap-6">
                        <div>
                            <label class="block text-sm text-zinc-400 mb-2">Year of Study</label>
                            <select id="year" required
                                    class="w-full bg-zinc-900 border border-zinc-700 rounded-2xl px-5 py-4 focus:outline-none focus:border-blue-600 transition-colors">
                                <option value="">Select</option>
                                <option value="1">1st Year</option>
                                <option value="2">2nd Year</option>
                                <option value="3">3rd Year</option>
                                <option value="4">4th Year</option>
                            </select>
                        </div>
                        <div>
                            <label class="block text-sm text-zinc-400 mb-2">Field of Study</label>
                            <input type="text" id="field" placeholder="Computer Science, AI, etc." required
                                   class="w-full bg-zinc-900 border border-zinc-700 rounded-2xl px-5 py-4 focus:outline-none focus:border-blue-600 transition-colors">
                        </div>
                    </div>
                    
                    <div>
                        <label class="block text-sm text-zinc-400 mb-2">Why do you want to join? (min 50 words)</label>
                        <textarea id="why" rows="4" required
                                  class="w-full bg-zinc-900 border border-zinc-700 rounded-3xl px-5 py-4 focus:outline-none focus:border-blue-600 transition-colors"></textarea>
                    </div>
                    
                    <button type="submit"
                            class="w-full bg-gradient-to-r from-blue-600 to-violet-600 hover:from-blue-500 hover:to-violet-500 py-5 rounded-3xl font-semibold text-lg transition-all active:scale-[0.985]">
                        Submit Application
                    </button>
                </form>
            </div>
        </div>
    </section>

    <!-- RECORDS / DASHBOARD -->
    <section id="records" class="py-20 bg-zinc-950">
        <div class="max-w-6xl mx-auto px-6">
            <div class="flex items-end justify-between mb-10">
                <div>
                    <h2 class="heading-font text-5xl font-semibold tracking-tight">Enrolled Students</h2>
                    <p class="text-zinc-400">Current cohort • <span id="count" class="font-mono text-emerald-400">0</span> students</p>
                </div>
                <button onclick="clearRecords()" 
                        class="text-red-400 hover:text-red-500 text-sm flex items-center gap-2">
                    <i class="fas fa-trash"></i> Clear All
                </button>
            </div>
            
            <div class="bg-zinc-900 border border-zinc-800 rounded-3xl overflow-hidden">
                <table class="w-full">
                    <thead>
                        <tr class="border-b border-zinc-800">
                            <th class="text-left py-5 px-8 font-medium text-zinc-400">Name</th>
                            <th class="text-left py-5 px-8 font-medium text-zinc-400">College</th>
                            <th class="text-left py-5 px-8 font-medium text-zinc-400">Field</th>
                            <th class="text-left py-5 px-8 font-medium text-zinc-400">Applied On</th>
                        </tr>
                    </thead>
                    <tbody id="recordsTable" class="divide-y divide-zinc-800 text-sm"></tbody>
                </table>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="bg-black py-16 border-t border-zinc-900">
        <div class="max-w-6xl mx-auto px-6 text-center text-zinc-500 text-sm">
            <div class="flex justify-center gap-8 mb-8">
                <a href="#" class="hover:text-zinc-300">Twitter</a>
                <a href="#" class="hover:text-zinc-300">LinkedIn</a>
                <a href="#" class="hover:text-zinc-300">Discord</a>
            </div>
            <p>&copy; 2026 InternForge. All rights reserved.</p>
            <p class="mt-2">Made with ❤️ for the next generation of AI builders</p>
        </div>
    </footer>

    <script>
        // Tailwind script already included via CDN
        
        function navigateToSection(section) {
            document.getElementById(section).scrollIntoView({ behavior: 'smooth' });
        }
        
        // Enrollment handling
        let enrolledStudents = JSON.parse(localStorage.getItem('internforge_students')) || [
            {
                name: "Anika Patel",
                email: "anika@example.edu",
                college: "IIT Bombay",
                year: "3",
                field: "Computer Science",
                date: "2026-06-20"
            },
            {
                name: "Vikram Singh",
                email: "vikram@nitk.edu",
                college: "NIT Karnataka",
                year: "4",
                field: "AI & ML",
                date: "2026-06-19"
            }
        ];
        
        function renderRecords() {
            const tbody = document.getElementById('recordsTable');
            tbody.innerHTML = '';
            
            enrolledStudents.forEach(student => {
                const row = document.createElement('tr');
                row.className = 'hover:bg-zinc-800 transition-colors';
                row.innerHTML = `
                    <td class="py-5 px-8 font-medium">${student.name}</td>
                    <td class="py-5 px-8 text-zinc-400">${student.college}</td>
                    <td class="py-5 px-8 text-zinc-400">${student.field}</td>
                    <td class="py-5 px-8 text-zinc-400 font-mono">${student.date}</td>
                `;
                tbody.appendChild(row);
            });
            
            document.getElementById('count').textContent = enrolledStudents.length;
        }
        
        function handleEnroll(e) {
            e.preventDefault();
            
            const name = document.getElementById('name').value;
            const email = document.getElementById('email').value;
            const college = document.getElementById('college').value;
            const field = document.getElementById('field').value;
            
            const newStudent = {
                name: name,
                email: email,
                college: college,
                year: document.getElementById('year').value,
                field: field,
                date: new Date().toISOString().split('T')[0]
            };
            
            enrolledStudents.unshift(newStudent);
            localStorage.setItem('internforge_students', JSON.stringify(enrolledStudents));
            
            // Reset form
            document.getElementById('enrollForm').reset();
            
            // Show success
            const btn = e.target.querySelector('button');
            const originalText = btn.innerHTML;
            btn.innerHTML = '✅ Application Received!';
            btn.style.background = '#10b981';
            
            setTimeout(() => {
                btn.innerHTML = originalText;
                btn.style.background = '';
                navigateToSection('records');
            }, 1800);
            
            renderRecords();
        }
        
        function clearRecords() {
            if (confirm('Clear all enrollment records?')) {
                enrolledStudents = [];
                localStorage.setItem('internforge_students', JSON.stringify(enrolledStudents));
                renderRecords();
            }
        }
        
        // Initialize
        window.onload = function() {
            renderRecords();
            
            // Keyboard shortcut hint
            console.log('%cInternForge ready 🚀\nPress "E" to quickly scroll to enrollment', 'color:#60a5fa; font-family:monospace');
            
            document.addEventListener('keydown', function(e) {
                if (e.key.toLowerCase() === 'e') {
                    navigateToSection('enroll');
                }
            });
        };
    </script>
</body>
</html>
