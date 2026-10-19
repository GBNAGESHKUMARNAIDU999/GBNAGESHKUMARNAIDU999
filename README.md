<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>GBNAGESHKUMARNAIDU999 - Portfolio & GitHub</title>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=DM+Mono:wght@400;500&family=Manrope:wght@400;500;600;700;800&display=swap" rel="stylesheet" />
  <style>
    :root{
      --bg:#070a12; --panel:rgba(16,22,37,.72); --text:#f4f7ff; --muted:#9aa8c2; --line:rgba(182,205,255,.16);
      --cyan:#65e5ff; --violet:#a88bff; --lime:#b8ff72; --orange:#ffa566;
    }
    *,*::before,*::after{box-sizing:border-box;html{scroll-behavior:smooth}}
    body{margin:0;background:var(--bg);color:var(--text);font-family:Manrope,Arial,sans-serif;overflow-x:hidden}
    body::before{
      content:"";position:fixed;inset:0;pointer-events:none;
      background:
        radial-gradient(circle at 76% 12%,rgba(82,74,218,.24),transparent 24rem),
        radial-gradient(circle at 8% 54%,rgba(0,215,255,.10),transparent 27rem),
        linear-gradient(rgba(255,255,255,.018) 1px,transparent 1px),
        linear-gradient(90deg,rgba(255,255,255,.018) 1px,transparent 1px);
      background-size:auto,auto,46px 46px,46px 46px
    }
    .progress{position:fixed;z-index:20;top:0;left:0;height:3px;width:0%;background:linear-gradient(90deg,var(--cyan),var(--violet),var(--lime));box-shadow:0 0 18px var(--cyan)}
    .wrap{width:min(1130px,calc(100% - 48px));margin:auto;padding:1rem}
    nav{height:80px;display:flex;align-items:center;justify-content:space-between;position:relative;z-index:4}
    .brand{font:500 12px/1 "DM Mono";letter-spacing:.12em;text-decoration:none;color:var(--text)}
    .brand b{color:var(--cyan)}
    .navlinks{display:flex;gap:20px}
    .navlinks a,.button{font:500 11px "DM Mono";letter-spacing:.08em;text-decoration:none;color:var(--muted);text-transform:uppercase;transition:.2s}
    .navlinks a:hover{color:var(--cyan)}
    .button{display:inline-flex;align-items:center;gap:9px;padding:12px 18px;border:1px solid var(--line);color:var(--text);border-radius:99px;background:rgba(255,255,255,.035);transition:.2s}
    .button:hover{border-color:var(--cyan);transform:translateY(-2px);box-shadow:0 8px 25px rgba(65,222,255,.14)}
    .hero{min-height:300px;display:grid;grid-template-columns:1.15fr .85fr;align-items:center;padding:80px 0 40px;gap:40px;position:relative}
    .eyebrow{color:var(--cyan);font:500 11px "DM Mono";letter-spacing:.13em;text-transform:uppercase;display:flex;align-items:center;gap:8px}
    .eyebrow::before{content:"";width:20px;height:1px;background:currentColor}
    h1{font-size:clamp(2.5rem,5vw,4.5rem);line-height:.95;letter-spacing:-.05em;margin:0 0 20px;max-width:700px}
    h1 em{font-style:normal;color:transparent;background:linear-gradient(100deg,var(--cyan),var(--violet));background-clip:text;-webkit-background-clip:text}
    .lead{color:var(--muted);line-height:1.6;font-size:15px;max-width:560px}
    .hero-actions{display:flex;gap:12px;margin-top:24px;flex-wrap:wrap}
    .primary{background:var(--text);color:#0b0e17;border-color:var(--text);border-radius:6px;padding:12px 20px;transition:.2s}
    .primary:hover{color:#071018;background:var(--cyan);border-color:var(--cyan)}
    .hero-meta{margin-top:30px;display:flex;gap:20px;flex-wrap:wrap}
    .hero-meta div{padding-left:12px;border-left:1px solid var(--line);font-size:14px}
    .orb{width:260px;height:260px;border-radius:50%;margin:auto;border:1px solid rgba(101,229,255,.22);position:relative;background:radial-gradient(circle at 50% 50%,rgba(183,247,255,.12),transparent 40%),radial-gradient(circle at 30% 25%,rgba(151,114,255,.20),transparent 45%);box-shadow:inset 0 0 60px rgba(95,217,255,.08),0 0 50px rgba(92,74,255,.14);animation:float 6s ease-in-out infinite}
    .orb::before,.orb::after{content:"";position:absolute;border-radius:50%;inset:22px;border:1px dashed rgba(167,221,255,.15);animation:spin 20s linear infinite}
    .orb::after{inset:-16px;animation-direction:reverse;animation-duration:28s}
    .orb span{position:absolute;inset:0;display:grid;place-content:center;text-align:center;font:500 10px/1.6 "DM Mono";letter-spacing:.1em;color:var(--cyan)}
    section{padding:80px 0;border-top:1px solid var(--line)}
    .section-top{display:flex;justify-content:space-between;align-items:flex-end;gap:12px;margin-bottom:30px}
    .number{font:500 10px "DM Mono";color:var(--cyan);letter-spacing:.11em}
    .section-title{font-size:clamp(2rem,3.5vw,3.2rem);letter-spacing:-.04em;margin:8px 0 0}
    .section-note{max-width:280px;color:var(--muted);font-size:12px;line-height:1.6}
    .reveal{opacity:0;transform:translateY(18px);transition:opacity .6s ease,.3s transform ease}
    .reveal.visible{opacity:1;transform:none}
    .grid{display:grid;gap:1.2rem}
    .grid-3{grid-template-columns:repeat(auto-fit,minmax(260px,1fr));grid-auto-flow:dense}
    .card{background:var(--panel);border:1px solid var(--line);border-radius:12px;padding:20px;transition:.3s}
    .card:hover{border-color:rgba(101,229,255,.45);transform:translateY(-4px);box-shadow:0 12px 30px rgba(100,80,255,.12)}
    .card h3{margin:10px 0 6px;font-size:15px;color:var(--cyan)}
    .card p{color:var(--muted);font-size:13px;line-height:1.5;margin:0}
    .tags{font:9px "DM Mono";color:var(--cyan);line-height:1.5;margin-top:8px;padding-top:6px;border-top:1px solid var(--line)}
    .project{position:relative;display:flex;flex-direction:column;gap:8px;padding:20px 24px;border:1px solid var(--line);border-radius:14px;background:linear-gradient(140deg,rgba(18,26,44,.92),rgba(9,13,24,.78));text-decoration:none;color:inherit;overflow:hidden;transition:transform .28s,border-color .28s,box-shadow .28s}
    .project::before{content:"";position:absolute;inset:0;background:radial-gradient(circle at 80% 10%,rgba(101,229,255,.07),transparent 55%);pointer-events:none}
    .project:hover{transform:translateY(-6px);border-color:rgba(168,139,255,.6);box-shadow:0 18px 48px rgba(100,80,255,.16)}
    .project h3{font-size:15px;margin:0 0 4px;letter-spacing:-.03em;line-height:1.2}
    .project p{font-size:11px;color:var(--muted);line-height:1.4;margin:0 0 10px;flex:1}
    .tags{font:8px "DM Mono";color:var(--cyan);line-height:1.5;margin-top:auto;padding-top:8px;border-top:1px solid var(--line)}
    .proj-arrow{position:absolute;top:16px;right:16px;color:var(--cyan);font-size:13px;opacity:.5;transition:opacity .2s,transform .2s}
    .project:hover .proj-arrow{opacity:1;transform:translate(3px,-3px)}
    .project.featured{grid-column:1/-1;flex-direction:row;align-items:center;gap:32px;padding:28px 36px;background:linear-gradient(120deg,rgba(22,32,56,.95),rgba(10,15,30,.85));border-color:rgba(101,229,255,.18)}
    .project.featured h3{font-size:20px;margin-bottom:8px}
    .project.featured p{font-size:13px;max-width:600px;margin-bottom:0}
    .project.featured .tags{border-top:none;padding-top:0;text-align:right}
    .project.featured .feat-badge{font:700 9px "DM Mono";letter-spacing:.12em;color:#0b0e17;background:linear-gradient(90deg,var(--cyan),var(--violet));padding:4px 12px;border-radius:96px;white-space:nowrap}
    .project.featured .proj-arrow{top:50%;transform:translateY(-50%);right:24px;font-size:18px}
    .project.featured:hover .proj-arrow{transform:translateY(-50%) translate(4px,-4px)}
    .skill{background:var(--panel);border:1px solid var(--line);border-radius:10px;padding:18px;transition:.3s;min-height:100px}
    .skill:hover{border-color:rgba(101,229,255,.55);background:#111a2c;transform:translateY(-4px)}
    .skill i{font:10px "DM Mono";color:var(--cyan)}
    .skill h3{margin:10px 0 6px;font-size:14px}
    .skill p{margin:0;color:var(--muted);font-size:12px;line-height:1.5}
    .timeline article{padding:20px;border:1px solid var(--line);border-radius:10px;background:var(--panel)}
    .timeline .year{font:9px "DM Mono";color:var(--lime)}
    .timeline h3{margin:20px 0 5px;font-size:16px;letter-spacing:-.03em}
    .timeline p{margin:0;color:var(--muted);font-size:12px;line-height:1.5}
    .contact{text-align:center;padding:120px 0}
    .contact h2{font-size:clamp(2.5rem,5vw,4rem);line-height:.95;letter-spacing:-.05em;margin:20px auto 20px;max-width:800px}
    .contact h2 span{color:var(--cyan)}
    .contact p{color:var(--muted);font-size:14px;margin-bottom:30px}
    .socials{display:flex;justify-content:center;gap:18px;margin-top:20px}
    .socials a{font:10px "DM Mono";color:var(--muted);text-decoration:none;transition:.2s}
    .socials a:hover{color:var(--cyan)}
    footer{border-top:1px solid var(--line);padding:20px 0;color:var(--muted);font:9px "DM Mono";display:flex;justify-content:space-between}
    .detail-grid{display:grid;grid-template-columns:1fr 1fr;gap:16px;margin:0 0 80px}
    .detail-card{padding:20px;border:1px solid var(--line);border-radius:12px;background:var(--panel}}
    .detail-card h3{margin:10px 0 12px;font-size:15px}
    .detail-card ul{padding:0;margin:0;list-style:none;color:var(--muted);font-size:12px;line-height:1.7}
    .detail-card li::before{content:"+";color:var(--cyan);margin-right:6px;font-family:"DM Mono"}
    .intro{position:fixed;z-index:100;inset:0;background:#050811;display:grid;place-items:center;overflow:hidden;animation:intro-out .8s ease 4.5s forwards}
    .intro::before{content:"";position:absolute;inset:-30%;background:repeating-linear-gradient(0deg,transparent 0 4px,rgba(101,229,255,.04) 4px 5px),radial-gradient(circle,rgba(98,78,255,.35),transparent 34%);animation:scan 2.5s linear infinite}
    .intro-inner{position:relative;text-align:center}
    .intro-kicker{font:10px "DM Mono";color:var(--cyan);letter-spacing:.2em;animation:fade-up .6s both}
    .intro-name{font-size:clamp(2rem,4.5vw,3.5rem);letter-spacing:-.05em;white-space:nowrap;line-height:.85;margin:20px 0;color:white;animation:fade-up .75s .25s both}
    .intro-name span{color:var(--cyan)}
    .loader{height:2px;width:min(280px,65vw);background:rgba(255,255,255,.12);margin:30px auto 15px;overflow:hidden}
    .loader::after{content:"";display:block;width:100%;height:100%;background:linear-gradient(90deg,var(--cyan),var(--violet),var(--lime));transform:translateX(-100%);animation:load 3s .5s ease forwards}
    intro small{font:9px "DM Mono";letter-spacing:.1em;color:var(--muted);animation:fade-up .6s .7s both}
    .skip{position:absolute;right:20px;bottom:18px;border:0;background:transparent;color:#9aa8c2;font:10px "DM Mono";letter-spacing:.1em;cursor:pointer}
    .skip:hover{color:var(--cyan)}
    @keyframes fade-up{from{opacity:0;transform:translateY(15px)}to{opacity:1;transform:none}}
    @keyframes load{to{transform:translateX(0)}}
    @keyframes scan{to{transform:translateY(22px)}}
    @keyframes intro-out{to{opacity:0;visibility:hidden;pointer-events:none}}
    @keyframes float{50%{transform:translateY(-10px)}}
    @keyframes spin{to{transform:rotate(360deg)}}
    @media(max-width:1100px){.grid-3{grid-template-columns:repeat(auto-fit,minmax(220px,1fr))}}
    @media(max-width:900px){.hero{grid-template-columns:1fr}.orb{display:none}.navlinks{display:none}.project.featured{grid-column:auto}.detail-grid{grid-template-columns:1fr}}
    @media(max-width:560px){.wrap{width:min(calc(100% - 34px),1130px)}.hero{padding-top:40px}.contact{padding:80px 0}}
  </style>
</head>
<body>
  <!-- Intro Screen -->
  <div class="intro" id="intro" role="presentation">
    <div class="intro-stage">
      <div class="road"></div>
      <div class="drift-car"><div class="car-shell"></div><i class="wheel rear"></i><i class="wheel front"></i><i class="smoke"></i><i class="smoke s2"></i><i class="smoke s3"></i></div>
    </div>
    <div class="intro-inner">
      <div class="intro-kicker">INITIALISING PORTFOLIO // 2026</div>
      <div class="intro-name">G B NAGESH <span>KUMAR</span></div>
      <div class="loader"></div>
      <small>GENERATIVE AI / DATA / INTELLIGENCE</small>
    </div>
    <button class="skip" type="button" onclick="document.getElementById('intro').remove()">SKIP INTRO</button>
  </div>

  <div class="progress" id="progress"></div>

  <main class="wrap">
    <nav>
      <a class="brand" href="#top">G B <b>NAGESH</b> KUMAR</a>
      <div class="navlinks">
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#work">Work</a>
        <a href="#contact">Contact</a>
      </div>
      <a class="button primary" href="#work">Explore my work</a>
    </nav>

    <!-- Hero with Three.js Canvas -->
    <section class="hero" id="top">
      <div>
        <div class="eyebrow">Bangalore, India / Available for opportunities</div>
        <h1>Building <em>intelligent</em> ideas into useful experiences.</h1>
        <p class="lead">I'm G B Nagesh Kumar, an AI/ML engineer focused on Generative AI, LLM-powered applications, conversational systems, and data-driven problem solving.</p>
        <div class="hero-actions">
          <a class="button primary" href="#work">Explore my work</a>
          <a class="button" href="mailto:gbnageshkumar999@gmail.com">Email me</a>
        </div>
        <div class="hero-meta">
          <div><strong>2025</strong><span>AI/ML Graduate</span></div>
          <div><strong>7.9 / 10</strong><span>BE CGPA</span></div>
          <div><strong>15</strong><span>Projects</span></div>
        </div>
      </div>
      <div class="orb"><span>GEN AI<br/>x<br/>HUMAN CURIOSITY</span></div>
    </section>

    <section id="about">
      <div class="section-top reveal"><div><span class="number">01 / WHO I AM</span><h2 class="section-title">Thoughtful AI,<br/>built to matter.</h2></div><p class="section-note">A fresh engineering perspective grounded in practical application and clear outcomes.</p></div>
      <div class="about reveal"><span class="eyebrow">The short version</span><p>I build <b>context-aware AI experiences</b> that turn natural conversation into helpful outcomes. From styling recommendations to interview prep, I enjoy shaping prompts, flows, and data into products people can actually use.</p></div>
    </section>

    <section id="skills">
      <div class="section-top reveal"><div><span class="number">02 / TOOLKIT</span><h2 class="section-title">Skills with range.</h2></div><p class="section-note">Technical foundations paired with a product-minded approach to solving problems.</p></div>
      <div class="skills">
        <article class="skill reveal"><i>01 / CODE</i><h3>Python & SQL</h3><p>Python, SQL, HTML, CSS, Git, GitHub, and VS Code.</p></article>
        <article class="skill reveal"><i>02 / INTELLIGENCE</i><h3>Generative AI</h3><p>LLMs, prompt engineering, NLP, ML fundamentals, and conversational AI.</p></article>
        <article class="skill reveal"><i>03 / INSIGHT</i><h3>Data Analytics</h3><p>Power BI, Excel, data analysis, visualisation, and reporting.</p></article>
      </div>
    </section>

    <div class="detail-grid reveal" style="margin:0 0 60px">
      <article class="detail-card"><span class="number">TECHNICAL SKILLS</span><h3>Engineering toolkit</h3><ul><li>Programming: Python, SQL, HTML, CSS</li><li>AI/ML: Generative AI, LLMs, Prompt Engineering, NLP & ML Fundamentals</li><li>Data: Power BI, Microsoft Excel, Data Analysis, Visualisation & Reporting</li><li>Tools: Git, GitHub, ChatGPT, Google Bard, VS Code</li></ul></article>
      <article class="detail-card"><span class="number">CORE STRENGTHS</span><h3>How I work</h3><ul><li>Problem-Solving & Analytical Thinking</li><li>Team Collaboration & Adaptability</li><li>Clear Communication</li><li>Business requirement to AI workflow translation</li></ul></article>
    </div>

    <!-- Work/Projects Section -->
    <section id="work">
      <div class="section-top reveal"><div><span class="number">03 / SELECTED WORK</span><h2 class="section-title">Projects in motion.</h2></div><p class="section-note">15 live projects spanning AI, computer vision, web tools, and data-driven applications.</p></div>

      <!-- Featured Project -->
      <a class="project featured" href="https://dark-fashion-ai.lovable.app" target="_blank" rel="noopener noreferrer">
        <span class="proj-arrow">&#x2197;</span>
        <span class="project-index">01 / GEN AI</span>
        <h3>Dark Fashion AI</h3>
        <p>AI-powered virtual styling assistant generating personalized outfit recommendations with LLMs and structured prompt engineering. Context-aware workflows adapt to conversational input.</p>
        <span class="tags">PYTHON / LLMS / PROMPTS</span>
      </a>

      <!-- Projects Grid -->
      <div class="projects reveal" style="margin:24px 0 0;">
        <a class="project" href="https://dark-disiple.lovable.app" target="_blank" rel="noopener noreferrer">
          <span class="proj-arrow">&#x2197;</span>
          <span class="project-index">02 / CONV AI</span>
          <h3>DARK-AI</h3>
          <p>Adaptive conversational assistant delivering analytical, context-aware responses with reusable prompt templates and interaction workflows for consistent on-topic answers.</p>
          <span class="tags">PYTHON / CONVERSATIONAL AI</span>
        </a>
        <a class="project" href="https://dark-smart-questioans-bot.lovable.app" target="_blank" rel="noopener noreferrer">
          <span class="proj-arrow">&#x2197;</span>
          <span class="project-index">03 / PYTHON BOT</span>
          <h3>Dark Smart Questions Bot</h3>
          <p>Python assistant focused on answering Python-related questions, helping users explore concepts and receive useful guidance through an interactive Q&A experience.</p>
          <span class="tags">PYTHON ASSISTANT / LLMS</span>
        </a>
        <a class="project" href="https://colordectordark-gubex7q2zrbhwnoqcj2gva.streamlit.app/" target="_blank" rel="noopener noreferrer">
          <span class="proj-arrow">&#x2197;</span>
          <span class="project-index">04 / COMPUTER VISION</span>
          <h3>AI Color Detector & Tracker</h3>
          <p>Real-time color detection & tracking using OpenCV, FastAPI & Streamlit. K-Means clustering, 200+ named colors, fashion matching, and interior design suggestions.</p>
          <span class="tags">OPENCV / FASTAPI / STREAMLIT</span>
        </a>
        <a class="project" href="https://resumeanaliserdark.netlify.app/" target="_blank" rel="noopener noreferrer">
          <span class="proj-arrow">&#x2197;</span>
          <span class="project-index">05 / AI TOOL</span>
          <h3>AI Resume Analyzer</h3>
          <p>Zero-dependency, browser-only AI resume analyzer. Reads PDF, DOCX & TXT files, scores ATS readiness, and surfaces missing sections — no backend required.</p>
          <span class="tags">VANILLA JS / PDF / ATS SCORING</span>
        </a>
        <a class="project" href="https://playit-playful-forge.lovable.app/" target="_blank" rel="noopener noreferrer">
          <span class="proj-arrow">&#x2197;</span>
          <span class="project-index">06 / MEDIA</span>
          <h3>Play It — Interactive Media Player</h3>
          <p>Playful media player that handles imported video and music, built with Lovable using prompt-driven development. Engaging visual & audio experience.</p>
          <span class="tags">LOVABLE / PROMPTING</span>
        </a>
        <a class="project" href="https://darklawrules.lovable.app" target="_blank" rel="noopener noreferrer">
          <span class="proj-arrow">&#x2197;</span>
          <span class="project-index">07 / SEARCH</span>
          <h3>Dark Law Rules</h3>
          <p>Legal search website providing information on rules and regulations, helping users explore and find relevant legal guidance through a clear, accessible search experience.</p>
          <span class="tags">LEGAL SEARCH / LOVABLE</span>
        </a>
        <a class="project" href="https://stooop.netlify.app/" target="_blank" rel="noopener noreferrer">
          <span class="proj-arrow">&#x2197;</span>
          <span class="project-index">08 / UTILITY</span>
          <h3>Stop Watch</h3>
          <p>Responsive stopwatch with lap tracking. Precise millisecond timing, intuitive controls, automatic lap recording, and a modern gradient interface. Zero dependencies.</p>
          <span class="tags">HTML / CSS / JAVASCRIPT</span>
        </a>
        <a class="project" href="https://darkagecalculator.netlify.app/" target="_blank" rel="noopener noreferrer">
          <span class="proj-arrow">&#x2197;</span>
          <span class="project-index">09 / UTILITY</span>
          <h3>Age Calculator — Age Chronos</h3>
          <p>High-precision age calculator with glassmorphic aesthetic. Years, months, days, real-time seconds counter, and birthday countdown. Zero-dependency vanilla JS.</p>
          <span class="tags">HTML / CSS / VANILLA JS</span>
        </a>
        <a class="project" href="https://lehladakhwebdark.netlify.app/" target="_blank" rel="noopener noreferrer">
          <span class="proj-arrow">&#x2197;</span>
          <span class="project-index">10 / TRAVEL</span>
          <h3>Leh Ladakh Travel Website</h3>
          <p>Premium travel tour website for Leh Ladakh. Stunning visuals, modern animations, and a fully responsive design that brings the beauty of the Himalayas to life.</p>
          <span class="tags">HTML / CSS / ANIMATIONS</span>
        </a>
        <a class="project" href="https://srishivashakathilighting.netlify.app/" target="_blank" rel="noopener noreferrer">
          <span class="proj-arrow">&#x2197;</span>
          <span class="project-index">11 / BUSINESS</span>
          <h3>Sri Shiva Shakathi Lighting</h3>
          <p>Business website for a lighting shop where customers can contact the owner to book lighting and event items. Clean, functional storefront built to convert visitors into clients.</p>
          <span class="tags">HTML / CSS / BUSINESS</span>
        </a>
        <a class="project" href="https://dark-python-ntr-web.netlify.app/" target="_blank" rel="noopener noreferrer">
          <span class="proj-arrow">&#x2197;</span>
          <span class="project-index">12 / TRIBUTE</span>
          <h3>Python Teacher Farewell Tribute</h3>
          <p>Premium farewell tribute website honoring a Python teacher. Modern UI with high-quality visuals, videos, smooth animations, and interactive sections for an emotional experience.</p>
          <span class="tags">HTML / CSS / JAVASCRIPT</span>
        </a>
        <a class="project" href="https://eventcalanderdark.netlify.app/" target="_blank" rel="noopener noreferrer">
          <span class="proj-arrow">&#x2197;</span>
          <span class="project-index">13 / WEB APP</span>
          <h3>EventCal</h3>
          <p>Modern, premium web application for creating, managing, and discovering events. Built with React + Vite, runs entirely in the browser with zero backend.</p>
          <span class="tags">REACT / VITE</span>
        </a>
        <a class="project" href="https://watertrackerdark.netlify.app/" target="_blank" rel="noopener noreferrer">
          <span class="proj-arrow">&#x2197;</span>
          <span class="project-index">14 / WEB APP</span>
          <h3>Water Tracker</h3>
          <p>💧 A sleek, modern React app for tracking daily hydration. Built with Vite and Tailwind CSS, featuring a beautiful dark mode UI, customizable themes, and progress tracking.</p>
          <span class="tags">REACT / TAILWIND</span>
        </a>
        <a class="project" href="https://123dmoduledark.netlify.app/" target="_blank" rel="noopener noreferrer">
          <span class="proj-arrow">&#x2197;</span>
          <span class="project-index">15 / 3D VISUALIZATION</span>
          <h3>Interactive 3D Visualizer</h3>
          <p>Transform 2D images into interactive 3D visualizations. Features dynamic theming, customizable depth scaling, and seamless mode transitions, wrapped in a premium UI.</p>
          <span class="tags">REACT / THREE.JS / TAILWIND</span>
        </a>
      </div>
    </section>

    <section>
      <div class="section-top reveal"><div><span class="number">04 / FOUNDATION</span><h2 class="section-title">Always learning.</h2></div></div>
      <div class="timeline">
        <article class="reveal"><span class="year">2025</span><h3>B.E. in Artificial Intelligence & Machine Learning</h3><p>Visvesvaraya Technological University<br/>CGPA: 7.9 / 10</p></article>
        <article class="reveal"><span class="year">2021</span><h3>Pre-University Course (PCMB - Science)</h3><p>Aditya PU College<br/>76%</p></article>
      </div>
    </section>

    <section id="credentials">
      <div class="section-top reveal"><div><span class="number">05 / CREDENTIALS</span><h2 class="section-title">The full picture.</h2></div><p class="section-note">Every credential and core competency from my professional resume.</p></div>
      <div class="detail-grid">
        <article class="detail-card reveal"><span class="number">CERTIFICATIONS</span><h3>Verified learning</h3><ul><li>Data Analyst Certification - PY SPIDERS</li><li>SQL Certification - PY SPIDERS</li><li>Excel & Power BI Certification - PY SPIDERS</li><li>Python Certification - GUVI</li></ul></article>
        <article class="detail-card reveal"><span class="number">CORE COMPETENCIES</span><h3>What I build for</h3><ul><li>AI-Powered Application Development</li><li>Generative AI Solutions</li><li>Conversational AI Systems</li><li>Data Analytics & Reporting</li><li>Intelligent Automation</li></ul></article>
      </div>
    </section>

    <section id="contact" style="background:var(--bg);padding:80px 0">
      <div class="reveal">
        <span class="number">06 / CONNECT</span>
        <h2>Let's build the future together</h2>
        <p>Bangalore, India. I'm looking for opportunities to learn, contribute, and build meaningful AI products.</p>
        <div class="socials">
          <a href="https://www.linkedin.com/in/g-b-nagesh-kumar-naidu" target="_blank" rel="noreferrer">LINKEDIN &#x2197;</a>
          <a href="https://github.com/GBNAGESHKUMARNAIDU999" target="_blank" rel="noreferrer">GITHUB &#x2197;</a>
          <a href="mailto:gbnageshkumar999@gmail.com">EMAIL &#x2197;</a>
          <a href="tel:+916304559351">+91 63045 59351</a>
        </div>
      </div>
    </section>
    <footer><span>&#169; 2026 G B NAGESH KUMAR</span><span>DESIGNED FOR THE CURIOUS</span></footer>
  </main>

  <!-- Three.js Motion Canvas -->
  <div id="three-canvas" style="position:fixed;inset:0;pointer-events:none;z-index:1"></div>

  <script type="importmap">
    {"imports":{"three":"https://unpkg.com/three@0.160.0/build/three.module.js","three/addons/":"https://unpkg.com/three@0.160.0/examples/jsm/"}}
  </script>

  <script type="module">
    import * as THREE from 'three'
    import { OrbitControls } from 'three/addons/controls/OrbitControls.js'
    import { gsap } from 'https://cdn.skypack.dev/gsap'

    // Scene setup
    const canvas = document.getElementById('three-canvas')
    const scene = new THREE.Scene()
    scene.background = new THREE.Color(0x050811)

    const camera = new THREE.PerspectiveCamera(60, window.innerWidth / window.innerHeight, 0.1, 1000)
    camera.position.set(0, 2, 5)

    const renderer = new THREE.WebGLRenderer({ antialias: true, alpha: true })
    renderer.setSize(window.innerWidth, window.innerHeight)
    renderer.setPixelRatio(Math.min(window.devicePixelRatio, 2))
    canvas.appendChild(renderer.domElement)

    const controls = new OrbitControls(camera, renderer.domElement)
    controls.enableDamping = true
    controls.dampingFactor = 0.05
    controls.maxPolarAngle = Math.PI / 2.3

    // Video texture
    const video = document.createElement('video')
    video.src = 'https://cdn.jsdelivr.net/gh/danleech/animated-loader@1.0.0/atom.gif'
    video.loop = true
    video.muted = true
    video.playsInline = true
    video.autoplay = true
    video.style.display = 'none'

    const videoTex = new THREE.VideoTexture(video)
    videoTex.minFilter = THREE.LinearFilter
    videoTex.magFilter = THREE.LinearFilter
    videoTex.format = THREE.RGBFormat

    // Materials
    const geometry = new THREE.SphereGeometry(1.8, 64, 64)

    // Main mesh with video texture
    const mainMaterial = new THREE.MeshStandardMaterial({ map: videoTex, transparent: true, opacity: 0.9 })
    const mainMesh = new THREE.Mesh(geometry, mainMaterial)
    scene.add(mainMesh)

    // Secondary orbiting meshes
    const mat1 = new THREE.MeshStandardMaterial({ color: 0x65e5ff, transparent: true, opacity: 0.4 })
    const mat2 = new THREE.MeshStandardMaterial({ color: 0xa88bff, transparent: true, opacity: 0.4 })
    const mat3 = new THREE.MeshStandardMaterial({ color: 0xb8ff72, transparent: true, opacity: 0.3 })

    const meshes = []
    for (let i = 0; i < 4; i++) {
      const mesh = new THREE.Mesh(new THREE.IcosahedronGeometry(0.4, 0), i % 2 === 0 ? mat1 : i < 3 ? mat2 : mat3)
      mesh.position.set(
        (Math.random() - 0.5) * 3,
        (Math.random() - 0.5) * 3,
        (Math.random() - 0.5) * 3
      )
      mesh.userData.speed = 0.5 + Math.random() * 0.5
      mesh.userData.rotationSpeed = (Math.random() - 0.5) * 0.3
      scene.add(mesh)
      meshes.push(mesh)
    }

    // Lighting
    const ambient = new THREE.AmbientLight(0x2a3045, 0.6)
    scene.add(ambient)

    const point1 = new THREE.PointLight(0x65e5ff, 0.8)
    point1.position.set(2, 2, 4)
    scene.add(point1)

    const point2 = new THREE.PointLight(0xa88bff, 0.5)
    point2.position.set(-2, -2, 4)
    scene.add(point2)

    const point3 = new THREE.PointLight(0xb8ff72, 0.3)
    point3.position.set(0, -3, 2)
    scene.add(point3)

    // Resize handler
    window.addEventListener('resize', () => {
      camera.aspect = window.innerWidth / window.innerHeight
      camera.updateProjectionMatrix()
      renderer.setSize(window.innerWidth, window.innerHeight)
    })

    // Animation loop
    const clock = new THREE.Clock()

    function animate() {
      requestAnimationFrame(animate)

      const elapsed = clock.getElapsedTime()

      // Rotate main mesh
      mainMesh.rotation.y = elapsed * 0.3
      mainMesh.rotation.x = elapsed * 0.15

      // Orbit meshes
      meshes.forEach((mesh, i) => {
        mesh.rotation.y += mesh.userData.rotationSpeed
        mesh.position.x += Math.sin(elapsed * mesh.userData.speed) * 0.02
        mesh.position.y += Math.cos(elapsed * mesh.userData.speed * 1.1) * 0.02
      })

      controls.update()
      renderer.render(scene, camera)
    }

    // GSAP motion graphics
    gsap.from('.navlinks a', {opacity: 0, y: -20, stagger: 0.1, delay: 0.5})
    gsap.from('.hero h1', {opacity: 0, x: -30, delay: 0.8})
    gsap.from('.hero p', {opacity: 0, x: 30, delay: 0.9})
    gsap.from('.hero-actions .button', {opacity: 0, y: 20, stagger: 0.15, delay: 1})
    gsap.from('.section-title', {opacity: 0, y: 15, stagger: 0.1, delay: 1.2})

    // Intro screen removal
    setTimeout(() => { document.getElementById('intro').style.display = 'none' }, 4500)

    // Start animation
    animate()

    // Play video when page loads
    video.addEventListener('canplay', () => {
      video.play().catch(() => { /* autoplay prevented */ })
    })
  </script>
</body>
</html>
