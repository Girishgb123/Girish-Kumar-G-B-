# Girish-Kumar-G-B-
Freelanceing platform hub 
<!doctype html>

<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Freelancing Platform Hub - Demo</title>
  <style>
    :root{--accent:#2563eb;--muted:#6b7280;--card:#ffffff;--bg:#f3f4f6}
    *{box-sizing:border-box}
    body{font-family:Inter,system-ui,Segoe UI,Roboto,Helvetica,Arial,sans-serif;background:var(--bg);color:#111;margin:0}
    .container{max-width:1100px;margin:28px auto;padding:24px}
    header{display:flex;align-items:center;gap:16px}
    .logo{width:62px;height:62px;border-radius:10px;background:linear-gradient(135deg,var(--accent),#7c3aed);display:flex;align-items:center;justify-content:center;color:#fff;font-weight:700;font-size:18px}
    h1{font-size:22px;margin:0}
    p.lead{color:var(--muted);margin:6px 0 18px}
    .grid{display:grid;grid-template-columns:1fr 420px;gap:20px}
    .card{background:var(--card);border-radius:12px;box-shadow:0 4px 12px rgba(15,23,42,0.06);padding:18px}
    .btn{display:inline-block;padding:10px 14px;border-radius:8px;background:var(--accent);color:#fff;text-decoration:none;font-weight:600}
    .features{display:flex;flex-direction:column;gap:12px}
    .small{color:var(--muted);font-size:13px}
    .techs{display:flex;flex-wrap:wrap;gap:8px;margin-top:10px}
    .chip{background:#eef2ff;padding:6px 8px;border-radius:999px;font-size:13px;color:#1f2937}
    /* SVG container */
    .flow-wrap{overflow:auto;padding:10px}
    footer{margin-top:18px;color:var(--muted);font-size:13px}
    @media(max-width:900px){.grid{grid-template-columns:1fr;}.logo{width:48px;height:48px}}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="logo">FP</div>
      <div>
        <h1>Freelancing Platform Hub — Demo Site</h1>
        <p class="lead">Prototype landing page and a visual flowchart of the platform workflow. Save this file as <code>index.html</code> and open in a browser.</p>
      </div>
    </header><main class="grid" aria-label="main content">
  <section class="card">
    <h2 style="margin-top:0">Quick Overview</h2>
    <p class="small">A simplified front-facing demo for your major project. The left panel contains project overview, features and tech stack. The right panel shows the system flowchart (SVG) — printable and editable.</p>

    <div style="margin-top:14px" class="features">
      <div><strong>Key Features</strong>
        <ul style="margin:8px 0 0 18px;color:var(--muted)">
          <li>Role-based authentication (Client / Freelancer)</li>
          <li>Project posting, bidding and hiring</li>
          <li>In-app messaging, payments and reviews</li>
        </ul>
      </div>

      <div>
        <strong>Technologies</strong>
        <div class="techs">
          <span class="chip">HTML</span>
          <span class="chip">CSS</span>
          <span class="chip">JavaScript</span>
          <span class="chip">Django / Flask</span>
          <span class="chip">MySQL / MongoDB</span>
          <span class="chip">AWS / Firebase</span>
        </div>
      </div>

      <div style="margin-top:8px">
        <a class="btn" href="#flow">View Flowchart</a>
      </div>
    </div>

    <footer>
      <div>Project: Freelancing Platform Hub</div>
      <div style="margin-top:6px">Tip: To make this a full website, replace dummy links with real pages (login/register, dashboard, projects).</div>
    </footer>
  </section>

  <aside class="card">
    <h3 id="flow" style="margin-top:0">System Flowchart</h3>
    <p class="small">SVG flowchart — copy, export as PNG, or include in your report/PPT.</p>
    <div class="flow-wrap">
      <!-- BEGIN FLOWCHART SVG -->
      <svg xmlns="http://www.w3.org/2000/svg" width="840" height="760" viewBox="0 0 840 760" role="img" aria-label="Freelancing Platform Hub Flowchart">
        <style>
          .box{fill:#fff;stroke:#0f172a;stroke-width:1;rx:10;}
          .big{fill:#fff;stroke:#0f172a;stroke-width:1.6;rx:12}
          .text{font:14px/1.2 'Segoe UI', Roboto, Arial;fill:#0f172a}
          .muted{font:12px/1.2 'Segoe UI', Roboto, Arial;fill:#475569}
          .arrow{stroke:#0f172a;stroke-width:2;fill:none;marker-end:url(#arrow)}
        </style>

        <defs>
          <marker id="arrow" markerWidth="10" markerHeight="10" refX="8" refY="5" orient="auto">
            <path d="M0 0 L10 5 L0 10 z" fill="#0f172a"/>
          </marker>
          <filter id="shadow" x="-20%" y="-20%" width="140%" height="140%">
            <feDropShadow dx="0" dy="6" stdDeviation="10" flood-opacity="0.08"/>
          </filter>
        </defs>

        <!-- Start -->
        <g transform="translate(270,18)">
          <rect class="big" x="150" y="0" width="180" height="48" rx="24"/>
          <text class="text" x="240" y="32" text-anchor="middle">Start</text>
        </g>

        <!-- Registration/Login -->
        <g transform="translate(170,100)">
          <rect class="box" x="120" y="0" width="300" height="60" rx="10"/>
          <text class="text" x="270" y="28" text-anchor="middle">User Registration / Login</text>
        </g>

        <!-- Role ID -->
        <g transform="translate(170,200)">
          <rect class="box" x="120" y="0" width="300" height="52" rx="10"/>
          <text class="text" x="270" y="30" text-anchor="middle">Role Identification (Client / Freelancer)</text>
        </g>

        <!-- Branch: Client -->
        <g transform="translate(0,300)">
          <rect class="box" x="24" y="0" width="280" height="60" rx="10"/>
          <text class="text" x="164" y="28" text-anchor="middle">Client: Post Project & Set Budget</text>
        </g>

        <!-- Branch: Freelancer -->
        <g transform="translate(400,300)">
          <rect class="box" x="24" y="0" width="280" height="60" rx="10"/>
          <text class="text" x="164" y="28" text-anchor="middle">Freelancer: View Projects & Bid</text>
        </g>

        <!-- Join -->
        <g transform="translate(170,420)">
          <rect class="box" x="120" y="0" width="300" height="60" rx="10"/>
          <text class="text" x="270" y="28" text-anchor="middle">Client Reviews Bids & Selects Freelancer</text>
        </g>

        <!-- Execution -->
        <g transform="translate(170,520)">
          <rect class="box" x="120" y="0" width="300" height="60" rx="10"/>
          <text class="text" x="270" y="30" text-anchor="middle">Project Execution & Communication Portal</text>
        </g>

        <!-- Payment -->
        <g transform="translate(170,620)">
          <rect class="box" x="120" y="0" width="300" height="60" rx="10"/>
          <text class="text" x="270" y="30" text-anchor="middle">Payment & Review / Submit Work</text>
        </g>

        <!-- End -->
        <g transform="translate(270,720)">
          <rect class="big" x="150" y="0" width="180" height="48" rx="24"/>
          <text class="text" x="240" y="32" text-anchor="middle">End / Logout</text>
        </g>

        <!-- Arrows -->
        <path class="arrow" d="M420 66 L420 100" />
        <path class="arrow" d="M420 152 L420 200" />

        <path class="arrow" d="M270 252 L110 300" />
        <path class="arrow" d="M420 252 L590 300" />

        <path class="arrow" d="M200 360 L350 420" />
        <path class="arrow" d="M620 360 L470 420" />

        <path class="arrow" d="M420 480 L420 520" />
        <path class="arrow" d="M420 580 L420 620" />
        <path class="arrow" d="M420 680 L420 720" />

        <!-- Labels (muted) -->
        <text class="muted" x="420" y="40" text-anchor="middle">Authentication</text>
        <text class="muted" x="420" y="190" text-anchor="middle">Identify user role</text>

      </svg>
      <!-- END FLOWCHART SVG -->
    </div>
  </aside>
</main>

  </div>
</body>
</html>
