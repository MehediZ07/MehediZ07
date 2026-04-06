<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Mehedi Zaman — GitHub Profile</title>
<style>
  :root {
    --color-background-primary: #ffffff;
    --color-background-secondary: #f5f4f0;
    --color-text-primary: #1a1a1a;
    --color-text-secondary: #555550;
    --color-text-tertiary: #888880;
    --color-border-tertiary: rgba(0,0,0,0.12);
    --color-border-secondary: rgba(0,0,0,0.22);
    --border-radius-md: 8px;
    --border-radius-lg: 12px;
    --font-sans: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
  }
  *{box-sizing:border-box;margin:0;padding:0}
  body{font-family:var(--font-sans);color:var(--color-text-primary);background:#f0efe9;padding:2rem 1rem}
  .wrap{max-width:900px;margin:0 auto;padding:2rem 1.25rem}
  .hero{text-align:center;padding:2.5rem 1.5rem 2rem;border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);background:var(--color-background-secondary);margin-bottom:1.25rem;position:relative;overflow:hidden}
  .top-bar{position:absolute;top:0;left:0;right:0;height:3px;background:linear-gradient(90deg,#534AB7 0%,#1D9E75 50%,#EF9F27 100%)}
  .av{width:88px;height:88px;border-radius:50%;background:#534AB7;display:flex;align-items:center;justify-content:center;font-size:28px;font-weight:500;color:#EEEDFE;margin:0 auto 1rem;border:2.5px solid #AFA9EC}
  .name{font-size:22px;font-weight:500;margin-bottom:4px}
  .role{font-size:13px;color:var(--color-text-secondary);margin-bottom:5px}
  .loc{font-size:12px;color:var(--color-text-tertiary);margin-bottom:1.1rem}
  .loc-dot{display:inline-block;width:6px;height:6px;border-radius:50%;background:#1D9E75;margin-right:5px;vertical-align:middle}
  .badges{display:flex;flex-wrap:wrap;gap:6px;justify-content:center;margin-bottom:1.1rem}
  .badge{font-size:11px;padding:3px 10px;border-radius:999px;border:0.5px solid}
  .bp{background:#EEEDFE;color:#3C3489;border-color:#AFA9EC}
  .bt{background:#E1F5EE;color:#085041;border-color:#5DCAA5}
  .ba{background:#FAEEDA;color:#633806;border-color:#EF9F27}
  .bc{background:#FAECE7;color:#712B13;border-color:#F0997B}
  .bb{background:#E6F1FB;color:#0C447C;border-color:#85B7EB}
  .socials{display:flex;gap:7px;justify-content:center;flex-wrap:wrap}
  .sb{font-size:11px;padding:5px 12px;border-radius:var(--border-radius-md);border:0.5px solid var(--color-border-secondary);color:var(--color-text-secondary);text-decoration:none;background:var(--color-background-primary)}
  .banner{border-radius:var(--border-radius-md);padding:.8rem 1rem;margin-bottom:1.25rem;display:flex;align-items:flex-start;gap:10px;font-size:12.5px;border:0.5px solid}
  .ban-p{background:#EEEDFE;color:#3C3489;border-color:#AFA9EC}
  .ban-t{background:#E1F5EE;color:#085041;border-color:#5DCAA5}
  .ban-icon{width:20px;height:20px;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:10px;font-weight:500;flex-shrink:0;margin-top:1px;color:#EEEDFE}
  .bi-p{background:#534AB7}
  .bi-t{background:#1D9E75}
  .metric-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:.7rem;margin-bottom:1.25rem}
  .metric{background:var(--color-background-secondary);border-radius:var(--border-radius-md);padding:.8rem .9rem;text-align:center}
  .mv{font-size:18px;font-weight:500;margin-bottom:2px}
  .ml{font-size:10px;color:var(--color-text-secondary)}
  .g2{display:grid;grid-template-columns:1fr 1fr;gap:1rem;margin-bottom:1.25rem}
  .card{border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);padding:1.1rem 1.2rem;background:var(--color-background-primary)}
  .clabel{font-size:10px;font-weight:500;letter-spacing:.08em;text-transform:uppercase;color:var(--color-text-tertiary);margin-bottom:.8rem}
  .dot-item{display:flex;gap:9px;align-items:flex-start;margin-bottom:8px}
  .dot-item:last-child{margin-bottom:0}
  .dot{width:5px;height:5px;border-radius:50%;background:#7F77DD;flex-shrink:0;margin-top:6px}
  .dot-text{font-size:12.5px;color:var(--color-text-secondary);line-height:1.5}
  .dot-text strong{font-weight:500;color:var(--color-text-primary)}
  .sr{display:flex;justify-content:space-between;align-items:center;padding:6px 0;border-bottom:0.5px solid var(--color-border-tertiary)}
  .sr:last-child{border-bottom:none}
  .sl{font-size:12px;color:var(--color-text-secondary)}
  .sv{font-size:12px;font-weight:500}
  .pill{padding:2px 8px;border-radius:999px;font-size:10px}
  .pill-g{background:#EAF3DE;color:#27500A}
  .pill-p{background:#EEEDFE;color:#3C3489}
  .pill-c{background:#FAECE7;color:#712B13}
  .pill-t{background:#E1F5EE;color:#085041}
  .stack-card{border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);padding:1.1rem 1.2rem;background:var(--color-background-primary);margin-bottom:1.25rem}
  .sg{margin-bottom:.85rem}
  .sg:last-child{margin-bottom:0}
  .sgl{font-size:10px;font-weight:500;letter-spacing:.08em;text-transform:uppercase;color:var(--color-text-tertiary);margin-bottom:6px}
  .pills{display:flex;flex-wrap:wrap;gap:5px}
  .tech{font-size:11px;padding:3px 9px;border-radius:var(--border-radius-md);border:0.5px solid var(--color-border-secondary);color:var(--color-text-secondary);background:var(--color-background-secondary)}
  .tech.h{background:#EEEDFE;color:#3C3489;border-color:#AFA9EC}
  .sdiv{font-size:10px;font-weight:500;letter-spacing:.1em;text-transform:uppercase;color:var(--color-text-tertiary);margin-bottom:.75rem;padding-bottom:.5rem;border-bottom:0.5px solid var(--color-border-tertiary)}
  .proj-wrap{display:grid;grid-template-columns:1fr 1fr;gap:1rem;margin-bottom:1.25rem}
  .proj{border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);background:var(--color-background-primary);overflow:hidden}
  .proj-top{padding:.9rem 1.1rem .7rem;border-bottom:0.5px solid var(--color-border-tertiary)}
  .proj-accent{display:flex;align-items:center;gap:8px;margin-bottom:.5rem}
  .proj-dot{width:8px;height:8px;border-radius:50%}
  .proj-name{font-size:14px;font-weight:500}
  .proj-role{font-size:10px;color:var(--color-text-tertiary);margin-bottom:.4rem}
  .proj-desc{font-size:12px;color:var(--color-text-secondary);line-height:1.55}
  .proj-body{padding:.8rem 1.1rem}
  .feat-list{margin-bottom:.7rem}
  .feat-item{display:flex;gap:7px;align-items:flex-start;margin-bottom:5px;font-size:11.5px;color:var(--color-text-secondary);line-height:1.45}
  .feat-dot{width:4px;height:4px;border-radius:50%;background:#AFA9EC;flex-shrink:0;margin-top:5px}
  .proj-tags{display:flex;flex-wrap:wrap;gap:4px;margin-bottom:.7rem}
  .ptag{font-size:10px;padding:2px 7px;border-radius:999px;background:var(--color-background-secondary);border:0.5px solid var(--color-border-secondary);color:var(--color-text-secondary)}
  .proj-links{display:flex;gap:6px;flex-wrap:wrap}
  .plink{font-size:10px;padding:3px 9px;border-radius:var(--border-radius-md);border:0.5px solid var(--color-border-secondary);color:var(--color-text-secondary);text-decoration:none;background:var(--color-background-secondary)}
  .plink.live{background:#EEEDFE;color:#3C3489;border-color:#AFA9EC}
  .footer{text-align:center;padding-top:1rem;font-size:11px;color:var(--color-text-tertiary);border-top:0.5px solid var(--color-border-tertiary);margin-top:1rem}
</style>
</head>
<body>
<div class="wrap">

  <div class="hero">
    <div class="top-bar"></div>
    <div class="av">MZ</div>
    <div class="name">Mehedi Zaman</div>
    <div class="role">Full Stack Web Developer &nbsp;·&nbsp; MERN &amp; Next.js Expert</div>
    <div class="loc"><span class="loc-dot"></span>Chittagong, Bangladesh &nbsp;·&nbsp; Software Developer at a tech company</div>
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

  <div class="banner ban-p">
    <div class="ban-icon bi-p">&#9670;</div>
    <div><strong>Currently shipping:</strong> Production-grade full-stack apps with Next.js 16, TypeScript, Tailwind CSS v4, Prisma &amp; PostgreSQL — exploring system design, scalable architecture, and open-source in 2026.</div>
  </div>

  <div class="metric-grid">
    <div class="metric"><div class="mv" style="color:#534AB7">MERN</div><div class="ml">Primary stack</div></div>
    <div class="metric"><div class="mv" style="color:#1D9E75">Next.js</div><div class="ml">App framework</div></div>
    <div class="metric"><div class="mv" style="color:#EF9F27">12–14h</div><div class="ml">Deep focus daily</div></div>
    <div class="metric"><div class="mv" style="color:#D85A30">2026</div><div class="ml">Going deeper</div></div>
  </div>

  <div class="g2">
    <div class="card">
      <div class="clabel">Focus areas</div>
      <div class="dot-item"><div class="dot"></div><div class="dot-text"><strong>Role-based dashboards</strong> &amp; admin panels with complex permissions</div></div>
      <div class="dot-item"><div class="dot"></div><div class="dot-text"><strong>Real-time systems</strong> — notifications, chat, live updates via Socket.io</div></div>
      <div class="dot-item"><div class="dot"></div><div class="dot-text"><strong>Payment &amp; settlement</strong> — Stripe, SSLCommerz, COD workflows</div></div>
      <div class="dot-item"><div class="dot"></div><div class="dot-text"><strong>Scalable REST API design</strong> — modular, type-safe, production-ready</div></div>
      <div class="dot-item"><div class="dot"></div><div class="dot-text">Clean, <strong>maintainable and testable</strong> production code</div></div>
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

  <div class="stack-card">
    <div class="clabel">Tech stack</div>
    <div class="sg">
      <div class="sgl">Frontend</div>
      <div class="pills">
        <span class="tech h">HTML5</span><span class="tech h">CSS3</span><span class="tech h">JavaScript</span><span class="tech h">TypeScript</span><span class="tech h">React 19</span><span class="tech h">Next.js 16</span><span class="tech h">Tailwind CSS v4</span><span class="tech h">shadcn/ui</span>
      </div>
    </div>
    <div class="sg">
      <div class="sgl">Backend &amp; Database</div>
      <div class="pills">
        <span class="tech">Node.js</span><span class="tech">Express.js 5</span><span class="tech">MongoDB</span><span class="tech">PostgreSQL</span><span class="tech">Prisma ORM</span><span class="tech">Firebase</span><span class="tech">REST API</span><span class="tech">JWT Auth</span>
      </div>
    </div>
    <div class="sg">
      <div class="sgl">Libraries &amp; Tools</div>
      <div class="pills">
        <span class="tech">TanStack Query</span><span class="tech">TanStack Form</span><span class="tech">TanStack Table</span><span class="tech">Socket.io</span><span class="tech">Zod</span><span class="tech">Axios</span><span class="tech">Recharts</span><span class="tech">Stripe</span><span class="tech">Cloudinary</span>
      </div>
    </div>
    <div class="sg">
      <div class="sgl">Workflow</div>
      <div class="pills">
        <span class="tech">Git &amp; GitHub</span><span class="tech">Vercel</span><span class="tech">Postman</span><span class="tech">Prisma Studio</span><span class="tech">ESLint</span><span class="tech">VS Code</span>
      </div>
    </div>
  </div>

  <div class="sdiv">Featured projects</div>

  <div class="proj-wrap">
    <div class="proj">
      <div class="proj-top">
        <div class="proj-accent">
          <div class="proj-dot" style="background:#534AB7"></div>
          <div>
            <div class="proj-name">SwiftShip — Backend</div>
            <div class="proj-role">Courier Management System API</div>
          </div>
        </div>
        <div class="proj-desc">Production-ready courier &amp; delivery management REST API — handles shipments, couriers, merchants, payments, dynamic pricing, and real-time tracking.</div>
      </div>
      <div class="proj-body">
        <div class="feat-list">
          <div class="feat-item"><div class="feat-dot"></div>JWT auth with 5 role-based access levels (Super Admin → User)</div>
          <div class="feat-item"><div class="feat-dot"></div>Dynamic pricing engine — region, weight, and express surcharge</div>
          <div class="feat-item"><div class="feat-dot"></div>Hub-based multi-leg delivery system with automatic route planning</div>
          <div class="feat-item"><div class="feat-dot"></div>Stripe &amp; SSLCommerz payment integration + COD settlement</div>
          <div class="feat-item"><div class="feat-dot"></div>Real-time notifications &amp; full shipment event audit trail</div>
        </div>
        <div class="proj-tags">
          <span class="ptag">Node.js</span><span class="ptag">Express 5</span><span class="ptag">TypeScript</span><span class="ptag">Prisma</span><span class="ptag">PostgreSQL</span><span class="ptag">JWT</span><span class="ptag">Stripe</span><span class="ptag">Zod</span><span class="ptag">Cloudinary</span>
        </div>
        <div class="proj-links">
          <a class="plink live" href="https://swiftship-backend.vercel.app">Live API</a>
          <a class="plink" href="https://swiftship-frontendv1.vercel.app">Frontend</a>
          <a class="plink" href="https://drive.google.com/file/d/1tifUZPwJU50tc23QoKL6e_zqzNV1w-aR/view">Video demo</a>
        </div>
      </div>
    </div>

    <div class="proj">
      <div class="proj-top">
        <div class="proj-accent">
          <div class="proj-dot" style="background:#1D9E75"></div>
          <div>
            <div class="proj-name">SwiftShip — Frontend</div>
            <div class="proj-role">Full-featured Dashboard App</div>
          </div>
        </div>
        <div class="proj-desc">Multi-role dashboard frontend for SwiftShip — built with Next.js 16 App Router, React 19, TanStack Query, and Tailwind CSS v4. Full dark mode support.</div>
      </div>
      <div class="proj-body">
        <div class="feat-list">
          <div class="feat-item"><div class="feat-dot"></div>4 role-specific dashboards — Admin, Courier, Merchant, User</div>
          <div class="feat-item"><div class="feat-dot"></div>Live price calculator — auto-fetches from backend as you type</div>
          <div class="feat-item"><div class="feat-dot"></div>Real-time notification dropdown with unread badge, auto-refresh</div>
          <div class="feat-item"><div class="feat-dot"></div>Server-managed tables — search, filter, sort, paginate via URL</div>
          <div class="feat-item"><div class="feat-dot"></div>Admin charts (shipment bar &amp; pie) via Recharts</div>
        </div>
        <div class="proj-tags">
          <span class="ptag">Next.js 16</span><span class="ptag">React 19</span><span class="ptag">TypeScript</span><span class="ptag">Tailwind v4</span><span class="ptag">shadcn/ui</span><span class="ptag">TanStack Query</span><span class="ptag">TanStack Form</span><span class="ptag">Recharts</span>
        </div>
        <div class="proj-links">
          <a class="plink live" href="https://swiftship-frontendv1.vercel.app">Live App</a>
          <a class="plink" href="https://swiftship-backend.vercel.app">Backend API</a>
          <a class="plink" href="https://drive.google.com/file/d/1tifUZPwJU50tc23QoKL6e_zqzNV1w-aR/view">Video demo</a>
        </div>
      </div>
    </div>
  </div>

  <div class="banner ban-t">
    <div class="ban-icon bi-t">&#8593;</div>
    <div><strong>2026 Ambitions:</strong> Contribute to major open-source projects &nbsp;·&nbsp; Master system design &amp; distributed systems &nbsp;·&nbsp; Launch a developer-focused SaaS product &nbsp;·&nbsp; Grow toward Lead / Architect role by 2028</div>
  </div>

  <div class="footer">github.com/MehediZ07 &nbsp;·&nbsp; Built with passion from Chittagong, BD</div>
</div>
</body>
</html>
