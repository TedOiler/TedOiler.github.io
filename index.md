<!doctype html>
<html lang="en" class="scroll-smooth">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Theodore Ladas — Statistics & Design of Experiments</title>
  <meta name="description" content="PhD in Statistics focusing on Optimal Design of Experiments and Functional Data. Projects, writing, and ways to connect." />
  <meta property="og:title" content="Theodore Ladas — Statistics & DOE" />
  <meta property="og:description" content="PhD in Statistics focusing on Optimal Design of Experiments and Functional Data." />
  <meta property="og:type" content="website" />

  <!-- Tailwind (CDN) -->
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    // Tailwind config: brand color + dark mode via class
    tailwind.config = {
      darkMode: 'class',
      theme: {
        extend: {
          colors: {
            brand: {
              50:'#eef7ff',100:'#d9ecff',200:'#bcdcff',300:'#8fc4ff',400:'#5aa4ff',500:'#2b84ff',600:'#1669e6',700:'#1254b4',800:'#104790',900:'#0f3b75'
            }
          }
        }
      }
    }
  </script>
  <style>
    /* Smooth fade-in for sections */
    .reveal { opacity: 0; transform: translateY(12px); transition: opacity .6s ease, transform .6s ease; }
    .reveal.show { opacity: 1; transform: translateY(0); }
  </style>
</head>
<body class="bg-white text-slate-900 dark:bg-slate-950 dark:text-slate-100 antialiased">
  <!-- Page wrapper -->
  <div class="min-h-screen">
    <!-- Header -->
    <header class="sticky top-0 z-40 backdrop-blur supports-[backdrop-filter]:bg-white/60 dark:supports-[backdrop-filter]:bg-slate-950/60 border-b border-slate-200/60 dark:border-slate-800/60">
      <div class="max-w-5xl mx-auto px-4 sm:px-6">
        <div class="flex items-center justify-between h-14">
          <a href="#" class="font-semibold tracking-tight">Theodore Ladas</a>
          <nav class="hidden sm:flex items-center gap-6 text-sm">
            <a href="#about" class="hover:text-brand-600">About</a>
            <a href="#research" class="hover:text-brand-600">Research</a>
            <a href="#projects" class="hover:text-brand-600">Projects</a>
            <a href="#writing" class="hover:text-brand-600">Writing</a>
          </nav>
          <div class="flex items-center gap-2">
            <button id="themeToggle" class="rounded-xl border border-slate-200 dark:border-slate-800 px-3 py-1.5 text-sm hover:bg-slate-50 dark:hover:bg-slate-900" aria-label="Toggle dark mode">🌓</button>
            <a href="mailto:theodore.ladas@kcl.ac.uk" class="hidden sm:inline-flex items-center rounded-xl bg-brand-600 hover:bg-brand-700 text-white text-sm px-3 py-1.5">Email</a>
          </div>
        </div>
      </div>
    </header>

    <!-- Hero -->
    <section class="max-w-5xl mx-auto px-4 sm:px-6 pt-16 sm:pt-24 pb-10">
      <div class="grid md:grid-cols-5 gap-8 items-center">
        <div class="md:col-span-3">
          <h1 class="text-3xl sm:text-4xl md:text-5xl font-extrabold leading-tight tracking-tight">
            Statistics PhD • Design of Experiments & Functional Data
          </h1>
          <p class="mt-4 text-lg text-slate-600 dark:text-slate-300">
            I work on optimal design of experiments, causality-adjacent questions, and clean, reproducible code. Splitting time between Athens and London.
          </p>
          <div class="mt-6 flex flex-wrap gap-3">
            <a href="https://contratenor.blot.im" class="inline-flex items-center rounded-xl border border-slate-300 dark:border-slate-700 px-4 py-2 hover:shadow-sm">📓 Read my blog</a>
            <a href="https://uk.linkedin.com/in/thodorisladas" class="inline-flex items-center rounded-xl bg-brand-600 hover:bg-brand-700 text-white px-4 py-2">🔗 Connect on LinkedIn</a>
            <a href="#projects" class="inline-flex items-center rounded-xl px-4 py-2 border border-transparent hover:border-slate-300 dark:hover:border-slate-700">🧪 See projects</a>
          </div>
          <div class="mt-4 text-sm text-slate-500 dark:text-slate-400">📍 Athens 🇬🇷 · London 🇬🇧</div>
        </div>
        <div class="md:col-span-2">
          <div class="rounded-2xl border border-slate-200 dark:border-slate-800 p-5 shadow-sm">
            <h2 class="font-semibold">At a glance</h2>
            <ul class="mt-3 space-y-2 text-sm">
              <li class="flex items-start gap-2"><span class="mt-0.5">🎓</span><span>PhD in Statistics (King's College London)</span></li>
              <li class="flex items-start gap-2"><span class="mt-0.5">📈</span><span>Optimal DOE • Functional Data • ML</span></li>
              <li class="flex items-start gap-2"><span class="mt-0.5">🛠️</span><span>Python, R, SQL · Clean experiment tooling</span></li>
              <li class="flex items-start gap-2"><span class="mt-0.5">📬</span><a class="underline hover:no-underline" href="mailto:theodore.ladas@kcl.ac.uk">theodore.ladas@kcl.ac.uk</a></li>
            </ul>
          </div>
        </div>
      </div>
    </section>

    <!-- About -->
    <section id="about" class="max-w-5xl mx-auto px-4 sm:px-6 py-14 border-t border-slate-200/70 dark:border-slate-800/70 reveal">
      <h2 class="text-xl font-semibold">About</h2>
      <p class="mt-3 text-slate-700 dark:text-slate-300 leading-relaxed">
        I'm Theodore Ladas. My research blends classical optimality criteria with modern representation learning for experiment design on complex (often functional) responses. Outside the thesis grind, I like building tidy tooling for experiments and data workflows, and I write about statistics, math, and the craft of coding on my blog.
      </p>
    </section>

    <!-- Research / Publications -->
    <section id="research" class="max-w-5xl mx-auto px-4 sm:px-6 py-14 border-t border-slate-200/70 dark:border-slate-800/70 reveal">
      <div class="flex items-end justify-between">
        <h2 class="text-xl font-semibold">Research</h2>
        <a href="#" class="text-sm text-brand-600 hover:underline" id="pubsToggle">Toggle abstracts</a>
      </div>
      <div id="pubs" class="mt-6 grid gap-4">
        <!-- Filled by JS below; edit the publications[] array to update -->
      </div>
    </section>

    <!-- Projects -->
    <section id="projects" class="max-w-5xl mx-auto px-4 sm:px-6 py-14 border-t border-slate-200/70 dark:border-slate-800/70 reveal">
      <div class="flex items-end justify-between">
        <h2 class="text-xl font-semibold">Projects</h2>
        <a href="https://github.com/TedOiler" class="text-sm text-brand-600 hover:underline">More on GitHub →</a>
      </div>
      <div id="projectsGrid" class="mt-6 grid sm:grid-cols-2 lg:grid-cols-3 gap-5">
        <!-- Cards populated by JS; edit projects[] below -->
      </div>
    </section>

    <!-- Writing -->
    <section id="writing" class="max-w-5xl mx-auto px-4 sm:px-6 py-14 border-t border-slate-200/70 dark:border-slate-800/70 reveal">
      <div class="flex items-end justify-between">
        <h2 class="text-xl font-semibold">Writing</h2>
        <a href="https://contratenor.blot.im" class="text-sm text-brand-600 hover:underline">Open blog →</a>
      </div>
      <p class="mt-3 text-slate-700 dark:text-slate-300">I post essays and notes on <a class="underline hover:no-underline" href="https://contratenor.blot.im">contratenor.blot.im</a>. Here are a few picks:</p>
      <ul id="blogList" class="mt-4 space-y-3">
        <!-- Statically curated links; replace with your posts -->
        <li>
          <a class="group block rounded-xl border border-slate-200 dark:border-slate-800 p-4 hover:bg-slate-50 dark:hover:bg-slate-900" href="https://contratenor.blot.im" target="_blank" rel="noopener">
            <div class="flex items-center justify-between">
              <span class="font-medium">On designing experiments when responses are functions</span>
              <span class="text-xs text-slate-500 group-hover:underline">blog →</span>
            </div>
            <p class="mt-1 text-sm text-slate-600 dark:text-slate-400">Some intuition, trade-offs, and practical heuristics I use.</p>
          </a>
        </li>
        <li>
          <a class="group block rounded-xl border border-slate-200 dark:border-slate-800 p-4 hover:bg-slate-50 dark:hover:bg-slate-900" href="https://contratenor.blot.im" target="_blank" rel="noopener">
            <div class="flex items-center justify-between">
              <span class="font-medium">Notes on optimality criteria (A, D, c, Bayesian)</span>
              <span class="text-xs text-slate-500 group-hover:underline">blog →</span>
            </div>
            <p class="mt-1 text-sm text-slate-600 dark:text-slate-400">A quick map of when/why each criterion shines.</p>
          </a>
        </li>
      </ul>
    </section>

    <!-- Footer -->
    <footer class="border-t border-slate-200/70 dark:border-slate-800/70 py-10 mt-10">
      <div class="max-w-5xl mx-auto px-4 sm:px-6">
        <div class="flex flex-col sm:flex-row items-start sm:items-center justify-between gap-4">
          <div>
            <div class="font-semibold">Theodore Ladas</div>
            <div class="text-sm text-slate-500">Statistics • DOE • Functional Data</div>
          </div>
          <div class="flex flex-wrap gap-3">
            <a href="https://contratenor.blot.im" class="inline-flex items-center rounded-xl border border-slate-300 dark:border-slate-700 px-3 py-1.5 hover:shadow-sm">📓 Blog</a>
            <a href="https://uk.linkedin.com/in/thodorisladas" class="inline-flex items-center rounded-xl border border-slate-300 dark:border-slate-700 px-3 py-1.5 hover:shadow-sm">🔗 LinkedIn</a>
            <a href="https://github.com/TedOiler" class="inline-flex items-center rounded-xl border border-slate-300 dark:border-slate-700 px-3 py-1.5 hover:shadow-sm">💻 GitHub</a>
          </div>
        </div>
        <p class="mt-4 text-xs text-slate-500">Built with a tiny sprinkle of Tailwind. No build step, just one HTML file.</p>
      </div>
    </footer>
  </div>

  <!-- Data (edit these arrays) -->
  <script>
    const publications = [
      {
        title: 'Neural Bayesian Design of Experiments (NBDO)',
        venue: 'preprint / in progress',
        year: '2025',
        links: [
          { label: 'Code', url: 'https://github.com/TedOiler' },
        ],
        abstract: 'A neural-network-assisted framework combining autoencoders with classical DOE criteria for complex, possibly functional, responses.'
      },
      {
        title: 'Optimal design with functional responses',
        venue: 'thesis chapter',
        year: '2025',
        links: [],
        abstract: 'Design criteria and computational recipes when responses are curves; includes efficient summaries and stability concerns.'
      }
    ];

    const projects = [
      {
        title: 'NBDO — neural-network-based DOE',
        description: 'Autoencoders + classical optimality -> robust designs for complex outputs.',
        tags: ['Python','TensorFlow','DOE'],
        url: 'https://github.com/TedOiler'
      },
      {
        title: 'The Lindy List',
        description: 'Community site for jazz social dance parties in Athens.',
        tags: ['Django','Product'],
        url: 'https://github.com/TedOiler'
      },
      {
        title: 'Clean Experiments Toolkit',
        description: 'Tiny helpers for reproducible simulation studies and DOE workflows.',
        tags: ['Python','R','CLI'],
        url: 'https://github.com/TedOiler'
      }
    ];
  </script>

  <!-- JS to render content & interactivity -->
  <script>
    // Dark mode persistence
    const themeToggle = document.getElementById('themeToggle');
    const root = document.documentElement;
    const stored = localStorage.getItem('theme');
    if (stored === 'dark' || (!stored && window.matchMedia('(prefers-color-scheme: dark)').matches)) {
      root.classList.add('dark');
    }
    themeToggle?.addEventListener('click', () => {
      root.classList.toggle('dark');
      localStorage.setItem('theme', root.classList.contains('dark') ? 'dark' : 'light');
    });

    // Reveal on scroll
    const io = new IntersectionObserver((entries) => {
      entries.forEach(e => { if (e.isIntersecting) e.target.classList.add('show'); });
    }, { threshold: 0.1 });
    document.querySelectorAll('.reveal').forEach(el => io.observe(el));

    // Render publications
    const pubsEl = document.getElementById('pubs');
    publications.forEach(p => {
      const card = document.createElement('article');
      card.className = 'rounded-2xl border border-slate-200 dark:border-slate-800 p-5 hover:shadow-sm transition-shadow';
      card.innerHTML = `
        <div class="flex items-start justify-between gap-4">
          <div>
            <h3 class="font-medium">${p.title}</h3>
            <div class="text-sm text-slate-500">${p.venue} · ${p.year}</div>
          </div>
          <div class="flex gap-2">
            ${p.links.map(l => `<a class='text-sm underline hover:no-underline' href='${l.url}' target='_blank' rel='noopener'>${l.label}</a>`).join('')}
          </div>
        </div>
        <p class="mt-3 text-sm text-slate-700 dark:text-slate-300 hidden">${p.abstract}</p>
      `;
      pubsEl.appendChild(card);
    });

    // Toggle abstracts
    document.getElementById('pubsToggle')?.addEventListener('click', (e) => {
      e.preventDefault();
      document.querySelectorAll('#pubs p').forEach(p => p.classList.toggle('hidden'));
    });

    // Render projects
    const grid = document.getElementById('projectsGrid');
    projects.forEach(pr => {
      const a = document.createElement('a');
      a.href = pr.url;
      a.target = '_blank';
      a.rel = 'noopener';
      a.className = 'group block rounded-2xl border border-slate-200 dark:border-slate-800 p-5 hover:shadow-sm hover:-translate-y-0.5 transition-all';
      a.innerHTML = `
        <div class="flex items-start justify-between gap-4">
          <h3 class="font-medium">${pr.title}</h3>
          <span class="text-xs text-slate-500 group-hover:underline">open →</span>
        </div>
        <p class="mt-2 text-sm text-slate-700 dark:text-slate-300">${pr.description}</p>
        <div class="mt-3 flex flex-wrap gap-2">${pr.tags.map(t => `<span class='text-xs px-2 py-1 rounded-md border border-slate-200 dark:border-slate-700'>${t}</span>`).join('')}</div>
      `;
      grid.appendChild(a);
    });
  </script>
</body>
</html>
