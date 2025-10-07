
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Praveen.V — Cybersecurity Portfolio</title>
  <meta name="description" content="Portfolio of Praveen V — Cybersecurity specialist. Ethical hacking, network security and digital forensics." />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0f1724;         /* deep navy */
      --card:#0b1220;
      --muted:#9aa7b2;
      --accent:#00d1b2;     /* teal accent */
      --accent-2:#5eead4;
      --glass: rgba(255,255,255,0.04);
      --glass-2: rgba(255,255,255,0.02);
      --radius:16px;
      --maxw:1100px;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family:"Inter",system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial;
      background:linear-gradient(180deg,var(--bg) 0%, #071022 100%);
      color:#d7e3ea;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.45;
    }

    /* Container */
    .wrap{
      max-width:var(--maxw);
      margin:36px auto;
      padding:28px;
    }

    /* Header / Nav */
    header{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:16px;
      margin-bottom:28px;
    }
    .brand{
      display:flex;
      gap:14px;
      align-items:center;
    }
    .avatar{
      width:64px;
      height:64px;
      border-radius:12px;
      background:linear-gradient(135deg,var(--accent),var(--accent-2));
      display:grid;
      place-items:center;
      font-weight:800;
      color:#021018;
      font-size:20px;
      box-shadow:0 6px 18px rgba(2,16,24,0.6);
    }
    .brand h1{font-size:18px;margin:0}
    .brand p{margin:0;font-size:13px;color:var(--muted)}

    nav a{
      color:var(--muted);
      text-decoration:none;
      margin-left:18px;
      font-weight:600;
      font-size:14px;
    }
    nav a:hover{color:var(--accent)}

    /* Hero */
    .hero{
      display:grid;
      grid-template-columns: 1fr 360px;
      gap:28px;
      align-items:center;
      margin-bottom:28px;
    }
    .hero-card{
      background:linear-gradient(180deg,var(--card), rgba(11,18,32,0.6));
      border-radius:var(--radius);
      padding:28px;
      box-shadow: 0 10px 30px rgba(2,8,20,0.6);
      position:relative;
      overflow:hidden;
      border:1px solid rgba(255,255,255,0.03);
    }
    .hero h2{margin:0 0 8px 0;font-size:28px}
    .hero h3{margin:0;color:var(--accent);font-size:14px;font-weight:700}
    .hero p{color:var(--muted);margin-top:14px;font-size:15px}

    .cta{
      margin-top:18px;
      display:flex;
      gap:12px;
      flex-wrap:wrap;
    }
    .btn{
      display:inline-flex;
      align-items:center;
      gap:8px;
      padding:10px 16px;
      border-radius:12px;
      background:linear-gradient(90deg,var(--accent),var(--accent-2));
      color:#012022;
      font-weight:700;
      cursor:pointer;
      border:none;
      box-shadow:0 8px 18px rgba(0,209,178,0.15);
      text-decoration:none;
    }
    .btn.ghost{
      background:transparent;
      color:var(--accent-2);
      border:1px solid rgba(94,234,212,0.12);
      font-weight:600;
    }

    /* Right column profile */
    .profile{
      background:var(--glass);
      padding:18px;
      border-radius:12px;
      border:1px solid rgba(255,255,255,0.02);
      text-align:center;
    }
    .profile img{
      width:120px;height:120px;border-radius:12px;object-fit:cover;margin-bottom:12px;
      display:block;margin-left:auto;margin-right:auto;
      box-shadow:0 8px 20px rgba(2,16,24,0.6);
    }
    .profile h4{margin:8px 0 4px 0;font-size:16px}
    .profile p{margin:0;font-size:13px;color:var(--muted)}

    /* Sections */
    section{
      margin-top:28px;
      display:grid;
      gap:16px;
    }
    .grid-2{
      display:grid;
      grid-template-columns: 1fr 360px;
      gap:20px;
      align-items:start;
    }
    .card{
      background: linear-gradient(180deg, rgba(255,255,255,0.02), transparent);
      border-radius:12px;
      padding:18px;
      border:1px solid rgba(255,255,255,0.03);
    }
    .card h3{margin-top:0;margin-bottom:12px}
    .skill-list{
      display:flex;
      gap:10px;
      flex-wrap:wrap;
    }
    .skill{
      background:var(--glass-2);
      padding:8px 12px;
      border-radius:999px;
      font-weight:600;
      color:var(--muted);
      border:1px solid rgba(255,255,255,0.02);
      font-size:13px;
    }

    /* Projects placeholder */
    .projects{
      display:grid;
      grid-template-columns: repeat(auto-fit,minmax(220px,1fr));
      gap:16px;
    }
    .project{
      padding:14px;
      border-radius:12px;
      min-height:120px;
      background:linear-gradient(180deg, rgba(255,255,255,0.01), transparent);
      border:1px solid rgba(255,255,255,0.02);
    }
    .project h4{margin:0 0 8px 0}

    /* Contact form */
    form.contact{
      display:grid;
      gap:12px;
    }
    input[type="text"], input[type="email"], textarea{
      background:transparent;
      border:1px solid rgba(255,255,255,0.04);
      padding:10px 12px;
      color:var(--muted);
      border-radius:10px;
      resize:vertical;
    }
    textarea{min-height:110px}
    .muted{color:var(--muted);font-size:14px}

    /* Footer */
    footer{
      margin-top:40px;
      text-align:center;
      color:var(--muted);
      font-size:13px;
      padding:28px 0 10px 0;
    }

    /* Responsive */
    @media (max-width:980px){
      .hero, .grid-2{grid-template-columns: 1fr;}
      nav a{display:none}
      .brand p{display:none}
    }

    /* small helpers */
    .row{display:flex;gap:12px;align-items:center}
    .center{display:grid;place-items:center}
    .badge{font-size:12px;padding:6px 10px;border-radius:999px;background:rgba(255,255,255,0.02);border:1px solid rgba(255,255,255,0.02)}
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="brand">
        <div class="avatar" aria-hidden="true">PV</div>
        <div>
          <h1>Praveen.V</h1>
          <p>Cybersecurity • BE Cyber Security</p>
        </div>
      </div>
      <nav aria-label="Main navigation">
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#projects">Projects</a>
        <a href="#services">Services</a>
        <a href="#contact">Contact</a>
      </nav>
    </header>

    <!-- HERO -->
    <section id="home" class="hero" aria-labelledby="intro-heading">
      <div class="hero-card card" role="region" aria-label="Introduction">
        <h3 id="intro-heading">Hello, I'm</h3>
        <h2>Praveen.V — Cybersecurity Specialist</h2>
        <p><strong>Focus:</strong> cyber security. I design secure systems, learn offensive security techniques, and pursue hands-on experience in network defense, penetration testing, and digital forensics.</p>

        <div class="cta" role="group" aria-label="Primary calls to action">
          <a class="btn" href="#projects">View Projects</a>
          <a class="btn ghost" href="#contact">Contact Me</a>
          <a class="btn ghost" href="#" id="downloadResume">Download Resume</a>
        </div>

        <div style="margin-top:16px;color:var(--muted);font-size:13px;">
          <span class="badge">Degree: BE Cyber Security</span>
          <span class="badge" style="margin-left:8px">Experience: Student / Early-career</span>
        </div>
      </div>

      <aside class="profile">
        <!-- Placeholder image. Replace src with your photo file (e.g., images/profile.jpg) -->
        <img src="praveen.1.jpg.jpg" alt="Praveen V profile photo">
        <h4>Praveen.V</h4>
        <p class="muted">BE Cyber Security — Aspiring Security Engineer</p>
        <p style="font-size:13px;margin-top:10px;color:var(--muted)">Open to internships, freelance bug bounty work, and collaborative projects.</p>
      </aside>
    </section>

    <!-- ABOUT + CONTACT ASIDE -->
    <section class="grid-2" id="about" aria-label="About and contact">
      <div class="card">
        <h3>About</h3>
        <p><strong>Bio:</strong> Cyber security. I completed a BE in Cyber Security and am focused on building practical skills in ethical hacking, penetration testing, network security, and forensics. Currently seeking hands-on experience and projects to grow my portfolio.</p>

        <h3 style="margin-top:18px">Education</h3>
        <p class="muted"><strong>BE Cyber Security</strong><br>— (Institution name — update this) — Year of graduation: (update)</p>

        <h3 style="margin-top:18px">Work Experience</h3>
        <p class="muted">None — actively seeking internships and entry-level roles. Will update this section as I gain experience.</p>
      </div>

      <div class="card" id="contact" aria-labelledby="contact-heading">
        <h3 id="contact-heading">Contact</h3>
        <p class="muted">Add your preferred contact details (email, phone, LinkedIn, GitHub) where indicated below.</p>

        <div style="margin-top:10px">
          <p class="muted"><strong>Email</strong><br><span id="emailPlace">praveenv2956.com</span></p>
          <p class="muted"><strong>Phone</strong><br><span id="phonePlace">+91 7904869119</span></p>
          <p class="muted"><strong>Location</strong><br><span id="locPlace">India</span></p>
        </div>

        <hr style="border:none;border-top:1px solid rgba(255,255,255,0.03);margin:14px 0">

        <h4>Quick message</h4>
        <form class="contact" onsubmit="handleContact(event)">
          <input type="text" id="name" placeholder="Your name" required>
          <input type="email" id="email" placeholder="Your email" required>
          <textarea id="message" placeholder="Short message" required></textarea>
          <div style="display:flex;gap:8px">
            <button class="btn" type="submit">Send</button>
            <button class="btn ghost" type="button" onclick="copyEmail()">Copy Email</button>
          </div>
          <p id="formStatus" style="margin:0;color:var(--muted);font-size:13px"></p>
        </form>
      </div>
    </section>

    <!-- Skills -->
    <section id="skills" class="card" aria-label="Skills">
      <h3>Skills & Areas of Expertise</h3>
      <p class="muted">Below are suggested skills based on your field. Edit to match the skills you actually possess.</p>
      <div class="skill-list" id="skillsList">
        <!-- Default skills: edit/remove as necessary -->
        <div class="skill">Ethical Hacking</div>
        <div class="skill">Penetration Testing</div>
        <div class="skill">Network Security</div>
        <div class="skill">Digital Forensics</div>
        <div class="skill">Linux</div>
        <div class="skill">Wireshark</div>
        <div class="skill">Nmap</div>
        <div class="skill">Metasploit</div>
        <div class="skill">Python scripting</div>
      </div>
    </section>

    <!-- Projects -->
    <section id="projects" aria-label="Projects">
      <h3>Projects</h3>
      <p class="muted">You currently indicated no projects. Add project cards below as you complete them. Example: "Simple web app pentest report", "Network hardening project", "CTF challenges solved".</p>
      <div class="projects" id="projectsGrid">
        <!-- Example placeholder cards -->
        <article class="project" aria-labelledby="proj1">
          <h4 id="proj1">CTF: Web Exploitation (Placeholder)</h4>
          <p class="muted">Brief: Solved a web challenge involving SQL injection and XSS. Documented methodology and fix recommendations.</p>
        </article>

        <article class="project" aria-labelledby="proj2">
          <h4 id="proj2">Network Security Lab (Placeholder)</h4>
          <p class="muted">Brief: Set up a segmented lab environment and practiced traffic analysis using Wireshark and Suricata.</p>
        </article>
      </div>
    </section>

    <!-- Services -->
    <section id="services" class="card" aria-label="Services">
      <h3>Services</h3>
      <p class="muted">Example services you can offer — edit or remove as needed:</p>
      <ul style="margin-top:8px;color:var(--muted)">
        <li>Vulnerability assessment & basic penetration testing (non-destructive)</li>
        <li>Security configuration reviews & network hardening advice</li>
        <li>CTF coaching and beginner pentesting training</li>
        <li>Digital forensics basics and incident triage</li>
      </ul>
    </section>

    <footer>
      <div>© <span id="currentYear"></span> Praveen.V — Built with ♥ for cybersecurity</div>
      <div style="margin-top:8px;color:var(--muted)">Made with a clean, modern design — edit content and images to personalize.</div>
    </footer>
  </div>

  <script>
    // Small interactive behaviors

    // Update year
    document.getElementById('currentYear').textContent = new Date().getFullYear();

    // Download resume (placeholder)
    document.getElementById('downloadResume').addEventListener('click', function(e){
      e.preventDefault();
      // Replace '#' above with the actual resume path, e.g., 'assets/PraveenV_Resume.pdf'
      const url = '#'; 
      if(url === '#'){
        alert('Please replace the resume link (see index.html -> #downloadResume click handler) with your resume file path.');
      } else {
        window.open(url, '_blank');
      }
    });

    // Contact form handler (client-side) - opens mailto as an example
    function handleContact(e){
      e.preventDefault();
      const name = document.getElementById('name').value.trim();
      const email = document.getElementById('email').value.trim();
      const message = document.getElementById('message').value.trim();

      if(!name || !email || !message){
        document.getElementById('formStatus').textContent = 'Please fill all fields.';
        return;
      }

      // Replace with your email address below
      const targetEmail = 'praveenv2956@gmail.com';
      const subject = encodeURIComponent('Portfolio contact: ' + name);
      const body = encodeURIComponent('Name: ' + name + '\\nEmail: ' + email + '\\n\\nMessage:\\n' + message);
      window.location.href = `mailto:${targetEmail}?subject=${subject}&body=${body}`;
      // After this, user will open their default mail client to send the message.
    }

    // Copy email helper (will copy placeholder)
    function copyEmail(){
      const email = 'praveenv2956@gmail.com';
      navigator.clipboard && navigator.clipboard.writeText(email).then(() => {
        alert('Email copied to clipboard: ' + email);
      }, () => {
        alert('Copy failed. Please copy manually: ' + email);
      });
    }

    // Accessibility: simple focus outline for keyboard users
    document.body.addEventListener('keydown', (e) => {
      if(e.key === 'Tab') document.body.classList.add('show-focus');
    });

    // NOTE: Edit the following placeholders to your real values:
    // - Replace profile image src
    // - Replace institution & graduation year
    // - Replace contact email and phone in the Contact card
    // - Replace project placeholders with real projects and add links/reports/screenshots
    // - Remove or modify example skills to match your real skills
  </script>
</body>
</html>
# Praveen-V
