<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="theme-color" content="#0b0d12" />
  <meta name="description" content="Perfil de GitHub de Hector, desarrollador web enfocado en crear experiencias digitales útiles, modernas y responsive." />
  <title>Hector — Web Developer</title>
  <style>
    :root {
      color-scheme: dark;
      --bg: #0b0d12;
      --panel: #11151e;
      --panel-2: #151b26;
      --text: #f3f5f8;
      --muted: #9ca8b9;
      --line: rgba(255,255,255,.11);
      --lime: #c5ff4a;
      --cyan: #59e1e8;
      --violet: #a995ff;
      --radius: 22px;
    }
    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; }
    body {
      margin: 0;
      background:
        radial-gradient(ellipse at 12% 0%, rgba(89,225,232,.11), transparent 34rem),
        radial-gradient(ellipse at 88% 8%, rgba(169,149,255,.13), transparent 32rem),
        var(--bg);
      color: var(--text);
      font: 16px/1.65 Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
    }
    a { color: inherit; text-decoration: none; }
    a:hover { color: var(--lime); }
    .wrap { width: min(1050px, calc(100% - 36px)); margin: 0 auto; }
    .topbar {
      display: flex; align-items: center; justify-content: space-between; gap: 16px;
      padding: 24px 0;
      border-bottom: 1px solid var(--line);
    }
    .brand { display: flex; align-items: center; gap: 11px; font-weight: 800; letter-spacing: -.03em; }
    .brand-mark {
      display: grid; place-items: center; width: 38px; height: 38px; border-radius: 12px;
      background: var(--lime); color: #111; font-weight: 950; font-size: 20px;
      box-shadow: 0 0 28px rgba(197,255,74,.2);
    }
    .nav { display: flex; flex-wrap: wrap; gap: 20px; color: var(--muted); font-size: 13px; }
    .hero { padding: 76px 0 52px; display: grid; grid-template-columns: 1.4fr .6fr; gap: 38px; align-items: center; }
    .eyebrow { color: var(--lime); text-transform: uppercase; letter-spacing: .16em; font-size: 11px; font-weight: 800; }
    h1 { margin: 14px 0 18px; font-size: clamp(42px, 7vw, 76px); line-height: .99; letter-spacing: -.07em; }
    h1 span { color: var(--lime); }
    .intro { color: var(--muted); max-width: 620px; font-size: 17px; }
    .actions { display: flex; flex-wrap: wrap; gap: 12px; margin-top: 28px; }
    .button {
      display: inline-flex; align-items: center; justify-content: center; gap: 9px;
      border-radius: 999px; padding: 11px 17px; border: 1px solid var(--line);
      font-size: 13px; font-weight: 750; transition: transform .2s, border-color .2s;
    }
    .button:hover { transform: translateY(-2px); border-color: var(--lime); }
    .button.primary { background: var(--lime); color: #10130a; border-color: var(--lime); }
    .orbit-card {
      position: relative; min-height: 285px; display: grid; place-items: center; overflow: hidden;
      border: 1px solid var(--line); border-radius: 28px;
      background: linear-gradient(145deg, rgba(21,27,38,.96), rgba(12,15,22,.85));
    }
    .orbit-card::before, .orbit-card::after {
      content: ""; position: absolute; width: 190px; height: 190px; border: 1px solid rgba(197,255,74,.35);
      border-radius: 50%; transform: rotate(-28deg) scaleX(1.6);
    }
    .orbit-card::after { width: 130px; height: 130px; border-color: rgba(89,225,232,.45); transform: rotate(55deg) scaleX(1.5); }
    .code-symbol {
      z-index: 1; width: 124px; height: 124px; display: grid; place-items: center;
      border-radius: 32px; background: rgba(197,255,74,.09); border: 1px solid rgba(197,255,74,.4);
      color: var(--lime); font: 800 45px/1 ui-monospace, SFMono-Regular, Menlo, monospace;
      box-shadow: 0 0 70px rgba(197,255,74,.12);
    }
    .floating { position: absolute; z-index: 2; padding: 7px 11px; background: #1b2230; border: 1px solid var(--line); border-radius: 10px; font: 700 11px ui-monospace, monospace; }
    .float-one { top: 20%; left: 8%; color: var(--cyan); }
    .float-two { bottom: 19%; right: 7%; color: var(--violet); }
    section { padding: 28px 0 34px; }
    .section-head { display: flex; justify-content: space-between; align-items: end; gap: 20px; margin-bottom: 20px; }
    h2 { font-size: 23px; letter-spacing: -.04em; margin: 0; }
    .section-note { color: var(--muted); font-size: 12px; }
    .grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 14px; }
    .card {
      padding: 21px; border: 1px solid var(--line); border-radius: var(--radius);
      background: linear-gradient(145deg, rgba(21,27,38,.9), rgba(15,18,26,.9));
    }
    .card .icon { font-size: 23px; }
    .card h3 { margin: 12px 0 6px; font-size: 15px; }
    .card p { margin: 0; color: var(--muted); font-size: 13px; }
    .stack { display: flex; flex-wrap: wrap; gap: 9px; }
    .tag {
      border: 1px solid var(--line); border-radius: 10px; padding: 7px 11px;
      background: rgba(255,255,255,.035); color: #dce3ed; font: 12px ui-monospace, SFMono-Regular, Menlo, monospace;
    }
    .tag.highlight { border-color: rgba(197,255,74,.35); color: var(--lime); background: rgba(197,255,74,.06); }
    .feature {
      display: grid; grid-template-columns: 1fr 1fr; gap: 18px; align-items: stretch;
    }
    .feature .card { min-height: 180px; }
    .mini-label { color: var(--cyan); font: 700 10px ui-monospace, monospace; letter-spacing: .12em; text-transform: uppercase; }
    .quote { color: #e9edf3; font-size: 19px; line-height: 1.5; letter-spacing: -.025em; }
    .footer {
      margin-top: 34px; padding: 24px 0 34px; border-top: 1px solid var(--line);
      display: flex; flex-wrap: wrap; justify-content: space-between; gap: 12px; color: var(--muted); font-size: 12px;
    }
    .footer strong { color: var(--text); }
    .edit-note { margin: 18px 0 0; padding: 12px 14px; border: 1px dashed rgba(197,255,74,.35); border-radius: 12px; color: var(--muted); font-size: 12px; }
    .edit-note strong { color: var(--lime); }
    @media (max-width: 760px) {
      .hero { grid-template-columns: 1fr; padding-top: 54px; }
      .orbit-card { min-height: 230px; }
      .grid { grid-template-columns: 1fr; }
      .feature { grid-template-columns: 1fr; }
      .section-head { align-items: start; flex-direction: column; gap: 4px; }
      .nav { gap: 12px; }
    }
    @media (prefers-reduced-motion: reduce) { html { scroll-behavior: auto; } *, *::before, *::after { transition: none !important; } }
  </style>
</head>
<body>
  <div class="wrap">
    <header class="topbar">
      <a class="brand" href="#inicio" aria-label="Ir al inicio">
        <span class="brand-mark">H.</span><span>HECTOR<span style="color:var(--lime)">/</span>DEV</span>
      </a>
      <nav class="nav" aria-label="Navegación principal">
        <a href="#sobre-mi">Sobre mí</a>
        <a href="#stack">Tecnologías</a>
        <a href="#proyectos">Proyectos</a>
        <a href="#contacto">Contacto</a>
      </nav>
    </header>

    <main>
      <section class="hero" id="inicio">
        <div>
          <div class="eyebrow">Web Developer · Always learning</div>
          <h1>Construyo ideas<br />para el <span>mundo digital.</span></h1>
          <p class="intro">
            ¡Hola! Soy Hector, desarrollador web enfocado en crear sitios modernos,
            responsive y funcionales. Me gusta combinar diseño, código y atención al
            detalle para convertir ideas en experiencias digitales útiles.
          </p>
          <div class="actions">
            <!-- Cambia TU_USUARIO por tu nombre de usuario real de GitHub -->
            <a class="button primary" href="https://github.com/gonzaalzzdvp" target="_blank" rel="noreferrer">⌘ Ver mi GitHub ↗</a>
            <a class="button" href="#proyectos">Explorar proyectos ↓</a>
          </div>
        </div>
        <div class="orbit-card" aria-label="Ilustración decorativa de código">
          <span class="floating float-one">design.system()</span>
          <div class="code-symbol">&lt;/&gt;</div>
          <span class="floating float-two">build · learn · repeat</span>
        </div>
      </section>

      <section id="sobre-mi">
        <div class="section-head">
          <h2>Un poco sobre mí<span style="color:var(--lime)">.</span></h2>
          <span class="section-note">Curiosidad → práctica → progreso</span>
        </div>
        <div class="grid">
          <article class="card">
            <div class="icon">🧩</div>
            <h3>Desarrollo con intención</h3>
            <p>Me interesa crear experiencias claras, intuitivas y accesibles, sin perder de vista el rendimiento y la experiencia de usuario.</p>
          </article>
          <article class="card">
            <div class="icon">🛠️</div>
            <h3>De la idea al producto</h3>
            <p>Trabajo en interfaces web y funcionalidades de aplicaciones, aprendiendo a conectar el frontend con APIs y servicios backend.</p>
          </article>
          <article class="card">
            <div class="icon">📈</div>
            <h3>Aprendizaje continuo</h3>
            <p>Estoy fortaleciendo mis fundamentos, construyendo proyectos prácticos y explorando nuevas herramientas para crecer como desarrollador.</p>
          </article>
        </div>
      </section>

      <section id="stack">
        <div class="section-head">
          <h2>Mi caja de herramientas<span style="color:var(--lime)">.</span></h2>
          <span class="section-note">Tecnologías que uso y sigo practicando</span>
        </div>
        <div class="card">
          <div class="stack">
            <span class="tag highlight">HTML5</span>
            <span class="tag highlight">CSS3</span>
            <span class="tag highlight">JavaScript</span>
            <span class="tag">React</span>
            <span class="tag">Tailwind CSS</span>
            <span class="tag">Python</span>
            <span class="tag">Django REST Framework</span>
            <span class="tag">SQL</span>
            <span class="tag">Git & GitHub</span>
            <span class="tag">VS Code</span>
          </div>
          <p style="margin:16px 0 0;color:var(--muted);font-size:12px">
            Personaliza esta lista: deja solo las tecnologías con las que tengas experiencia práctica y mueve las que estés aprendiendo a una sección aparte.
          </p>
        </div>
      </section>

      <section id="proyectos">
        <div class="section-head">
          <h2>Proyectos destacados<span style="color:var(--lime)">.</span></h2>
          <span class="section-note">Reemplaza estas tarjetas por tus repositorios reales</span>
        </div>
        <div class="grid">
          <article class="card">
            <div class="mini-label">01 / Frontend</div>
            <h3>Tu proyecto de interfaz</h3>
            <p>Una web responsive con una interfaz cuidada, componentes reutilizables y una experiencia sencilla para el usuario.</p>
            <p style="margin-top:14px"><a href="https://github.com/TU_USUARIO" target="_blank" rel="noreferrer">Ver repositorio ↗</a></p>
          </article>
          <article class="card">
            <div class="mini-label">02 / Full stack</div>
            <h3>Tienda virtual</h3>
            <p>Un proyecto para mostrar catálogo, carrito, órdenes y la comunicación entre frontend y backend.</p>
            <p style="margin-top:14px"><a href="https://github.com/TU_USUARIO" target="_blank" rel="noreferrer">Ver repositorio ↗</a></p>
          </article>
          <article class="card">
            <div class="mini-label">03 / En progreso</div>
            <h3>Lo próximo que construiré</h3>
            <p>Un espacio para documentar lo que estás aprendiendo, los retos que resuelves y las mejoras que incorporas.</p>
            <p style="margin-top:14px"><a href="https://github.com/TU_USUARIO" target="_blank" rel="noreferrer">Ver repositorio ↗</a></p>
          </article>
        </div>
      </section>

      <section>
        <div class="feature">
          <article class="card">
            <div class="mini-label">Mi filosofía</div>
            <p class="quote">“No necesito saberlo todo para empezar. Necesito seguir construyendo, aprendiendo y mejorando.”</p>
          </article>
          <article class="card">
            <div class="mini-label">Ahora mismo</div>
            <h3 style="margin-top:10px">Enfocado en mejorar cada día</h3>
            <p>Perfeccionando mis habilidades de desarrollo web, practicando con proyectos reales y reforzando mis bases técnicas paso a paso.</p>
          </article>
        </div>
      </section>

      <section id="contacto">
        <div class="section-head">
          <h2>¿Creamos algo útil?<span style="color:var(--lime)">.</span></h2>
        </div>
        <div class="card" style="display:flex;justify-content:space-between;align-items:center;gap:20px;flex-wrap:wrap">
          <p style="margin:0;color:var(--muted);max-width:580px">Estoy abierto a conectar con otros desarrolladores, colaborar en proyectos y aprender de nuevos desafíos.</p>
          <div class="actions" style="margin:0">
            <a class="button primary" href="https://github.com/TU_USUARIO" target="_blank" rel="noreferrer">GitHub ↗</a>
            <!-- Añade aquí tu LinkedIn o correo cuando quieras compartirlos -->
            <a class="button" href="mailto:TU_CORREO@example.com">Email ↗</a>
          </div>
        </div>
      </section>
    </main>

    <footer class="footer">
      <span>Diseñado y construido con <strong>HTML + CSS</strong>.</span>
      <span>© <span id="year">2026</span> Hector · Hecho con intención.</span>
    </footer>
    <p class="edit-note"><strong>Antes de publicar:</strong> reemplaza <code>TU_USUARIO</code> por tu usuario de GitHub, actualiza el correo, añade enlaces a proyectos reales y ajusta el stack a tu experiencia actual.</p>
  </div>
  <script>
    document.getElementById("year").textContent = new Date().getFullYear();
  </script>
</body>
</html>
