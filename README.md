<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="Cybersecurity portfolio about page for a McGill University student focused on SOC and blue-team work." />
  <meta property="og:title" content="Cybersecurity Portfolio — About" />
  <meta property="og:description" content="SOC and blue-team focused portfolio featuring incident response, threat intelligence, governance, risk, and hands-on security labs." />
  <meta property="og:type" content="website" />
  <title>Cybersecurity Portfolio — About</title>
  <link rel="preconnect" href="https://api.fontshare.com" />
  <link href="https://api.fontshare.com/v2/css?f[]=general-sans@400,500,600,700&f[]=cabinet-grotesk@500,700,800&display=swap" rel="stylesheet" />
  <style>
    :root, [data-theme="light"] {
      --text-xs: clamp(0.75rem, 0.7rem + 0.25vw, 0.875rem);
      --text-sm: clamp(0.875rem, 0.8rem + 0.35vw, 1rem);
      --text-base: clamp(1rem, 0.95rem + 0.25vw, 1.125rem);
      --text-lg: clamp(1.125rem, 1rem + 0.75vw, 1.5rem);
      --text-xl: clamp(1.5rem, 1.2rem + 1.25vw, 2.25rem);
      --text-2xl: clamp(2rem, 1.2rem + 2.5vw, 3.75rem);
      --space-1: 0.25rem;
      --space-2: 0.5rem;
      --space-3: 0.75rem;
      --space-4: 1rem;
      --space-5: 1.25rem;
      --space-6: 1.5rem;
      --space-8: 2rem;
      --space-10: 2.5rem;
      --space-12: 3rem;
      --space-16: 4rem;
      --space-20: 5rem;
      --space-24: 6rem;
      --radius-sm: 0.375rem;
      --radius-md: 0.75rem;
      --radius-lg: 1rem;
      --radius-xl: 1.5rem;
      --radius-full: 9999px;
      --transition: 180ms cubic-bezier(0.16, 1, 0.3, 1);
      --font-body: 'General Sans', Inter, sans-serif;
      --font-display: 'Cabinet Grotesk', 'General Sans', sans-serif;
      --color-bg: #0b1220;
      --color-surface: #121a2b;
      --color-surface-2: #182235;
      --color-surface-offset: #1f2b42;
      --color-border: rgba(191, 219, 254, 0.14);
      --color-divider: rgba(191, 219, 254, 0.08);
      --color-text: #e6edf7;
      --color-text-muted: #9fb0ca;
      --color-text-faint: #73839b;
      --color-text-inverse: #09111d;
      --color-primary: #4fd1c5;
      --color-primary-hover: #37b9ac;
      --color-primary-highlight: rgba(79, 209, 197, 0.14);
      --color-blue: #60a5fa;
      --shadow-sm: 0 1px 2px rgba(0,0,0,0.25);
      --shadow-md: 0 12px 32px rgba(0,0,0,0.24);
      --content-default: 1100px;
    }

    [data-theme="light"] {
      --color-bg: #f4f7fb;
      --color-surface: #ffffff;
      --color-surface-2: #edf3fa;
      --color-surface-offset: #e4edf8;
      --color-border: rgba(11, 18, 32, 0.12);
      --color-divider: rgba(11, 18, 32, 0.08);
      --color-text: #0f172a;
      --color-text-muted: #475569;
      --color-text-faint: #64748b;
      --color-text-inverse: #eff6ff;
      --color-primary-highlight: rgba(79, 209, 197, 0.18);
      --shadow-sm: 0 1px 2px rgba(15,23,42,0.08);
      --shadow-md: 0 20px 48px rgba(15,23,42,0.10);
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }
    html { scroll-behavior: smooth; }
    body {
      min-height: 100vh;
      font-family: var(--font-body);
      font-size: var(--text-base);
      line-height: 1.65;
      background:
        radial-gradient(circle at top right, rgba(96,165,250,0.12), transparent 28%),
        radial-gradient(circle at top left, rgba(79,209,197,0.10), transparent 24%),
        var(--color-bg);
      color: var(--color-text);
    }
    a { color: inherit; text-decoration: none; }
    img, svg { max-width: 100%; display: block; }
    button { font: inherit; color: inherit; background: none; border: 0; cursor: pointer; }
    .skip-link {
      position: absolute; left: var(--space-4); top: -40px; z-index: 100;
      background: var(--color-primary); color: var(--color-text-inverse);
      padding: var(--space-2) var(--space-4); border-radius: var(--radius-full);
      transition: top var(--transition);
    }
    .skip-link:focus { top: var(--space-4); }
    :focus-visible { outline: 2px solid var(--color-primary); outline-offset: 3px; border-radius: var(--radius-sm); }

    .container { width: min(calc(100% - 2rem), var(--content-default)); margin: 0 auto; }
    .site-header {
      position: sticky; top: 0; z-index: 20;
      background: color-mix(in srgb, var(--color-bg) 78%, transparent);
      backdrop-filter: blur(16px);
      border-bottom: 1px solid var(--color-divider);
    }
    .nav {
      display: flex; align-items: center; justify-content: space-between;
      min-height: 4.5rem; gap: var(--space-4);
    }
    .brand { display: inline-flex; align-items: center; gap: var(--space-3); font-size: var(--text-sm); font-weight: 600; letter-spacing: 0.03em; }
    .brand-mark {
      width: 2.5rem; height: 2.5rem; padding: 0.55rem;
      border-radius: 0.85rem; border: 1px solid var(--color-border);
      background: linear-gradient(135deg, var(--color-surface-2), var(--color-surface));
      box-shadow: var(--shadow-sm);
    }
    .nav-links { display: flex; align-items: center; gap: var(--space-4); flex-wrap: wrap; }
    .nav-links a { color: var(--color-text-muted); font-size: var(--text-sm); }
    .nav-links a:hover { color: var(--color-text); }
    .theme-toggle {
      display: inline-flex; align-items: center; justify-content: center;
      width: 2.75rem; height: 2.75rem; border-radius: var(--radius-full);
      border: 1px solid var(--color-border); background: var(--color-surface);
    }

    main { padding: clamp(var(--space-12), 9vw, var(--space-24)) 0; }
    .hero {
      display: grid; grid-template-columns: 1.2fr 0.8fr; gap: var(--space-8);
      align-items: stretch;
    }
    .hero-copy, .hero-panel, .card { border: 1px solid var(--color-border); background: color-mix(in srgb, var(--color-surface) 88%, transparent); box-shadow: var(--shadow-md); }
    .hero-copy {
      border-radius: var(--radius-xl);
      padding: clamp(var(--space-8), 5vw, var(--space-16));
    }
    .eyebrow {
      display: inline-flex; align-items: center; gap: var(--space-2);
      padding: var(--space-2) var(--space-3); margin-bottom: var(--space-5);
      border-radius: var(--radius-full); background: var(--color-primary-highlight);
      color: var(--color-primary); font-size: var(--text-xs); font-weight: 700; letter-spacing: 0.08em; text-transform: uppercase;
    }
    h1 {
      font-family: var(--font-display); font-size: var(--text-2xl); line-height: 0.98;
      letter-spacing: -0.04em; max-width: 12ch;
    }
    .lede {
      margin-top: var(--space-5); color: var(--color-text-muted); max-width: 62ch;
    }
    .cta-row {
      display: flex; gap: var(--space-3); flex-wrap: wrap; margin-top: var(--space-8);
    }
    .btn {
      display: inline-flex; align-items: center; gap: var(--space-2);
      min-height: 44px; padding: 0.85rem 1.1rem; border-radius: var(--radius-full);
      font-size: var(--text-sm); font-weight: 600; transition: transform var(--transition), background var(--transition), border-color var(--transition);
      border: 1px solid transparent;
    }
    .btn:hover { transform: translateY(-1px); }
    .btn-primary { background: var(--color-primary); color: var(--color-text-inverse); }
    .btn-primary:hover { background: var(--color-primary-hover); }
    .btn-secondary { background: var(--color-surface-2); border-color: var(--color-border); }

    .hero-panel {
      border-radius: var(--radius-xl);
      padding: clamp(var(--space-6), 4vw, var(--space-10));
      display: grid; gap: var(--space-4); align-content: start;
    }
    .panel-grid { display: grid; gap: var(--space-4); }
    .mini-stat {
      padding: var(--space-4); border-radius: var(--radius-lg);
      background: var(--color-surface-2); border: 1px solid var(--color-border);
    }
    .mini-stat strong { display: block; font-size: var(--text-lg); font-family: var(--font-display); }
    .mini-stat span { color: var(--color-text-muted); font-size: var(--text-sm); }

    .section {
      padding-top: clamp(var(--space-12), 8vw, var(--space-20));
      display: grid; gap: var(--space-6);
    }
    .section-heading { display: grid; gap: var(--space-3); max-width: 65ch; }
    .section-heading h2 {
      font-family: var(--font-display); font-size: var(--text-xl); line-height: 1.05; letter-spacing: -0.03em;
    }
    .section-heading p { color: var(--color-text-muted); }

    .about-grid, .highlights-grid {
      display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: var(--space-6);
    }
    .card {
      border-radius: var(--radius-xl); padding: clamp(var(--space-6), 3vw, var(--space-8));
      background: color-mix(in srgb, var(--color-surface) 92%, transparent);
    }
    .card h3 {
      font-size: var(--text-lg); font-family: var(--font-display); line-height: 1.1; letter-spacing: -0.02em;
      margin-bottom: var(--space-3);
    }
    .card p { color: var(--color-text-muted); }
    .stack { display: grid; gap: var(--space-4); }
    .tags { display: flex; flex-wrap: wrap; gap: var(--space-2); margin-top: var(--space-4); }
    .tag {
      padding: 0.45rem 0.75rem; border-radius: var(--radius-full); font-size: var(--text-xs);
      color: var(--color-blue); background: rgba(96,165,250,0.12); border: 1px solid rgba(96,165,250,0.18);
    }
    .timeline { list-style: none; display: grid; gap: var(--space-4); }
    .timeline li {
      padding-left: var(--space-5); position: relative; color: var(--color-text-muted);
      border-left: 1px solid var(--color-divider); margin-left: var(--space-2);
    }
    .timeline li::before {
      content: ''; position: absolute; left: -0.4rem; top: 0.4rem; width: 0.75rem; height: 0.75rem;
      border-radius: 50%; background: var(--color-primary); box-shadow: 0 0 0 6px var(--color-primary-highlight);
    }
    .timeline strong { color: var(--color-text); display: block; margin-bottom: 0.25rem; }

    .footer {
      padding: var(--space-12) 0 var(--space-8);
      color: var(--color-text-faint); font-size: var(--text-sm);
    }

    @media (max-width: 900px) {
      .hero, .about-grid, .highlights-grid { grid-template-columns: 1fr; }
      h1 { max-width: 14ch; }
    }

    @media (max-width: 640px) {
      .nav { align-items: flex-start; padding: var(--space-3) 0; }
      .nav, .nav-links { flex-direction: column; }
      .cta-row { flex-direction: column; align-items: stretch; }
      .btn { justify-content: center; }
    }

    @media (prefers-reduced-motion: reduce) {
      html { scroll-behavior: auto; }
      *, *::before, *::after { animation-duration: 0.01ms !important; transition-duration: 0.01ms !important; }
    }
  </style>
</head>
<body>
  <a class="skip-link" href="#content">Skip to content</a>
  <header class="site-header">
    <div class="container nav">
      <a class="brand" href="#top" aria-label="Portfolio home">
        <span class="brand-mark" aria-hidden="true">
          <svg viewBox="0 0 64 64" fill="none" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Shield logo">
            <path d="M32 6L50 13V28C50 39.5 42.8 50.2 32 56C21.2 50.2 14 39.5 14 28V13L32 6Z" stroke="currentColor" stroke-width="4"/>
            <path d="M24 31L29.5 36.5L40.5 25.5" stroke="currentColor" stroke-width="4" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </span>
        <span>Cybersecurity Portfolio</span>
      </a>
      <nav class="nav-links" aria-label="Primary">
        <a href="#about">About</a>
        <a href="#focus">Focus</a>
        <a href="#experience">Experience</a>
        <button class="theme-toggle" type="button" data-theme-toggle aria-label="Switch theme">
          <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" aria-hidden="true">
            <path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"></path>
          </svg>
        </button>
      </nav>
    </div>
  </header>

  <main id="content" class="container">
    <section class="hero" id="top">
      <div class="hero-copy">
        <div class="eyebrow">SOC • Blue Team • Incident Response</div>
        <h1>About this cybersecurity portfolio.</h1>
        <p class="lede">
          I am a cybersecurity student at McGill University focused on Security Operations Center (SOC) and blue-team work. My coursework and labs span threat intelligence, incident response, governance and risk, and hands-on lab work with tools like Nmap, Wireshark, ELK Stack, Kali Linux, and Metasploit.
        </p>
        <p class="lede">
          I also work as a Security Screening Officer in a high-security airport environment, which has strengthened my discipline around procedures, documentation, and escalation. This portfolio highlights selected academic projects and labs that show how I analyze incidents, design security policies, and work through practical detection and response workflows.
        </p>
        <div class="cta-row">
          <a class="btn btn-primary" href="#about">Read the overview</a>
          <a class="btn btn-secondary" href="#experience">View strengths</a>
        </div>
      </div>

      <aside class="hero-panel" aria-label="Profile summary">
        <div class="panel-grid">
          <div class="mini-stat">
            <strong>McGill University</strong>
            <span>Cybersecurity student with a defensive security focus.</span>
          </div>
          <div class="mini-stat">
            <strong>SOC mindset</strong>
            <span>Detection, triage, escalation, documentation, and response.</span>
          </div>
          <div class="mini-stat">
            <strong>Hands-on labs</strong>
            <span>Nmap, Wireshark, ELK Stack, Kali Linux, and Metasploit.</span>
          </div>
        </div>
      </aside>
    </section>

    <section class="section" id="about">
      <div class="section-heading">
        <h2>Professional profile</h2>
        <p>This section is written to work well as an About block in a GitHub portfolio repository, personal site, or README-driven project showcase.</p>
      </div>
      <div class="about-grid">
        <article class="card stack">
          <div>
            <h3>Who I am</h3>
            <p>I am a cybersecurity student at McGill University with a strong interest in blue-team operations, security monitoring, and incident handling. I am especially motivated by work that improves visibility, response readiness, and operational discipline in security environments.</p>
          </div>
          <div class="tags" aria-label="Core topics">
            <span class="tag">Threat Intelligence</span>
            <span class="tag">Incident Response</span>
            <span class="tag">Governance & Risk</span>
            <span class="tag">Detection Workflows</span>
          </div>
        </article>
        <article class="card stack" id="focus">
          <div>
            <h3>Technical focus</h3>
            <p>My academic work combines structured security concepts with practical lab execution. I use platforms and tools such as Nmap, Wireshark, ELK Stack, Kali Linux, and Metasploit to investigate activity, validate findings, and understand how attacks are detected and contained.</p>
          </div>
          <div class="tags" aria-label="Tools used">
            <span class="tag">Nmap</span>
            <span class="tag">Wireshark</span>
            <span class="tag">ELK Stack</span>
            <span class="tag">Kali Linux</span>
            <span class="tag">Metasploit</span>
          </div>
        </article>
      </div>
    </section>

    <section class="section" id="experience">
      <div class="section-heading">
        <h2>What this portfolio demonstrates</h2>
        <p>The content is framed to emphasize operational thinking, communication, and technical depth without sounding generic.</p>
      </div>
      <div class="highlights-grid">
        <article class="card">
          <h3>Operational discipline</h3>
          <p>Working as a Security Screening Officer in a high-security airport environment has reinforced habits that matter in security operations: following procedure, documenting clearly, escalating appropriately, and staying consistent in high-pressure settings.</p>
        </article>
        <article class="card">
          <h3>Applied analysis</h3>
          <p>The projects highlighted here are selected to show how I approach real incidents, move from observation to assessment, and translate findings into practical response actions or policy recommendations.</p>
        </article>
      </div>
      <article class="card">
        <h3>Suggested GitHub README version</h3>
        <ul class="timeline" aria-label="About summary bullets">
          <li><strong>Cybersecurity student at McGill University.</strong> Focused on Security Operations Center work, blue-team practice, and practical defensive workflows.</li>
          <li><strong>Hands-on lab experience.</strong> Built coursework and lab skills across threat intelligence, incident response, governance, risk, and core security tooling.</li>
          <li><strong>Operational background.</strong> Current airport security role has strengthened procedure, documentation, accountability, and escalation discipline.</li>
          <li><strong>Portfolio purpose.</strong> Showcases academic projects and labs that demonstrate incident analysis, policy design, and detection-and-response thinking.</li>
        </ul>
      </article>
    </section>

    <footer class="footer">
      <p>Built as a clean, single-file About section suitable for a GitHub repo or personal cybersecurity portfolio.</p>
    </footer>
  </main>

  <script>
    (function () {
      const root = document.documentElement;
      const toggle = document.querySelector('[data-theme-toggle]');
      let theme = window.matchMedia('(prefers-color-scheme: light)').matches ? 'light' : 'dark';
      root.setAttribute('data-theme', theme);

      const renderIcon = () => {
        toggle.innerHTML = theme === 'dark'
          ? '<svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" aria-hidden="true"><path d="M12 3v2M12 19v2M4.22 4.22l1.42 1.42M18.36 18.36l1.42 1.42M3 12h2M19 12h2M4.22 19.78l1.42-1.42M18.36 5.64l1.42-1.42"/><circle cx="12" cy="12" r="4"/></svg>'
          : '<svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" aria-hidden="true"><path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"></path></svg>';
        toggle.setAttribute('aria-label', theme === 'dark' ? 'Switch to light mode' : 'Switch to dark mode');
      };

      renderIcon();
      toggle.addEventListener('click', function () {
        theme = theme === 'dark' ? 'light' : 'dark';
        root.setAttribute('data-theme', theme);
        renderIcon();
      });
    })();
  </script>
</body>
</html>
