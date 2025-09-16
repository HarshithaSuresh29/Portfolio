<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Harshitha SS - Portfolio</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
  <style>
    body {
      background-color: #0d0d0d;
      color: #f0f0f0;
      font-family: 'Inter', sans-serif;
    }
    .fade-in {
      opacity: 0;
      transform: translateY(20px);
      transition: opacity 0.6s ease-out, transform 0.6s ease-out;
      transition-delay: var(--delay);
    }
    .fade-in.is-visible {
      opacity: 1;
      transform: translateY(0);
    }
  </style>
</head>
<body class="antialiased">

  <!-- Header -->
  <header class="flex justify-between items-center py-8 px-6 md:px-16 lg:px-24">
    <h1 class="text-2xl font-bold text-white">HS</h1>
    <div class="flex items-center space-x-6">
      <a href="https://www.linkedin.com/in/harshitha-s-s-51aaa525b" target="_blank" class="text-gray-400 hover:text-white transition">
        LinkedIn
      </a>
      <a href="https://github.com/HarshithaSuresh29" target="_blank" class="text-gray-400 hover:text-white transition">
        GitHub
      </a>
      <a href="mailto:harshitha29ss@gmail.com" class="text-gray-400 hover:text-white transition">
        Email
      </a>
    </div>
  </header>

  <main class="container mx-auto px-6 md:px-12 lg:px-20">

    <!-- Hero -->
    <section id="hero" class="py-16 text-center fade-in" style="--delay:0s;">
      <h2 class="text-4xl md:text-5xl font-bold mb-4">Harshitha SS</h2>
      <h3 class="text-xl md:text-2xl text-purple-400 mb-6">Java Full Stack Developer</h3>
      <p class="max-w-3xl mx-auto text-gray-300">Motivated Computer Science student with a strong background in Java, Data Structures, Web Development, and App Development. Seeking to apply technical knowledge and problem-solving skills to real-world projects and deliver high-quality solutions as a dedicated member of a development team.</p>
    </section>

    <!-- Education -->
    <section id="education" class="py-16 fade-in" style="--delay:0.2s;">
      <h3 class="text-3xl font-bold mb-8 text-center">Education</h3>
      <div class="space-y-6">
        <div class="bg-[#1a1a1a] p-6 rounded-xl shadow-lg">
          <h4 class="font-semibold text-lg">Presidency University</h4>
          <p class="text-gray-400">Aug 2022 – Present | B.Tech in Computer Science | Bengaluru</p>
          <p class="text-purple-400">CGPA: 9.08</p>
        </div>
        <div class="bg-[#1a1a1a] p-6 rounded-xl shadow-lg">
          <h4 class="font-semibold text-lg">Jnana Bharathi PU College</h4>
          <p class="text-gray-400">2021 – 2022 | PCMB | Kunigal</p>
          <p class="text-purple-400">Percentage: 93.5%</p>
        </div>
        <div class="bg-[#1a1a1a] p-6 rounded-xl shadow-lg">
          <h4 class="font-semibold text-lg">Jnana Bharathi English Higher Secondary</h4>
          <p class="text-gray-400">2019 – 2020 | High School | Kunigal</p>
          <p class="text-purple-400">Percentage: 85.44%</p>
        </div>
      </div>
    </section>

    <!-- Experience -->
    <section id="experience" class="py-16 fade-in" style="--delay:0.4s;">
      <h3 class="text-3xl font-bold mb-8 text-center">Experience</h3>
      <div class="bg-[#1a1a1a] p-6 rounded-xl shadow-lg">
        <h4 class="text-xl font-semibold">Mobile Application Development Intern — Untitled Needleworks</h4>
        <p class="text-gray-400 mb-2">Jul 2025 – Present</p>
        <ul class="list-disc list-inside text-gray-300">
          <li>Developed new payment pages and outfit sections, integrating a virtual try-on feature that increased user engagement by 15%.</li>
          <li>Engineered an in-app chat with like and comment functionality, boosting user interaction by 5%.</li>
        </ul>
      </div>
    </section>

    <!-- Projects -->
    <section id="projects" class="py-16 fade-in" style="--delay:0.6s;">
      <h3 class="text-3xl font-bold mb-8 text-center">Projects</h3>
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <div class="bg-[#1a1a1a] p-6 rounded-xl shadow-lg">
          <h4 class="text-lg font-semibold">Event Management System</h4>
          <p class="text-gray-400">HTML, CSS, JS, Bootstrap, AngularJS (2025)</p>
          <ul class="list-disc list-inside text-gray-300">
            <li>Developed a responsive web platform for event creation, registration, and attendee tracking, reducing manual effort by 30%.</li>
            <li>Integrated AngularJS for dynamic data handling, boosting event registrations by 25%.</li>
          </ul>
        </div>
        <div class="bg-[#1a1a1a] p-6 rounded-xl shadow-lg">
          <h4 class="text-lg font-semibold">Women Safety Application</h4>
          <p class="text-gray-400">Android Studio, Java, MySQL (2024)</p>
          <ul class="list-disc list-inside text-gray-300">
            <li>Engineered a mobile safety app with SOS feature providing real-time location sharing and emergency alerts.</li>
            <li>Integrated secure MySQL backend ensuring 90% data retrieval success.</li>
          </ul>
        </div>
        <div class="bg-[#1a1a1a] p-6 rounded-xl shadow-lg">
          <h4 class="text-lg font-semibold">Camouflage Multi-Functional Army Robot</h4>
          <p class="text-gray-400">Arduino (2024)</p>
          <p class="text-gray-300">Built an Arduino-powered robot with camouflage and remote navigation capabilities, enhancing simulated mission success by 40%.</p>
        </div>
        <div class="bg-[#1a1a1a] p-6 rounded-xl shadow-lg">
          <h4 class="text-lg font-semibold">Autonomous Boat with Waste Collection</h4>
          <p class="text-gray-400">Raspberry Pi (2023)</p>
          <p class="text-gray-300">Designed an autonomous boat with waste collection using GPS navigation, completing cleaning routes 20% faster than manual methods.</p>
        </div>
      </div>
    </section>

    <!-- Skills -->
    <section id="skills" class="py-16 fade-in" style="--delay:0.8s;">
      <h3 class="text-3xl font-bold mb-8 text-center">Skills</h3>
      <div class="flex flex-wrap justify-center gap-3">
        <span class="bg-purple-800 text-white px-4 py-2 rounded-full">Java</span>
        <span class="bg-purple-800 text-white px-4 py-2 rounded-full">Python</span>
        <span class="bg-purple-800 text-white px-4 py-2 rounded-full">HTML</span>
        <span class="bg-purple-800 text-white px-4 py-2 rounded-full">CSS</span>
        <span class="bg-purple-800 text-white px-4 py-2 rounded-full">JavaScript</span>
        <span class="bg-purple-800 text-white px-4 py-2 rounded-full">MySQL</span>
        <span class="bg-purple-800 text-white px-4 py-2 rounded-full">Android Studio</span>
        <span class="bg-purple-800 text-white px-4 py-2 rounded-full">Flutter</span>
        <span class="bg-purple-800 text-white px-4 py-2 rounded-full">GitHub</span>
      </div>
    </section>

    <!-- Certificates -->
    <section id="certificates" class="py-16 fade-in" style="--delay:1s;">
      <h3 class="text-3xl font-bold mb-8 text-center">Certificates</h3>
      <ul class="list-disc list-inside text-gray-300 max-w-2xl mx-auto space-y-2">
        <li>Problem Solving for DSA in Java — CodeChef</li>
        <li>Oracle Java Foundation — Oracle Badge</li>
        <li>Smart India Hackathon — SIH</li>
        <li>Introduction to Machine Learning — Infosys Springboard</li>
      </ul>
    </section>

    <!-- Contact -->
    <section id="contact" class="py-16 text-center fade-in" style="--delay:1.2s;">
      <h3 class="text-3xl font-bold mb-4">Get In Touch</h3>
      <p class="text-gray-300 mb-2">Bengaluru, Karnataka, India</p>
      <p class="font-semibold text-lg">+91 9113822713</p>
      <a href="mailto:harshitha29ss@gmail.com" class="text-purple-400 hover:underline text-lg">harshitha29ss@gmail.com</a>
    </section>

  </main>

  <script>
    const observer = new IntersectionObserver((entries, observer) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add('is-visible');
          observer.unobserve(entry.target);
        }
      });
    }, { threshold: 0.1 });

    document.querySelectorAll('.fade-in').forEach(section => {
      observer.observe(section);
    });
  </script>
</body>
</html>
