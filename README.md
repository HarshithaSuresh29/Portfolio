<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Harshitha SS — Portfolio</title>

  <!-- Tailwind CDN -->
  <script src="https://cdn.tailwindcss.com"></script>

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">

  <style>
    :root{
      --accent:#8b5cf6; /* purple */
      --muted:#9ca3af;
      --card:#0f1720;
      --bg:#0b0b0d;
    }

    html,body{
      height:100%;
      background: var(--bg);
      font-family: 'Inter', system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      color:#e6eef8;
    }

    /* animated gradient background */
    body::before{
      content:"";
      position:fixed;
      inset:0;
      z-index:-1;
      background:
        radial-gradient(600px 400px at 10% 20%, rgba(139,92,246,0.12), transparent 15%),
        radial-gradient(500px 300px at 90% 80%, rgba(34,197,94,0.06), transparent 12%),
        linear-gradient(180deg, rgba(6,7,11,1) 0%, rgba(12,13,15,1) 100%);
      animation: floatBG 18s ease-in-out infinite;
      opacity:1;
      transition:opacity .3s;
    }

    @keyframes floatBG{
      0% { transform: translateY(0) scale(1); }
      50% { transform: translateY(-10px) scale(1.02); }
      100% { transform: translateY(0) scale(1); }
    }

    /* fade-in used with IntersectionObserver */
    .fade-in {
      opacity: 0;
      transform: translateY(20px);
      transition: opacity .7s ease-out, transform .7s ease-out;
      will-change: opacity, transform;
    }
    .fade-in.is-visible {
      opacity: 1;
      transform: translateY(0);
    }

    /* small card */
    .card {
      background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      border: 1px solid rgba(255,255,255,0.04);
      box-shadow: 0 6px 18px rgba(2,6,23,0.6);
      border-radius: 14px;
    }

    /* typewriter caret */
    .typewriter {
      display:inline-block;
      border-right: 2px solid rgba(230,238,248,0.9);
      padding-right: 6px;
    }

    /* small responsive tweaks */
    @media (max-width:640px){
      .hero-title { font-size: 1.75rem; }
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header class="max-w-6xl mx-auto px-6 py-6 flex items-center justify-between">
    <div class="flex items-center gap-3">
      <div class="w-12 h-12 rounded-lg bg-gradient-to-br from-purple-600 to-indigo-500 flex items-center justify-center text-white font-bold">HS</div>
      <div>
        <div class="text-sm font-semibold">Harshitha SS</div>
        <div class="text-xs text-[--muted]">Java Full Stack • Mobile & Web</div>
      </div>
    </div>

    <nav class="flex items-center gap-4">
      <a href="#projects" class="text-sm text-[--muted] hover:text-white">Projects</a>
      <a href="#experience" class="text-sm text-[--muted] hover:text-white">Experience</a>
      <a href="#contact" class="text-sm text-[--muted] hover:text-white">Contact</a>

      <div class="flex items-center gap-3 ml-4">
        <a href="https://www.linkedin.com/in/harshitha-s-s-51aaa525b" target="_blank" aria-label="LinkedIn" class="p-2 rounded-md hover:bg-white/5">
          <!-- LinkedIn SVG -->
          <svg class="w-5 h-5 text-[--muted]" viewBox="0 0 24 24" fill="currentColor"><path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.762 2.239 5 5 5h14c2.762 0 5-2.238 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.765S5.534 3.2 6.5 3.2s1.75.79 1.75 1.765S7.466 6.732 6.5 6.732zM20 19h-3v-5.604c0-3.368-4-3.114-4 0V19h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476V19z"/></svg>
        </a>
        <a href="https://github.com/HarshithaSuresh29" target="_blank" aria-label="GitHub" class="p-2 rounded-md hover:bg-white/5">
          <!-- GitHub SVG -->
          <svg class="w-5 h-5 text-[--muted]" viewBox="0 0 24 24" fill="currentColor"><path d="M12 0C5.37 0 0 5.373 0 12c0 5.303 3.438 9.8 8.205 11.387.6.111.82-.261.82-.577v-2.234C6.73 20.092 6.14 18.6 6.14 18.6c-.546-1.387-1.333-1.756-1.333-1.756-1.09-.745.083-.73.083-.73 1.205.085 1.84 1.237 1.84 1.237 1.07 1.834 2.81 1.309 3.49.997.108-.775.418-1.309.762-1.605-2.665-.305-5.467-1.334-5.467-5.933 0-1.31.468-2.381 1.236-3.221-.124-.303-.536-1.524.117-3.176 0 0 1.01-.322 3.302 1.23.958-.266 1.984-.399 3.004-.404 1.02.005 2.046.138 3.006.404 2.292-1.552 3.298-1.23 3.298-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.48 5.922.43.371.823 1.102.823 2.222v3.293c0 .319.193.607.803.577C20.565 21.798 24 17.303 24 12 24 5.373 18.627 0 12 0z"/></svg>
        </a>
      </div>
    </nav>
  </header>

  <!-- Main content -->
  <main class="max-w-6xl mx-auto px-6 pb-24">

    <!-- Hero -->
    <section id="hero" class="text-center py-12 md:py-20 fade-in" style="--delay:0s;">
      <div class="max-w-3xl mx-auto">
        <h1 class="hero-title text-4xl md:text-5xl font-extrabold mb-4">Harshitha SS</h1>

        <h2 class="text-2xl md:text-3xl font-semibold mb-6">
          <span class="typewriter" id="typewriter"></span>
        </h2>

        <p class="text-gray-300 leading-relaxed mb-6">Motivated Computer Science student with a strong background in Java, Data Structures, Web Development and App Development. Seeking to apply technical knowledge and problem-solving skills to real-world projects and deliver high-quality solutions as a dedicated member of a development team.</p>

        <div class="flex items-center justify-center gap-4">
          <a href="#projects" class="px-5 py-2 bg-[--accent] rounded-md text-white font-medium hover:opacity-95">View Projects</a>
          <a href="mailto:harshitha29ss@gmail.com" class="px-5 py-2 border border-white/10 rounded-md text-white/90 hover:bg-white/5">Contact Me</a>
        </div>
      </div>
    </section>

    <!-- Two column: Contact + Objective -->
    <section class="grid md:grid-cols-3 gap-6 mb-12 fade-in" style="--delay:0.15s;">
      <div class="md:col-span-2 card p-6">
        <h3 class="text-xl font-semibold mb-3">Objective</h3>
        <p class="text-gray-300">Motivated Computer Science student with a strong background in Java, Data Structures, Web Development and App Development. Seeking to apply technical knowledge and problem-solving skills to real-world projects and deliver high-quality solutions as a dedicated member of a development team.</p>
      </div>

      <aside class="card p-6">
        <h4 class="text-lg font-semibold mb-2">Contact</h4>
        <p class="text-sm text-[--muted]">Bangalore, Karnataka, India</p>
        <p class="font-medium mt-2">+91 9113822713</p>
        <a class="text-[--accent] block mt-1" href="mailto:harshitha29ss@gmail.com">harshitha29ss@gmail.com</a>
        <div class="mt-4 text-xs text-[--muted]">GitHub · LinkedIn</div>
      </aside>
    </section>

    <!-- Education -->
    <section id="education" class="fade-in mb-12" style="--delay:0.25s;">
      <h3 class="text-2xl font-bold mb-6">Education</h3>
      <div class="grid md:grid-cols-3 gap-6">
        <div class="card p-5">
          <h4 class="font-semibold">Presidency University</h4>
          <p class="text-[--muted] text-sm">Aug 2022 – Present</p>
          <p class="mt-2 text-gray-300">B.Tech in Computer Science — CGPA: <span class="text-purple-300 font-semibold">9.08</span></p>
        </div>
        <div class="card p-5">
          <h4 class="font-semibold">Jnana Bharathi PU College</h4>
          <p class="text-[--muted] text-sm">2021 – 2022</p>
          <p class="mt-2 text-gray-300">Intermediate (PCMB) — <span class="text-purple-300">93.5%</span></p>
        </div>
        <div class="card p-5">
          <h4 class="font-semibold">Jnana Bharathi English Higher Secondary</h4>
          <p class="text-[--muted] text-sm">2019 – 2020</p>
          <p class="mt-2 text-gray-300">High School — <span class="text-purple-300">85.44%</span></p>
        </div>
      </div>
    </section>

    <!-- Experience -->
    <section id="experience" class="fade-in mb-12" style="--delay:0.35s;">
      <h3 class="text-2xl font-bold mb-6">Experience</h3>
      <div class="card p-6">
        <h4 class="text-lg font-semibold">Mobile Application Development Intern — Untitled Needleworks</h4>
        <p class="text-[--muted] text-sm">Jul 2025 – Present</p>
        <ul class="list-disc list-inside mt-3 text-gray-300 space-y-2">
          <li>Developed payment pages and outfit sections with a virtual try-on feature, increasing user engagement by ~15%.</li>
          <li>Engineered an in-app chat with like & comment functionality, improving interaction by ~5%.</li>
        </ul>
      </div>
    </section>

    <!-- Projects -->
    <section id="projects" class="fade-in mb-12" style="--delay:0.45s;">
      <h3 class="text-2xl font-bold mb-6">Projects</h3>
      <div class="grid md:grid-cols-2 gap-6">
        <div class="card p-5">
          <h4 class="font-semibold">Event Management System</h4>
          <p class="text-[--muted] text-sm">HTML • CSS • JS • Bootstrap • AngularJS (2025)</p>
          <p class="mt-2 text-gray-300">Responsive platform for event creation, registration & tracking. Reduced manual effort by 30% and improved registrations by 25%.</p>
        </div>
        <div class="card p-5">
          <h4 class="font-semibold">Women Safety Application</h4>
          <p class="text-[--muted] text-sm">Android Studio • Java • MySQL (2024)</p>
          <p class="mt-2 text-gray-300">SOS app with real-time location sharing & alerts. Secure MySQL backend ensuring ~90% data retrieval success.</p>
        </div>
        <div class="card p-5">
          <h4 class="font-semibold">Camouflage Multi-Functional Army Robot</h4>
          <p class="text-[--muted] text-sm">Arduino (2024)</p>
          <p class="mt-2 text-gray-300">Arduino-powered robot with camouflage & remote navigation — improved simulated mission success by ~40%.</p>
        </div>
        <div class="card p-5">
          <h4 class="font-semibold">Autonomous Boat with Waste Collection</h4>
          <p class="text-[--muted] text-sm">Raspberry Pi (2023)</p>
          <p class="mt-2 text-gray-300">Autonomous boat collecting waste using GPS — completed routes 20% faster than manual methods.</p>
        </div>
      </div>
    </section>

    <!-- Skills & Certificates -->
    <section class="grid md:grid-cols-2 gap-6 fade-in" style="--delay:0.6s;">
      <div class="card p-6">
        <h3 class="text-xl font-semibold mb-4">Skills</h3>
        <div class="flex flex-wrap gap-3">
          <span class="bg-purple-700 text-white px-3 py-1 rounded-full text-sm">Java</span>
          <span class="bg-purple-700 text-white px-3 py-1 rounded-full text-sm">Python</span>
          <span class="bg-purple-700 text-white px-3 py-1 rounded-full text-sm">HTML</span>
          <span class="bg-purple-700 text-white px-3 py-1 rounded-full text-sm">CSS</span>
          <span class="bg-purple-700 text-white px-3 py-1 rounded-full text-sm">JavaScript</span>
          <span class="bg-purple-700 text-white px-3 py-1 rounded-full text-sm">MySQL</span>
          <span class="bg-purple-700 text-white px-3 py-1 rounded-full text-sm">Android Studio</span>
          <span class="bg-purple-700 text-white px-3 py-1 rounded-full text-sm">Flutter</span>
          <span class="bg-purple-700 text-white px-3 py-1 rounded-full text-sm">Git</span>
        </div>
      </div>

      <div class="card p-6">
        <h3 class="text-xl font-semibold mb-4">Certificates</h3>
        <ul class="list-disc list-inside text-gray-300 space-y-2">
          <li>Problem Solving for DSA in Java — CodeChef</li>
          <li>Oracle Java Foundation — Oracle Badge</li>
          <li>Smart India Hackathon — SIH</li>
          <li>Introduction to Machine Learning — Infosys Springboard</li>
        </ul>
      </div>
    </section>

    <!-- Contact -->
    <section id="contact" class="fade-in text-center py-12" style="--delay:0.75s;">
      <h3 class="text-2xl font-bold mb-3">Get in touch</h3>
      <p class="text-gray-300 mb-1">Bengaluru, Karnataka, India</p>
      <p class="font-medium text-lg mb-1">+91 9113822713</p>
      <a href="mailto:harshitha29ss@gmail.com" class="text-[--accent] hover:underline">harshitha29ss@gmail.com</a>
    </section>

  </main>

  <!-- Footer -->
  <footer class="text-center text-[--muted] py-8">
    © <span id="year"></span> Harshitha SS — Built with HTML, Tailwind & ❤️
  </footer>

  <!-- Scripts: typewriter + intersection observer -->
  <script>
    // year
    document.getElementById('year').textContent = new Date().getFullYear();

    // Typewriter effect
    (function(){
      const el = document.getElementById('typewriter');
      const words = ["Java Full Stack Developer","Front-end Developer","Mobile App Developer"];
      let wIndex = 0, charIndex = 0, typing = true, delayAfter = 1500;

      function type() {
        const word = words[wIndex];
        if (typing) {
          charIndex++;
          el.textContent = word.slice(0,charIndex);
          if (charIndex === word.length) {
            typing = false;
            setTimeout(type, delayAfter);
          } else {
            setTimeout(type, 80);
          }
        } else {
          charIndex--;
          el.textContent = word.slice(0,charIndex);
          if (charIndex === 0) {
            typing = true;
            wIndex = (wIndex + 1) % words.length;
            setTimeout(type, 300);
          } else {
            setTimeout(type, 40);
          }
        }
      }
      type();
    })();

    // IntersectionObserver fade-in
    (function(){
      const io = new IntersectionObserver((entries, observer) => {
        entries.forEach(entry => {
          if (entry.isIntersecting) {
            entry.target.classList.add('is-visible');
            observer.unobserve(entry.target);
          }
        });
      }, {threshold: 0.12});

      document.querySelectorAll('.fade-in').forEach(el => io.observe(el));
    })();
  </script>
</body>
</html>
