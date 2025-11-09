<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>PRAVIN A | Portfolio</title>
  <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
  <script src="https://unpkg.com/scrollreveal"></script>
  <style>
    body {
      background: radial-gradient(circle at top left, #111, #000);
    }
    .btn-3d {
      background: linear-gradient(135deg, #ff7eb3, #ff758c);
      border: none;
      color: white;
      padding: 10px 20px;
      border-radius: 10px;
      font-weight: bold;
      box-shadow: 0 6px #c93a63;
      transition: all 0.2s ease;
    }
    .btn-3d:hover {
      transform: translateY(-4px);
      box-shadow: 0 10px #b32d56;
    }
    .card-3d {
      background: linear-gradient(145deg, #1a1a1a, #0d0d0d);
      border: 1px solid rgba(255, 255, 255, 0.1);
      border-radius: 16px;
      box-shadow: 8px 8px 15px rgba(0, 0, 0, 0.6), -8px -8px 15px rgba(255, 255, 255, 0.05);
      transition: transform 0.4s ease, box-shadow 0.4s ease;
    }
    .card-3d:hover {
      transform: translateY(-10px) scale(1.02);
      box-shadow: 0 0 25px rgba(255, 120, 150, 0.4);
    }
  </style>
</head>
<body class="text-gray-100 font-sans">
  <header class="p-6 bg-gradient-to-r from-pink-600 via-red-500 to-yellow-500 text-white shadow-lg sticky top-0 z-50">
    <div class="flex justify-between items-center">
      <h1 class="text-3xl font-extrabold tracking-wide">PRAVIN A</h1>
      <nav class="space-x-3">
        <button onclick="scrollToSection('profile')" class="btn-3d">Profile</button>
        <button onclick="scrollToSection('experience')" class="btn-3d">Experience</button>
        <button onclick="scrollToSection('education')" class="btn-3d">Education</button>
        <button onclick="scrollToSection('projects')" class="btn-3d">Projects</button>
        <button onclick="scrollToSection('certifications')" class="btn-3d">Certifications</button>
        <button onclick="scrollToSection('skills')" class="btn-3d">Skills</button>
        <button onclick="scrollToSection('achievements')" class="btn-3d">Achievements</button>
      </nav>
    </div>
  </header>

  <!-- PROFILE OVERVIEW -->
  <section id="profile" class="p-10 max-w-5xl mx-auto text-center">
    <h2 class="text-4xl font-extrabold mb-4 text-pink-400 drop-shadow-lg">Profile Overview</h2>
    <p class="text-lg leading-relaxed text-gray-300 max-w-3xl mx-auto">Aspiring professional in the semiconductor industry, pursuing B.E. in Electronics and Communication Engineering at Sri Eshwar College of Engineering. Passionate about VLSI, circuit simulation, and digital IC development.</p>
  </section>

  <!-- EXPERIENCE -->
  <section id="experience" class="p-10 max-w-6xl mx-auto">
    <h2 class="text-3xl font-bold mb-6 text-pink-400">Experience</h2>
    <div class="grid md:grid-cols-2 gap-8">
      <div class="card-3d p-6">
        <h3 class="text-2xl font-semibold">FOSSEE, IIT Bombay (Remote)</h3>
        <p class="italic text-gray-400">Oct 2025 – Present | Research Migration Contributor</p>
        <ul class="list-disc text-gray-300 ml-6 mt-3">
          <li>Migrated and simulated analog circuits using open-source EDA tools.</li>
          <li>Worked on CMOS-based charge pump and analog modeling.</li>
        </ul>
      </div>
      <div class="card-3d p-6">
        <h3 class="text-2xl font-semibold">Circuit Designer – FOSSEE</h3>
        <p class="italic text-gray-400">Sep 2025 – Oct 2025</p>
        <ul class="list-disc text-gray-300 ml-6 mt-3">
          <li>Focused on DC-DC converters and analog circuit optimization.</li>
          <li>Developed open-source compatible eSim models.</li>
        </ul>
      </div>
    </div>
  </section>

  <!-- EDUCATION -->
  <section id="education" class="p-10 max-w-5xl mx-auto">
    <h2 class="text-3xl font-bold mb-6 text-pink-400">Education</h2>
    <div class="grid md:grid-cols-2 gap-6">
      <div class="card-3d p-5">
        <h3 class="text-xl font-semibold">B.E - ECE</h3>
        <p>Sri Eshwar College of Engineering (2024–2028)</p>
      </div>
      <div class="card-3d p-5">
        <h3 class="text-xl font-semibold">HSC - Maths & Computer Science</h3>
        <p>Holy Angel’s MHSS (95%)</p>
      </div>
    </div>
  </section>

  <!-- PROJECTS -->
  <section id="projects" class="p-10 max-w-6xl mx-auto">
    <h2 class="text-3xl font-bold mb-6 text-pink-400">Projects & Research</h2>
    <div class="grid md:grid-cols-2 gap-8">
      <div class="card-3d p-6">
        <h3 class="text-lg font-semibold">Electronic Voting System (Vivado)</h3>
        <p>Developed and simulated real-time digital voting using Verilog modules.</p>
      </div>
      <div class="card-3d p-6">
        <h3 class="text-lg font-semibold">Analog Design (Cadence Virtuoso)</h3>
        <p>Designed Common Emitter Amplifier and analyzed DC/transient performance.</p>
      </div>
      <div class="card-3d p-6">
        <h3 class="text-lg font-semibold">Adaptive Vision (IoT + AI)</h3>
        <p>Smart lighting system using sensors and rain detection. Won Hackathon Prize.</p>
      </div>
      <div class="card-3d p-6">
        <h3 class="text-lg font-semibold">FOSSEE Research Migration</h3>
        <p>Simulated CMOS charge pumps; contributions published under NMEICT.</p>
      </div>
    </div>
  </section>

  <!-- SKILLS -->
  <section id="skills" class="p-10 max-w-6xl mx-auto">
    <h2 class="text-3xl font-bold mb-6 text-pink-400">Skills</h2>
    <div class="grid md:grid-cols-2 gap-6">
      <div class="card-3d p-6">
        <h3 class="text-xl font-semibold mb-2">Technical</h3>
        <p>VLSI Tools: Cadence, Vivado, eSim, LTSpice<br>Programming: Verilog, C, C++, Python<br>Hardware: Arduino, FPGA</p>
      </div>
      <div class="card-3d p-6">
        <h3 class="text-xl font-semibold mb-2">Soft Skills</h3>
        <p>Team Collaboration, Debugging, Documentation, Research Analysis</p>
      </div>
    </div>
  </section>

  <!-- ACHIEVEMENTS -->
  <section id="achievements" class="p-10 max-w-6xl mx-auto text-center">
    <h2 class="text-3xl font-bold mb-6 text-pink-400">Achievements</h2>
    <div class="grid md:grid-cols-2 gap-8">
      <div class="card-3d p-6">
        <h3 class="text-lg font-semibold">🏆 FOSSEE Internship @ IIT Bombay</h3>
        <p>Contributed to open-source analog simulation and migration projects.</p>
      </div>
      <div class="card-3d p-6">
        <h3 class="text-lg font-semibold">🎖 SelfE Hackathon 2024</h3>
        <p>Won Special Prize for Adaptive Vision IoT Project.</p>
      </div>
    </div>
    <div class="mt-8">
      <a href="https://github.com/pravin2007-ctrl" class="btn-3d inline-block">Visit GitHub</a>
      <a href="mailto:pravin.a2024ece@sece.ac.in" class="btn-3d inline-block ml-4">Contact Me</a>
    </div>
  </section>

  <footer class="p-6 text-center bg-gradient-to-r from-red-500 via-pink-600 to-orange-500 mt-10 rounded-t-2xl text-white">
    <p>© 2025 PRAVIN A | Designed with ❤️ and Tailwind</p>
  </footer>

  <script>
    function scrollToSection(id) {
      document.getElementById(id).scrollIntoView({ behavior: 'smooth' });
    }
    ScrollReveal().reveal('.card-3d', { interval: 150, origin: 'bottom', distance: '40px', duration: 800 });
  </script>
</body>
</html>
