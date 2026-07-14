<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Tu Empresa — Higiene profesional para restaurantes</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;600;700&family=Inter:wght@400;500;600;700&family=IBM+Plex+Mono:wght@500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --ink:#12211D;
    --teal:#0B5351;
    --teal-dark:#082F2E;
    --lime:#C7DC3F;
    --lime-dark:#9EB730;
    --steel:#7E9490;
    --panel:#E7ECE7;
    --cream:#F5F7F3;
    --white:#FFFFFF;
    --danger:#C24444;
    --success:#3E8E5A;
    --line: rgba(18,33,29,0.12);
    --radius: 16px;
    --radius-sm: 10px;
    --shadow-sm: 0 4px 14px -6px rgba(11,83,81,0.18);
    --shadow: 0 10px 30px -12px rgba(11,83,81,0.25);
    --shadow-lg: 0 30px 60px -20px rgba(0,0,0,0.35);
    --font-display:'Space Grotesk', sans-serif;
    --font-body:'Inter', sans-serif;
    --font-mono:'IBM Plex Mono', monospace;
  }

  *{margin:0;padding:0;box-sizing:border-box;}
  html{scroll-behavior:smooth;}
  @media (prefers-reduced-motion: reduce){
    html{scroll-behavior:auto;}
    *{animation-duration:0.001ms !important; transition-duration:0.001ms !important;}
  }

  body{
    font-family:var(--font-body);
    color:var(--ink);
    background:var(--cream);
    line-height:1.55;
    -webkit-font-smoothing:antialiased;
    overflow-x:hidden;
  }
  body.lock{ overflow:hidden; }

  a{color:inherit; text-decoration:none;}
  ul{list-style:none;}
  img,svg{display:block; max-width:100%;}
  button{ font-family:inherit; }

  ::selection{ background:var(--lime); color:var(--teal-dark); }
  ::-webkit-scrollbar{ width:10px; height:10px; }
  ::-webkit-scrollbar-track{ background:transparent; }
  ::-webkit-scrollbar-thumb{ background:var(--steel); border-radius:999px; }
  :focus-visible{ outline:3px solid var(--teal); outline-offset:3px; border-radius:4px; }

  .wrap{ max-width:1200px; margin:0 auto; padding:0 28px; }
  h1,h2,h3,h4{ font-family:var(--font-display); font-weight:600; letter-spacing:-0.01em; line-height:1.12; }
  .eyebrow{ font-family:var(--font-mono); font-size:0.72rem; letter-spacing:0.14em; text-transform:uppercase; color:var(--teal); font-weight:600; }

  .btn{
    display:inline-flex; align-items:center; justify-content:center; gap:8px;
    font-family:var(--font-body); font-weight:600; font-size:0.95rem;
    padding:13px 24px; border-radius:999px; border:1.5px solid transparent; cursor:pointer;
    transition:transform .18s ease, background .18s ease, color .18s ease, border-color .18s ease, box-shadow .18s ease;
    white-space:nowrap;
  }
  .btn-primary{ background:var(--lime); color:var(--teal-dark); }
  .btn-primary:hover{ transform:translateY(-2px); background:#d5e857; box-shadow:0 12px 24px -8px rgba(199,220,63,0.5); }
  .btn-primary:disabled{ opacity:.45; cursor:not-allowed; transform:none; box-shadow:none; }
  .btn-ghost{ background:transparent; color:var(--white); border-color:rgba(255,255,255,0.4); }
  .btn-ghost:hover{ border-color:var(--white); transform:translateY(-2px); }
  .btn-outline{ background:transparent; color:var(--teal); border-color:var(--teal); }
  .btn-outline:hover{ background:var(--teal); color:var(--white); transform:translateY(-2px); }
  .btn-dark{ background:var(--teal-dark); color:var(--white); }
  .btn-dark:hover{ background:var(--ink); transform:translateY(-2px); }
  .btn-sm{ padding:8px 16px; font-size:0.82rem; }
  .btn-block{ width:100%; }
  .btn:disabled{ opacity:.5; cursor:not-allowed; transform:none !important; box-shadow:none !important; }

  /* ---------- Header ---------- */
  header{ position:sticky; top:0; z-index:60; background:rgba(245,247,243,0.9); backdrop-filter:blur(10px); border-bottom:1px solid var(--line); }
  .nav{ display:flex; align-items:center; justify-content:space-between; padding:16px 28px; max-width:1200px; margin:0 auto; gap:20px; }
  .logo{ display:flex; align-items:center; gap:10px; font-family:var(--font-display); font-weight:700; font-size:1.3rem; letter-spacing:-0.02em; }
  .logo .dot{ width:11px;height:11px;border-radius:50%; background:var(--lime); box-shadow:0 0 0 4px rgba(199,220,63,0.25); }
  .nav-links{ display:flex; gap:30px; font-size:0.92rem; font-weight:500; margin-left:auto; }
  .nav-links a{ position:relative; padding:4px 0; color:var(--ink); }
  .nav-links a::after{ content:''; position:absolute; left:0; bottom:-2px; width:0; height:2px; background:var(--teal); transition:width .2s ease; }
  .nav-links a:hover::after{ width:100%; }
  .nav-cta{ display:flex; align-items:center; gap:10px; }

  .cart-btn{ position:relative; display:flex; align-items:center; gap:8px; background:var(--teal-dark); color:var(--white); border:none; border-radius:999px; padding:10px 16px 10px 12px; cursor:pointer; transition:transform .18s ease, background .18s ease; }
  .cart-btn:hover{ transform:translateY(-2px); background:var(--ink); }
  .cart-btn svg{ width:19px; height:19px; }
  .cart-count{ position:absolute; top:-7px; right:-7px; background:var(--lime); color:var(--teal-dark); font-family:var(--font-mono); font-size:0.68rem; font-weight:700; min-width:19px; height:19px; border-radius:999px; display:flex; align-items:center; justify-content:center; padding:0 4px; transition:transform .15s ease; }
  .cart-count.bump{ transform:scale(1.3); }
  .cart-count[data-empty="true"]{ opacity:0; transform:scale(0.4); }

  .account-btn{ display:flex; align-items:center; gap:8px; background:var(--panel); color:var(--teal-dark); border:1.5px solid transparent; border-radius:999px; padding:9px 15px; font-size:0.85rem; font-weight:600; cursor:pointer; transition:all .18s ease; max-width:190px; }
  .account-btn:hover{ background:var(--white); border-color:var(--teal); }
  .account-btn svg{ width:16px; height:16px; flex-shrink:0; }
  .account-btn span{ overflow:hidden; text-overflow:ellipsis; white-space:nowrap; }

  .nav-toggle{ display:none; background:none; border:1px solid var(--line); border-radius:8px; width:40px; height:40px; align-items:center; justify-content:center; cursor:pointer; }
  .nav-toggle svg{ width:20px; height:20px; }
  .mobile-menu{ display:none; flex-direction:column; gap:2px; background:var(--white); border-bottom:1px solid var(--line); padding:8px 28px 18px; }
  .mobile-menu.open{ display:flex; }
  .mobile-menu a{ padding:12px 4px; font-size:0.95rem; font-weight:500; border-bottom:1px solid var(--line); }
  .mobile-menu a:last-child{ border-bottom:none; }

  /* ---------- Hero ---------- */
  .hero{ background:linear-gradient(160deg,var(--teal-dark) 0%, var(--teal) 68%); color:var(--white); position:relative; overflow:hidden; }
  .hero::before{ content:''; position:absolute; inset:0; z-index:0; opacity:0.5; background-image:radial-gradient(circle, rgba(255,255,255,0.07) 1px, transparent 1.3px); background-size:24px 24px; }
  .hero::after{ content:''; position:absolute; top:-120px; right:-160px; width:520px; height:520px; background:radial-gradient(circle, rgba(199,220,63,0.16), transparent 70%); z-index:1; }
  .hero .wrap{ display:grid; grid-template-columns:1.05fr 0.95fr; gap:48px; align-items:center; padding-top:80px; padding-bottom:80px; position:relative; z-index:2; }
  .hero-eyebrow{ font-family:var(--font-mono); font-size:0.75rem; letter-spacing:0.16em; text-transform:uppercase; color:var(--lime); font-weight:600; margin-bottom:18px; display:flex; align-items:center; gap:10px; }
  .hero-eyebrow::before{ content:''; width:26px; height:1.5px; background:var(--lime); }
  .hero h1{ font-size:clamp(2.1rem, 4vw, 3.3rem); max-width:12ch; margin-bottom:20px; }
  .hero h1 em{ font-style:normal; color:var(--lime); }
  .hero > .wrap > .hero-copy > p{ font-size:1.06rem; color:rgba(255,255,255,0.82); max-width:46ch; margin-bottom:30px; }
  .hero-actions{ display:flex; gap:16px; flex-wrap:wrap; margin-bottom:36px;}
  .hero-meta{ display:flex; gap:28px; flex-wrap:wrap; padding-top:24px; border-top:1px solid rgba(255,255,255,0.18); }
  .hero-meta div{ display:flex; flex-direction:column; gap:2px; }
  .hero-meta strong{ font-family:var(--font-display); font-size:1.3rem; color:var(--lime); }
  .hero-meta span{ font-size:0.76rem; color:rgba(255,255,255,0.7); }

  .hero-art{ position:relative; }
  .hero-art svg{ width:100%; height:auto; filter:drop-shadow(0 30px 40px rgba(0,0,0,0.28)); animation:float 6s ease-in-out infinite; }
  @keyframes float{ 0%,100%{ transform:translateY(0); } 50%{ transform:translateY(-10px); } }

  /* ---------- Trust strip ---------- */
  .trust{ background:var(--white); border-bottom:1px solid var(--line); }
  .trust .wrap{ display:grid; grid-template-columns:repeat(4,1fr); gap:0; padding-top:32px; padding-bottom:32px; }
  .trust-item{ padding:0 22px; border-left:1px solid var(--line); }
  .trust-item:first-child{ border-left:none; padding-left:0; }
  .trust-item strong{ display:block; font-family:var(--font-display); font-size:1.4rem; color:var(--teal); margin-bottom:4px; }
  .trust-item span{ font-size:0.83rem; color:var(--steel); }

  /* ---------- Search + category pill nav ---------- */
  .cat-nav-wrap{ position:sticky; top:73px; z-index:40; background:rgba(245,247,243,0.95); backdrop-filter:blur(8px); border-bottom:1px solid var(--line); }
  .cat-nav-inner{ max-width:1200px; margin:0 auto; padding:14px 28px; display:flex; align-items:center; gap:16px; }
  .search-box{ position:relative; flex-shrink:0; width:220px; }
  .search-box input{
    width:100%; font-family:var(--font-body); font-size:0.85rem; padding:9px 14px 9px 34px;
    border:1px solid var(--line); border-radius:999px; background:var(--white); color:var(--ink);
    transition:border-color .18s ease, box-shadow .18s ease;
  }
  .search-box input:focus{ border-color:var(--teal); outline:none; box-shadow:0 0 0 3px rgba(11,83,81,0.12); }
  .search-box svg{ position:absolute; left:12px; top:50%; transform:translateY(-50%); width:15px; height:15px; color:var(--steel); pointer-events:none; }
  .search-clear{ position:absolute; right:8px; top:50%; transform:translateY(-50%); background:none; border:none; color:var(--steel); cursor:pointer; width:22px; height:22px; display:none; align-items:center; justify-content:center; border-radius:50%; }
  .search-clear:hover{ background:var(--panel); color:var(--ink); }
  .search-box.has-value .search-clear{ display:flex; }

  .cat-nav{ display:flex; gap:10px; overflow-x:auto; scrollbar-width:none; flex:1; min-width:0; }
  .cat-nav::-webkit-scrollbar{ display:none; }
  .cat-pill{
    flex-shrink:0; display:flex; align-items:center; gap:7px;
    font-size:0.84rem; font-weight:600; color:var(--steel);
    background:var(--white); border:1px solid var(--line);
    padding:9px 16px; border-radius:999px; cursor:pointer; transition:all .18s ease;
  }
  .cat-pill:hover{ border-color:var(--teal); color:var(--teal); }
  .cat-pill.active{ background:var(--teal-dark); border-color:var(--teal-dark); color:var(--lime); }
  .cat-pill .pill-count{ font-family:var(--font-mono); font-size:0.7rem; opacity:0.75; }

  /* ---------- Section heading ---------- */
  .section{ padding:88px 0; }
  .section-head{ display:flex; justify-content:space-between; align-items:flex-end; gap:24px; margin-bottom:46px; flex-wrap:wrap; }
  .section-head h2{ font-size:clamp(1.6rem, 3vw, 2.2rem); max-width:16ch; margin-top:10px; }
  .section-head p{ max-width:38ch; color:var(--steel); font-size:0.96rem; }

  /* ---------- Catalog ---------- */
  .catalog{ background:var(--cream); padding-top:52px; }
  .cat-group{ padding-top:36px; scroll-margin-top:150px; }
  .cat-group:first-child{ padding-top:0; }
  .cat-group + .cat-group{ border-top:1px solid var(--line); margin-top:52px; }
  .cat-group.is-filtered-out{ display:none; }
  .cat-group-head{ display:flex; align-items:flex-start; gap:16px; margin-bottom:28px; }
  .cat-group-icon{ width:50px; height:50px; border-radius:12px; background:var(--panel); display:flex; align-items:center; justify-content:center; color:var(--teal); flex-shrink:0; }
  .cat-group-icon svg{ width:26px; height:26px; }
  .cat-group-head h3{ font-size:1.3rem; margin-bottom:4px; display:flex; align-items:center; gap:10px; }
  .cat-group-head .group-count{ font-family:var(--font-mono); font-size:0.72rem; font-weight:600; color:var(--teal); background:var(--panel); padding:3px 9px; border-radius:999px; }
  .cat-group-head p{ color:var(--steel); font-size:0.92rem; max-width:56ch; }

  .grid{ display:grid; grid-template-columns:repeat(auto-fill, minmax(230px,1fr)); gap:20px; }

  .no-results{ display:none; flex-direction:column; align-items:center; gap:14px; text-align:center; padding:80px 20px; color:var(--steel); }
  .no-results.show{ display:flex; }
  .no-results svg{ width:40px; height:40px; color:var(--panel); }
  .no-results strong{ color:var(--ink); font-family:var(--font-display); font-size:1.1rem; }

  .card{
    display:flex; flex-direction:column; height:100%;
    background:var(--white); border-radius:18px; overflow:hidden;
    border:1px solid var(--line);
    transition:transform .22s ease, box-shadow .22s ease, border-color .22s ease;
  }
  .card:hover{ transform:translateY(-4px); box-shadow:var(--shadow); }
  .card.in-cart{ border-color:var(--lime-dark); box-shadow:0 0 0 3px rgba(199,220,63,0.22); }
  .card.is-hidden{ display:none; }

  .card-media{
    position:relative; width:100%; height:132px; background:var(--panel);
    display:flex; align-items:center; justify-content:center; overflow:hidden;
  }
  .card-media svg{ width:36px; height:36px; color:var(--teal); }
  .card-media .card-ref{
    position:absolute; top:10px; left:10px;
    background:rgba(8,20,18,0.72); color:var(--lime);
    font-family:var(--font-mono); font-size:0.63rem; letter-spacing:0.03em;
    padding:4px 9px; border-radius:6px;
  }
  .card.in-cart .card-media::after{
    content:'En tu pedido'; position:absolute; bottom:0; left:0; right:0;
    background:var(--teal-dark); color:var(--lime); text-align:center;
    font-size:0.66rem; font-weight:600; letter-spacing:0.03em; padding:4px 0;
  }

  .card-content{ display:flex; flex-direction:column; flex:1; padding:18px; gap:10px; }
  .card h4{ font-family:var(--font-display); font-size:0.98rem; font-weight:600; line-height:1.28; }
  .card-pres{ font-family:var(--font-mono); font-size:0.7rem; color:var(--teal); background:var(--panel); display:inline-block; padding:3px 9px; border-radius:999px; align-self:flex-start; }
  .card-bottom{ margin-top:auto; display:flex; align-items:center; justify-content:flex-end; gap:10px; }

  .stepper{ display:flex; align-items:center; gap:0; border:1.5px solid var(--line); border-radius:999px; overflow:hidden; }
  .stepper button{ width:32px; height:32px; border:none; background:var(--panel); color:var(--teal-dark); font-size:1.05rem; font-weight:700; cursor:pointer; display:flex; align-items:center; justify-content:center; transition:background .15s ease; }
  .stepper button:hover{ background:var(--lime); }
  .stepper button:disabled{ opacity:.4; cursor:not-allowed; }
  .stepper .qty{ width:34px; text-align:center; font-family:var(--font-mono); font-weight:600; font-size:0.9rem; }

  /* ---------- Why us ---------- */
  .why{ background:var(--white); border-top:1px solid var(--line); border-bottom:1px solid var(--line);}
  .why .wrap{ display:grid; grid-template-columns:0.9fr 1.1fr; gap:64px; align-items:center; }
  .why-visual{ background:var(--panel); border-radius:var(--radius); padding:36px; aspect-ratio:1/1; display:flex; align-items:center; justify-content:center; }
  .why-visual svg{ width:100%; height:100%; }
  .why-list{ display:flex; flex-direction:column; gap:24px; margin-top:26px; }
  .why-list li{ display:flex; gap:16px; }
  .why-num{ font-family:var(--font-mono); font-size:0.8rem; color:var(--teal); background:var(--panel); width:34px; height:34px; border-radius:8px; display:flex; align-items:center; justify-content:center; flex-shrink:0; }
  .why-list h4{ font-size:1.0rem; margin-bottom:4px; }
  .why-list p{ color:var(--steel); font-size:0.9rem; max-width:44ch; }

  /* ---------- Final CTA ---------- */
  .final-cta{ background:linear-gradient(160deg,var(--teal-dark) 0%, var(--teal) 75%); color:var(--white); }
  .final-cta .wrap{ text-align:center; display:flex; flex-direction:column; align-items:center; gap:18px; }
  .final-cta h2{ color:var(--white); font-size:clamp(1.6rem,3vw,2.2rem); max-width:22ch; }
  .final-cta p{ color:rgba(255,255,255,0.78); max-width:48ch; }
  .final-actions{ display:flex; gap:16px; flex-wrap:wrap; justify-content:center; margin-top:10px; }
  .final-direct{ margin-top:18px; font-size:0.88rem; color:rgba(255,255,255,0.65); }
  .final-direct a{ color:var(--lime); font-weight:600; }

  /* ---------- Footer ---------- */
  footer{ background:var(--ink); color:rgba(255,255,255,0.7); }
  footer .wrap{ display:grid; grid-template-columns:1.3fr 1fr 1fr 1fr; gap:40px; padding-top:60px; padding-bottom:32px; }
  .footer-brand .logo{ color:var(--white); margin-bottom:14px; }
  .footer-brand p{ font-size:0.87rem; max-width:32ch; color:rgba(255,255,255,0.55); }
  footer h5{ font-family:var(--font-mono); font-size:0.72rem; letter-spacing:0.1em; text-transform:uppercase; color:rgba(255,255,255,0.45); margin-bottom:16px; }
  footer ul{ display:flex; flex-direction:column; gap:10px; font-size:0.87rem; }
  footer ul a:hover{ color:var(--lime); }
  .footer-bottom{ border-top:1px solid rgba(255,255,255,0.1); padding:20px 28px; max-width:1200px; margin:0 auto; display:flex; justify-content:space-between; font-size:0.78rem; color:rgba(255,255,255,0.4); flex-wrap:wrap; gap:10px; }

  /* ---------- Overlay ---------- */
  .overlay{ position:fixed; inset:0; background:rgba(8,20,18,0.55); opacity:0; visibility:hidden; transition:opacity .25s ease, visibility .25s ease; z-index:80; }
  .overlay.show{ opacity:1; visibility:visible; }

  /* ---------- Cart drawer ---------- */
  .cart-drawer{ position:fixed; top:0; right:0; height:100%; width:min(420px,92vw); background:var(--white); z-index:90; display:flex; flex-direction:column; transform:translateX(100%); transition:transform .3s ease; box-shadow:-20px 0 50px rgba(0,0,0,0.2); }
  .cart-drawer.open{ transform:translateX(0); }
  .cart-head{ display:flex; align-items:center; justify-content:space-between; padding:22px 22px 18px; border-bottom:1px solid var(--line); }
  .cart-head h3{ font-size:1.1rem; }
  .cart-close{ background:var(--panel); border:none; width:34px; height:34px; border-radius:999px; cursor:pointer; display:flex; align-items:center; justify-content:center; }
  .cart-close svg{ width:16px; height:16px; }
  .cart-items{ flex:1; overflow-y:auto; padding:16px 22px; display:flex; flex-direction:column; gap:14px; }
  .cart-empty{ text-align:center; color:var(--steel); font-size:0.9rem; padding:60px 10px; display:flex; flex-direction:column; align-items:center; gap:14px; }
  .cart-empty svg{ width:44px; height:44px; color:var(--panel); }
  .cart-row{ display:flex; gap:12px; align-items:flex-start; border-bottom:1px solid var(--line); padding-bottom:14px; }
  .cart-row-media{ width:44px; height:44px; border-radius:10px; overflow:hidden; position:relative; background:var(--panel); flex-shrink:0; display:flex; align-items:center; justify-content:center; }
  .cart-row-media svg{ width:20px; height:20px; color:var(--teal); }
  .cart-row-info{ flex:1; }
  .cart-row-info h5{ font-family:var(--font-display); font-size:0.9rem; font-weight:600; line-height:1.3; }
  .cart-row-info span{ font-family:var(--font-mono); font-size:0.7rem; color:var(--steel); }
  .cart-row-actions{ display:flex; align-items:center; gap:8px; margin-top:8px; }
  .cart-row-remove{ background:none; border:none; color:var(--danger); font-size:0.75rem; cursor:pointer; text-decoration:underline; margin-top:8px; }
  .cart-foot{ padding:18px 22px 24px; border-top:1px solid var(--line); display:flex; flex-direction:column; gap:10px; }
  .cart-summary{ display:flex; justify-content:space-between; font-size:0.9rem; color:var(--steel); }
  .cart-summary strong{ color:var(--ink); font-family:var(--font-mono); }
  .cart-clear{ text-align:center; font-size:0.78rem; color:var(--steel); background:none; border:none; cursor:pointer; text-decoration:underline; }
  .cart-clear:hover{ color:var(--danger); }

  /* ---------- Modal (checkout + auth) ---------- */
  .modal{ position:fixed; top:50%; left:50%; transform:translate(-50%,-48%); width:min(520px,92vw); max-height:88vh; overflow-y:auto; background:var(--white); border-radius:18px; z-index:95; opacity:0; visibility:hidden; transition:opacity .25s ease, transform .25s ease, visibility .25s ease; box-shadow:var(--shadow-lg); }
  .modal.show{ opacity:1; visibility:visible; transform:translate(-50%,-50%); }
  .modal-head{ display:flex; align-items:flex-start; justify-content:space-between; gap:14px; padding:26px 26px 6px; }
  .modal-head h3{ font-size:1.25rem; margin-bottom:6px; }
  .modal-head p{ font-size:0.88rem; color:var(--steel); }
  .modal-close{ background:var(--panel); border:none; width:32px; height:32px; border-radius:999px; cursor:pointer; display:flex; align-items:center; justify-content:center; flex-shrink:0; }
  .modal-close svg{ width:15px; height:15px; }
  .modal-body{ padding:16px 26px 26px; }
  .modal-summary{ background:var(--cream); border:1px solid var(--line); border-radius:10px; padding:12px 14px; margin-bottom:18px; font-size:0.82rem; color:var(--steel); max-height:130px; overflow-y:auto; }
  .modal-summary div{ display:flex; justify-content:space-between; padding:4px 0; color:var(--ink); gap:10px; }
  .modal-summary div span:first-child{ overflow:hidden; text-overflow:ellipsis; white-space:nowrap; }
  .modal-summary div span:last-child{ font-family:var(--font-mono); color:var(--teal); flex-shrink:0; }
  .field{ display:flex; flex-direction:column; gap:6px; margin-bottom:15px; }
  .field label{ font-size:0.8rem; font-weight:600; color:var(--teal-dark); }
  .field label .opt{ color:var(--steel); font-weight:400; }
  .field input, .field select, .field textarea{ font-family:var(--font-body); font-size:0.92rem; padding:11px 13px; border:1.5px solid var(--line); border-radius:9px; background:var(--cream); color:var(--ink); transition:border-color .18s ease; }
  .field input:focus, .field select:focus, .field textarea:focus{ border-color:var(--teal); outline:none; }
  .field .field-error{ font-size:0.76rem; color:var(--danger); display:none; }
  .field.invalid input{ border-color:var(--danger); }
  .field.invalid .field-error{ display:block; }
  .form-row{ display:grid; grid-template-columns:1fr 1fr; gap:14px; }
  .modal-note{ font-size:0.76rem; color:var(--steel); margin-top:12px; text-align:center; }
  .wa-icon{ width:18px; height:18px; }

  /* ---------- Auth modal specific ---------- */
  .auth-tabs{ display:flex; gap:6px; background:var(--panel); border-radius:999px; padding:4px; margin-bottom:20px; }
  .auth-tab{ flex:1; text-align:center; padding:9px 0; border-radius:999px; font-size:0.85rem; font-weight:600; color:var(--steel); cursor:pointer; border:none; background:none; transition:all .18s ease; }
  .auth-tab.active{ background:var(--white); color:var(--teal-dark); box-shadow:var(--shadow-sm); }
  .auth-panel{ display:none; }
  .auth-panel.active{ display:block; }
  .auth-error{ background:rgba(194,68,68,0.08); border:1px solid rgba(194,68,68,0.3); color:var(--danger); font-size:0.82rem; padding:10px 12px; border-radius:9px; margin-bottom:14px; display:none; }
  .auth-error.show{ display:block; }
  .auth-disabled-note{ background:rgba(199,220,63,0.16); border:1px solid rgba(199,220,63,0.45); color:var(--teal-dark); font-size:0.78rem; padding:11px 13px; border-radius:9px; margin-bottom:18px; display:none; line-height:1.5; }
  .auth-disabled-note.show{ display:block; }
  .auth-success{ text-align:center; padding:10px 0 4px; }
  .auth-success svg{ width:44px; height:44px; color:var(--success); margin:0 auto 14px; }

  /* ---------- Toast ---------- */
  .toast{ position:fixed; bottom:24px; left:50%; transform:translateX(-50%) translateY(20px); background:var(--teal-dark); color:var(--white); padding:13px 22px; border-radius:999px; font-size:0.85rem; font-weight:500; display:flex; align-items:center; gap:8px; opacity:0; visibility:hidden; transition:all .25s ease; z-index:100; box-shadow:0 15px 30px -10px rgba(0,0,0,0.4); max-width:90vw; }
  .toast.show{ opacity:1; visibility:visible; transform:translateX(-50%) translateY(0); }
  .toast svg{ width:16px; height:16px; color:var(--lime); flex-shrink:0; }

  /* ---------- Favoritos ---------- */
  .card-fav{
    position:absolute; top:8px; right:8px; z-index:2;
    width:30px; height:30px; border-radius:999px; border:none;
    background:rgba(255,255,255,0.88); color:var(--steel);
    display:flex; align-items:center; justify-content:center; cursor:pointer;
    transition:transform .15s ease, color .15s ease, background .15s ease;
  }
  .card-fav svg{ width:16px; height:16px; }
  .card-fav:hover{ transform:scale(1.08); color:var(--lime-dark); }
  .card-fav.active{ color:#B8860B; }
  .card-fav.active svg{ fill:currentColor; }
  .cat-pill.fav-pill{ background:var(--white); }
  .cat-pill.fav-pill svg{ width:14px; height:14px; }
  .cat-pill.fav-pill.active{ background:#3E3410; border-color:#3E3410; color:#F0D97A; }

  /* ---------- Búsqueda: resaltado ---------- */
  mark.hit{ background:rgba(199,220,63,0.55); color:var(--teal-dark); border-radius:3px; padding:0 1px; }

  /* ---------- Presets de cantidad rápida ---------- */
  .qty-presets{ display:flex; gap:6px; margin-top:2px; }
  .qty-presets button{
    font-family:var(--font-mono); font-size:0.68rem; font-weight:600;
    color:var(--teal); background:var(--panel); border:1px solid transparent;
    border-radius:999px; padding:4px 9px; cursor:pointer; transition:all .15s ease;
  }
  .qty-presets button:hover{ background:var(--teal); color:var(--white); }
  .card-bottom{ flex-wrap:wrap; justify-content:space-between; }

  /* ---------- Notas por producto en el carrito ---------- */
  .cart-row-note{
    width:100%; font-family:var(--font-body); font-size:0.78rem;
    padding:7px 10px; border:1px solid var(--line); border-radius:8px;
    background:var(--cream); color:var(--ink); margin-top:8px; resize:none;
  }
  .cart-row-note:focus{ border-color:var(--teal); outline:none; }
  .cart-row-note-toggle{ background:none; border:none; color:var(--steel); font-size:0.75rem; cursor:pointer; text-decoration:underline; margin-top:8px; }

  /* ---------- Descargar resumen ---------- */
  .cart-secondary-actions{ display:flex; gap:8px; }
  .cart-secondary-actions .btn{ flex:1; }

  /* ---------- Barra fija de pedido (móvil) ---------- */
  .mobile-order-bar{
    position:fixed; left:0; right:0; bottom:0; z-index:70;
    background:var(--teal-dark); color:var(--white);
    display:none; align-items:center; justify-content:space-between; gap:14px;
    padding:12px 18px calc(12px + env(safe-area-inset-bottom));
    box-shadow:0 -10px 30px -8px rgba(0,0,0,0.35);
    transform:translateY(100%); transition:transform .25s ease;
  }
  .mobile-order-bar.show{ transform:translateY(0); }
  .mobile-order-bar-info{ display:flex; flex-direction:column; gap:1px; }
  .mobile-order-bar-info strong{ font-family:var(--font-display); font-size:0.95rem; }
  .mobile-order-bar-info span{ font-size:0.72rem; color:var(--lime); font-family:var(--font-mono); }
  .mobile-order-bar .btn{ flex-shrink:0; }

  /* ---------- Responsive ---------- */
  @media (max-width: 1024px){
    .grid{ grid-template-columns:repeat(auto-fill, minmax(200px,1fr)); }
  }
  @media (max-width: 900px){
    .hero .wrap{ grid-template-columns:1fr; padding-top:44px; padding-bottom:44px; gap:36px; }
    .hero-art{ order:-1; max-width:300px; margin:0 auto; }
    .hero-meta{ gap:20px; }
    .trust .wrap{ grid-template-columns:repeat(2,1fr); row-gap:22px; }
    .trust-item{ border-left:none !important; padding-left:0 !important; }
    .why .wrap{ grid-template-columns:1fr; gap:36px; }
    .why-visual{ max-width:280px; margin:0 auto; }
    footer .wrap{ grid-template-columns:1fr 1fr; gap:32px 24px; }
    .cat-nav-inner{ flex-wrap:wrap; padding:12px 20px; }
    .search-box{ width:100%; order:1; }
    .cat-nav{ order:2; width:100%; }
    body{ padding-bottom:0; }
  }
  @media (max-width: 640px){
    .nav-links{ display:none; }
    .nav-toggle{ display:flex; }
    .account-btn span{ display:none; }
    .account-btn{ padding:9px; }
    .cart-btn span:not(.cart-count){ display:none; }
    .form-row{ grid-template-columns:1fr; }
    footer .wrap{ grid-template-columns:1fr; gap:28px; }
    .section{ padding:52px 0; }
    .section-head{ margin-bottom:32px; }
    .nav{ padding:12px 16px; }
    .wrap{ padding:0 16px; }
    .grid{ grid-template-columns:repeat(auto-fill, minmax(150px,1fr)); gap:12px; }
    .card-media{ height:96px; }
    .hero-meta{ justify-content:space-between; }
    .hero-meta div{ flex:1 1 30%; }
    .modal{ width:100vw; max-width:100vw; left:0; right:0; top:auto; bottom:0; transform:translateY(100%); border-radius:20px 20px 0 0; max-height:92vh; }
    .modal.show{ transform:translateY(0); }
    .cart-drawer{ width:100vw; }
    body.has-cart-items{ padding-bottom:74px; }
    .mobile-order-bar{ display:flex; }
    .final-actions{ flex-direction:column; width:100%; }
    .final-actions .btn{ width:100%; }
  }
  @media (max-width: 400px){
    .hero h1{ max-width:14ch; }
    .trust .wrap{ grid-template-columns:1fr 1fr; }
    .grid{ grid-template-columns:repeat(auto-fill, minmax(135px,1fr)); }
  }

  /* Altura de header dinámica para offsets de scroll (fallback si JS no corre) */
  .cat-nav-wrap{ position:sticky; top:var(--header-h, 73px); }
</style>
</head>
<body>

<header>
  <nav class="nav">
    <a href="#" class="logo"><span class="dot"></span>Tu Empresa</a>
    <ul class="nav-links">
      <li><a href="#catalogo">Catálogo</a></li>
      <li><a href="#nosotros">Por qué nosotros</a></li>
      <li><a href="#contacto">Contacto</a></li>
    </ul>
    <div class="nav-cta">
      <button class="account-btn" id="accountBtn" onclick="openAuth()" aria-label="Iniciar sesión">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="8" r="4"/><path d="M4 20c0-4 4-6 8-6s8 2 8 6"/></svg>
        <span id="accountBtnLabel">Iniciar sesión</span>
      </button>
      <button class="cart-btn" onclick="openCart()" aria-label="Ver pedido">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M6 6h15l-1.5 9h-12L6 6Z"/><path d="M6 6 4.5 3H2"/><circle cx="9" cy="20" r="1.3" fill="currentColor" stroke="none"/><circle cx="17" cy="20" r="1.3" fill="currentColor" stroke="none"/></svg>
        <span>Mi pedido</span>
        <span class="cart-count" id="cartCount" data-empty="true">0</span>
      </button>
      <button class="nav-toggle" onclick="toggleMobileMenu()" aria-label="Abrir menú">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M4 7h16M4 12h16M4 17h16"/></svg>
      </button>
    </div>
  </nav>
  <div class="mobile-menu" id="mobileMenu">
    <a href="#catalogo" onclick="toggleMobileMenu()">Catálogo</a>
    <a href="#nosotros" onclick="toggleMobileMenu()">Por qué nosotros</a>
    <a href="#contacto" onclick="toggleMobileMenu()">Contacto</a>
  </div>
</header>

<section class="hero">
  <div class="wrap">
    <div class="hero-copy">
      <div class="hero-eyebrow">Suministro para HORECA</div>
      <h1>Higiene profesional para cocinas que <em>no se detienen</em>.</h1>
      <p>Surtimos a restaurantes, cocinas industriales y cadenas de alimentos con productos de limpieza y desinfección pensados para el ritmo de un servicio real — no para el hogar.</p>
      <div class="hero-actions">
        <a href="#catalogo" class="btn btn-primary">Ver catálogo completo</a>
        <button class="btn btn-ghost" onclick="openCart()">Armar mi pedido</button>
      </div>
      <div class="hero-meta">
        <div><strong>+150</strong><span>cocinas comerciales surtidas</span></div>
        <div><strong>24–48h</strong><span>tiempo de entrega</span></div>
        <div><strong id="catCountMeta">6</strong><span>líneas de producto especializadas</span></div>
      </div>
    </div>
    <div class="hero-art">
      <svg viewBox="0 0 420 460" xmlns="http://www.w3.org/2000/svg">
        <defs>
          <linearGradient id="bottleGrad" x1="0" y1="0" x2="1" y2="1"><stop offset="0" stop-color="#C7DC3F"/><stop offset="1" stop-color="#93B02C"/></linearGradient>
          <linearGradient id="drumGrad" x1="0" y1="0" x2="0" y2="1"><stop offset="0" stop-color="#F5F7F3"/><stop offset="1" stop-color="#CFDAD3"/></linearGradient>
        </defs>
        <ellipse cx="210" cy="430" rx="160" ry="18" fill="#03201F" opacity="0.35"/>
        <rect x="70" y="230" width="150" height="180" rx="16" fill="url(#drumGrad)"/>
        <rect x="70" y="230" width="150" height="34" rx="16" fill="#0B5351" opacity="0.15"/>
        <rect x="86" y="300" width="118" height="26" rx="4" fill="#0B5351"/>
        <text x="145" y="318" font-family="IBM Plex Mono, monospace" font-size="12" fill="#C7DC3F" text-anchor="middle" font-weight="600">DES-02</text>
        <rect x="86" y="345" width="70" height="8" rx="4" fill="#7E9490" opacity="0.5"/>
        <rect x="86" y="362" width="95" height="8" rx="4" fill="#7E9490" opacity="0.5"/>
        <g>
          <rect x="230" y="150" width="118" height="230" rx="18" fill="#FFFFFF"/>
          <rect x="230" y="150" width="118" height="230" rx="18" fill="#0B5351" opacity="0.06"/>
          <rect x="252" y="180" width="74" height="150" rx="10" fill="url(#bottleGrad)"/>
          <rect x="264" y="196" width="50" height="18" rx="3" fill="#082F2E"/>
          <text x="289" y="209" font-family="IBM Plex Mono, monospace" font-size="9" fill="#C7DC3F" text-anchor="middle" font-weight="600">DEG-01</text>
          <rect x="270" y="110" width="42" height="46" rx="8" fill="#082F2E"/>
          <rect x="278" y="70" width="8" height="46" rx="4" fill="#082F2E"/>
          <circle cx="282" cy="66" r="8" fill="#C7DC3F"/>
        </g>
        <g>
          <rect x="20" y="290" width="70" height="120" rx="12" fill="#0B5351"/>
          <rect x="34" y="270" width="42" height="26" rx="6" fill="#0B5351"/>
          <rect x="48" y="255" width="14" height="20" rx="4" fill="#082F2E"/>
          <rect x="32" y="330" width="46" height="18" rx="4" fill="#F5F7F3" opacity="0.9"/>
          <text x="55" y="343" font-family="IBM Plex Mono, monospace" font-size="8" fill="#0B5351" text-anchor="middle" font-weight="600">LOZ-03</text>
        </g>
        <circle cx="340" cy="120" r="4" fill="#C7DC3F" opacity="0.8"/>
        <circle cx="360" cy="150" r="2.5" fill="#C7DC3F" opacity="0.6"/>
        <circle cx="40" cy="240" r="3" fill="#C7DC3F" opacity="0.6"/>
      </svg>
    </div>
  </div>
</section>

<section class="trust">
  <div class="wrap">
    <div class="trust-item"><strong>24–48 h</strong><span>Entrega a tu restaurante</span></div>
    <div class="trust-item"><strong>+150</strong><span>Cocinas comerciales surtidas</span></div>
    <div class="trust-item"><strong id="totalProductsMeta">0</strong><span>Productos disponibles en catálogo</span></div>
    <div class="trust-item"><strong>A tu medida</strong><span>Asesoría en dilución, uso y almacenamiento</span></div>
  </div>
</section>

<div class="cat-nav-wrap">
  <div class="cat-nav-inner">
    <div class="search-box" id="searchBox">
      <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="11" cy="11" r="7"/><path d="m21 21-4.3-4.3"/></svg>
      <input type="text" id="searchInput" placeholder="Buscar producto..." oninput="filterCatalog(this.value)" aria-label="Buscar producto">
      <button class="search-clear" onclick="clearSearch()" aria-label="Limpiar búsqueda">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M6 6l12 12M18 6L6 18"/></svg>
      </button>
    </div>
    <div class="cat-nav" id="catNav"></div>
  </div>
</div>

<section class="section catalog" id="catalogo">
  <div class="wrap">
    <div class="section-head">
      <div>
        <span class="eyebrow">Catálogo</span>
        <h2>Selecciona lo que necesita tu cocina</h2>
      </div>
      <p>No manejamos precios en línea: agrega los productos que necesitas a tu pedido y lo enviamos directo a tu asesor por WhatsApp para cotizarlo.</p>
    </div>

    <div id="catalogGroups"></div>

    <div class="no-results" id="noResults">
      <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"><circle cx="11" cy="11" r="7"/><path d="m21 21-4.3-4.3"/></svg>
      <strong>No encontramos ese producto</strong>
      <span>Intenta con otra palabra o revisa las categorías del catálogo.</span>
      <button class="btn btn-outline btn-sm" onclick="clearSearch()">Ver todo el catálogo</button>
    </div>
  </div>
</section>

<section class="section why" id="nosotros">
  <div class="wrap">
    <div class="why-visual">
      <svg viewBox="0 0 300 300" xmlns="http://www.w3.org/2000/svg">
        <circle cx="150" cy="150" r="130" fill="#0B5351" opacity="0.06"/>
        <circle cx="150" cy="150" r="95" fill="#0B5351" opacity="0.08"/>
        <rect x="105" y="70" width="90" height="150" rx="14" fill="#0B5351"/>
        <rect x="120" y="100" width="60" height="10" rx="5" fill="#C7DC3F"/>
        <rect x="120" y="120" width="44" height="8" rx="4" fill="#F5F7F3" opacity="0.7"/>
        <rect x="120" y="136" width="52" height="8" rx="4" fill="#F5F7F3" opacity="0.7"/>
        <rect x="120" y="152" width="38" height="8" rx="4" fill="#F5F7F3" opacity="0.7"/>
        <circle cx="150" cy="190" r="14" fill="#C7DC3F"/>
        <path d="M144 190l4 4 8-8" stroke="#082F2E" stroke-width="2.4" fill="none" stroke-linecap="round" stroke-linejoin="round"/>
        <rect x="60" y="200" width="34" height="50" rx="8" fill="#7E9490"/>
        <rect x="206" y="180" width="34" height="70" rx="8" fill="#7E9490"/>
      </svg>
    </div>
    <div class="why-copy">
      <span class="eyebrow">Por qué nosotros</span>
      <h2 style="margin-top:10px; max-width:18ch;">Diseñado para cocinas que trabajan a diario, no para el hogar</h2>
      <ul class="why-list">
        <li><span class="why-num">01</span><div><h4>Formulado para el ritmo de una cocina real</h4><p>Concentraciones y rendimiento pensados para servicio diario, no para uso doméstico ocasional.</p></div></li>
        <li><span class="why-num">02</span><div><h4>Cumplimiento con normativa sanitaria</h4><p>Cada línea cuenta con ficha técnica y de seguridad disponible para tus auditorías e inspecciones.</p></div></li>
        <li><span class="why-num">03</span><div><h4>Reposición programada</h4><p>Coordinamos entregas recurrentes para que nunca te falte insumo en plena operación.</p></div></li>
      </ul>
    </div>
  </div>
</section>

<section class="section final-cta" id="contacto">
  <div class="wrap">
    <span class="eyebrow" style="color:var(--lime)">Tu pedido</span>
    <h2>Agrega lo que necesitas y lo enviamos directo por WhatsApp</h2>
    <p>Selecciona los productos del catálogo, ábrelo desde el botón "Mi pedido" y en un minuto tu solicitud llega ordenada a tu asesor — sin llamadas, sin esperar cotización por correo.</p>
    <div class="final-actions">
      <button class="btn btn-primary" onclick="openCart()">Ver mi pedido</button>
      <a href="#catalogo" class="btn btn-ghost">Seguir viendo el catálogo</a>
    </div>
    <p class="final-direct">¿Prefieres hablar directo? Escríbenos a <a href="https://wa.me/529613267670" target="_blank" rel="noopener">WhatsApp</a> o al correo <a href="mailto:ventas@tuempresa.mx">ventas@tuempresa.mx</a></p>
  </div>
</section>

<footer>
  <div class="wrap">
    <div class="footer-brand">
      <a href="#" class="logo"><span class="dot"></span>Tu Empresa</a>
      <p>Suministro de productos de limpieza e higiene para restaurantes, cocinas industriales y cadenas de alimentos.</p>
    </div>
    <div>
      <h5>Catálogo</h5>
      <ul id="footerCatLinks"></ul>
    </div>
    <div>
      <h5>Empresa</h5>
      <ul>
        <li><a href="#nosotros">Por qué nosotros</a></li>
        <li><a href="#contacto">Contacto</a></li>
        <li><a href="#">Aviso de privacidad</a></li>
      </ul>
    </div>
    <div>
      <h5>Contacto directo</h5>
      <ul>
        <li>ventas@tuempresa.mx</li>
        <li>+52 961 326 7670</li>
        <li>Tabasco, México</li>
      </ul>
    </div>
  </div>
  <div class="footer-bottom">
    <span>© 2026 Tu Empresa. Todos los derechos reservados.</span>
    <span>Higiene profesional para restaurantes</span>
  </div>
</footer>

<!-- Barra fija de pedido (solo visible en móvil con productos en el pedido) -->
<div class="mobile-order-bar" id="mobileOrderBar">
  <div class="mobile-order-bar-info">
    <strong id="mobileOrderUnits">0 piezas</strong>
    <span id="mobileOrderLines">0 productos</span>
  </div>
  <button type="button" class="btn btn-primary btn-sm" onclick="openCart()">Ver pedido</button>
</div>

<!-- Overlay -->
<div class="overlay" id="overlay" onclick="closeAll()"></div>

<!-- Cart drawer -->
<aside class="cart-drawer" id="cartDrawer" aria-label="Mi pedido">
  <div class="cart-head">
    <h3>Mi pedido</h3>
    <button class="cart-close" onclick="closeCart()" aria-label="Cerrar"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M6 6l12 12M18 6L6 18"/></svg></button>
  </div>
  <div class="cart-items" id="cartItems"></div>
  <div class="cart-foot">
    <div class="cart-summary">
      <span>Productos distintos</span>
      <strong id="cartLinesCount">0</strong>
    </div>
    <div class="cart-summary">
      <span>Piezas / envases en total</span>
      <strong id="cartUnitsCount">0</strong>
    </div>
    <button class="btn btn-primary btn-block" id="checkoutBtn" onclick="openCheckout()" disabled>Enviar pedido por WhatsApp</button>
    <div class="cart-secondary-actions">
      <button class="btn btn-outline btn-sm" id="downloadBtn" onclick="downloadOrderSummary()" style="display:none;">Descargar resumen</button>
      <button class="cart-clear" id="cartClearBtn" onclick="clearCart()" style="display:none;">Vaciar pedido</button>
    </div>
  </div>
</aside>

<!-- Checkout modal -->
<div class="modal" id="checkoutModal" role="dialog" aria-label="Datos para tu pedido">
  <div class="modal-head">
    <div>
      <h3>Un último paso</h3>
      <p>Con estos datos armamos tu pedido y lo mandamos directo a WhatsApp.</p>
    </div>
    <button class="modal-close" onclick="closeCheckout()" aria-label="Cerrar"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M6 6l12 12M18 6L6 18"/></svg></button>
  </div>
  <div class="modal-body">
    <div class="modal-summary" id="modalSummary"></div>
    <form id="checkoutForm" onsubmit="return sendOrder(event)" novalidate>
      <div class="field" id="fieldNegocio">
        <label for="negocio">Nombre del negocio / restaurante</label>
        <input id="negocio" type="text" placeholder="Ej. Restaurante El Buen Sabor" required>
        <span class="field-error">Escribe el nombre de tu negocio.</span>
      </div>
      <div class="form-row">
        <div class="field" id="fieldContacto">
          <label for="contacto2">Nombre de quien solicita</label>
          <input id="contacto2" type="text" placeholder="Tu nombre" required>
          <span class="field-error">Escribe tu nombre.</span>
        </div>
        <div class="field" id="fieldTelefono">
          <label for="telefono">Teléfono</label>
          <input id="telefono" type="tel" inputmode="numeric" placeholder="10 dígitos" required>
          <span class="field-error">Escribe un teléfono a 10 dígitos.</span>
        </div>
      </div>
      <div class="field">
        <label for="direccion">Dirección o sucursal <span class="opt">(opcional)</span></label>
        <input id="direccion" type="text" placeholder="Dirección de entrega o nombre de sucursal">
      </div>
      <div class="field">
        <label for="fechaEntrega">Fecha de entrega preferida <span class="opt">(opcional)</span></label>
        <input id="fechaEntrega" type="date">
      </div>
      <div class="field">
        <label for="notas">Notas adicionales <span class="opt">(opcional)</span></label>
        <textarea id="notas" rows="2" placeholder="Horario de entrega, referencias, etc."></textarea>
      </div>
      <button type="submit" class="btn btn-primary btn-block" id="sendOrderBtn">
        <svg class="wa-icon" viewBox="0 0 24 24" fill="currentColor"><path d="M17.5 14.4c-.3-.1-1.7-.8-2-.9-.3-.1-.5-.1-.7.1-.2.3-.7.9-.9 1-.2.2-.4.2-.7.1-.3-.1-1.3-.5-2.4-1.5-.9-.8-1.5-1.8-1.7-2.1-.2-.3 0-.5.1-.6.1-.1.3-.4.4-.5.1-.2.2-.3.1-.6-.1-.3-.7-1.7-.9-2.1-.2-.4-.4-.4-.6-.4h-.5c-.2 0-.5.1-.7.4-.2.3-.9 1-.9 2.3 0 1.3 1 2.6 1.1 2.8.1.2 1.9 2.9 4.6 4 2.7 1.1 2.7.7 3.2.7.5-.1 1.7-.7 1.9-1.4.2-.7.2-1.3.2-1.4 0-.1-.1-.2-.3-.3Z"/><path d="M12 2a10 10 0 0 0-8.6 15.1L2 22l5-1.3A10 10 0 1 0 12 2Zm0 18.2c-1.6 0-3.1-.4-4.5-1.2l-.3-.2-3 .8.8-2.9-.2-.3A8.2 8.2 0 1 1 20.2 12 8.2 8.2 0 0 1 12 20.2Z"/></svg>
        Enviar pedido por WhatsApp
      </button>
      <p class="modal-note">Se abrirá WhatsApp con tu pedido ya redactado, listo para enviarlo.</p>
    </form>
  </div>
</div>

<!-- Auth modal (login / registro) -->
<div class="modal" id="authModal" role="dialog" aria-label="Iniciar sesión o crear cuenta">
  <div class="modal-head">
    <div>
      <h3 id="authTitle">Tu cuenta</h3>
      <p>Regístrate una vez y tus datos se autocompletan en cada pedido.</p>
    </div>
    <button class="modal-close" onclick="closeAuth()" aria-label="Cerrar"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M6 6l12 12M18 6L6 18"/></svg></button>
  </div>
  <div class="modal-body">

    <div class="auth-disabled-note" id="authDisabledNote">
      ⚠️ El inicio de sesión aún no está conectado a una base de datos (Firebase). Puedes seguir armando tu pedido y enviarlo por WhatsApp sin iniciar sesión.
    </div>

    <div id="authLoggedInView" style="display:none;">
      <div class="auth-success">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M20 6 9 17l-5-5"/></svg>
        <p style="margin-bottom:4px;"><strong id="loggedInName">—</strong></p>
        <p style="color:var(--steel); font-size:0.88rem;" id="loggedInEmail">—</p>
      </div>
      <button type="button" class="btn btn-outline btn-block" style="margin-top:18px;" onclick="handleLogout()">Cerrar sesión</button>
    </div>

    <div id="authFormsView">
      <div class="auth-tabs">
        <button type="button" class="auth-tab active" id="tabLogin" onclick="switchAuthTab('login')">Iniciar sesión</button>
        <button type="button" class="auth-tab" id="tabRegister" onclick="switchAuthTab('register')">Crear cuenta</button>
      </div>

      <div class="auth-error" id="authError"></div>

      <div class="auth-panel active" id="panelLogin">
        <form id="loginForm" onsubmit="return handleLogin(event)">
          <div class="field">
            <label for="loginEmail">Correo</label>
            <input id="loginEmail" type="email" placeholder="tucorreo@ejemplo.com" required>
          </div>
          <div class="field">
            <label for="loginPassword">Contraseña</label>
            <input id="loginPassword" type="password" placeholder="Tu contraseña" required minlength="6">
          </div>
          <button type="submit" class="btn btn-primary btn-block" id="loginBtn">Iniciar sesión</button>
        </form>
      </div>

      <div class="auth-panel" id="panelRegister">
        <form id="registerForm" onsubmit="return handleRegister(event)">
          <div class="field">
            <label for="regNegocio">Nombre del negocio</label>
            <input id="regNegocio" type="text" placeholder="Ej. Restaurante El Buen Sabor" required>
          </div>
          <div class="form-row">
            <div class="field">
              <label for="regContacto">Nombre de contacto</label>
              <input id="regContacto" type="text" placeholder="Tu nombre" required>
            </div>
            <div class="field">
              <label for="regTelefono">Teléfono</label>
              <input id="regTelefono" type="tel" placeholder="10 dígitos" required>
            </div>
          </div>
          <div class="field">
            <label for="regEmail">Correo</label>
            <input id="regEmail" type="email" placeholder="tucorreo@ejemplo.com" required>
          </div>
          <div class="form-row">
            <div class="field">
              <label for="regPassword">Contraseña</label>
              <input id="regPassword" type="password" placeholder="Mínimo 6 caracteres" required minlength="6">
            </div>
            <div class="field">
              <label for="regPassword2">Confirmar</label>
              <input id="regPassword2" type="password" placeholder="Repite la contraseña" required minlength="6">
            </div>
          </div>
          <button type="submit" class="btn btn-primary btn-block" id="registerBtn">Crear cuenta</button>
        </form>
      </div>
    </div>

  </div>
</div>

<!-- Toast -->
<div class="toast" id="toast" role="status" aria-live="polite"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.4" stroke-linecap="round" stroke-linejoin="round"><path d="M20 6 9 17l-5-5"/></svg><span id="toastMsg">Agregado a tu pedido</span></div>

<!-- ================= FIREBASE SDK (compat) =================
     Si no vas a usar el login por ahora, puedes dejar estas líneas tal cual:
     la página seguirá funcionando normal (catálogo + WhatsApp) sin registro. -->
<script src="https://www.gstatic.com/firebasejs/10.12.2/firebase-app-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/10.12.2/firebase-auth-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/10.12.2/firebase-firestore-compat.js"></script>

<script>
  /* ======================================================================
     CONFIGURACIÓN — edita solo estos dos bloques
     ====================================================================== */

  // 1) Tu número de WhatsApp de negocio.
  //    Formato: código de país + número, SIN espacios, signos ni "+".
  const WHATSAPP_NUMBER = "529613267670";

  // 2) Tu configuración de Firebase (Firebase Console > Configuración del proyecto > SDK de Firebase).
  //    Mientras dejes "TU_API_KEY" tal cual, el registro/login queda desactivado
  //    de forma segura y el resto de la página funciona normal.
  const firebaseConfig = {
    apiKey: "TU_API_KEY",
    authDomain: "TU_PROYECTO.firebaseapp.com",
    projectId: "TU_PROYECTO",
    storageBucket: "TU_PROYECTO.appspot.com",
    messagingSenderId: "TU_ID_MENSAJERIA",
    appId: "TU_APP_ID"
  };

  /* ======================================================================
     CATEGORÍAS
     ====================================================================== */
  const CATEGORIES = [
    {
      id:'cat-deg', label:'Desengrasantes y limpieza general',
      short:'Desengrasantes',
      desc:'Limpiadores multiusos y desengrasantes de uso diario para cocina y superficies generales.',
      icon:'<path d="M8 3h8l1 4H7l1-4Z"/><path d="M6 7h12l1 13a1 1 0 0 1-1 1H6a1 1 0 0 1-1-1L6 7Z"/><path d="M9 12h6"/><path d="M9 16h6"/>'
    },
    {
      id:'cat-des', label:'Desinfección y control de plagas',
      short:'Desinfectantes',
      desc:'Cloro, ácidos y línea de insecticidas para mantener tus áreas libres de bacterias y plagas.',
      icon:'<path d="M12 2s6 6.5 6 11a6 6 0 1 1-12 0c0-4.5 6-11 6-11Z"/><path d="M9.5 15.5a2.5 2.5 0 0 0 3 2.4"/>'
    },
    {
      id:'cat-loz', label:'Loza, cocina y lavandería',
      short:'Loza y lavandería',
      desc:'Jabones, fibras y detergentes para vajilla, ollas, utensilios y ropa de trabajo.',
      icon:'<circle cx="12" cy="13" r="7"/><path d="M9 13a3 3 0 0 0 3 3"/><path d="M12 3v3"/>'
    },
    {
      id:'cat-hig', label:'Higiene de manos y papel',
      short:'Higiene de manos',
      desc:'Jabón para manos y línea de papel institucional para baños, vestidores y cocina.',
      icon:'<path d="M7 11V7a5 5 0 0 1 10 0v4"/><path d="M5 11h14l-1.2 8.4a2 2 0 0 1-2 1.6H8.2a2 2 0 0 1-2-1.6L5 11Z"/>'
    },
    {
      id:'cat-pis', label:'Pisos, sanitarios y ambientación',
      short:'Pisos',
      desc:'Trapeadores, escobas, cepillos y tapetes para el mantenimiento diario de pisos y baños.',
      icon:'<path d="M3 17h18"/><path d="M3 21h18"/><path d="M8 17c0-5 2-9 4-13 2 4 4 8 4 13"/>'
    },
    {
      id:'cat-eqp', label:'Equipos, accesorios y textiles',
      short:'Equipos',
      desc:'Trapos, franelas, bolsas y accesorios de apoyo para el equipo de limpieza.',
      icon:'<path d="M14 3l7 7-8.5 8.5L4 20l1.5-8.5L14 3Z"/><path d="M12 8l4 4"/>'
    }
  ];

  /* ======================================================================
     PRODUCTOS — tu catálogo real, organizado por categoría
     ====================================================================== */
  const PRODUCTS = [
    // Desengrasantes y limpieza general
    { id:'deg-1', cat:'cat-deg', ref:'DEG-01', name:'Multiuso Fabuloso', pres:'Botella 1L' },
    { id:'deg-2', cat:'cat-deg', ref:'DEG-02', name:'Multiuso Desengrasante', pres:'Botella 1L' },
    { id:'deg-3', cat:'cat-deg', ref:'DEG-03', name:'Limpia vidrios', pres:'Botella 650ml' },

    // Desinfección y control de plagas
    { id:'des-1', cat:'cat-des', ref:'DES-01', name:'Cloro a granel al 6%', pres:'Litro (a granel)' },
    { id:'des-2', cat:'cat-des', ref:'DES-02', name:'Ácido muriático rosado', pres:'Botella 1L' },
    { id:'des-3', cat:'cat-des', ref:'DES-03', name:'Raid Casa y Jardín', pres:'Aerosol 400ml' },
    { id:'des-4', cat:'cat-des', ref:'DES-04', name:'Raid Max', pres:'Aerosol 360ml' },
    { id:'des-5', cat:'cat-des', ref:'DES-05', name:'Aerosol Raid', pres:'Aerosol 227ml' },
    { id:'des-6', cat:'cat-des', ref:'DES-06', name:'Pato discos activos', pres:'Paquete 2 piezas' },

    // Loza, cocina y lavandería
    { id:'loz-1', cat:'cat-loz', ref:'LOZ-01', name:'Jabón lavatrastes tipo Axion', pres:'Pieza 400g' },
    { id:'loz-2', cat:'cat-loz', ref:'LOZ-02', name:'Fibra verde Scotch Brite', pres:'Paquete 3 piezas' },
    { id:'loz-3', cat:'cat-loz', ref:'LOZ-03', name:'Fibra esponja Scotch Brite', pres:'Paquete 3 piezas' },
    { id:'loz-4', cat:'cat-loz', ref:'LOZ-04', name:'Fibra negra Scotch Brite', pres:'Pieza' },
    { id:'loz-5', cat:'cat-loz', ref:'LOZ-05', name:'Detergente en polvo', pres:'Bolsa 1kg' },

    // Higiene de manos y papel
    { id:'hig-1', cat:'cat-hig', ref:'HIG-01', name:'Shampoo para manos', pres:'Bidón 1L' },
    { id:'hig-2', cat:'cat-hig', ref:'HIG-02', name:'Toalla en rollo (GC Paper)', pres:'Rollo institucional' },
    { id:'hig-3', cat:'cat-hig', ref:'HIG-03', name:'Toalla interdoblada (GC Paper)', pres:'Paquete 150 hojas' },
    { id:'hig-4', cat:'cat-hig', ref:'HIG-04', name:'Papel higiénico (GC Paper)', pres:'Paquete 4 rollos' },

    // Pisos, sanitarios y ambientación
    { id:'pis-1', cat:'cat-pis', ref:'PIS-01', name:'Trapeador Magitel', pres:'Pieza' },
    { id:'pis-2', cat:'cat-pis', ref:'PIS-02', name:'Trapeador Twister', pres:'Pieza' },
    { id:'pis-3', cat:'cat-pis', ref:'PIS-03', name:'Trapeador Pabilo', pres:'Pieza' },
    { id:'pis-4', cat:'cat-pis', ref:'PIS-04', name:'Escoba Veneciana', pres:'Pieza' },
    { id:'pis-5', cat:'cat-pis', ref:'PIS-05', name:'Escoba Abanico', pres:'Pieza' },
    { id:'pis-6', cat:'cat-pis', ref:'PIS-06', name:'Cepillo para baño', pres:'Pieza' },
    { id:'pis-7', cat:'cat-pis', ref:'PIS-07', name:'Tapete mingitorio Weise', pres:'Pieza' },
    { id:'pis-8', cat:'cat-pis', ref:'PIS-08', name:'Aerosol Weise', pres:'Aerosol 400ml' },

    // Equipos, accesorios y textiles
    { id:'eqp-1', cat:'cat-eqp', ref:'EQP-01', name:'Cepillo plancha para ropa', pres:'Pieza' },
    { id:'eqp-2', cat:'cat-eqp', ref:'EQP-02', name:'Trapo microfibra', pres:'Paquete 3 piezas' },
    { id:'eqp-3', cat:'cat-eqp', ref:'EQP-03', name:'Franela gris', pres:'Paquete 5 piezas' },
    { id:'eqp-4', cat:'cat-eqp', ref:'EQP-04', name:'Bolsas negras', pres:'Paquete' },
    { id:'eqp-5', cat:'cat-eqp', ref:'EQP-05', name:'Atomizador de 1 litro', pres:'Pieza' }
  ];

  let cart = {};           // id -> qty
  let cartNotes = {};      // id -> nota opcional del producto
  let favorites = new Set(); // ids marcados como favoritos (sesión actual)
  let currentUser = null;  // { uid, email, negocio, contacto, telefono } | null
  let activeQuery = '';
  let showOnlyFavorites = false;
  const FAV_PILL_ID = 'fav-pill';

  const catById = id => CATEGORIES.find(c => c.id === id);
  const iconFor = cat => `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round">${cat.icon}</svg>`;

  /* ---------------------------------------------------------------------
     RENDER: navegación de categorías + catálogo + footer
     --------------------------------------------------------------------- */
  function renderCatNav(){
    const nav = document.getElementById('catNav');
    const favBtn = `<button type="button" class="cat-pill fav-pill" id="${FAV_PILL_ID}" onclick="toggleFavoritesFilter()" aria-pressed="false">
      <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M12 3.5l2.6 5.3 5.9.8-4.3 4.1 1 5.8-5.2-2.8-5.2 2.8 1-5.8-4.3-4.1 5.9-.8L12 3.5Z"/></svg>
      Favoritos<span class="pill-count" id="favPillCount">0</span>
    </button>`;
    const catBtns = CATEGORIES.map(cat=>{
      const count = PRODUCTS.filter(p=>p.cat===cat.id).length;
      return `<button type="button" class="cat-pill" data-target="${cat.id}" onclick="scrollToCat('${cat.id}')">${cat.short}<span class="pill-count">${count}</span></button>`;
    }).join('');
    nav.innerHTML = favBtn + catBtns;
  }

  function toggleFavoritesFilter(){
    showOnlyFavorites = !showOnlyFavorites;
    const pill = document.getElementById(FAV_PILL_ID);
    if(pill){
      pill.classList.toggle('active', showOnlyFavorites);
      pill.setAttribute('aria-pressed', String(showOnlyFavorites));
    }
    filterCatalog(document.getElementById('searchInput') ? document.getElementById('searchInput').value : '');
  }

  function toggleFavorite(id){
    if(favorites.has(id)) favorites.delete(id); else favorites.add(id);
    const btn = document.querySelector(`.card-fav[data-id="${id}"]`);
    if(btn) btn.classList.toggle('active', favorites.has(id));
    const countEl = document.getElementById('favPillCount');
    if(countEl) countEl.textContent = favorites.size;
    if(showOnlyFavorites) filterCatalog(document.getElementById('searchInput').value);
  }

  function renderFooterLinks(){
    const el = document.getElementById('footerCatLinks');
    el.innerHTML = CATEGORIES.slice(0,4).map(cat=>`<li><a href="#${cat.id}">${cat.short}</a></li>`).join('');
  }

  function renderCatalog(){
    const wrap = document.getElementById('catalogGroups');
    wrap.innerHTML = CATEGORIES.map(cat=>{
      const items = PRODUCTS.filter(p=>p.cat===cat.id);
      return `
      <div class="cat-group" id="${cat.id}" data-cat="${cat.id}">
        <div class="cat-group-head">
          <div class="cat-group-icon">${iconFor(cat)}</div>
          <div>
            <h3>${cat.label} <span class="group-count" data-role="group-count">${items.length}</span></h3>
            <p>${cat.desc}</p>
          </div>
        </div>
        <div class="grid" data-grid="${cat.id}">
          ${items.map(p=>cardHTML(p)).join('')}
        </div>
      </div>`;
    }).join('');

    document.getElementById('catCountMeta').textContent = CATEGORIES.length;
    document.getElementById('totalProductsMeta').textContent = PRODUCTS.length + '+';
  }

  function cardHTML(p){
    const cat = catById(p.cat);
    return `
    <div class="card" id="card-${p.id}" data-name="${p.name.toLowerCase()}" data-ref="${p.ref.toLowerCase()}">
      <div class="card-media">
        ${iconFor(cat)}
        <span class="card-ref">REF. ${p.ref}</span>
        <button type="button" class="card-fav" data-id="${p.id}" onclick="toggleFavorite('${p.id}')" aria-label="Marcar ${p.name} como favorito">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M12 3.5l2.6 5.3 5.9.8-4.3 4.1 1 5.8-5.2-2.8-5.2 2.8 1-5.8-4.3-4.1 5.9-.8L12 3.5Z"/></svg>
        </button>
      </div>
      <div class="card-content">
        <h4 data-role="card-title">${p.name}</h4>
        <span class="card-pres">${p.pres}</span>
        <div class="card-bottom">
          <div class="qty-presets">
            <button type="button" onclick="addQty('${p.id}', 5)">+5</button>
            <button type="button" onclick="addQty('${p.id}', 10)">+10</button>
          </div>
          <div class="stepper">
            <button type="button" aria-label="Quitar uno de ${p.name}" onclick="changeQty('${p.id}', -1)">−</button>
            <span class="qty" id="qty-${p.id}">0</span>
            <button type="button" aria-label="Agregar uno de ${p.name}" onclick="changeQty('${p.id}', 1)">+</button>
          </div>
        </div>
      </div>
    </div>`;
  }

  /* ---------------------------------------------------------------------
     BUSCADOR
     --------------------------------------------------------------------- */
  function highlightText(text, query){
    if(!query) return text;
    try{
      const escaped = query.replace(/[.*+?^${}()|[\]\\]/g, '\\$&');
      const re = new RegExp(`(${escaped})`, 'ig');
      return text.replace(re, '<mark class="hit">$1</mark>');
    } catch(err){ return text; }
  }

  let searchDebounce = null;
  function filterCatalog(query){
    clearTimeout(searchDebounce);
    searchDebounce = setTimeout(()=> applyFilters(query), 90);
  }

  function applyFilters(query){
    activeQuery = (query || '').trim().toLowerCase();
    const searchBox = document.getElementById('searchBox');
    searchBox.classList.toggle('has-value', activeQuery.length > 0);

    let anyVisible = false;

    CATEGORIES.forEach(cat=>{
      const group = document.getElementById(cat.id);
      if(!group) return;
      const cards = group.querySelectorAll('.card');
      let visibleInGroup = 0;

      cards.forEach(card=>{
        const id = card.id.replace('card-','');
        const p = PRODUCTS.find(x=>x.id===id);
        const matchesQuery = !activeQuery || card.dataset.name.includes(activeQuery) || card.dataset.ref.includes(activeQuery);
        const matchesFav = !showOnlyFavorites || favorites.has(id);
        const matches = matchesQuery && matchesFav;
        card.classList.toggle('is-hidden', !matches);
        if(matches) visibleInGroup++;

        const titleEl = card.querySelector('[data-role="card-title"]');
        if(titleEl && p) titleEl.innerHTML = highlightText(p.name, activeQuery);
      });

      group.classList.toggle('is-filtered-out', visibleInGroup === 0);
      const countEl = group.querySelector('[data-role="group-count"]');
      if(countEl) countEl.textContent = visibleInGroup;
      if(visibleInGroup > 0) anyVisible = true;
    });

    document.getElementById('noResults').classList.toggle('show', !anyVisible);
  }

  function clearSearch(){
    const input = document.getElementById('searchInput');
    input.value = '';
    applyFilters('');
    input.focus();
  }

  function scrollToCat(catId){
    if(activeQuery) clearSearch();
    const target = document.getElementById(catId);
    if(!target) return;
    const offset = window._scrollOffset || 150;
    window.scrollTo({ top: target.getBoundingClientRect().top + window.scrollY - offset, behavior:'smooth' });
  }

  /* ---------------------------------------------------------------------
     CARRITO
     --------------------------------------------------------------------- */
  function changeQty(id, delta){
    const current = cart[id] || 0;
    const next = Math.max(0, current + delta);
    cart[id] = next;
    if(next === 0) delete cart[id];

    const qtyEl = document.getElementById(`qty-${id}`);
    if(qtyEl) qtyEl.textContent = next;
    const cardEl = document.getElementById(`card-${id}`);
    if(cardEl) cardEl.classList.toggle('in-cart', next > 0);

    updateCartBadge();
    renderCartDrawer();
    if(delta > 0) showToast('Agregado a tu pedido');
  }

  function addQty(id, amount){
    changeQty(id, amount);
  }

  function setQty(id, value){
    const next = Math.max(0, value);
    cart[id] = next;
    if(next === 0) delete cart[id];
    const qtyEl = document.getElementById(`qty-${id}`);
    if(qtyEl) qtyEl.textContent = next;
    const cardEl = document.getElementById(`card-${id}`);
    if(cardEl) cardEl.classList.toggle('in-cart', next > 0);
    updateCartBadge();
    renderCartDrawer();
  }

  function clearCart(){
    if(Object.keys(cart).length === 0) return;
    if(!confirm('¿Vaciar todo tu pedido actual?')) return;
    Object.keys(cart).forEach(id => setQty(id, 0));
    showToast('Pedido vaciado');
  }

  function totalUnits(){ return Object.values(cart).reduce((a,b)=>a+b,0); }
  function totalLines(){ return Object.keys(cart).length; }

  function updateCartBadge(){
    const el = document.getElementById('cartCount');
    if(!el) return;
    const units = totalUnits();
    el.textContent = units;
    el.dataset.empty = units === 0 ? 'true' : 'false';
    el.classList.remove('bump');
    requestAnimationFrame(()=> el.classList.add('bump'));

    const bar = document.getElementById('mobileOrderBar');
    if(bar){
      bar.classList.toggle('show', units > 0);
      document.getElementById('mobileOrderUnits').textContent = `${units} pieza${units===1?'':'s'}`;
      document.getElementById('mobileOrderLines').textContent = `${totalLines()} producto${totalLines()===1?'':'s'}`;
    }
    document.body.classList.toggle('has-cart-items', units > 0);
  }

  function renderCartDrawer(){
    const wrap = document.getElementById('cartItems');
    if(!wrap) return;
    const ids = Object.keys(cart);
    document.getElementById('cartLinesCount').textContent = totalLines();
    document.getElementById('cartUnitsCount').textContent = totalUnits();
    document.getElementById('checkoutBtn').disabled = ids.length === 0;
    document.getElementById('cartClearBtn').style.display = ids.length === 0 ? 'none' : 'block';
    document.getElementById('downloadBtn').style.display = ids.length === 0 ? 'none' : 'block';

    if(ids.length === 0){
      wrap.innerHTML = `
        <div class="cart-empty">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><path d="M6 6h15l-1.5 9h-12L6 6Z"/><path d="M6 6 4.5 3H2"/></svg>
          <span>Tu pedido está vacío.<br>Agrega productos desde el catálogo.</span>
        </div>`;
      return;
    }

    wrap.innerHTML = ids.map(id=>{
      const p = PRODUCTS.find(x=>x.id===id);
      if(!p) return '';
      const cat = catById(p.cat);
      const qty = cart[id];
      const note = cartNotes[id] || '';
      return `
      <div class="cart-row">
        <div class="cart-row-media">${iconFor(cat)}</div>
        <div class="cart-row-info">
          <h5>${p.name}</h5>
          <span>${p.pres}</span>
          <div class="cart-row-actions">
            <div class="stepper">
              <button type="button" aria-label="Quitar uno" onclick="changeQty('${p.id}', -1)">−</button>
              <span class="qty">${qty}</span>
              <button type="button" aria-label="Agregar uno" onclick="changeQty('${p.id}', 1)">+</button>
            </div>
          </div>
          <textarea class="cart-row-note" placeholder="Nota para este producto (ej. marca, color)" oninput="setCartNote('${p.id}', this.value)">${note}</textarea>
          <button type="button" class="cart-row-remove" onclick="setQty('${p.id}', 0)">Quitar</button>
        </div>
      </div>`;
    }).join('');
  }

  function setCartNote(id, value){
    if(value && value.trim()){ cartNotes[id] = value; }
    else { delete cartNotes[id]; }
  }

  /* ---------------------------------------------------------------------
     OVERLAY / DRAWER / MODALES
     --------------------------------------------------------------------- */
  function openCart(){
    document.getElementById('overlay').classList.add('show');
    document.getElementById('cartDrawer').classList.add('open');
    document.body.classList.add('lock');
  }
  function closeCart(){
    document.getElementById('cartDrawer').classList.remove('open');
    if(!document.getElementById('checkoutModal').classList.contains('show') &&
       !document.getElementById('authModal').classList.contains('show')){
      document.getElementById('overlay').classList.remove('show');
      document.body.classList.remove('lock');
    }
  }
  function openCheckout(){
    if(totalLines() === 0) return;
    renderModalSummary();
    if(currentUser){
      const negocioEl = document.getElementById('negocio');
      const contactoEl = document.getElementById('contacto2');
      const telEl = document.getElementById('telefono');
      if(negocioEl && !negocioEl.value) negocioEl.value = currentUser.negocio || '';
      if(contactoEl && !contactoEl.value) contactoEl.value = currentUser.contacto || '';
      if(telEl && !telEl.value) telEl.value = currentUser.telefono || '';
    }
    document.getElementById('cartDrawer').classList.remove('open');
    document.getElementById('overlay').classList.add('show');
    document.getElementById('checkoutModal').classList.add('show');
    document.body.classList.add('lock');
    setTimeout(()=>{
      const negocioEl = document.getElementById('negocio');
      if(negocioEl && !negocioEl.value) negocioEl.focus();
    }, 260);
  }
  function closeCheckout(){
    document.getElementById('checkoutModal').classList.remove('show');
    document.getElementById('overlay').classList.remove('show');
    document.body.classList.remove('lock');
  }
  function openAuth(){
    clearAuthError();
    document.getElementById('overlay').classList.add('show');
    document.getElementById('authModal').classList.add('show');
    document.body.classList.add('lock');
  }
  function closeAuth(){
    document.getElementById('authModal').classList.remove('show');
    document.getElementById('overlay').classList.remove('show');
    document.body.classList.remove('lock');
  }
  function closeAll(){
    closeCart();
    closeCheckout();
    closeAuth();
    document.getElementById('overlay').classList.remove('show');
    document.body.classList.remove('lock');
  }
  document.addEventListener('keydown', (e)=>{ if(e.key === 'Escape') closeAll(); });

  function renderModalSummary(){
    const ids = Object.keys(cart);
    const el = document.getElementById('modalSummary');
    if(!el) return;
    el.innerHTML = ids.map(id=>{
      const p = PRODUCTS.find(x=>x.id===id);
      if(!p) return '';
      return `<div><span>${p.name} (${p.pres})</span><span>x${cart[id]}</span></div>`;
    }).join('');
  }

  function showToast(msg){
    const t = document.getElementById('toast');
    if(!t) return;
    document.getElementById('toastMsg').textContent = msg;
    t.classList.add('show');
    clearTimeout(window._toastTimer);
    window._toastTimer = setTimeout(()=> t.classList.remove('show'), 2400);
  }

  function toggleMobileMenu(){
    const el = document.getElementById('mobileMenu');
    if(el) el.classList.toggle('open');
  }

  /* ---------------------------------------------------------------------
     VALIDACIÓN Y ENVÍO DE PEDIDO POR WHATSAPP
     --------------------------------------------------------------------- */
  function setFieldValid(fieldId, valid){
    const field = document.getElementById(fieldId);
    if(field) field.classList.toggle('invalid', !valid);
  }

  function sendOrder(e){
    e.preventDefault();
    try{
      const negocio = document.getElementById('negocio').value.trim();
      const contacto = document.getElementById('contacto2').value.trim();
      const telefono = document.getElementById('telefono').value.trim();
      const direccion = document.getElementById('direccion').value.trim();
      const fechaEntrega = document.getElementById('fechaEntrega').value;
      const notas = document.getElementById('notas').value.trim();

      const telDigits = telefono.replace(/\D/g,'');
      let valid = true;
      setFieldValid('fieldNegocio', !!negocio); if(!negocio) valid = false;
      setFieldValid('fieldContacto', !!contacto); if(!contacto) valid = false;
      setFieldValid('fieldTelefono', telDigits.length >= 10); if(telDigits.length < 10) valid = false;

      if(!valid || totalLines() === 0) return false;

      const lines = [];
      lines.push('📄 *Nuevo pedido*');
      lines.push('');
      lines.push(`🏬 Negocio: ${negocio}`);
      lines.push(`👤 Solicita: ${contacto}`);
      lines.push(`📞 Teléfono: ${telefono}`);
      if(direccion) lines.push(`📍 Dirección / sucursal: ${direccion}`);
      if(fechaEntrega) lines.push(`📅 Entrega preferida: ${fechaEntrega}`);
      lines.push('');
      lines.push('🛒 *Productos solicitados:*');
      Object.keys(cart).forEach((id, i)=>{
        const p = PRODUCTS.find(x=>x.id===id);
        if(!p) return;
        let line = `${i+1}. ${p.name} (${p.pres}) — cantidad: ${cart[id]}`;
        if(cartNotes[id]) line += ` — nota: ${cartNotes[id]}`;
        lines.push(line);
      });
      lines.push('');
      if(notas) lines.push(`📄 Notas: ${notas}`);
      lines.push('');
      lines.push('Quedo al pendiente de la cotización, gracias.');

      const message = lines.join('\n');
      const url = `https://wa.me/${WHATSAPP_NUMBER}?text=${encodeURIComponent(message)}`;
      window.open(url, '_blank');
      closeCheckout();
      showToast('Pedido listo — revisa WhatsApp para enviarlo');
    } catch(err){
      console.error('No se pudo generar el pedido:', err);
      showToast('Hubo un problema al armar el pedido, intenta de nuevo');
    }
    return false;
  }

  /* ---------------------------------------------------------------------
     DESCARGAR RESUMEN DEL PEDIDO (respaldo en texto, sin depender de WhatsApp)
     --------------------------------------------------------------------- */
  function downloadOrderSummary(){
    try{
      const ids = Object.keys(cart);
      if(ids.length === 0) return;
      const fecha = new Date().toLocaleString('es-MX');
      const lines = [`Resumen de pedido — Tu Empresa`, `Generado: ${fecha}`, ''];
      ids.forEach((id,i)=>{
        const p = PRODUCTS.find(x=>x.id===id);
        if(!p) return;
        let line = `${i+1}. ${p.name} (${p.pres}) — cantidad: ${cart[id]}`;
        if(cartNotes[id]) line += ` — nota: ${cartNotes[id]}`;
        lines.push(line);
      });
      lines.push('', `Total de productos distintos: ${totalLines()}`, `Total de piezas: ${totalUnits()}`);
      const blob = new Blob([lines.join('\n')], { type:'text/plain;charset=utf-8' });
      const url = URL.createObjectURL(blob);
      const a = document.createElement('a');
      a.href = url;
      a.download = `pedido-tu-empresa-${Date.now()}.txt`;
      document.body.appendChild(a);
      a.click();
      a.remove();
      URL.revokeObjectURL(url);
      showToast('Resumen descargado');
    } catch(err){
      console.error('No se pudo descargar el resumen:', err);
      showToast('No se pudo descargar el resumen, intenta de nuevo');
    }
  }

  /* ---------------------------------------------------------------------
     OFFSETS DINÁMICOS (evita números "mágicos" fijos en el responsive)
     --------------------------------------------------------------------- */
  function updateStickyOffsets(){
    try{
      const header = document.querySelector('header');
      const catNavWrap = document.querySelector('.cat-nav-wrap');
      if(!header) return;
      const headerH = header.getBoundingClientRect().height;
      document.documentElement.style.setProperty('--header-h', `${headerH}px`);
      const catNavH = catNavWrap ? catNavWrap.getBoundingClientRect().height : 0;
      document.querySelectorAll('.cat-group').forEach(g=>{
        g.style.scrollMarginTop = `${headerH + catNavH + 16}px`;
      });
      window._scrollOffset = headerH + catNavH + 16;
    } catch(err){ console.error('Error al calcular offsets de scroll:', err); }
  }

  /* ---------------------------------------------------------------------
     SCROLLSPY DE CATEGORÍAS
     --------------------------------------------------------------------- */
  function initScrollSpy(){
    const pills = Array.from(document.querySelectorAll('.cat-pill'));
    const groups = CATEGORIES.map(c=>document.getElementById(c.id)).filter(Boolean);
    if(!('IntersectionObserver' in window) || groups.length === 0) return;
    const observer = new IntersectionObserver((entries)=>{
      entries.forEach(entry=>{
        if(entry.isIntersecting){
          const idx = groups.indexOf(entry.target);
          pills.forEach(p=>p.classList.remove('active'));
          if(idx>-1 && pills[idx]) pills[idx].classList.add('active');
        }
      });
    }, { rootMargin:'-160px 0px -60% 0px', threshold:0 });
    groups.forEach(g=> observer.observe(g));
  }

  /* =======================================================================
     FIREBASE — AUTENTICACIÓN Y PERFIL DE CLIENTE (opcional)
     Todo va protegido con try/catch: si Firebase no está configurado o
     falla la conexión, la página sigue funcionando normal sin login.
     ======================================================================= */
  let firebaseReady = false;
  let fbAuth = null;
  let fbDb = null;

  function initFirebase(){
    try{
      const isConfigured = firebaseConfig && firebaseConfig.apiKey && firebaseConfig.apiKey !== 'TU_API_KEY';
      if(!isConfigured || typeof firebase === 'undefined'){
        firebaseReady = false;
        return;
      }
      firebase.initializeApp(firebaseConfig);
      fbAuth = firebase.auth();
      fbDb = firebase.firestore();
      firebaseReady = true;

      fbAuth.onAuthStateChanged(async (user)=>{
        if(user){
          let profile = {};
          try{
            const doc = await fbDb.collection('clientes').doc(user.uid).get();
            if(doc.exists) profile = doc.data();
          } catch(err){
            console.error('No se pudo leer el perfil del cliente:', err);
          }
          currentUser = {
            uid: user.uid,
            email: user.email || '',
            negocio: profile.negocio || '',
            contacto: profile.contacto || '',
            telefono: profile.telefono || ''
          };
        } else {
          currentUser = null;
        }
        updateAccountUI();
      });
    } catch(err){
      console.error('Firebase no se pudo inicializar:', err);
      firebaseReady = false;
    }
  }

  function updateAccountUI(){
    const btn = document.getElementById('accountBtn');
    const label = document.getElementById('accountBtnLabel');
    const loggedInView = document.getElementById('authLoggedInView');
    const formsView = document.getElementById('authFormsView');
    if(!btn || !label) return;

    if(currentUser){
      label.textContent = currentUser.negocio || currentUser.email || 'Mi cuenta';
      if(loggedInView) loggedInView.style.display = 'block';
      if(formsView) formsView.style.display = 'none';
      const nameEl = document.getElementById('loggedInName');
      const emailEl = document.getElementById('loggedInEmail');
      if(nameEl) nameEl.textContent = currentUser.negocio || 'Cliente';
      if(emailEl) emailEl.textContent = currentUser.email || '';
    } else {
      label.textContent = 'Iniciar sesión';
      if(loggedInView) loggedInView.style.display = 'none';
      if(formsView) formsView.style.display = 'block';
    }
  }

  function switchAuthTab(tab){
    const tabLogin = document.getElementById('tabLogin');
    const tabRegister = document.getElementById('tabRegister');
    const panelLogin = document.getElementById('panelLogin');
    const panelRegister = document.getElementById('panelRegister');
    if(!tabLogin || !tabRegister || !panelLogin || !panelRegister) return;
    clearAuthError();
    if(tab === 'register'){
      tabRegister.classList.add('active'); tabLogin.classList.remove('active');
      panelRegister.classList.add('active'); panelLogin.classList.remove('active');
    } else {
      tabLogin.classList.add('active'); tabRegister.classList.remove('active');
      panelLogin.classList.add('active'); panelRegister.classList.remove('active');
    }
  }

  function showAuthError(msg){
    const el = document.getElementById('authError');
    if(!el) return;
    el.textContent = msg;
    el.classList.add('show');
  }
  function clearAuthError(){
    const el = document.getElementById('authError');
    if(!el) return;
    el.textContent = '';
    el.classList.remove('show');
  }

  function mapFirebaseError(err){
    const code = err && err.code ? err.code : '';
    const map = {
      'auth/email-already-in-use': 'Ese correo ya tiene una cuenta registrada.',
      'auth/invalid-email': 'El correo no es válido.',
      'auth/weak-password': 'La contraseña debe tener al menos 6 caracteres.',
      'auth/user-not-found': 'No encontramos una cuenta con ese correo.',
      'auth/wrong-password': 'La contraseña es incorrecta.',
      'auth/invalid-credential': 'Correo o contraseña incorrectos.',
      'auth/too-many-requests': 'Demasiados intentos. Espera un momento e inténtalo de nuevo.',
      'auth/network-request-failed': 'Problema de conexión. Revisa tu internet e intenta de nuevo.'
    };
    return map[code] || (err && err.message) || 'Ocurrió un error inesperado. Intenta de nuevo.';
  }

  async function handleLogin(e){
    e.preventDefault();
    clearAuthError();

    if(!firebaseReady){
      showAuthError('El inicio de sesión aún no está conectado a una base de datos.');
      return false;
    }

    const emailEl = document.getElementById('loginEmail');
    const passEl = document.getElementById('loginPassword');
    const btn = document.getElementById('loginBtn');
    if(!emailEl || !passEl) return false;

    const email = emailEl.value.trim();
    const password = passEl.value;

    if(!email || !password){
      showAuthError('Completa correo y contraseña.');
      return false;
    }

    try{
      if(btn){ btn.disabled = true; btn.textContent = 'Entrando...'; }
      await fbAuth.signInWithEmailAndPassword(email, password);
      showToast('Sesión iniciada');
      closeAuth();
    } catch(err){
      console.error('Error de inicio de sesión:', err);
      showAuthError(mapFirebaseError(err));
    } finally {
      if(btn){ btn.disabled = false; btn.textContent = 'Iniciar sesión'; }
    }
    return false;
  }

  async function handleRegister(e){
    e.preventDefault();
    clearAuthError();

    if(!firebaseReady){
      showAuthError('El registro aún no está conectado a una base de datos.');
      return false;
    }

    const negocioEl = document.getElementById('regNegocio');
    const contactoEl = document.getElementById('regContacto');
    const telefonoEl = document.getElementById('regTelefono');
    const emailEl = document.getElementById('regEmail');
    const passEl = document.getElementById('regPassword');
    const pass2El = document.getElementById('regPassword2');
    const btn = document.getElementById('registerBtn');
    if(!negocioEl || !contactoEl || !telefonoEl || !emailEl || !passEl || !pass2El) return false;

    const negocio = negocioEl.value.trim();
    const contacto = contactoEl.value.trim();
    const telefono = telefonoEl.value.trim();
    const email = emailEl.value.trim();
    const password = passEl.value;
    const password2 = pass2El.value;

    if(!negocio || !contacto || !telefono || !email || !password || !password2){
      showAuthError('Completa todos los campos.');
      return false;
    }
    if(password.length < 6){
      showAuthError('La contraseña debe tener al menos 6 caracteres.');
      return false;
    }
    if(password !== password2){
      showAuthError('Las contraseñas no coinciden.');
      return false;
    }

    try{
      if(btn){ btn.disabled = true; btn.textContent = 'Creando cuenta...'; }
      const cred = await fbAuth.createUserWithEmailAndPassword(email, password);
      try{
        await fbDb.collection('clientes').doc(cred.user.uid).set({
          negocio, contacto, telefono, email,
          creadoEn: firebase.firestore.FieldValue.serverTimestamp()
        });
      } catch(err){
        console.error('La cuenta se creó pero no se pudo guardar el perfil:', err);
      }
      showToast('Cuenta creada, ¡bienvenido!');
      closeAuth();
    } catch(err){
      console.error('Error de registro:', err);
      showAuthError(mapFirebaseError(err));
    } finally {
      if(btn){ btn.disabled = false; btn.textContent = 'Crear cuenta'; }
    }
    return false;
  }

  async function handleLogout(){
    try{
      if(firebaseReady && fbAuth){
        await fbAuth.signOut();
      } else {
        currentUser = null;
        updateAccountUI();
      }
      showToast('Sesión cerrada');
      closeAuth();
    } catch(err){
      console.error('Error al cerrar sesión:', err);
      showToast('No se pudo cerrar sesión, intenta de nuevo');
    }
  }

  /* ---------------------------------------------------------------------
     INICIALIZACIÓN
     --------------------------------------------------------------------- */
  document.addEventListener('DOMContentLoaded', function(){
    try{ renderCatNav(); } catch(err){ console.error('Error al iniciar la navegación de categorías:', err); }
    try{ renderFooterLinks(); } catch(err){ console.error('Error al iniciar el pie de página:', err); }
    try{ renderCatalog(); } catch(err){ console.error('Error al renderizar el catálogo:', err); }
    try{ initScrollSpy(); } catch(err){ console.error('Error al iniciar el scrollspy:', err); }
    try{ initFirebase(); } catch(err){ console.error('Error al iniciar Firebase:', err); }
    try{ renderCartDrawer(); } catch(err){ console.error('Error al iniciar el carrito:', err); }
    try{ updateStickyOffsets(); } catch(err){ console.error('Error al calcular offsets:', err); }

    const fechaInput = document.getElementById('fechaEntrega');
    if(fechaInput){ fechaInput.min = new Date().toISOString().split('T')[0]; }

    let resizeTimer = null;
    window.addEventListener('resize', ()=>{
      clearTimeout(resizeTimer);
      resizeTimer = setTimeout(updateStickyOffsets, 150);
    });

    const note = document.getElementById('authDisabledNote');
    if(note){
      setTimeout(()=>{ if(!firebaseReady) note.classList.add('show'); }, 0);
    }
    updateAccountUI();
  });
</script>

</body>
</html>
