<style>
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:var(--font-sans);color:var(--color-text-primary)}
@keyframes fadeUp{from{opacity:0;transform:translateY(18px)}to{opacity:1;transform:translateY(0)}}
@keyframes barGrow{from{width:0}to{width:var(--w)}}
@keyframes pulse{0%,100%{opacity:1}50%{opacity:0.4}}
.fade1{animation:fadeUp .5s ease both}
.fade2{animation:fadeUp .5s .1s ease both}
.fade3{animation:fadeUp .5s .2s ease both}
.fade4{animation:fadeUp .5s .3s ease both}
.fade5{animation:fadeUp .5s .4s ease both}
.fade6{animation:fadeUp .5s .5s ease both}
.fade7{animation:fadeUp .5s .6s ease both}
.fade8{animation:fadeUp .5s .7s ease both}
.wrap{max-width:900px;margin:0 auto;padding:1.5rem 1.25rem}
.hero{text-align:center;padding:2.5rem 1.5rem 2rem;border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);background:var(--color-background-secondary);margin-bottom:1.25rem;position:relative;overflow:hidden}
.hero-bar{position:absolute;top:0;left:0;right:0;height:3px;background:linear-gradient(90deg,#534AB7,#1D9E75,#EF9F27)}
.av{width:88px;height:88px;border-radius:50%;background:#534AB7;display:flex;align-items:center;justify-content:center;font-size:26px;font-weight:500;color:#EEEDFE;margin:0 auto 1rem;border:2.5px solid #AFA9EC;transition:transform .2s}
.av:hover{transform:scale(1.06)}
.name{font-size:22px;font-weight:500;margin-bottom:4px}
.role{font-size:13px;color:var(--color-text-secondary);margin-bottom:4px}
.loc{font-size:12px;color:var(--color-text-tertiary);margin-bottom:1rem;display:flex;align-items:center;justify-content:center;gap:6px}
.live-dot{width:7px;height:7px;border-radius:50%;background:#1D9E75;animation:pulse 2s infinite;display:inline-block;flex-shrink:0}
.badges{display:flex;flex-wrap:wrap;gap:6px;justify-content:center;margin-bottom:1rem}
.badge{font-size:11px;padding:3px 10px;border-radius:999px;border:0.5px solid;transition:transform .15s}
.badge:hover{transform:scale(1.05)}
.bp{background:#EEEDFE;color:#3C3489;border-color:#AFA9EC}
.bt{background:#E1F5EE;color:#085041;border-color:#5DCAA5}
.ba{background:#FAEEDA;color:#633806;border-color:#EF9F27}
.bc{background:#FAECE7;color:#712B13;border-color:#F0997B}
.bb{background:#E6F1FB;color:#0C447C;border-color:#85B7EB}
.socials{display:flex;gap:7px;justify-content:center;flex-wrap:wrap}
.sb{font-size:11px;padding:5px 13px;border-radius:var(--border-radius-md);border:0.5px solid var(--color-border-secondary);color:var(--color-text-secondary);text-decoration:none;background:var(--color-background-primary);transition:background .15s,transform .15s}
.sb:hover{background:var(--color-background-secondary);transform:translateY(-1px)}
.stats-grid{display:grid;grid-template-columns:repeat(4,minmax(0,1fr));gap:.75rem;margin-bottom:1.25rem}
.stat-box{background:var(--color-background-secondary);border-radius:var(--border-radius-md);padding:1rem;text-align:center;border:0.5px solid var(--color-border-tertiary);transition:transform .2s}
.stat-box:hover{transform:translateY(-2px)}
.stat-num{font-size:22px;font-weight:500;margin-bottom:2px}
.stat-lbl{font-size:10px;color:var(--color-text-secondary)}
.banner{border-radius:var(--border-radius-md);padding:.85rem 1.1rem;margin-bottom:1.25rem;display:flex;align-items:flex-start;gap:10px;font-size:12.5px;border:0.5px solid}
.ban-p{background:#EEEDFE;color:#3C3489;border-color:#AFA9EC}
.ban-t{background:#E1F5EE;color:#085041;border-color:#5DCAA5}
.ban-icon{width:20px;height:20px;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:11px;flex-shrink:0;margin-top:1px;color:#EEEDFE}
.bi-p{background:#534AB7}
.bi-t{background:#1D9E75}
.g2{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:1rem;margin-bottom:1.25rem}
.card{border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);padding:1.1rem 1.2rem;background:var(--color-background-primary)}
.clabel{font-size:10px;font-weight:500;letter-spacing:.08em;text-transform:uppercase;color:var(--color-text-tertiary);margin-bottom:.8rem}
.dot-item{display:flex;gap:9px;align-items:flex-start;margin-bottom:8px}
.dot-item:last-child{margin-bottom:0}
.di-dot{width:5px;height:5px;border-radius:50%;background:#7F77DD;flex-shrink:0;margin-top:6px}
.dit{font-size:12.5px;color:var(--color-text-secondary);line-height:1.5}
.dit strong{font-weight:500;color:var(--color-text-primary)}
.sr{display:flex;justify-content:space-between;align-items:center;padding:7px 0;border-bottom:0.5px solid var(--color-border-tertiary)}
.sr:last-child{border-bottom:none}
.sl{font-size:12px;color:var(--color-text-secondary)}
.sv{font-size:12px;font-weight:500}
.pill{padding:2px 9px;border-radius:999px;font-size:10px}
.pill-g{background:#EAF3DE;color:#27500A}
.pill-p{background:#EEEDFE;color:#3C3489}
.pill-c{background:#FAECE7;color:#712B13}
.pill-t{background:#E1F5EE;color:#085041}
.skill-section{border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);padding:1.1rem 1.2rem;background:var(--color-background-primary)}
.skill-row{margin-bottom:.85rem}
.skill-row:last-child{margin-bottom:0}
.skill-head{display:flex;justify-content:space-between;margin-bottom:5px}
.skill-name{font-size:12px;color:var(--color-text-secondary)}
.skill-pct{font-size:11px;color:var(--color-text-tertiary)}
.skill-track{height:4px;background:var(--color-background-secondary);border-radius:2px;overflow:hidden}
.skill-bar{height:100%;border-radius:2px;width:0;transition:width 1.2s ease}
.contrib-section{border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);padding:1.1rem 1.2rem;background:var(--color-background-primary)}
.contrib-grid{display:grid;grid-template-columns:repeat(13,1fr);gap:3px}
.cday{aspect-ratio:1;border-radius:2px;background:var(--color-background-secondary);transition:transform .1s}
.cday:hover{transform:scale(1.3)}
.stack-card{border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);padding:1.1rem 1.2rem;background:var(--color-background-primary);margin-bottom:1.25rem}
.sg{margin-bottom:.85rem}
.sg:last-child{margin-bottom:0}
.sgl{font-size:10px;font-weight:500;letter-spacing:.08em;text-transform:uppercase;color:var(--color-text-tertiary);margin-bottom:6px}
.pills{display:flex;flex-wrap:wrap;gap:5px}
.tech{font-size:11px;padding:3px 9px;border-radius:var(--border-radius-md);border:0.5px solid var(--color-border-secondary);color:var(--color-text-secondary);background:var(--color-background-secondary);transition:transform .15s}
.tech:hover{transform:scale(1.04)}
.tech.h{background:#EEEDFE;color:#3C3489;border-color:#AFA9EC}
.sdiv{font-size:10px;font-weight:500;letter-spacing:.1em;text-transform:uppercase;color:var(--color-text-tertiary);margin-bottom:.75rem;padding-bottom:.5rem;border-bottom:0.5px solid var(--color-border-tertiary)}
.proj-grid{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:1rem;margin-bottom:1.25rem}
.proj{border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);background:var(--color-background-primary);overflow:hidden;transition:transform .2s}
.proj:hover{transform:translateY(-2px)}
.proj-head{padding:.9rem 1.1rem .75rem;border-bottom:0.5px solid var(--color-border-tertiary)}
.proj-title-row{display:flex;align-items:center;gap:8px;margin-bottom:4px}
.pdot{width:8px;height:8px;border-radius:50%;flex-shrink:0}
.proj-name{font-size:14px;font-weight:500}
.proj-sub{font-size:10px;color:var(--color-text-tertiary);margin-bottom:.4rem}
.proj-desc{font-size:12px;color:var(--color-text-secondary);line-height:1.55}
.proj-body{padding:.8rem 1.1rem}
.fi{display:flex;gap:7px;align-items:flex-start;margin-bottom:5px;font-size:11.5px;color:var(--color-text-secondary);line-height:1.45}
.fi:last-of-type{margin-bottom:.7rem}
.fd{width:4px;height:4px;border-radius:50%;background:#AFA9EC;flex-shrink:0;margin-top:5px}
.ptags{display:flex;flex-wrap:wrap;gap:4px;margin-bottom:.7rem}
.ptag{font-size:10px;padding:2px 7px;border-radius:999px;background:var(--color-background-secondary);border:0.5px solid var(--color-border-secondary);color:var(--color-text-secondary)}
.plinks{display:flex;gap:6px;flex-wrap:wrap}
.plink{font-size:10px;padding:3px 9px;border-radius:var(--border-radius-md);border:0.5px solid var(--color-border-secondary);color:var(--color-text-secondary);text-decoration:none;background:var(--color-background-secondary);transition:background .15s}
.plink:hover{background:var(--color-background-primary)}
.plink.live{background:#EEEDFE;color:#3C3489;border-color:#AFA9EC}
.footer{text-align:center;padding-top:1rem;font-size:11px;color:var(--color-text-tertiary);border-top:0.5px solid var(--color-border-tertiary);margin-top:.5rem}
@media(max-width:600px){
  .stats-grid{grid-template-columns:repeat(2,minmax(0,1fr))}
  .g2,.proj-grid{grid-template-columns:1fr}
  .name{font-size:18px}
  .hero{padding:2rem 1rem 1.5rem}
}
</style>

<div class="wrap">

<div class="hero fade1">
  <div class="hero-bar"></div>
  <div class="av">MZ</div>
  <div class="name">Mehedi Zaman</div>
  <div class="role">Full Stack Web Developer &nbsp;·&nbsp; MERN &amp; Next.js Expert</div>
  <div class="loc"><span class="live-dot"></span><span>Chittagong, Bangladesh &nbsp;·&nbsp; Software Developer at Nexbell.Inc</span></div>
  <div class="badges">
    <span class="badge bp">React &amp; Next.js 16</span>
    <span class="badge bt">Node.js &amp; Express</span>
    <span class="badge ba">TypeScript</span>
    <span class="badge bc">PostgreSQL &amp; Prisma</span>
    <span class="badge bb">MongoDB</span>
  </div>
  <div class="socials">
    <a class="sb" href="https://www.linkedin.com/in/mehediz07">LinkedIn</a>
    <a class="sb" href="https://twitter.com/MehediZ07">Twitter / X</a>
    <a class="sb" href="https://discord.com/users/MehediZ07">Discord</a>
    <a class="sb" href="https://www.youtube.com/@MehediZ07">YouTube</a>
  </div>
</div>

<div class="stats-grid fade2">
  <div class="stat-box"><div class="stat-num" style="color:#534AB7" id="s1">10+</div><div class="stat-lbl">Projects shipped</div></div>
  <div class="stat-box"><div class="stat-num" style="color:#1D9E75" id="s2">50+</div><div class="stat-lbl">Repos on GitHub</div></div>
  <div class="stat-box"><div class="stat-num" style="color:#EF9F27" id="s3">20+</div><div class="stat-lbl">Technologies used</div></div>
  <div class="stat-box"><div class="stat-num" style="color:#D85A30" id="s4">12+</div><div class="stat-lbl">Hours deep focus / day</div></div>
</div>

<div class="banner ban-p fade3">
  <div class="ban-icon bi-p">&#9670;</div>
  <div><strong>Currently shipping:</strong> Production-grade full-stack apps with Next.js 16, TypeScript, Tailwind CSS v4, Prisma &amp; PostgreSQL — exploring system design, scalable architecture, and open-source contributions in 2026.</div>
</div>

<div class="g2 fade3">
  <div class="card">
    <div class="clabel">Focus areas</div>
    <div class="dot-item"><div class="di-dot"></div><div class="dit"><strong>Role-based dashboards</strong> &amp; admin panels with complex permission systems</div></div>
    <div class="dot-item"><div class="di-dot"></div><div class="dit"><strong>Real-time systems</strong> — notifications, chat, live updates via Socket.io</div></div>
    <div class="dot-item"><div class="di-dot"></div><div class="dit"><strong>Payment &amp; settlement</strong> — Stripe, SSLCommerz, COD workflows</div></div>
    <div class="dot-item"><div class="di-dot"></div><div class="dit"><strong>Scalable REST API design</strong> — modular, type-safe, production-ready</div></div>
    <div class="dot-item"><div class="di-dot"></div><div class="dit">Clean, <strong>maintainable and testable</strong> production code</div></div>
  </div>
  <div class="card">
    <div class="clabel">At a glance</div>
    <div class="sr"><span class="sl">Position</span><span class="pill pill-g">Dev at tech company</span></div>
    <div class="sr"><span class="sl">GitHub streak</span><span class="pill pill-t">Active</span></div>
    <div class="sr"><span class="sl">Primary stack</span><span class="sv">MERN + Next.js</span></div>
    <div class="sr"><span class="sl">Work style</span><span class="sv">12–14 hr deep focus</span></div>
    <div class="sr"><span class="sl">2026 goal</span><span class="pill pill-p">Ship open-source SaaS</span></div>
    <div class="sr"><span class="sl">Dream goal</span><span class="pill pill-c">Lead Architect by 2028</span></div>
  </div>
</div>

<div class="g2 fade4">
  <div class="skill-section">
    <div class="clabel">Skill levels</div>
    <div class="skill-row">
      <div class="skill-head"><span class="skill-name">Next.js / React</span><span class="skill-pct">95%</span></div>
      <div class="skill-track"><div class="skill-bar" id="b1" style="background:#534AB7"></div></div>
    </div>
    <div class="skill-row">
      <div class="skill-head"><span class="skill-name">Node.js / Express</span><span class="skill-pct">92%</span></div>
      <div class="skill-track"><div class="skill-bar" id="b2" style="background:#534AB7"></div></div>
    </div>
    <div class="skill-row">
      <div class="skill-head"><span class="skill-name">TypeScript</span><span class="skill-pct">88%</span></div>
      <div class="skill-track"><div class="skill-bar" id="b3" style="background:#1D9E75"></div></div>
    </div>
    <div class="skill-row">
      <div class="skill-head"><span class="skill-name">PostgreSQL / Prisma</span><span class="skill-pct">85%</span></div>
      <div class="skill-track"><div class="skill-bar" id="b4" style="background:#1D9E75"></div></div>
    </div>
    <div class="skill-row">
      <div class="skill-head"><span class="skill-name">MongoDB</span><span class="skill-pct">90%</span></div>
      <div class="skill-track"><div class="skill-bar" id="b5" style="background:#EF9F27"></div></div>
    </div>
    <div class="skill-row">
      <div class="skill-head"><span class="skill-name">System design</span><span class="skill-pct">75%</span></div>
      <div class="skill-track"><div class="skill-bar" id="b6" style="background:#EF9F27"></div></div>
    </div>
  </div>

  <div class="contrib-section">
    <div class="clabel">Contribution activity — 2026</div>
    <div class="contrib-grid" id="contrib-grid"></div>
    <div style="display:flex;gap:8px;margin-top:10px;align-items:center">
      <span style="font-size:10px;color:var(--color-text-tertiary)">Less</span>
      <div style="width:10px;height:10px;border-radius:2px;background:var(--color-background-secondary);border:0.5px solid var(--color-border-tertiary)"></div>
      <div style="width:10px;height:10px;border-radius:2px;background:#CECBF6"></div>
      <div style="width:10px;height:10px;border-radius:2px;background:#7F77DD"></div>
      <div style="width:10px;height:10px;border-radius:2px;background:#534AB7"></div>
      <span style="font-size:10px;color:var(--color-text-tertiary)">More</span>
    </div>
  </div>
</div>

<div class="stack-card fade5">
  <div class="clabel">Tech stack</div>
  <div class="sg"><div class="sgl">Frontend</div><div class="pills"><span class="tech h">HTML5</span><span class="tech h">CSS3</span><span class="tech h">JavaScript</span><span class="tech h">TypeScript</span><span class="tech h">React 19</span><span class="tech h">Next.js 16</span><span class="tech h">Tailwind v4</span><span class="tech h">shadcn/ui</span></div></div>
  <div class="sg"><div class="sgl">Backend &amp; Database</div><div class="pills"><span class="tech">Node.js</span><span class="tech">Express 5</span><span class="tech">MongoDB</span><span class="tech">PostgreSQL</span><span class="tech">Prisma ORM</span><span class="tech">Firebase</span><span class="tech">REST API</span><span class="tech">JWT Auth</span></div></div>
  <div class="sg"><div class="sgl">Libraries &amp; Tools</div><div class="pills"><span class="tech">TanStack Query</span><span class="tech">TanStack Form</span><span class="tech">TanStack Table</span><span class="tech">Socket.io</span><span class="tech">Zod</span><span class="tech">Axios</span><span class="tech">Recharts</span><span class="tech">Stripe</span><span class="tech">Cloudinary</span></div></div>
  <div class="sg"><div class="sgl">Workflow</div><div class="pills"><span class="tech">Git &amp; GitHub</span><span class="tech">Vercel</span><span class="tech">Postman</span><span class="tech">Prisma Studio</span><span class="tech">ESLint</span><span class="tech">VS Code</span><span class="tech">Bun</span></div></div>
</div>

<div class="sdiv fade6">Featured projects</div>
<div class="proj-grid fade6">
  <div class="proj">
    <div class="proj-head">
      <div class="proj-title-row"><div class="pdot" style="background:#534AB7"></div><div><div class="proj-name">SwiftShip — Backend</div><div class="proj-sub">Courier Management System API</div></div></div>
      <div class="proj-desc">Production-ready courier &amp; delivery management REST API — shipments, couriers, merchants, payments, dynamic pricing, and real-time tracking at scale.</div>
    </div>
    <div class="proj-body">
      <div class="fi"><div class="fd"></div>JWT auth with 5 role-based access levels (Super Admin → User)</div>
      <div class="fi"><div class="fd"></div>Dynamic pricing engine — region, weight &amp; express surcharge</div>
      <div class="fi"><div class="fd"></div>Hub-based multi-leg delivery with automatic route planning</div>
      <div class="fi"><div class="fd"></div>Stripe &amp; SSLCommerz integration + COD courier settlement</div>
      <div class="fi"><div class="fd"></div>Real-time notifications &amp; full shipment event audit trail</div>
      <div class="ptags"><span class="ptag">Node.js</span><span class="ptag">Express 5</span><span class="ptag">TypeScript</span><span class="ptag">Prisma</span><span class="ptag">PostgreSQL</span><span class="ptag">Stripe</span><span class="ptag">Zod</span><span class="ptag">Cloudinary</span></div>
      <div class="plinks"><a class="plink live" href="https://swiftship-backend.vercel.app">Live API</a><a class="plink" href="https://swiftship-frontendv1.vercel.app">Frontend</a><a class="plink" href="https://drive.google.com/file/d/1tifUZPwJU50tc23QoKL6e_zqzNV1w-aR/view">Video demo</a></div>
    </div>
  </div>
  <div class="proj">
    <div class="proj-head">
      <div class="proj-title-row"><div class="pdot" style="background:#1D9E75"></div><div><div class="proj-name">SwiftShip — Frontend</div><div class="proj-sub">Full-featured Multi-role Dashboard</div></div></div>
      <div class="proj-desc">Multi-role dashboard — Next.js 16 App Router, React 19, TanStack Query, Tailwind CSS v4, full dark mode. Built for scale with server-managed state.</div>
    </div>
    <div class="proj-body">
      <div class="fi"><div class="fd"></div>4 role-specific dashboards — Admin, Courier, Merchant, User</div>
      <div class="fi"><div class="fd"></div>Live price calculator — auto-fetches from backend as you type</div>
      <div class="fi"><div class="fd"></div>Real-time notification dropdown, unread badge, 30s auto-refresh</div>
      <div class="fi"><div class="fd"></div>Server-managed tables — search, filter, sort, paginate via URL</div>
      <div class="fi"><div class="fd"></div>Admin analytics charts (bar &amp; pie) via Recharts · Dark mode</div>
      <div class="ptags"><span class="ptag">Next.js 16</span><span class="ptag">React 19</span><span class="ptag">TypeScript</span><span class="ptag">Tailwind v4</span><span class="ptag">shadcn/ui</span><span class="ptag">TanStack Query</span><span class="ptag">Recharts</span></div>
      <div class="plinks"><a class="plink live" href="https://swiftship-frontendv1.vercel.app">Live App</a><a class="plink" href="https://swiftship-backend.vercel.app">Backend API</a><a class="plink" href="https://drive.google.com/file/d/1tifUZPwJU50tc23QoKL6e_zqzNV1w-aR/view">Video demo</a></div>
    </div>
  </div>
</div>

<div class="banner ban-t fade7">
  <div class="ban-icon bi-t">&#8593;</div>
  <div><strong>2026 Ambitions:</strong> Contribute to major open-source projects &nbsp;·&nbsp; Master system design &amp; distributed systems &nbsp;·&nbsp; Launch a developer-focused SaaS product &nbsp;·&nbsp; Grow toward Lead / Architect role by 2028</div>
</div>

<div class="footer fade8">github.com/MehediZ07 &nbsp;·&nbsp; Built with passion from Chittagong, BD</div>
</div>

<script>
(function(){
  const bars = [
    {id:'b1',w:'95%'},{id:'b2',w:'92%'},{id:'b3',w:'88%'},
    {id:'b4',w:'85%'},{id:'b5',w:'90%'},{id:'b6',w:'75%'}
  ];
  bars.forEach(function(b){
    var el = document.getElementById(b.id);
    if(el) el.style.width = b.w;
  });

  var levels = [0,1,2,3,2,1,0,1,3,2,1,2,3,
                1,0,2,3,1,0,2,3,1,2,0,1,3,
                2,1,3,0,2,1,0,3,2,1,0,2,3,
                1,2,0,3,1,2,3,0,1,2,3,1,0,
                2,3,1,0,2,1,3,0,2,1,0,3,2,
                1,2,3,0,1,2,0,3,1,2,3,1,0,
                2,1,3,2,0,1,2,3,1,0,2,3,1];
  var colors = ['var(--color-background-secondary)','#CECBF6','#7F77DD','#534AB7'];
  var grid = document.getElementById('contrib-grid');
  if(grid){
    levels.forEach(function(l){
      var d = document.createElement('div');
      d.className = 'cday';
      d.style.background = colors[l];
      grid.appendChild(d);
    });
  }
})();
</script>



## Featured Projects

### SwiftShip — Courier Management System

> Full-stack production-grade courier & delivery platform — backend API + multi-role dashboard frontend

| | Backend | Frontend |
|---|---|---|
| **Live** | [swiftship-backend.vercel.app](https://swiftship-backend.vercel.app) | [swiftship-frontendv1.vercel.app](https://swiftship-frontendv1.vercel.app) |
| **Stack** | Node.js · Express 5 · TypeScript · Prisma · PostgreSQL | Next.js 16 · React 19 · TanStack Query · Tailwind v4 · shadcn/ui |
| **Demo** | [Watch video overview](https://drive.google.com/file/d/1tifUZPwJU50tc23QoKL6e_zqzNV1w-aR/view) | |

**Backend highlights**
- JWT auth with 5 role-based access levels (Super Admin → User)
- Dynamic pricing engine — region, weight & express surcharge auto-calculation
- Hub-based multi-leg delivery system with automatic route planning
- Stripe & SSLCommerz payment integration + COD settlement for couriers
- Real-time notifications & full shipment event audit trail

**Frontend highlights**
- 4 role-specific dashboards — Admin, Courier, Merchant, User
- Live price calculator — auto-fetches from backend as you fill in cities & weight
- Real-time notification dropdown with unread count badge, auto-refresh every 30s
- Server-managed data tables — search, filter, sort, paginate via URL params
- Admin analytics charts (bar & pie) via Recharts · Full dark mode support

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js_16-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)
![Stripe](https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white)
