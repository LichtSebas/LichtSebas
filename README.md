<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Perfil GitHub — Tu Nombre</title>
  <meta name="description" content="Página personal / perfil para GitHub Pages">
  <style>
    :root{
      --bg:#0f1724; --card:#0b1320; --muted:#93a3b8; --accent:#56ccf2; --glass: rgba(255,255,255,0.03);
      --radius:14px; --maxw:900px;
      color-scheme: dark;
    }
    *{box-sizing:border-box}
    body{font-family:Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial; background:linear-gradient(180deg,#071025 0%, #081426 60%); color:#e6eef6; margin:0; padding:40px; display:flex; justify-content:center}
    .container{width:100%; max-width:var(--maxw)}
    .card{background:var(--card); border-radius:var(--radius); padding:28px; box-shadow:0 6px 30px rgba(2,6,23,0.6); backdrop-filter:blur(6px)}
    header{display:flex; gap:20px; align-items:center}
    .avatar{width:110px; height:110px; border-radius:16px; overflow:hidden; flex:0 0 110px; border:2px solid rgba(255,255,255,0.06)}
    .avatar img{width:100%; height:100%; object-fit:cover}
    .heading{flex:1}
    h1{margin:0; font-size:22px}
    p.lead{margin:6px 0 0; color:var(--muted)}
    .badges{margin-top:10px; display:flex; gap:8px; flex-wrap:wrap}
    .badge{background:var(--glass); padding:6px 10px; border-radius:999px; font-size:13px; color:var(--muted)}

    .grid{display:grid; grid-template-columns:1fr 320px; gap:20px; margin-top:18px}
    @media (max-width:880px){.grid{grid-template-columns:1fr} .heading{order:2} .avatar{order:1; margin-bottom:8px}}

    .section{margin-top:18px}
    .section h2{font-size:16px; margin:0 0 10px}
    .about{line-height:1.6; color:#d7e6f2}

    .skills{display:flex; flex-wrap:wrap; gap:10px}
    .skill{background:linear-gradient(90deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01)); padding:8px 10px; border-radius:8px; font-size:13px; color:var(--muted)}

    .projects{display:grid; grid-template-columns:repeat(auto-fit,minmax(220px,1fr)); gap:12px}
    .proj{background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.02)); padding:12px; border-radius:10px}
    .proj h3{margin:0 0 8px; font-size:14px}
    .proj p{margin:0; color:var(--muted); font-size:13px}

    .side-card{background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.02)); padding:16px; border-radius:12px}
    .socials{display:flex; gap:10px; margin-top:8px}
    .socials a{display:inline-flex; align-items:center; gap:8px; padding:8px 10px; border-radius:8px; text-decoration:none; color:inherit; background:transparent}
    .muted{color:var(--muted); font-size:13px}

    footer{margin-top:18px; text-align:center; color:var(--muted); font-size:13px}

    /* small utilities */
    .copy-btn{cursor:pointer; border:1px solid rgba(255,255,255,0.04); padding:6px 8px; border-radius:8px; font-size:13px}

  </style>
</head>
<body>
  <div class="container">
    <div class="card">
      <header>
        <div class="avatar"><img src="https://avatars.githubusercontent.com/u/000000?v=4" alt="Avatar"></div>
        <div class="heading">
          <h1>Tu Nombre <span style="font-size:13px; color:var(--muted)">/ @tuusuario</span></h1>
          <p class="lead">Desarrollador/a de software • Estudiante de Ingeniería • Apasionado por web, backend y data</p>
          <div class="badges">
            <span class="badge">🏷️ Disponible para proyectos</span>
            <span class="badge">🎓 Estudiante - Universidad</span>
            <span class="badge">📍 Lima, Perú</span>
          </div>
        </div>
      </header>

      <div class="grid">
        <main>
          <section class="section about">
            <h2>Sobre mí</h2>
            <p>Soy <strong>Tu Nombre</strong>, estudiante de Ingeniería de Software con interés en desarrollo web, sistemas distribuidos y análisis de datos. Actualmente trabajo en proyectos personales que integran PHP, MySQL, Python y JavaScript. Me encanta aprender y compartir conocimiento en GitHub.</p>
          </section>

          <section class="section">
            <h2>Habilidades</h2>
            <div class="skills">
              <span class="skill">HTML</span>
              <span class="skill">CSS</span>
              <span class="skill">JavaScript</span>
              <span class="skill">PHP</span>
              <span class="skill">MySQL</span>
              <span class="skill">Python</span>
              <span class="skill">Git</span>
              <span class="skill">Docker (básico)</span>
            </div>
          </section>

          <section class="section">
            <h2>Proyectos destacados</h2>
            <div class="projects">
              <article class="proj">
                <h3>EdanDecorMuebleria</h3>
                <p>Tienda web en PHP + MySQL con panel administrativo, sistema de eventos y carrito de compras.</p>
              </article>
              <article class="proj">
                <h3>Sistema Bancario (Proyecto académico)</h3>
                <p>Analizador de pagos con generación de gráficos, predicciones y simulación de préstamos en Python.</p>
              </article>
              <article class="proj">
                <h3>Otro Proyecto</h3>
                <p>Descripción breve del proyecto, tecnologías y enlace al repositorio.</p>
              </article>
            </div>
          </section>

          <section class="section">
            <h2>Contacto</h2>
            <p class="muted">¿Quieres colaborar o contratarme? Escríbeme a <span id="email">tu.email@ejemplo.com</span> <button class="copy-btn" onclick="copyEmail()">Copiar</button></p>
          </section>
        </main>

        <aside>
          <div class="side-card">
            <h2>Redes</h2>
            <div class="socials">
              <a href="#" target="_blank">GitHub · github.com/tuusuario</a>
            </div>
            <div class="socials">
              <a href="#" target="_blank">LinkedIn · linkedin.com/in/tuusuario</a>
            </div>
            <div class="socials">
              <a href="#" target="_blank">Twitter · @tuusuario</a>
            </div>

            <hr style="margin:12px 0; border-color: rgba(255,255,255,0.03)">
            <p class="muted">Estadísticas (placeholder):</p>
            <p class="muted">⭐ Repos públicos: <strong>12</strong></p>
            <p class="muted">📊 Contribuciones (últimos 12 meses): <strong>420</strong></p>
          </div>

          <div style="height:12px"></div>

          <div class="side-card">
            <h2>Herramientas</h2>
            <p class="muted">Editor: VSCode · Terminal: bash · Sistema: Linux/Windows</p>
          </div>
        </aside>
      </div>

      <footer>
        Hecho con ♥ — Actualiza este perfil con tus datos reales antes de publicar.
      </footer>
    </div>
  </div>

  <script>
    function copyEmail(){
      const text = document.getElementById('email').innerText;
      navigator.clipboard?.writeText(text).then(()=>alert('Email copiado al portapapeles'))
    }
  </script>
</body>
</html>

<!--
**LichtSebas/LichtSebas** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
