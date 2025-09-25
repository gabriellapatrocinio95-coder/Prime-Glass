# Prime-Glass
Site institucional da Prime Glass — vidros e esquadrias em Goiânia
<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Prime Glass — Vidros e Esquadrias | Goiânia & Aparecida de Goiânia</title>
  <meta name="description" content="Prime Glass - vidros, boxes, espelhos e esquadrias planejadas em Goiânia e Aparecida de Goiânia. Atendimento de alto padrão." />
  <meta property="og:title" content="Prime Glass — Vidros e Esquadrias" />
  <meta property="og:description" content="Transformando sonhos em realidade com vidros e esquadrias de alto padrão." />
  <meta property="og:type" content="website" />
  <meta property="og:image" content="assets/hero.jpg" />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;700&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">

  <style>
    /* ====== VARIÁVEIS DE COR (Paleta da logo Prime Glass) ====== */
    :root{
      --primary:#003366;   /* Azul escuro sofisticado */
      --accent:#C9A04F;    /* Dourado elegante */
      --muted:#6b6f76;
      --bg:#ffffff;
      --card:#fbfbfb;
      --radius:12px;
      --maxw:1200px;
      --container-pad:20px;
    }

    /* ====== RESET e tipografia ====== */
    *{box-sizing:border-box}
    html,body{margin:0;padding:0;font-family:Inter,system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial; color:#222;background:var(--bg);-webkit-font-smoothing:antialiased}
    h1,h2,h3{font-family:"Playfair Display",serif;margin:0;color:var(--primary)}
    p{margin:0 0 1rem 0;line-height:1.5;color:var(--muted)}

    /* ====== LAYOUT ====== */
    header{position:sticky;top:0;z-index:50;background:rgba(255,255,255,0.95);backdrop-filter:blur(4px);box-shadow:0 4px 18px rgba(10,10,10,0.04)}
    .header-inner{max-width:var(--maxw);margin:0 auto;display:flex;align-items:center;justify-content:space-between;padding:16px var(--container-pad);height:72px}
    .logo{display:flex;align-items:center;gap:12px}
    .logo img{height:48px;object-fit:contain}
    nav{display:flex;gap:18px;align-items:center}
    nav a{color:var(--primary);text-decoration:none;font-weight:600}
    .btn-primary{background:var(--accent);color:white;padding:10px 16px;border-radius:8px;text-decoration:none;font-weight:600;transition:.3s}
    .btn-primary:hover{background:#b3863b}
    .btn-ghost{border:1px solid var(--accent);padding:8px 12px;border-radius:8px;color:var(--accent);text-decoration:none;transition:.3s}
    .btn-ghost:hover{background:var(--accent);color:white}

    /* ====== HERO ====== */
    .hero{max-width:var(--maxw);margin:0 auto;display:grid;grid-template-columns:1fr 1fr;gap:24px;align-items:center;padding:56px var(--container-pad)}
    .hero h1{font-size:2.4rem}
    .hero p{max-width:720px;font-size:1.1rem}
    .hero-ctas{display:flex;gap:12px;flex-wrap:wrap}
    .hero-visual{border-radius:16px;overflow:hidden;box-shadow:0 20px 60px rgba(11,42,59,0.12)}
    .hero-visual img{width:100%;height:100%;display:block;object-fit:cover;min-height:320px}

    /* ====== SEÇÕES ====== */
    section{max-width:var(--maxw);margin:0 auto;padding:48px var(--container-pad);border-top:1px solid #f2f2f2}
    .grid{display:grid;gap:20px}
    .grid-3{grid-template-columns:repeat(3,1fr)}
    .grid-2{grid-template-columns:1fr 1fr}
    .service-card{background:var(--card);padding:20px;border-radius:12px;box-shadow:0 8px 30px rgba(10,10,10,0.04);min-height:160px;border-left:4px solid var(--accent)}
    .service-card h3{margin-bottom:8px;color:var(--primary)}

    /* ====== GALERIA ====== */
    .gallery{display:grid;grid-template-columns:repeat(3,1fr);gap:12px}
    .gallery img{width:100%;height:100%;object-fit:cover;border-radius:10px;cursor:pointer;display:block;aspect-ratio:4/3;transition:.3s}
    .gallery img:hover{transform:scale(1.02)}

    /* ====== TESTIMONIALS ====== */
    .testimonial{background:var(--card);padding:18px;border-radius:12px;border-left:4px solid var(--accent)}

    /* ====== CONTATO ====== */
    .contact-wrap{display:grid;grid-template-columns:1fr 420px;gap:24px;align-items:start}
    .contact-form{background:var(--card);padding:20px;border-radius:12px;box-shadow:0 8px 30px rgba(0,0,0,0.04)}
    .field{display:flex;flex-direction:column;gap:8px;margin-bottom:12px}
    .field input,.field textarea{padding:10px;border-radius:8px;border:1px solid #e6e6e6;font-size:1rem}
    .map{border-radius:12px;overflow:hidden;box-shadow:0 12px 30px rgba(10,10,10,0.05)}

    /* ====== RODAPÉ ====== */
    footer{max-width:var(--maxw);margin:0 auto;padding:28px var(--container-pad);color:var(--muted);font-size:0.95rem;display:flex;justify-content:space-between;align-items:center;border-top:1px solid #f2f2f2}

    /* ====== RESPONSIVO ====== */
    @media (max-width:900px){
      .grid-3{grid-template-columns:1fr}
      .grid-2{grid-template-columns:1fr}
      .contact-wrap{grid-template-columns:1fr}
      .gallery{grid-template-columns:repeat(2,1fr)}
      .hero{grid-template-columns:1fr;padding:36px var(--container-pad)}
    }
    @media (max-width:520px){
      .gallery{grid-template-columns:1fr}
      .hero h1{font-size:1.6rem}
      .logo img{height:40px}
    }
  </style>
</head>
<body>
  <!-- Cabeçalho -->
  <header>
    <div class="header-inner">
      <div class="logo">
        <img src="assets/logo.png" alt="Prime Glass">
        <div style="line-height:1;">
          <div style="font-weight:700;color:var(--primary)">Prime Glass</div>
          <div style="font-size:12px;color:var(--muted)">Vidros & Esquadrias • Goiânia e Aparecida</div>
        </div>
      </div>

      <nav aria-label="Menu principal">
        <a href="#inicio">Início</a>
        <a href="#sobre">Sobre</a>
        <a href="#servicos">Serviços</a>
        <a href="#portfolio">Portfólio</a>
        <a href="#contato">Contato</a>
      </nav>

      <div style="display:flex;gap:10px;align-items:center">
        <a class="btn-ghost" href="https://www.instagram.com/vidrosprimeglass" target="_blank" rel="noopener">Instagram</a>
        <a class="btn-primary" href="https://wa.me/5562993053517" target="_blank" rel="noopener">WhatsApp (62) 99305-3517</a>
      </div>
    </div>
  </header>

  <!-- Aqui segue igual ao modelo anterior (hero, sobre, serviços, portfólio, depoimentos, contato e rodapé) -->

</body>
</html>
