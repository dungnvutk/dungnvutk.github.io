---
permalink: /
layout: null
---
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="Viet Dung Nguyen, Ph.D. — AI and Computer Vision Engineer specializing in medical imaging, 3D vision, orthopedic biomechanics, and real-time systems." />
  <title>Viet Dung Nguyen, Ph.D. | AI & Computer Vision</title>
  <style>
    :root {
      --bg: #08111f;
      --panel: #0f1b2d;
      --panel-2: #132238;
      --text: #eef4ff;
      --muted: #a9b8ce;
      --line: rgba(255,255,255,.10);
      --accent: #62d0ff;
      --accent-2: #8b7cff;
      --good: #6de0b3;
      --shadow: 0 18px 50px rgba(0,0,0,.25);
      --radius: 20px;
      --max: 1120px;
    }
    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; }
    body {
      margin: 0;
      font-family: Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      color: var(--text);
      background:
        radial-gradient(circle at 12% 6%, rgba(98,208,255,.14), transparent 29%),
        radial-gradient(circle at 92% 4%, rgba(139,124,255,.16), transparent 31%),
        var(--bg);
      line-height: 1.65;
    }
    a { color: inherit; text-decoration: none; }
    .wrap { width: min(calc(100% - 36px), var(--max)); margin: 0 auto; }
    nav {
      position: sticky; top: 0; z-index: 20;
      backdrop-filter: blur(16px);
      background: rgba(8,17,31,.76);
      border-bottom: 1px solid var(--line);
    }
    .nav-inner { min-height: 68px; display: flex; align-items: center; justify-content: space-between; gap: 24px; }
    .brand { font-weight: 800; letter-spacing: -.02em; }
    .nav-links { display: flex; gap: 22px; color: var(--muted); font-size: .94rem; }
    .nav-links a:hover { color: var(--text); }
    .hero { padding: 110px 0 78px; }
    .hero-grid { display: grid; grid-template-columns: 1.45fr .85fr; gap: 56px; align-items: center; }
    .eyebrow { color: var(--accent); text-transform: uppercase; letter-spacing: .15em; font-size: .8rem; font-weight: 800; }
    h1 { margin: 12px 0 20px; font-size: clamp(3rem, 7vw, 6.2rem); line-height: .95; letter-spacing: -.065em; }
    h1 span { display: block; color: var(--muted); font-size: .48em; letter-spacing: -.04em; margin-top: 18px; line-height: 1.12; }
    .lead { max-width: 760px; color: #cfdaea; font-size: clamp(1.05rem, 2vw, 1.24rem); }
    .actions { display: flex; flex-wrap: wrap; gap: 12px; margin-top: 30px; }
    .btn { display: inline-flex; align-items: center; justify-content: center; padding: 12px 18px; border-radius: 12px; font-weight: 750; border: 1px solid var(--line); background: rgba(255,255,255,.04); transition: .2s ease; }
    .btn.primary { background: linear-gradient(135deg, var(--accent), var(--accent-2)); color: #06101d; border: none; }
    .btn:hover { transform: translateY(-2px); box-shadow: 0 10px 28px rgba(0,0,0,.22); }
    .profile-card { padding: 26px; border: 1px solid var(--line); border-radius: var(--radius); background: linear-gradient(180deg, rgba(255,255,255,.055), rgba(255,255,255,.025)); box-shadow: var(--shadow); }
    .initials { width: 88px; height: 88px; border-radius: 24px; display: grid; place-items: center; font-size: 1.8rem; font-weight: 900; color: #07111f; background: linear-gradient(135deg, var(--accent), var(--good)); }
    .profile-card h2 { margin: 22px 0 4px; font-size: 1.35rem; }
    .profile-card p { color: var(--muted); margin: 0; }
    .mini-stats { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; margin-top: 22px; }
    .stat { border: 1px solid var(--line); border-radius: 14px; padding: 14px; background: rgba(255,255,255,.025); }
    .stat strong { display: block; font-size: 1.35rem; }
    .stat span { color: var(--muted); font-size: .82rem; }
    section { padding: 82px 0; }
    .section-head { display: flex; justify-content: space-between; align-items: end; gap: 24px; margin-bottom: 34px; }
    .section-head h2 { font-size: clamp(2rem, 4vw, 3.2rem); letter-spacing: -.045em; margin: 0; }
    .section-head p { margin: 0; color: var(--muted); max-width: 620px; }
    .grid-3 { display: grid; grid-template-columns: repeat(3, 1fr); gap: 18px; }
    .card { border: 1px solid var(--line); border-radius: var(--radius); background: rgba(255,255,255,.035); padding: 24px; }
    .card h3 { margin: 10px 0 8px; font-size: 1.18rem; }
    .card p { color: var(--muted); margin: 0; }
    .icon { font-size: 1.35rem; }
    .timeline { display: grid; gap: 18px; }
    .role { display: grid; grid-template-columns: 190px 1fr; gap: 24px; padding: 26px; border: 1px solid var(--line); border-radius: var(--radius); background: rgba(255,255,255,.03); }
    .role .date { color: var(--accent); font-weight: 750; }
    .role h3 { margin: 0 0 4px; font-size: 1.25rem; }
    .role .org { color: #cad6e6; font-weight: 650; margin-bottom: 12px; }
    .role ul { padding-left: 18px; margin: 0; color: var(--muted); }
    .role li + li { margin-top: 7px; }
    .project-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 18px; }
    .project { position: relative; overflow: hidden; min-height: 260px; }
    .project::after { content: ""; position: absolute; width: 150px; height: 150px; border-radius: 50%; filter: blur(45px); background: rgba(98,208,255,.14); right: -35px; bottom: -45px; }
    .kicker { color: var(--good); font-size: .8rem; font-weight: 800; letter-spacing: .08em; text-transform: uppercase; }
    .project h3 { font-size: 1.45rem; margin: 10px 0 10px; }
    .metrics { display: flex; flex-wrap: wrap; gap: 8px; margin-top: 18px; }
    .pill { border: 1px solid var(--line); border-radius: 999px; padding: 6px 10px; font-size: .82rem; color: #cad6e6; background: rgba(255,255,255,.025); }
    .skills { display: flex; flex-wrap: wrap; gap: 10px; }
    .skill { padding: 9px 12px; border-radius: 10px; border: 1px solid var(--line); background: rgba(255,255,255,.04); color: #d8e3f1; }
    .edu-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 18px; }
    .degree { color: var(--accent); font-weight: 750; }
    .school { font-size: 1.1rem; font-weight: 800; margin: 7px 0 5px; }
    .year { color: var(--muted); }
    footer { padding: 40px 0 54px; border-top: 1px solid var(--line); color: var(--muted); }
    footer .row { display: flex; justify-content: space-between; gap: 20px; align-items: center; }
    @media (max-width: 900px) {
      .hero-grid, .grid-3, .edu-grid { grid-template-columns: 1fr; }
      .project-grid { grid-template-columns: 1fr; }
      .hero { padding-top: 78px; }
      .profile-card { max-width: 540px; }
      .role { grid-template-columns: 1fr; gap: 8px; }
    }
    @media (max-width: 640px) {
      .nav-links { display: none; }
      .section-head { align-items: start; flex-direction: column; }
      .mini-stats { grid-template-columns: 1fr; }
      footer .row { flex-direction: column; align-items: start; }
    }
  </style>
</head>
<body>
  <nav>
    <div class="wrap nav-inner">
      <a class="brand" href="#top">VDN / Portfolio</a>
      <div class="nav-links">
        <a href="#about">About</a>
        <a href="#experience">Experience</a>
        <a href="#work">Selected Work</a>
        <a href="#skills">Skills</a>
        <a href="#education">Education</a>
      </div>
    </div>
  </nav>

  <main id="top">
    <header class="hero">
      <div class="wrap hero-grid">
        <div>
          <div class="eyebrow">AI · Computer Vision · Medical Imaging</div>
          <h1>Viet Dung Nguyen, Ph.D.<span>Building intelligent systems for medical imaging, 3D vision, and biomechanical analysis.</span></h1>
          <p class="lead">AI and computer vision engineer with a research-to-production background spanning deep learning, geometric computer vision, 2D–3D registration, 3D reconstruction, orthopedic imaging, GPU computing, and high-performance scientific software.</p>
          <div class="actions">
            <a class="btn primary" href="#work">View selected work</a>
            <a class="btn" href="https://github.com/dungnvutk" target="_blank" rel="noreferrer">GitHub profile ↗</a>
          </div>
        </div>
        <aside class="profile-card" aria-label="Professional summary">
          <div class="initials">VN</div>
          <h2>Research + Applied Engineering</h2>
          <p>Focused on clinically relevant AI, computer vision, real-time imaging systems, and patient-specific computational methods.</p>
          <div class="mini-stats">
            <div class="stat"><strong>25 FPS</strong><span>real-time fluoroscopic tracking pipeline</span></div>
            <div class="stat"><strong>11k+</strong><span>radiographs used in deep-learning workflows</span></div>
            <div class="stat"><strong>1k+</strong><span>TKA patient images used for pose estimation</span></div>
            <div class="stat"><strong>0.52 mm</strong><span>3D reconstruction accuracy vs. CT reference</span></div>
          </div>
        </aside>
      </div>
    </header>

    <section id="about">
      <div class="wrap">
        <div class="section-head">
          <h2>What I work on</h2>
          <p>I develop computational methods that connect AI research, geometry, biomechanics, and deployable engineering systems.</p>
        </div>
        <div class="grid-3">
          <article class="card"><div class="icon">◫</div><h3>Medical Computer Vision</h3><p>Segmentation, detection, pose estimation, radiographic image analysis, and fluoroscopic tracking for orthopedic applications.</p></article>
          <article class="card"><div class="icon">◇</div><h3>3D Vision & Geometry</h3><p>2D–3D registration, projective geometry, multiview reasoning, rigid transformations, CAD alignment, and 3D reconstruction.</p></article>
          <article class="card"><div class="icon">⌁</div><h3>Scientific Systems</h3><p>High-performance C++/Python software, GPU computing, optimization, simulation, kinematics, and real-time research pipelines.</p></article>
        </div>
      </div>
    </section>

    <section id="experience">
      <div class="wrap">
        <div class="section-head"><h2>Experience</h2><p>A progression from physics-based simulation to machine learning, biomedical engineering, and translational medical AI.</p></div>
        <div class="timeline">
          <article class="role">
            <div class="date">2023 — Present</div>
            <div><h3>Lead AI/ML Engineer</h3><div class="org">Orthopaedic Innovation Technology Center</div><ul><li>Developed real-time 3D CAD overlay and implant-tracking pipelines for fluoroscopic orthopedic imaging.</li><li>Built deep-learning workflows using modern segmentation and instance-segmentation architectures across 11,000+ postoperative radiographs.</li><li>Developed 6-DOF implant pose-estimation and patient-specific kinematic methods for orthopedic analysis.</li></ul></div>
          </article>
          <article class="role">
            <div class="date">2021 — 2023</div>
            <div><h3>Graduate Researcher — Computer Vision for Medical Imaging</h3><div class="org">Center for Musculoskeletal Research, University of Tennessee</div><ul><li>Led work on patient-specific 3D orthopedic implant reconstruction from sparse X-ray imaging.</li><li>Integrated deep learning, 3D reconstruction, and rigid-body biomechanics for postoperative TKA motion analysis.</li></ul></div>
          </article>
          <article class="role">
            <div class="date">2019 — 2020</div>
            <div><h3>Graduate Researcher — Machine Learning & Signal Processing</h3><div class="org">Institute for Information Sciences, University of Kansas</div><ul><li>Developed deep-reinforcement-learning and large-scale optimization methods for spatial system modeling and decision-making.</li><li>Implemented GPU-accelerated simulation and rendering workflows using CUDA and OpenGL.</li></ul></div>
          </article>
          <article class="role">
            <div class="date">2017 — 2018</div>
            <div><h3>Research & Development Engineer</h3><div class="org">Viettel High Tech</div><ul><li>Developed real-time aircraft and ground-vehicle simulations using 6-DOF dynamics, control theory, MATLAB/Simulink, and C++.</li><li>Integrated physics-based models into interactive real-time simulation systems.</li></ul></div>
          </article>
        </div>
      </div>
    </section>

    <section id="work">
      <div class="wrap">
        <div class="section-head"><h2>Selected work</h2><p>Representative projects selected to communicate technical depth without exposing proprietary source code or private employer information.</p></div>
        <div class="project-grid">
          <article class="card project"><div class="kicker">Real-time vision</div><h3>Fluoroscopic 3D CAD Overlay</h3><p>End-to-end pipeline for aligning and tracking orthopedic implant CAD geometry on fluoroscopic imagery, combining learned vision components with geometric optimization.</p><div class="metrics"><span class="pill">25 FPS</span><span class="pill">Python</span><span class="pill">PyTorch</span><span class="pill">MATLAB</span><span class="pill">C++</span></div></article>
          <article class="card project"><div class="kicker">Medical AI</div><h3>Automated Orthopedic Image Analysis</h3><p>Deep-learning pipelines for segmentation and structure identification on postoperative radiographs, using architectures including MedSAM, nnU-Net, and YOLACT.</p><div class="metrics"><span class="pill">11,000+ images</span><span class="pill">92% mAP</span><span class="pill">Segmentation</span><span class="pill">Detection</span></div></article>
          <article class="card project"><div class="kicker">3D reconstruction</div><h3>Patient-Specific Implant Reconstruction</h3><p>Non-rigid registration and numerical optimization framework for reconstructing orthopedic implant geometry from sparse radiographic measurements.</p><div class="metrics"><span class="pill">0.52 mm accuracy</span><span class="pill">Optimization</span><span class="pill">3D geometry</span></div></article>
          <article class="card project"><div class="kicker">Biomechanics</div><h3>Joint Kinematics & Motion Estimation</h3><p>Forward and inverse kinematic models for knee and hip motion analysis, supporting implant evaluation and patient-specific biomechanical research.</p><div class="metrics"><span class="pill">6-DOF</span><span class="pill">C++</span><span class="pill">MATLAB</span><span class="pill">Rigid-body mechanics</span></div></article>
        </div>
      </div>
    </section>

    <section id="skills">
      <div class="wrap">
        <div class="section-head"><h2>Technical toolkit</h2><p>A cross-disciplinary stack covering machine learning, geometric vision, numerical computing, and real-time engineering.</p></div>
        <div class="skills">
          <span class="skill">Python</span><span class="skill">C++</span><span class="skill">MATLAB</span><span class="skill">PyTorch</span><span class="skill">OpenCV</span><span class="skill">CUDA</span><span class="skill">OpenGL</span><span class="skill">VTK</span><span class="skill">Deep Learning</span><span class="skill">Medical Image Analysis</span><span class="skill">Segmentation</span><span class="skill">Pose Estimation</span><span class="skill">2D–3D Registration</span><span class="skill">3D Reconstruction</span><span class="skill">Projective Geometry</span><span class="skill">Numerical Optimization</span><span class="skill">Rigid-Body Dynamics</span><span class="skill">GPU Computing</span><span class="skill">Real-Time Systems</span><span class="skill">Signal Processing</span>
        </div>
      </div>
    </section>

    <section id="education">
      <div class="wrap">
        <div class="section-head"><h2>Education</h2><p>Engineering training spanning mechanical systems, electrical engineering, and biomedical engineering.</p></div>
        <div class="edu-grid">
          <article class="card"><div class="degree">Ph.D. · Biomedical Engineering</div><div class="school">University of Tennessee, Knoxville</div><div class="year">2023</div></article>
          <article class="card"><div class="degree">M.S. · Electrical Engineering</div><div class="school">University of Kansas</div><div class="year">2020</div></article>
          <article class="card"><div class="degree">B.E. · Mechanical Engineering</div><div class="school">Hanoi University of Science and Technology</div><div class="year">2017 · Honors Program</div></article>
        </div>
      </div>
    </section>

  </main>

  <footer>
    <div class="wrap row">
      <div>© 2026 Viet Dung Nguyen, Ph.D.</div>
      <a href="https://github.com/dungnvutk" target="_blank" rel="noreferrer">github.com/dungnvutk ↗</a>
    </div>
  </footer>
</body>
</html>