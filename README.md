<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Arish Islam — README-only Preview</title>
<style>
  :root {
    --ink: #e6edf3;
    --soft: #aab7c4;
    --muted: #718096;
    --cyan: #22d3ee;
    --blue: #60a5fa;
    --purple: #a78bfa;
    --line: rgba(96,165,250,.24);
    --line-purple: rgba(167,139,250,.25);
    --page: #080d18;
  }
  * { box-sizing: border-box; }
  body {
    margin: 0;
    background: var(--page);
    color: var(--ink);
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
  }
  .readme {
    max-width: 1000px;
    margin: 0 auto;
    padding: 24px 26px 30px;
    overflow: hidden;
  }
  .hero {
    text-align: center;
    position: relative;
    padding-bottom: 22px;
  }
  .hero::after {
    content: "";
    position: absolute;
    left: 14%; right: 14%; bottom: 0; height: 1px;
    background: linear-gradient(90deg, transparent, var(--cyan), var(--purple), transparent);
    box-shadow: 0 0 16px rgba(34,211,238,.6);
  }
  .capsule { display: block; width: 100%; height: auto; min-height: 150px; object-fit: cover; }
  .avatar {
    width: 132px; height: 132px; display: block; margin: -40px auto 14px;
    border-radius: 50%; border: 4px solid var(--page); outline: 2px solid var(--cyan);
    box-shadow: 0 0 0 5px rgba(34,211,238,.09), 0 0 34px rgba(34,211,238,.42);
    position: relative;
  }
  h1 {
    margin: 0; font-size: 32px; letter-spacing: 5px; font-weight: 800;
    background: linear-gradient(90deg, #f8fafc 10%, #67e8f9 50%, #c4b5fd 90%);
    -webkit-background-clip: text; background-clip: text; color: transparent;
  }
  .eyebrow { margin: 8px 0 0; color: #dbeafe; font-size: 15px; font-weight: 700; }
  .role { margin-top: 8px; color: #c3d1df; font-size: 14px; letter-spacing: .2px; }
  .typing { width: min(760px, 100%); margin: 18px auto 0; display: block; }
  .links { display: flex; justify-content: center; gap: 9px; flex-wrap: wrap; margin-top: 16px; }
  .links img { height: 27px; }
  .typing-mockup { width: min(760px, 100%); margin: 18px auto 0; color: var(--cyan); font: 600 18px/1.35 "SFMono-Regular", Consolas, monospace; white-space: nowrap; overflow: hidden; text-align: left; animation: typeLine 4.5s steps(35, end) infinite alternate; }
  .typing-mockup i { display: inline-block; width: 9px; height: 21px; margin-left: 4px; vertical-align: -3px; background: var(--purple); animation: blink .9s steps(1) infinite; }
  @keyframes typeLine { from { width: 0; } to { width: 35ch; } }
  @keyframes blink { 50% { opacity: 0; } }
  .section { margin-top: 30px; }
  .section-title {
    display: flex; align-items: center; gap: 12px; margin: 0 0 14px;
    color: var(--cyan); font: 700 14px "SFMono-Regular", Consolas, monospace;
    letter-spacing: .4px;
  }
  .section-title::after { content: ""; height: 1px; flex: 1; background: linear-gradient(90deg, var(--line), transparent); }
  .about { max-width: 840px; margin: 0 auto; text-align: center; color: var(--soft); line-height: 1.75; font-size: 14px; }
  .about strong { color: var(--ink); }
  .stack { text-align: center; }
  .stack-icons { display: flex; justify-content: center; gap: 7px; flex-wrap: wrap; }
  .stack-icons img { height: 29px; }
  .hero-art { display: block; width: 100%; height: auto; }
  .footer-art { display: block; width: 100%; height: auto; }
  .tool-row { display: flex; justify-content: center; gap: 7px; flex-wrap: wrap; }
  .tool-row img { height: 26px; }
  .portfolio-card, .cert-card { display: flex; align-items: center; justify-content: space-between; gap: 20px; padding: 18px 20px; border: 1px solid var(--line-purple); border-left: 3px solid var(--purple); border-radius: 7px; background: linear-gradient(100deg, rgba(35,24,67,.48), rgba(11,31,58,.28)); }
  .portfolio-copy, .cert-copy { color: var(--soft); font-size: 12px; line-height: 1.55; }
  .portfolio-copy strong, .cert-copy strong { display: block; color: var(--ink); font-size: 14px; margin-bottom: 5px; }
  .portfolio-copy p, .cert-copy p { margin: 0; }
  .portfolio-card img { height: 31px; flex: 0 0 auto; }
  .cert-card { border-color: var(--line); border-left-color: var(--cyan); background: rgba(11,31,58,.32); }
  .placeholder-label { color: var(--cyan); font: 700 10px monospace; letter-spacing: 1px; white-space: nowrap; }
  .tool-note { text-align: center; color: var(--muted); font-size: 11px; margin-top: 11px; }
  table { width: 100%; border-collapse: separate; border-spacing: 12px; margin: -12px; width: calc(100% + 24px); }
  td { vertical-align: top; padding: 0; }
  .project-card {
    min-height: 183px; padding: 19px 18px 17px; border-radius: 7px;
    border: 1px solid var(--line); border-top: 2px solid var(--cyan);
    background: linear-gradient(145deg, rgba(11,31,58,.72), rgba(8,13,24,.72));
  }
  .project-card.purple { border-color: var(--line-purple); border-top-color: var(--purple); background: linear-gradient(145deg, rgba(35,24,67,.55), rgba(8,13,24,.72)); }
  .project-index { color: var(--muted); font: 700 10px "SFMono-Regular", Consolas, monospace; letter-spacing: 1.6px; }
  .project-card h3 { margin: 10px 0 9px; font-size: 16px; color: var(--ink); }
  .project-card p { margin: 0 0 20px; color: var(--soft); font-size: 12px; line-height: 1.55; }
  .project-link { color: var(--cyan); font-size: 12px; font-weight: 700; text-decoration: none; }
  .project-link:hover { text-decoration: underline; }
  .learning { text-align: center; color: var(--soft); line-height: 1.8; }
  .learning b { color: var(--purple); font-size: 12px; letter-spacing: .3px; }
  .learning span { color: var(--muted); margin: 0 8px; }
  .goals { display: flex; justify-content: center; gap: 8px; flex-wrap: wrap; }
  .goal { padding: 8px 11px; border: 1px solid var(--line); border-radius: 999px; color: #c9d8e8; background: rgba(11,31,58,.38); font-size: 11px; }
  .goal:nth-child(even) { border-color: var(--line-purple); background: rgba(35,24,67,.35); }
  .analytics { text-align: center; }
  .analytics-top { display: flex; justify-content: center; align-items: stretch; gap: 10px; }
  .analytics-top img { width: 49%; object-fit: contain; border: 1px solid rgba(96,165,250,.16); border-radius: 7px; background: rgba(13,17,23,.45); }
  .streak { display: block; width: min(720px, 92%); margin: 12px auto; }
  .contrib { display: block; width: 100%; margin: 8px auto 0; border-radius: 5px; }
  .live { color: var(--muted); font-size: 10px; margin-top: 7px; }
  .contact { text-align: center; }
  .contact img { height: 31px; margin: 4px; }
  .footer { text-align: center; margin-top: 28px; }
  .footer img { width: 100%; display: block; }
  @media (max-width: 680px) {
    .readme { padding: 14px 12px 20px; }
    h1 { font-size: 24px; letter-spacing: 3px; }
    .role { font-size: 12px; line-height: 1.5; }
    .portfolio-card, .cert-card { align-items: flex-start; flex-direction: column; }
    .avatar { width: 110px; height: 110px; margin-top: -32px; }
    table, tbody, tr, td { display: block; width: 100%; }
    table { margin: 0; width: 100%; }
    td + td { margin-top: 12px; }
    .analytics-top { display: block; }
    .analytics-top img { width: 100%; margin-bottom: 9px; }
  }
</style>
</head>
<body>
<main class="readme">
  <section class="hero">
    <svg class="hero-art" viewBox="0 0 1200 270" role="img" aria-label="Animated futuristic ARISH ISLAM hero banner" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="heroBg" x1="0" y1="0" x2="1" y2="1"><stop stop-color="#020617"/><stop offset=".52" stop-color="#0b1f3a"/><stop offset="1" stop-color="#24163f"/></linearGradient>
    <linearGradient id="heroLine" x1="0" y1="0" x2="1" y2="0"><stop stop-color="#22d3ee" stop-opacity="0"/><stop offset=".5" stop-color="#22d3ee"/><stop offset="1" stop-color="#a78bfa" stop-opacity="0"/></linearGradient>
    <pattern id="heroGrid" width="42" height="42" patternUnits="userSpaceOnUse"><path d="M42 0H0V42" fill="none" stroke="#60a5fa" stroke-opacity=".12"/></pattern>
    <filter id="heroGlow"><feGaussianBlur stdDeviation="9"/></filter>
  </defs>
  <rect width="1200" height="270" fill="url(#heroBg)"/>
  <rect width="1200" height="270" fill="url(#heroGrid)"/>
  <ellipse cx="600" cy="242" rx="370" ry="18" fill="#22d3ee" opacity=".16" filter="url(#heroGlow)"><animate attributeName="rx" values="260;420;260" dur="4s" repeatCount="indefinite"/></ellipse>
  <path d="M0 216 C180 168 250 250 430 206 S720 152 880 202 S1050 247 1200 186" fill="none" stroke="url(#heroLine)" stroke-width="2" opacity=".9">
    <animate attributeName="d" dur="5s" repeatCount="indefinite" values="M0 216 C180 168 250 250 430 206 S720 152 880 202 S1050 247 1200 186;M0 192 C180 244 290 166 450 215 S720 246 900 190 S1060 160 1200 220;M0 216 C180 168 250 250 430 206 S720 152 880 202 S1050 247 1200 186"/>
  </path>
  <circle cx="104" cy="68" r="3" fill="#22d3ee"><animate attributeName="cy" values="68;92;68" dur="2.8s" repeatCount="indefinite"/></circle>
  <circle cx="1092" cy="112" r="3" fill="#a78bfa"><animate attributeName="cy" values="112;85;112" dur="3.4s" repeatCount="indefinite"/></circle>
  <text x="600" y="112" text-anchor="middle" fill="#f8fafc" font-family="Arial, sans-serif" font-size="56" font-weight="800" letter-spacing="8">ARISH ISLAM</text>
  <text x="600" y="151" text-anchor="middle" fill="#bceff7" font-family="Arial, sans-serif" font-size="16" letter-spacing="1.2">WEB DEVELOPER  |  AI &amp; PROMPT ENGINEERING  |  AI-POWERED APPLICATIONS</text>
  <text x="600" y="208" text-anchor="middle" fill="#22d3ee" font-family="monospace" font-size="12" letter-spacing="2">BUILDING THE NEXT USEFUL THING</text>
</svg>
    <img class="avatar" src="https://avatars.githubusercontent.com/u/295182403?v=4" alt="Arish Islam GitHub avatar" />
    <h1>ARISH ISLAM</h1>
    <div class="role">Web Developer&nbsp; | &nbsp;AI &amp; Prompt Engineering&nbsp; | &nbsp;AI-Powered Applications</div>
    <div class="typing-mockup" aria-label="Typing animation preview"><span>Building AI-Powered Web Applications</span><i></i></div>
      <div class="eyebrow">Hi, I'm Arish Islam 👋</div>
  <div class="links">
      <a href="https://github.com/arish096"><img src="https://img.shields.io/badge/GitHub-arish096-0b1f3a?style=for-the-badge&logo=github&logoColor=white" alt="GitHub arish096" /></a>
      <a href="mailto:arishislam096@gmail.com"><img src="https://img.shields.io/badge/Email-00b8d9?style=for-the-badge&logo=gmail&logoColor=white" alt="Email Arish Islam" /></a>
    </div>
  </section>

  <section class="section">
    <h2 class="section-title">&gt; about.me</h2>
    <p class="about">I build practical web applications and explore <strong>AI, prompt engineering, AI workflows, and automation</strong>—while strengthening my problem-solving foundation through DSA with C++.</p>
  </section>

  <section class="section stack">
    <h2 class="section-title">// tech stack</h2>
    <div class="stack-icons">
      <img src="https://img.shields.io/badge/HTML5-0b1f3a?style=for-the-badge&logo=html5&logoColor=E34F26" alt="HTML5" />
      <img src="https://img.shields.io/badge/CSS3-0b1f3a?style=for-the-badge&logo=css3&logoColor=1572B6" alt="CSS3" />
      <img src="https://img.shields.io/badge/JavaScript-0b1f3a?style=for-the-badge&logo=javascript&logoColor=F7DF1E" alt="JavaScript" />
      <img src="https://img.shields.io/badge/C%2B%2B-0b1f3a?style=for-the-badge&logo=cplusplus&logoColor=00599C" alt="C++" />
      <img src="https://img.shields.io/badge/Python-0b1f3a?style=for-the-badge&logo=python&logoColor=3776AB" alt="Python" />
      <img src="https://img.shields.io/badge/Git-0b1f3a?style=for-the-badge&logo=git&logoColor=F05032" alt="Git" />
      <img src="https://img.shields.io/badge/GitHub-0b1f3a?style=for-the-badge&logo=github&logoColor=ffffff" alt="GitHub" />
      <img src="https://img.shields.io/badge/VS%20Code-0b1f3a?style=for-the-badge&logo=visualstudiocode&logoColor=007ACC" alt="VS Code" />
    </div>
  </section>

  <section class="section">
    <h2 class="section-title">// ai tools</h2>
    <div class="tool-row">
      <img src="https://img.shields.io/badge/ChatGPT-0b1f3a?style=for-the-badge&logo=openai&logoColor=74AA9C" alt="ChatGPT" />
      <img src="https://img.shields.io/badge/Claude-0b1f3a?style=for-the-badge&logo=anthropic&logoColor=D97757" alt="Claude" />
      <img src="https://img.shields.io/badge/Gemini-0b1f3a?style=for-the-badge&logo=googlegemini&logoColor=8AB4F8" alt="Gemini" />
      <img src="https://img.shields.io/badge/DeepSeek-0b1f3a?style=for-the-badge&logoColor=22d3ee" alt="DeepSeek" />
      <img src="https://img.shields.io/badge/Perplexity-0b1f3a?style=for-the-badge&logo=perplexity&logoColor=20B8CD" alt="Perplexity" />
    </div>
    <div class="tool-note">AI tools I explore for research, prompting, and practical workflows.</div>
  </section>

  <section class="section">
    <h2 class="section-title">// featured projects</h2>
    <table aria-label="Featured projects"><tbody><tr>
      <td><div class="project-card"><div class="project-index">PROJECT 01</div><h3>AI Radar — Live Flight Tracker</h3><p>Live flight tracking project focused on real-time data, AI/web technology, and an interactive radar-style experience.</p><a class="project-link" href="https://github.com/arish096/AI-Radar---Live-Flight-Tracker-">View repository ↗</a></div></td>
      <td><div class="project-card purple"><div class="project-index">PROJECT 02</div><h3>Apple Support AI Agent</h3><p>AI-powered customer support agent using Python, NLP, TF-IDF, Logistic Regression, Streamlit, intent classification, case retrieval, evidence-grounded replies, and AUTO-HANDLE vs ESCALATE decisions.</p><a class="project-link" href="https://github.com/arish096/apple-support-ai-agent">View repository ↗</a></div></td>
    </tr></tbody></table>
  </section>

  <section class="section">
    <h2 class="section-title">🌐 my portfolio</h2>
    <div class="portfolio-card">
      <div class="portfolio-copy"><strong>Arish Islam · Portfolio</strong><p>Explore projects, skills, experience/work, certification, and contact information.</p></div>
      <a href="https://arish-islam-portfolio.lovable.app/"><img src="https://img.shields.io/badge/Visit%20Portfolio-24163f?style=for-the-badge&logo=googlechrome&logoColor=22d3ee" alt="Visit Arish Islam portfolio" /></a>
    </div>
  </section>

  <section class="section">
    <h2 class="section-title">🏆 certification</h2>
    <div class="cert-card">
      <div class="cert-copy"><strong>Professional Certification</strong><p>Certificate name, issuer, date, and verification link can be added here.</p></div>
      <span class="placeholder-label">DETAILS PENDING</span>
    </div>
  </section>

  <section class="section">
    <h2 class="section-title">// learning &amp; goals</h2>
    <div class="learning"><b>LEARNING</b><span>DSA with C++</span><span>·</span><span>AI Agents</span><span>·</span><span>AI Automation</span><span>·</span><span>Web Development</span></div>
    <div class="goals" style="margin-top: 14px;"><span class="goal">Build AI-powered applications</span><span class="goal">Improve DSA with C++</span><span class="goal">Create practical AI agents</span><span class="goal">Explore AI automation</span><span class="goal">Improve modern web development</span><span class="goal">Document projects consistently</span></div>
  </section>

  <section class="section analytics">
    <h2 class="section-title">// github activity</h2>
    <div class="analytics-top">
      <img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=arish096&theme=github_dark" alt="GitHub stats" />
      <img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=arish096&theme=github_dark" alt="Top languages" />
    </div>
    <img class="streak" src="https://streak-stats.demolab.com?user=arish096&theme=transparent&hide_border=true&background=00000000&stroke=1e3a8a&ring=22d3ee&fire=60a5fa&currStreakLabel=22d3ee&sideLabels=cbd5e1&dates=94a3b8&currStreakNum=f8fafc&sideNums=f8fafc" alt="GitHub streak" />
    <img class="contrib" src="https://ghchart.rshah.org/22d3ee/arish096" alt="GitHub contribution graph" />
    <div class="live">These analytics are live external embeds; no statistics are hardcoded.</div>
  </section>

  <section class="section contact">
    <h2 class="section-title">// connect</h2>
    <a href="https://github.com/arish096"><img src="https://img.shields.io/badge/GitHub-@arish096-0b1f3a?style=for-the-badge&logo=github&logoColor=white" alt="GitHub @arish096" /></a>
    <a href="mailto:arishislam096@gmail.com"><img src="https://img.shields.io/badge/arishislam096%40gmail.com-0b1f3a?style=for-the-badge&logo=gmail&logoColor=EA4335" alt="Email arishislam096@gmail.com" /></a>
    <a href="https://arish-islam-portfolio.lovable.app/"><img src="https://img.shields.io/badge/Portfolio-24163f?style=for-the-badge&logo=googlechrome&logoColor=22d3ee" alt="Portfolio" /></a>
  </section>

  <footer class="footer"><svg class="footer-art" viewBox="0 0 1200 150" role="img" aria-label="Animated futuristic footer" xmlns="http://www.w3.org/2000/svg">
  <defs><linearGradient id="footerBg" x1="0" y1="0" x2="1" y2="0"><stop stop-color="#7c3aed"/><stop offset=".5" stop-color="#075985"/><stop offset="1" stop-color="#020617"/></linearGradient></defs>
  <path d="M0 44 C190 2 280 85 470 44 S770 4 950 52 S1090 75 1200 28 V150 H0 Z" fill="url(#footerBg)" opacity=".82"/>
  <path d="M0 44 C190 2 280 85 470 44 S770 4 950 52 S1090 75 1200 28" fill="none" stroke="#22d3ee" stroke-width="2"><animate attributeName="d" dur="5s" repeatCount="indefinite" values="M0 44 C190 2 280 85 470 44 S770 4 950 52 S1090 75 1200 28;M0 58 C180 92 300 6 490 55 S760 88 940 42 S1080 12 1200 58;M0 44 C190 2 280 85 470 44 S770 4 950 52 S1090 75 1200 28"/></path>
  <text x="600" y="105" text-anchor="middle" fill="#f8fafc" font-family="monospace" font-size="20" font-weight="700" letter-spacing="2">BUILD. LEARN. EXPERIMENT. REPEAT.</text>
</svg></footer>
</main>
</body>
</html>
