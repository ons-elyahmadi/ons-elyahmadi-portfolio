 <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Ons El Yahmadi - MLOps & ML Engineer Portfolio">
  <title>Ons El Yahmadi | MLOps &amp; ML Engineer</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css">
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&amp;family=Space+Grotesk:wght@500;600&amp;display=swap');
    
    :root {
      --cyan: #22d3ee;
    }
    
    .tail-container { font-family: 'Inter', system_ui, sans-serif; }
    .heading-font { font-family: 'Space Grotesk', sans-serif; }
    
    .hero-bg {
      background: linear-gradient(135deg, #0a0a0a 0%, #111827 100%);
    }
    
    .nav-link {
      position: relative;
      transition: all 0.3s ease;
    }
    .nav-link:after {
      content: '';
      position: absolute;
      width: 0;
      height: 2px;
      bottom: -2px;
      left: 0;
      background-color: #22d3ee;
      transition: all 0.3s ease;
    }
    .nav-link:hover:after { width: 100%; }
    
    .glow-cyan { text-shadow: 0 0 25px rgb(34 211 238); }
    .card-hover { transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1); }
    .card-hover:hover {
      transform: translateY(-6px);
      box-shadow: 0 25px 50px -12px rgb(34 211 238 / 0.25);
    }
    
    .project-filter.active {
      background-color: #22d3ee;
      color: #111827;
      box-shadow: 0 0 15px rgb(34 211 238);
    }
    
    .progress-bar {
      transition: width 1.5s ease-in-out;
    }
  </style>
</head>
<body class="tail-container bg-gray-950 text-white">

  <!-- NAVBAR -->
  <nav class="fixed top-0 w-full bg-gray-950/90 backdrop-blur-xl border-b border-gray-800 z-50">
    <div class="max-w-7xl mx-auto px-8 py-5 flex justify-between items-center">
      <div class="flex items-center gap-3">
        <div class="w-9 h-9 bg-cyan-400 rounded-2xl flex items-center justify-center text-gray-950 font-bold text-2xl">O</div>
        <h1 class="heading-font text-2xl tracking-tighter">Ons El Yahmadi</h1>
      </div>
      
      <div class="hidden md:flex items-center gap-10 text-sm font-medium">
        <a href="#about" class="nav-link">About</a>
        <a href="#experience" class="nav-link">Experience</a>
        <a href="#skills" class="nav-link">Skills</a>
        <a href="#projects" class="nav-link">Projects</a>
        <a href="#education" class="nav-link">Education</a>
        <a href="#contact" class="nav-link">Contact</a>
      </div>

      <a href="#" onclick="downloadCV()" 
         class="flex items-center gap-3 bg-cyan-400 hover:bg-cyan-300 text-gray-950 px-7 py-3 rounded-3xl font-semibold text-sm transition-all">
        <i class="fas fa-download"></i>
        <span>Download CV</span>
      </a>
    </div>
  </nav>

  <!-- HERO -->
  <section id="hero" class="hero-bg min-h-screen flex items-center pt-20">
    <div class="max-w-7xl mx-auto px-8 grid md:grid-cols-12 gap-12 items-center">
      <div class="md:col-span-7">
        <div class="inline-flex items-center gap-2 px-5 py-2 bg-gray-900 border border-cyan-400/30 rounded-3xl text-cyan-400 text-sm mb-6">
          <span class="relative flex h-3 w-3">
            <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-cyan-400 opacity-75"></span>
            <span class="relative inline-flex rounded-full h-3 w-3 bg-cyan-400"></span>
          </span>
          Available for opportunities • Tunis, Tunisia
        </div>
        
        <h1 class="heading-font text-7xl md:text-8xl leading-none font-semibold tracking-tighter mb-4">
          Ons El Yahmadi
        </h1>
        <p class="text-4xl text-cyan-400 mb-8">MLOps &amp; ML Engineer</p>
        
        <p class="max-w-2xl text-xl text-gray-300 leading-relaxed mb-10">
          Dynamic MLOps Engineer with expertise in deploying machine learning models, 
          building scalable AI solutions, and automating CI/CD pipelines.
        </p>
        
        <div class="flex flex-wrap gap-4">
          <a href="#projects" 
             class="flex items-center gap-3 bg-cyan-400 hover:bg-white text-gray-950 px-8 py-4 rounded-3xl font-semibold text-lg">
            View My Projects
            <i class="fas fa-arrow-right"></i>
          </a>
          
          <a href="https://www.linkedin.com/in/ons-elyahmadi" target="_blank"
             class="flex items-center gap-3 border-2 border-cyan-400 hover:bg-cyan-400/10 px-8 py-4 rounded-3xl font-semibold text-lg">
            <i class="fab fa-linkedin text-2xl"></i>
            LinkedIn
          </a>
          
          <a href="mailto:ons.elyahmadi@fsb.ucar.tn" 
             class="flex items-center gap-3 border border-gray-600 hover:border-cyan-400 px-8 py-4 rounded-3xl font-semibold text-lg">
            <i class="fas fa-envelope"></i>
            Get in touch
          </a>
        </div>
        
        <div class="mt-16 flex items-center gap-10 text-sm">
          <div class="flex items-center gap-3">
            <i class="fas fa-phone text-cyan-400"></i>
            <div>
              <p class="font-medium">+216 58 217 800</p>
            </div>
          </div>
          <div class="flex items-center gap-3">
            <i class="fas fa-envelope text-cyan-400"></i>
            <div>
              <p class="font-medium">ons.elyahmadi@fsb.ucar.tn</p>
            </div>
          </div>
          <div class="flex items-center gap-3">
            <i class="fas fa-map-marker-alt text-cyan-400"></i>
            <div>
              <p class="font-medium">Tunis, Tunisia</p>
            </div>
          </div>
        </div>
      </div>
      
      <!-- Profile Photo -->
      <div class="md:col-span-5 flex justify-center">
        <div class="relative">
          <div class="w-80 h-80 rounded-[3rem] overflow-hidden border-8 border-cyan-400 shadow-2xl shadow-cyan-500/50">
            <img src="https://picsum.photos/id/64/800/800" alt="Ons El Yahmadi" 
                 class="w-full h-full object-cover grayscale-0 hover:grayscale-0 transition-all">
          </div>
          <div class="absolute -bottom-4 -right-4 bg-gray-900 border border-cyan-400 rounded-3xl px-6 py-3 flex items-center gap-3">
            <span class="text-4xl">🇹🇳</span>
            <div>
              <p class="text-xs text-gray-400">Nationality</p>
              <p class="font-semibold text-cyan-400">Tunisian</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ABOUT -->
  <section id="about" class="py-24 bg-gray-900">
    <div class="max-w-5xl mx-auto px-8">
      <div class="grid md:grid-cols-2 gap-16 items-center">
        <div>
          <span class="px-4 py-2 bg-cyan-400/10 text-cyan-400 rounded-full text-sm font-medium">WHO AM I</span>
          <h2 class="heading-font text-5xl font-semibold tracking-tighter mt-4 mb-8">Dynamic MLOps Engineer turning models into production-ready AI solutions</h2>
          <p class="text-lg text-gray-300 leading-relaxed">
            I specialize in deploying machine learning models at scale, building robust MLOps pipelines, 
            and integrating CI/CD workflows to ensure models are reliable, monitored, and performant in real-world environments.
          </p>
          <p class="text-lg text-gray-300 leading-relaxed mt-6">
            Passionate about bridging the gap between data science and engineering with modern tools like Docker, 
            Jenkins, TensorFlow, and cloud platforms.
          </p>
        </div>
        
        <div class="grid grid-cols-2 gap-6">
          <div class="bg-gray-950 border border-cyan-400/20 rounded-3xl p-8 text-center">
            <i class="fas fa-rocket text-5xl text-cyan-400 mb-4"></i>
            <h4 class="font-semibold text-xl">MLOps Pipelines</h4>
            <p class="text-gray-400 text-sm mt-2">CI/CD • Monitoring • Automation</p>
          </div>
          <div class="bg-gray-950 border border-cyan-400/20 rounded-3xl p-8 text-center">
            <i class="fas fa-brain text-5xl text-cyan-400 mb-4"></i>
            <h4 class="font-semibold text-xl">Machine Learning</h4>
            <p class="text-gray-400 text-sm mt-2">Computer Vision • NLP • Time Series</p>
          </div>
          <div class="bg-gray-950 border border-cyan-400/20 rounded-3xl p-8 text-center">
            <i class="fas fa-laptop-code text-5xl text-cyan-400 mb-4"></i>
            <h4 class="font-semibold text-xl">Full-Stack Development</h4>
            <p class="text-gray-400 text-sm mt-2">NestJS • Next.js • Spring Boot</p>
          </div>
          <div class="bg-gray-950 border border-cyan-400/20 rounded-3xl p-8 text-center">
            <i class="fas fa-chart-line text-5xl text-cyan-400 mb-4"></i>
            <h4 class="font-semibold text-xl">Data Science</h4>
            <p class="text-gray-400 text-sm mt-2">Python • scikit-learn • Tableau</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- EXPERIENCE -->
  <section id="experience" class="py-24">
    <div class="max-w-7xl mx-auto px-8">
      <h2 class="heading-font text-5xl font-semibold text-center mb-16 tracking-tighter">Professional Experience</h2>
      
      <div class="space-y-16 relative before:content-[''] before:absolute before:left-8 md:before:left-1/2 before:top-8 before:bottom-8 before:w-px before:bg-gradient-to-b before:from-transparent before:via-cyan-400/30 before:to-transparent">
        
        <!-- Exp 1 -->
        <div class="flex flex-col md:flex-row gap-8 md:items-start relative">
          <div class="md:w-1/2 md:text-right">
            <div class="bg-cyan-400 text-gray-950 px-6 py-2 rounded-3xl inline-flex items-center gap-2 text-sm font-semibold">
              <span class="w-2 h-2 bg-white rounded-full animate-pulse"></span>
              Jan 2025 – Jun 2025
            </div>
            <h3 class="text-2xl font-semibold mt-3">MLOps Intern</h3>
            <p class="text-cyan-400 text-xl">EduZEN • Tunis</p>
          </div>
          <div class="md:w-1/2 bg-gray-900 rounded-3xl p-8 card-hover">
            <ul class="space-y-4 text-gray-300">
              <li class="flex gap-3"><i class="fas fa-check-circle text-cyan-400 mt-1"></i>Developed AI features for stress management and intelligent scheduling using NestJS + Next.js</li>
              <li class="flex gap-3"><i class="fas fa-check-circle text-cyan-400 mt-1"></i>Built end-to-end MLOps workflows with Google Colab for training ML &amp; LLM models</li>
              <li class="flex gap-3"><i class="fas fa-check-circle text-cyan-400 mt-1"></i>Implemented CI/CD pipelines with Jenkins for automated deployment</li>
            </ul>
          </div>
        </div>

        <!-- Exp 2 -->
        <div class="flex flex-col md:flex-row gap-8 md:items-start relative">
          <div class="md:w-1/2 md:text-right">
            <div class="bg-gray-800 text-white px-6 py-2 rounded-3xl inline-flex items-center text-sm font-semibold">Sep 2024 – Nov 2024</div>
            <h3 class="text-2xl font-semibold mt-3">Software Developer Intern</h3>
            <p class="text-cyan-400 text-xl">APAIA Technologies • Paris, France</p>
          </div>
          <div class="md:w-1/2 bg-gray-900 rounded-3xl p-8 card-hover">
            <ul class="space-y-4 text-gray-300">
              <li class="flex gap-3"><i class="fas fa-check-circle text-cyan-400 mt-1"></i>Built “Safe Life” mobile app using Ionic Framework and MongoDB for emergency equipment tracking</li>
              <li class="flex gap-3"><i class="fas fa-check-circle text-cyan-400 mt-1"></i>Documented and tested REST APIs with Swagger</li>
            </ul>
          </div>
        </div>

        <!-- Exp 3 -->
        <div class="flex flex-col md:flex-row gap-8 md:items-start relative">
          <div class="md:w-1/2 md:text-right">
            <div class="bg-gray-800 text-white px-6 py-2 rounded-3xl inline-flex items-center text-sm font-semibold">Feb 2024 – Oct 2024</div>
            <h3 class="text-2xl font-semibold mt-3">Data Scientist Intern</h3>
            <p class="text-cyan-400 text-xl">Coficab Group • Tunis</p>
          </div>
          <div class="md:w-1/2 bg-gray-900 rounded-3xl p-8 card-hover">
            <ul class="space-y-4 text-gray-300">
              <li class="flex gap-3"><i class="fas fa-check-circle text-cyan-400 mt-1"></i>Automated data pipelines using Python and SSIS</li>
              <li class="flex gap-3"><i class="fas fa-check-circle text-cyan-400 mt-1"></i>Developed time series forecasting models (ARIMA, ARCH) with 85% accuracy</li>
              <li class="flex gap-3"><i class="fas fa-check-circle text-cyan-400 mt-1"></i>Built Power BI dashboards with ETL integration</li>
            </ul>
          </div>
        </div>

        <!-- Exp 4 -->
        <div class="flex flex-col md:flex-row gap-8 md:items-start relative">
          <div class="md:w-1/2 md:text-right">
            <div class="bg-gray-800 text-white px-6 py-2 rounded-3xl inline-flex items-center text-sm font-semibold">Feb 2022 – Jun 2022</div>
            <h3 class="text-2xl font-semibold mt-3">Full-Stack Developer Intern</h3>
            <p class="text-cyan-400 text-xl">CNI • Tunis</p>
          </div>
          <div class="md:w-1/2 bg-gray-900 rounded-3xl p-8 card-hover">
            <ul class="space-y-4 text-gray-300">
              <li class="flex gap-3"><i class="fas fa-check-circle text-cyan-400 mt-1"></i>Designed municipal tax management application using Spring Boot + Angular + PostgreSQL</li>
              <li class="flex gap-3"><i class="fas fa-check-circle text-cyan-400 mt-1"></i>Integrated Google Maps API and PayPal payment gateway</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- SKILLS -->
  <section id="skills" class="py-24 bg-gray-900">
    <div class="max-w-7xl mx-auto px-8">
      <h2 class="heading-font text-5xl font-semibold text-center mb-16 tracking-tighter">Skills &amp; Tools</h2>
      
      <div class="grid md:grid-cols-3 gap-8">
        <!-- Programming -->
        <div class="bg-gray-950 rounded-3xl p-8">
          <h4 class="text-cyan-400 uppercase text-sm mb-6 flex items-center gap-2"><i class="fas fa-code"></i> Programming</h4>
          <div class="space-y-8">
            <div>
              <div class="flex justify-between text-sm mb-2"><span>Python</span><span class="font-mono">95%</span></div>
              <div class="h-2 bg-gray-800 rounded-full"><div class="progress-bar h-2 bg-cyan-400 rounded-full w-[95%]"></div></div>
            </div>
            <div>
              <div class="flex justify-between text-sm mb-2"><span>Java / Spring Boot</span><span class="font-mono">90%</span></div>
              <div class="h-2 bg-gray-800 rounded-full"><div class="progress-bar h-2 bg-cyan-400 rounded-full w-[90%]"></div></div>
            </div>
            <div>
              <div class="flex justify-between text-sm mb-2"><span>JavaScript / TypeScript</span><span class="font-mono">85%</span></div>
              <div class="h-2 bg-gray-800 rounded-full"><div class="progress-bar h-2 bg-cyan-400 rounded-full w-[85%]"></div></div>
            </div>
            <div>
              <div class="flex justify-between text-sm mb-2"><span>SQL &amp; R</span><span class="font-mono">88%</span></div>
              <div class="h-2 bg-gray-800 rounded-full"><div class="progress-bar h-2 bg-cyan-400 rounded-full w-[88%]"></div></div>
            </div>
          </div>
        </div>

        <!-- MLOps &amp; DevOps -->
        <div class="bg-gray-950 rounded-3xl p-8">
          <h4 class="text-cyan-400 uppercase text-sm mb-6 flex items-center gap-2"><i class="fas fa-server"></i> MLOps &amp; DevOps</h4>
          <div class="grid grid-cols-2 gap-6 text-center">
            <div class="bg-gray-900 rounded-2xl p-5">Docker</div>
            <div class="bg-gray-900 rounded-2xl p-5">Jenkins</div>
            <div class="bg-gray-900 rounded-2xl p-5">GitLab CI/CD</div>
            <div class="bg-gray-900 rounded-2xl p-5">Prometheus + Grafana</div>
            <div class="bg-gray-900 rounded-2xl p-5">SonarQube</div>
            <div class="bg-gray-900 rounded-2xl p-5">SSIS + Linux</div>
          </div>
        </div>

        <!-- Frameworks &amp; ML -->
        <div class="bg-gray-950 rounded-3xl p-8">
          <h4 class="text-cyan-400 uppercase text-sm mb-6 flex items-center gap-2"><i class="fas fa-cubes"></i> Frameworks &amp; ML</h4>
          <div class="flex flex-wrap gap-3">
            <span class="px-5 py-2 bg-gray-900 rounded-3xl text-sm">TensorFlow / Keras</span>
            <span class="px-5 py-2 bg-gray-900 rounded-3xl text-sm">scikit-learn</span>
            <span class="px-5 py-2 bg-gray-900 rounded-3xl text-sm">NestJS</span>
            <span class="px-5 py-2 bg-gray-900 rounded-3xl text-sm">Next.js</span>
            <span class="px-5 py-2 bg-gray-900 rounded-3xl text-sm">Angular</span>
            <span class="px-5 py-2 bg-gray-900 rounded-3xl text-sm">Flask / Django</span>
            <span class="px-5 py-2 bg-gray-900 rounded-3xl text-sm">Spring Boot</span>
            <span class="px-5 py-2 bg-gray-900 rounded-3xl text-sm">MERN Stack</span>
            <span class="px-5 py-2 bg-gray-900 rounded-3xl text-sm">.NET Core</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- PROJECTS -->
  <section id="projects" class="py-24">
    <div class="max-w-7xl mx-auto px-8">
      <div class="flex justify-between items-end mb-12">
        <h2 class="heading-font text-5xl font-semibold tracking-tighter">Featured Projects</h2>
        
        <!-- Filters -->
        <div class="flex flex-wrap gap-3" id="project-filters">
          <button onclick="filterProjects('all')" class="project-filter active px-6 py-3 rounded-3xl text-sm font-medium">All</button>
          <button onclick="filterProjects('ml')" class="project-filter px-6 py-3 rounded-3xl text-sm font-medium">ML &amp; AI</button>
          <button onclick="filterProjects('mlops')" class="project-filter px-6 py-3 rounded-3xl text-sm font-medium">MLOps &amp; DevOps</button>
          <button onclick="filterProjects('fullstack')" class="project-filter px-6 py-3 rounded-3xl text-sm font-medium">Full-Stack</button>
          <button onclick="filterProjects('mobile')" class="project-filter px-6 py-3 rounded-3xl text-sm font-medium">Mobile</button>
        </div>
      </div>

      <div id="projects-grid" class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
        <!-- Projects populated by JS below -->
      </div>
    </div>
  </section>

  <!-- EDUCATION -->
  <section id="education" class="py-24 bg-gray-900">
    <div class="max-w-7xl mx-auto px-8">
      <h2 class="heading-font text-5xl font-semibold text-center mb-16 tracking-tighter">Education</h2>
      
      <div class="space-y-12">
        <div class="flex flex-col md:flex-row gap-8 bg-gray-950 rounded-3xl p-8">
          <div class="md:w-72 shrink-0">
            <p class="text-cyan-400 font-medium">2023 – 2025</p>
            <h3 class="text-2xl font-semibold">Engineering Degree in Software Engineering</h3>
            <p class="text-gray-400">TEK-UP University</p>
          </div>
          <div class="flex-1 text-gray-300">
            • Built potato disease classification model (TensorFlow/Keras) – 90% accuracy<br>
            • Created credit scoring model for loan approval
          </div>
        </div>

        <div class="flex flex-col md:flex-row gap-8 bg-gray-950 rounded-3xl p-8">
          <div class="md:w-72 shrink-0">
            <p class="text-cyan-400 font-medium">2022 – 2024</p>
            <h3 class="text-2xl font-semibold">Professional Master’s in Data Science</h3>
            <p class="text-gray-400">Faculty of Science of Bizerte</p>
          </div>
          <div class="flex-1 text-gray-300">
            • Credit card fraud detection system (scikit-learn) – 95% accuracy<br>
            • Automated CV screening using NLP (NLTK + TF-IDF)
          </div>
        </div>

        <div class="flex flex-col md:flex-row gap-8 bg-gray-950 rounded-3xl p-8">
          <div class="md:w-72 shrink-0">
            <p class="text-cyan-400 font-medium">2019 – 2022</p>
            <h3 class="text-2xl font-semibold">Bachelor’s in Software Engineering &amp; Information Systems</h3>
            <p class="text-gray-400">Faculty of Science of Bizerte</p>
          </div>
          <div class="flex-1 text-gray-300">
            • Library management system (.NET Core + GitLab CI/CD)<br>
            • Excel dashboard for market trend analysis
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- CERTIFICATIONS -->
  <section class="py-24">
    <div class="max-w-7xl mx-auto px-8">
      <h2 class="heading-font text-5xl font-semibold text-center mb-12 tracking-tighter">Certifications</h2>
      <div class="flex flex-wrap gap-4 justify-center">
        <div class="bg-gray-900 px-8 py-6 rounded-3xl text-center border border-gray-700">Microsoft Azure Data Fundamentals</div>
        <div class="bg-gray-900 px-8 py-6 rounded-3xl text-center border border-gray-700">Microsoft Azure Fundamentals</div>
        <div class="bg-gray-900 px-8 py-6 rounded-3xl text-center border border-gray-700">IBM Spark - Level 1</div>
        <div class="bg-gray-900 px-8 py-6 rounded-3xl text-center border border-gray-700">Kaggle Intro to Machine Learning</div>
        <div class="bg-gray-900 px-8 py-6 rounded-3xl text-center border border-gray-700">Cisco Advanced SQL</div>
        <div class="bg-gray-900 px-8 py-6 rounded-3xl text-center border border-gray-700">365 Data Science - Python, SQL, Tableau</div>
      </div>
    </div>
  </section>

  <!-- CONTACT -->
  <section id="contact" class="py-24 bg-gray-900">
    <div class="max-w-4xl mx-auto px-8 text-center">
      <h2 class="heading-font text-5xl font-semibold tracking-tighter mb-8">Let's build something great together</h2>
      <p class="text-xl text-gray-400 mb-12">Open to MLOps, ML Engineering, or Full-Stack opportunities</p>
      
      <div class="flex flex-col md:flex-row gap-8 justify-center">
        <a href="mailto:ons.elyahmadi@fsb.ucar.tn" 
           class="flex-1 bg-gray-950 hover:bg-cyan-400 hover:text-gray-950 border border-cyan-400 rounded-3xl p-8 text-left transition-all">
          <i class="fas fa-envelope text-4xl mb-6"></i>
          <p class="font-medium text-2xl">Email me</p>
          <p class="text-cyan-400">ons.elyahmadi@fsb.ucar.tn</p>
        </a>
        
        <a href="https://www.linkedin.com/in/ons-elyahmadi" target="_blank"
           class="flex-1 bg-gray-950 hover:bg-cyan-400 hover:text-gray-950 border border-cyan-400 rounded-3xl p-8 text-left transition-all">
          <i class="fab fa-linkedin text-4xl mb-6"></i>
          <p class="font-medium text-2xl">Connect on LinkedIn</p>
          <p class="text-cyan-400">linkedin.com/in/ons-elyahmadi</p>
        </a>
      </div>
      
      <p class="mt-16 text-gray-500">6, rue Mohamed Arjoun, Zahrouni, Tunis 2051 • +216 58 217 800</p>
    </div>
  </section>

  <!-- FOOTER -->
  <footer class="bg-black py-12 text-center text-sm text-gray-500">
    © 2026 Ons El Yahmadi • Built with ❤️ and Tailwind CSS • All projects are real and deployed
  </footer>

  <script>
    // Tailwind script already loaded via CDN
    function filterProjects(category) {
      const buttons = document.querySelectorAll('#project-filters button')
      buttons.forEach(btn => btn.classList.remove('active'))
      
      const activeBtn = Array.from(buttons).find(btn => 
        (category === 'all' && btn.textContent === 'All') ||
        (category === 'ml' && btn.textContent === 'ML & AI') ||
        (category === 'mlops' && btn.textContent === 'MLOps & DevOps') ||
        (category === 'fullstack' && btn.textContent === 'Full-Stack') ||
        (category === 'mobile' && btn.textContent === 'Mobile')
      )
      if (activeBtn) activeBtn.classList.add('active')

      const cards = document.querySelectorAll('.project-card')
      cards.forEach(card => {
        if (category === 'all') {
          card.style.display = 'block'
        } else {
          card.style.display = card.dataset.category === category ? 'block' : 'none'
        }
      })
    }

    // Projects data
    const projectsData = [
      {
        title: "Potato Disease Classification",
        desc: "Deep learning model using TensorFlow & Keras. Achieved 90% accuracy on 5 classes.",
        tech: "TensorFlow • Keras • Computer Vision",
        category: "ml",
        icon: "🧬"
      },
      {
        title: "Credit Card Fraud Detection",
        desc: "End-to-end ML system (95% accuracy) deployed as full-stack web app with Django.",
        tech: "scikit-learn • Django • Flask • Angular",
        category: "ml",
        icon: "💳"
      },
      {
        title: "MLOps Pipeline – EduZEN AI",
        desc: "Automated CI/CD pipeline for LLM & ML training using Google Colab, Jenkins & Docker.",
        tech: "NestJS • Jenkins • Docker • Google Colab",
        category: "mlops",
        icon: "🚀"
      },
      {
        title: "Safe Life – Emergency Mobile App",
        desc: "Ionic mobile app to locate medical equipment in real-time (Paris-based startup).",
        tech: "Ionic • MongoDB • Swagger",
        category: "mobile",
        icon: "📱"
      },
      {
        title: "Municipal Tax Management System",
        desc: "Full-stack Spring Boot + Angular application with Google Maps & PayPal integration.",
        tech: "Spring Boot • Angular • PostgreSQL",
        category: "fullstack",
        icon: "🏛️"
      },
      {
        title: "MERN Reservation System",
        desc: "Booking platform built during engineering studies with full authentication & admin panel.",
        tech: "MongoDB • Express • React • Node.js",
        category: "fullstack",
        icon: "📅"
      }
    ]

    // Render projects
    function renderProjects() {
      const container = document.getElementById('projects-grid')
      container.innerHTML = ''
      
      projectsData.forEach(project => {
        const card = document.createElement('div')
        card.className = `project-card bg-gray-900 rounded-3xl overflow-hidden card-hover`
        card.dataset.category = project.category
        card.innerHTML = `
          <div class="h-2 bg-gradient-to-r from-cyan-400 to-blue-400"></div>
          <div class="p-8">
            <div class="text-5xl mb-6">${project.icon}</div>
            <h3 class="text-2xl font-semibold mb-3">${project.title}</h3>
            <p class="text-gray-400 mb-6">${project.desc}</p>
            <div class="flex flex-wrap gap-2">
              ${project.tech.split('•').map(t => `<span class="text-xs bg-gray-800 text-cyan-400 px-4 py-1 rounded-3xl">${t.trim()}</span>`).join('')}
            </div>
          </div>
        `
        container.appendChild(card)
      })
    }

    // Fake CV download
    function downloadCV() {
      alert("✅ CV downloaded! (In real life this would trigger a PDF download. Replace this alert with your actual CV link)")
      // Example: window.open('https://your-cv-link.pdf', '_blank')
    }

    // Initialize
    window.onload = () => {
      renderProjects()
      
      // Animate progress bars
      setTimeout(() => {
        document.querySelectorAll('.progress-bar').forEach(bar => {
          bar.style.width = bar.style.width || '0%'
        })
      }, 800)
    }
  </script>
</body>
</html>
