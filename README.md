<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="Personal GitHub profile page focused on networking, information security, instrumentation, and electrical technician interests." />
  <meta property="og:title" content="Technical Portfolio | Networking, Security & Electrical Systems" />
  <meta property="og:description" content="A simple personal profile page for GitHub showcasing networking, information security, instrumentation, and electrical interests." />
  <title>Technical Portfolio</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;700&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
  <style>
    :root, [data-theme="light"] {
      --text-xs: clamp(0.75rem, 0.7rem + 0.25vw, 0.875rem);
      --text-sm: clamp(0.875rem, 0.8rem + 0.35vw, 1rem);
      --text-base: clamp(1rem, 0.95rem + 0.25vw, 1.125rem);
      --text-lg: clamp(1.125rem, 1rem + 0.75vw, 1.5rem);
      --text-xl: clamp(1.5rem, 1.2rem + 1.25vw, 2.25rem);
      --text-2xl: clamp(2rem, 1.2rem + 2.5vw, 3.5rem);
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
      --radius-sm: 0.375rem;
      --radius-md: 0.5rem;
      --radius-lg: 0.75rem;
      --radius-xl: 1rem;
      --radius-full: 9999px;
      --color-bg: #f4f6f4;
      --color-surface: #fbfcfb;
      --color-surface-2: #eef2ef;
      --color-border: rgba(19, 34, 29, 0.12);
      --color-text: #14201c;
      --color-text-muted: #5f6c66;
      --color-text-faint: #87918d;
      --color-primary: #0d6b64;
      --color-primary-hover: #0a5651;
      --color-primary-highlight: #d5e7e4;
      --color-accent: #b87427;
      --shadow-sm: 0 8px 24px rgba(20, 32, 28, 0.06);
      --shadow-md: 0 18px 40px rgba(20, 32, 28, 0.1);
      --content: 1120px;
      --font-display: 'Space Grotesk', 'Inter', sans-serif;
      --font-body: 'Inter', sans-serif;
      --transition-interactive: 180ms cubic-bezier(0.16, 1, 0.3, 1);
    }

    [data-theme="dark"] {
      --color-bg: #101413;
      --color-surface: #161c1a;
      --color-surface-2: #1d2522;
      --color-border: rgba(220, 232, 227, 0.12);
      --color-text: #e4ece8;
      --color-text-muted: #a5b2ac;
      --color-text-faint: #7d8884;
      --color-primary: #69b5af;
      --color-primary-hover: #86c7c1;
      --color-primary-highlight: rgba(105, 181, 175, 0.14);
      --color-accent: #d8a15d;
      --shadow-sm: 0 10px 26px rgba(0, 0, 0, 0.24);
      --shadow-md: 0 20px 50px rgba(0, 0, 0, 0.34);
    }

    @media (prefers-color-scheme: dark) {
      :root:not([data-theme]) {
        --color-bg: #101413;
        --color-surface: #161c1a;
        --color-surface-2: #1d2522;
        --color-border: rgba(220, 232, 227, 0.12);
        --color-text: #e4ece8;
        --color-text-muted: #a5b2ac;
        --color-text-faint: #7d8884;
        --color-primary: #69b5af;
        --color-primary-hover: #86c7c1;
        --color-primary-highlight: rgba(105, 181, 175, 0.14);
        --color-accent: #d8a15d;
        --shadow-sm: 0 10px 26px rgba(0, 0, 0, 0.24);
        --shadow-md: 0 20px 50px rgba(0, 0, 0, 0.34);
      }
    }

    *, *::before, *::after { box-sizing: border-box; }
    html { scroll-behavior: smooth; -webkit-text-size-adjust: 100%; text-size-adjust: 100%; }
    body {
      margin: 0;
      min-height: 100vh;
      font-family: var(--font-body);
      font-size: var(--text-base);
      line-height: 1.6;
      color: var(--color-text);
      background:
        radial-gradient(circle at top right, rgba(13, 107, 100, 0.09), transparent 26%),
        radial-gradient(circle at bottom left, rgba(184, 116, 39, 0.08), transparent 22%),
        var(--color-bg);
    }
    img { max-width: 100%; display: block; }
    a { color: inherit; }
    button { font: inherit; }
    :focus-visible { outline: 2px solid var(--color-primary); outline-offset: 3px; border-radius: var(--radius-sm); }
    .skip-link {
      position: absolute; left: -999px; top: var(--space-4); background: var(--color-surface); color: var(--color-text);
      padding: var(--space-3) var(--space-4); z-index: 1000; border-radius: var(--radius-md); border: 1px solid var(--color-border);
    }
    .skip-link:focus { left: var(--space-4); }
    .container { width: min(calc(100% - 2rem), var(--content)); margin: 0 auto; }
    .site-header {
      position: sticky; top: 0; z-index: 20; backdrop-filter: blur(14px);
      background: color-mix(in srgb, var(--color-bg) 86%, transparent); border-bottom: 1px solid var(--color-border);
    }
    .site-header__inner { display: flex; align-items: center; justify-content: space-between; gap: var(--space-4); padding: var(--space-4) 0; }
    .brand { display: inline-flex; align-items: center; gap: var(--space-3); text-decoration: none; font-weight: 600; }
    .brand svg { width: 36px; height: 36px; color: var(--color-primary); }
    .brand span { font-size: var(--text-sm); letter-spacing: 0.08em; text-transform: uppercase; }
    .header-actions { display: flex; align-items: center; gap: var(--space-3); }
    .theme-toggle {
      min-width: 44px; min-height: 44px; border-radius: var(--radius-full); border: 1px solid var(--color-border);
      background: var(--color-surface); color: var(--color-text); display: inline-flex; align-items: center; justify-content: center; box-shadow: var(--shadow-sm);
    }
    .hero { padding: clamp(var(--space-12), 9vw, var(--space-20)) 0 var(--space-12); }
    .hero-grid { display: grid; gap: var(--space-8); align-items: center; }
    .eyebrow {
      display: inline-flex; align-items: center; gap: var(--space-2); padding: var(--space-2) var(--space-3); border-radius: var(--radius-full);
      background: var(--color-primary-highlight); color: var(--color-primary); font-size: var(--text-xs); font-weight: 700; letter-spacing: 0.08em; text-transform: uppercase; margin-bottom: var(--space-4);
    }
    h1, h2 { font-family: var(--font-display); letter-spacing: -0.04em; margin: 0; }
    h1 { font-size: var(--text-2xl); max-width: 11ch; margin-bottom: var(--space-4); }
    .hero p { color: var(--color-text-muted); max-width: 62ch; margin: 0 0 var(--space-6); }
    .hero-actions { display: flex; flex-wrap: wrap; gap: var(--space-3); }
    .button {
      min-height: 44px; padding: 0.8rem 1.15rem; border-radius: var(--radius-full); text-decoration: none; font-size: var(--text-sm); font-weight: 600;
      display: inline-flex; align-items: center; justify-content: center; border: 1px solid transparent;
    }
    .button--primary { background: var(--color-primary); color: #f8fbfa; }
    .button--primary:hover { background: var(--color-primary-hover); }
    .button--secondary { background: var(--color-surface); border-color: var(--color-border); color: var(--color-text); }
    .button--secondary:hover { background: var(--color-surface-2); }
    .portrait-card {
      justify-self: end; width: min(100%, 340px); background: linear-gradient(180deg, var(--color-surface), var(--color-surface-2));
      border: 1px solid var(--color-border); border-radius: calc(var(--radius-xl) + 0.4rem); padding: var(--space-4); box-shadow: var(--shadow-md);
    }
    .portrait-frame {
      position: relative; overflow: hidden; border-radius: var(--radius-xl); aspect-ratio: 4 / 4.6; background: var(--color-surface-2); border: 1px solid var(--color-border);
    }
    .portrait-frame img { width: 100%; height: 100%; object-fit: cover; object-position: center top; }
    .portrait-meta {
      display: flex; justify-content: space-between; gap: var(--space-3); margin-top: var(--space-4); color: var(--color-text-muted); font-size: var(--text-xs); text-transform: uppercase; letter-spacing: 0.08em;
    }
    .section { padding: var(--space-8) 0; }
    .section-heading { display: grid; gap: var(--space-3); margin-bottom: var(--space-6); }
    .section-heading h2 { font-size: var(--text-xl); }
    .section-heading p { color: var(--color-text-muted); max-width: 58ch; margin: 0; }
    .grid { display: grid; gap: var(--space-4); }
    .cards-3 { grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); }
    .card {
      background: var(--color-surface); border: 1px solid var(--color-border); border-radius: var(--radius-xl); padding: var(--space-5); box-shadow: var(--shadow-sm); content-visibility: auto;
    }
    .card h3 { margin: 0 0 var(--space-3); font-size: var(--text-lg); }
    .card p, .card li { color: var(--color-text-muted); margin: 0; }
    .stat-line {
      display: inline-flex; align-items: center; gap: var(--space-2); color: var(--color-accent); font-size: var(--text-xs); font-weight: 700; text-transform: uppercase; letter-spacing: 0.08em; margin-bottom: var(--space-3);
    }
    .highlight { display: grid; gap: var(--space-4); grid-template-columns: 1.2fr 0.8fr; align-items: stretch; }
    .highlight-panel {
      background: linear-gradient(180deg, var(--color-surface), var(--color-surface-2)); border: 1px solid var(--color-border); border-radius: var(--radius-xl); padding: var(--space-6); box-shadow: var(--shadow-sm);
    }
    .bullet-list { list-style: none; padding: 0; margin: 0; display: grid; gap: var(--space-3); }
    .bullet-list li { display: grid; grid-template-columns: 14px 1fr; gap: var(--space-3); align-items: start; }
    .bullet-list li::before {
      content: ""; width: 10px; height: 10px; margin-top: 0.45rem; border-radius: 50%; background: var(--color-primary);
      box-shadow: 0 0 0 6px color-mix(in srgb, var(--color-primary) 16%, transparent);
    }
    .tag-row { display: flex; flex-wrap: wrap; gap: var(--space-2); margin-top: var(--space-4); }
    .tag {
      padding: 0.45rem 0.8rem; border-radius: var(--radius-full); background: var(--color-surface-2); border: 1px solid var(--color-border);
      font-size: var(--text-xs); font-weight: 600; color: var(--color-text-muted); letter-spacing: 0.03em;
    }
    .footer { padding: var(--space-12) 0 var(--space-8); color: var(--color-text-muted); }
    .footer-card {
      display: flex; flex-wrap: wrap; align-items: center; justify-content: space-between; gap: var(--space-4); padding: var(--space-5);
      background: var(--color-surface); border: 1px solid var(--color-border); border-radius: var(--radius-xl); box-shadow: var(--shadow-sm);
    }
    @media (min-width: 860px) { .hero-grid { grid-template-columns: minmax(0, 1.15fr) minmax(280px, 0.85fr); } }
    @media (max-width: 859px) { .portrait-card { justify-self: start; } .highlight { grid-template-columns: 1fr; } }
    @media (max-width: 620px) {
      .site-header__inner { align-items: flex-start; flex-direction: column; }
      .header-actions { width: 100%; justify-content: space-between; }
      h1 { max-width: 100%; }
      .hero { padding-top: var(--space-10); }
    }
    @media (prefers-reduced-motion: reduce) {
      *, *::before, *::after { scroll-behavior: auto !important; transition-duration: 0.01ms !important; animation-duration: 0.01ms !important; }
    }
  </style>
</head>
<body>
  <a class="skip-link" href="#main-content">Skip to content</a>
  <header class="site-header">
    <div class="container site-header__inner">
      <a class="brand" href="#top" aria-label="Back to top">
        <svg viewBox="0 0 48 48" fill="none" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
          <rect x="4" y="8" width="16" height="32" rx="4" stroke="currentColor" stroke-width="3"/>
          <path d="M20 16H31C36.523 16 41 20.477 41 26V26C41 31.523 36.523 36 31 36H20" stroke="currentColor" stroke-width="3" stroke-linecap="round"/>
          <path d="M10 16V32" stroke="currentColor" stroke-width="3" stroke-linecap="round"/>
          <circle cx="31" cy="26" r="3" fill="currentColor"/>
        </svg>
        <span>Network • Security • Systems</span>
      </a>
      <div class="header-actions">
        <a class="button button--secondary" href="#focus">View focus areas</a>
        <button class="theme-toggle" type="button" data-theme-toggle aria-label="Switch color theme">
          <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" aria-hidden="true">
            <path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"></path>
          </svg>
        </button>
      </div>
    </div>
  </header>
  <main id="main-content">
    <section class="hero container" id="top">
      <div class="hero-grid">
        <div>
          <span class="eyebrow">Technical profile</span>
          <h1>Networking, security, and industrial systems with a hands-on mindset.</h1>
          <p>
            I am building a career around networking and information security while staying closely connected to instrumentation, electrical troubleshooting, and reliable field systems. This page is designed as a clean public GitHub profile landing page that highlights technical direction, interests, and practical strengths.
          </p>
          <div class="hero-actions">
            <a class="button button--primary" href="#projects">Explore strengths</a>
            <a class="button button--secondary" href="#contact">GitHub-ready layout</a>
          </div>
        </div>
        <aside class="portrait-card" aria-label="Profile headshot card">
          <div class="portrait-frame">
            <img src="./profile.jpeg" alt="Professional headshot" width="600" height="690" loading="lazy" decoding="async" />
          </div>
          <div class="portrait-meta">
            <span>Public profile</span>
            <span>Tech + field systems</span>
          </div>
        </aside>
      </div>
    </section>
    <section class="section container" id="focus">
      <div class="section-heading">
        <h2>Core focus areas</h2>
        <p>These sections frame the mix of digital infrastructure knowledge and real-world technical interest that makes the page feel specific to your background.</p>
      </div>
      <div class="grid cards-3">
        <article class="card">
          <div class="stat-line">01 • Networking</div>
          <h3>Network foundations</h3>
          <p>Interest in routing, switching, structured troubleshooting, connectivity planning, and the systems thinking needed to keep infrastructure stable and efficient.</p>
        </article>
        <article class="card">
          <div class="stat-line">02 • InfoSec</div>
          <h3>Security mindset</h3>
          <p>Focused on secure design, defensive thinking, risk awareness, access control, and the habit of looking for weaknesses before they become problems.</p>
        </article>
        <article class="card">
          <div class="stat-line">03 • Electrical</div>
          <h3>Instrumentation & controls</h3>
          <p>Strong interest in instrumentation, electrical systems, troubleshooting logic, and the connection between digital systems and physical equipment.</p>
        </article>
      </div>
    </section>
    <section class="section container" id="projects">
      <div class="highlight">
        <article class="highlight-panel">
          <div class="section-heading" style="margin-bottom: 1rem;">
            <h2>What I bring</h2>
            <p>A balanced profile that combines structured IT knowledge with curiosity about industrial and electrical environments.</p>
          </div>
          <ul class="bullet-list">
            <li><span>Clear interest in networking and information security principles</span></li>
            <li><span>Hands-on mindset suited for diagnostics, maintenance, and troubleshooting</span></li>
            <li><span>Curiosity about control systems, instrumentation signals, and electrical workflows</span></li>
            <li><span>Strong fit for projects where reliability, safety, and system awareness matter</span></li>
          </ul>
        </article>
        <aside class="highlight-panel">
          <div class="stat-line">Technical themes</div>
          <h3 style="margin-top:0; margin-bottom: 0.75rem; font-size: var(--text-lg);">Keywords for your GitHub page</h3>
          <p style="margin:0; color: var(--color-text-muted);">Use these as section anchors, repo topics, or pinned project language to keep your public profile consistent.</p>
          <div class="tag-row" aria-label="Technical interests tags">
            <span class="tag">Network Security</span>
            <span class="tag">Routing & Switching</span>
            <span class="tag">Cyber Defense</span>
            <span class="tag">Instrumentation</span>
            <span class="tag">Electrical Systems</span>
            <span class="tag">Industrial Tech</span>
            <span class="tag">Troubleshooting</span>
            <span class="tag">Systems Reliability</span>
          </div>
        </aside>
      </div>
    </section>
    <section class="section container" id="chameleon">
      <div class="highlight">
        <article class="highlight-panel">
          <div class="section-heading" style="margin-bottom: 1rem;">
            <h2>Chameleon corner</h2>
          </div>
          <p style="margin:0; color: var(--color-text-muted); max-width: 58ch;">
            Chunk the chameleon loved her figs,
            Fat on sugar, thick on twigs.
            Flies were easy—life was sweet,
            ’Til one day there was no treat.
            Hungry, heavy, off she crept,
            To hunt where leaner hunters leapt.
            Crickets taught her how to move,
            Miss, then learn, then slowly improve.
            Now flies are snacks, not all she knows—
            She climbs, she hunts, her strength still grows.
            Soft and round, yet wise and free:
            Don’t let comfort still your tree.
          </p>
          <div class="tag-row" aria-label="Chameleon section tags">
            <span class="tag">Personal Interest</span>
            <span class="tag">Reptile Care</span>
            <span class="tag">Profile Detail</span>
          </div>
        </article>
        <aside class="highlight-panel">
          <img src="./chameleon.jpeg" alt="Chameleon perched on a branch" width="800" height="533" loading="lazy" decoding="async" style="width:100%; border-radius: var(--radius-lg); border: 1px solid var(--color-border); margin-bottom: var(--space-4); object-fit: cover; aspect-ratio: 16 / 10;">
        </aside>
      </div>
    </section>
  </main>
  <footer class="footer container">
    <div class="footer-card">
      <div>
        <strong style="display:block; margin-bottom: 0.35rem;">Technical profile page</strong>
        <span>Have a great Day! Thank you for taking the time to view my profile.</span>
      </div>
      <span style="font-size: var(--text-xs); text-transform: uppercase; letter-spacing: 0.08em;">Static HTML • Mobile friendly • Dark mode</span>
    </div>
  </footer>
  <script>
    (function () {
      const toggle = document.querySelector('[data-theme-toggle]');
      const root = document.documentElement;
      let theme = window.matchMedia('(prefers-color-scheme: dark)').matches ? 'dark' : 'light';
      function renderIcon(mode) {
        return mode === 'dark'
          ? '<svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" aria-hidden="true"><circle cx="12" cy="12" r="5"></circle><path d="M12 1v2M12 21v2M4.22 4.22l1.42 1.42M18.36 18.36l1.42 1.42M1 12h2M21 12h2M4.22 19.78l1.42-1.42M18.36 5.64l1.42-1.42"></path></svg>'
          : '<svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" aria-hidden="true"><path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"></path></svg>';
      }
      function applyTheme(mode) {
        root.setAttribute('data-theme', mode);
        toggle.setAttribute('aria-label', mode === 'dark' ? 'Switch to light mode' : 'Switch to dark mode');
        toggle.innerHTML = renderIcon(mode);
      }
      applyTheme(theme);
      toggle.addEventListener('click', function () {
        theme = theme === 'dark' ? 'light' : 'dark';
        applyTheme(theme);
      });
    })();
  </script>
</body>
</html>
