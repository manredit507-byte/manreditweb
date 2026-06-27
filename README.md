<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="ManRed-iT — Soporte técnico, mantenimiento preventivo y redes en Panamá y Colón. Menos problemas técnicos, más resultados.">
<meta name="keywords" content="soporte tecnico panama, mantenimiento computadoras colon, redes LAN wifi panama, IT support panama">
<title>ManRed-iT | Soporte IT · Panamá · Colón</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Space+Grotesk:wght@500;700&display=swap" rel="stylesheet">
<style>
/* ── RESET & BASE ─────────────────────────────────────────── */
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth;font-size:16px}
body{font-family:'Inter',sans-serif;color:#1a2332;background:#fff;line-height:1.6;overflow-x:hidden}
img{max-width:100%;display:block}
a{text-decoration:none;color:inherit}
button{cursor:pointer;font-family:inherit;border:none}
ul{list-style:none}

/* ── TOKENS ───────────────────────────────────────────────── */
:root{
  --navy:   #102B4C;
  --cyan:   #009BE2;
  --gray:   #4A4A4A;
  --white:  #FFFFFF;
  --light:  #F0F6FC;
  --border: #DDE6EF;
  --text:   #1a2332;
  --muted:  #5a6d80;
  --radius: 10px;
  --shadow: 0 2px 16px rgba(16,43,76,.08);
  --shadow-lg: 0 8px 40px rgba(16,43,76,.13);
}

/* ── UTILITIES ────────────────────────────────────────────── */
.container{max-width:1120px;margin:0 auto;padding:0 24px}
.section{padding:88px 0}
.section-label{font-size:11px;font-weight:600;letter-spacing:.1em;text-transform:uppercase;color:var(--cyan);margin-bottom:12px}
.section-title{font-family:'Space Grotesk',sans-serif;font-size:clamp(26px,4vw,40px);font-weight:700;color:var(--navy);line-height:1.18;margin-bottom:16px}
.section-sub{font-size:16px;color:var(--muted);max-width:540px;line-height:1.7}
.btn{display:inline-flex;align-items:center;gap:8px;padding:13px 26px;border-radius:var(--radius);font-size:15px;font-weight:600;transition:all .2s}
.btn-primary{background:var(--navy);color:#fff}
.btn-primary:hover{background:#0a1f38;transform:translateY(-1px);box-shadow:var(--shadow)}
.btn-outline{border:1.5px solid var(--navy);color:var(--navy)}
.btn-outline:hover{background:var(--navy);color:#fff}
.btn-cyan{background:var(--cyan);color:#fff}
.btn-cyan:hover{background:#007bbf;transform:translateY(-1px)}
.tag{display:inline-block;padding:4px 12px;border-radius:20px;font-size:12px;font-weight:500;background:var(--light);color:var(--navy)}
.card{background:#fff;border:1px solid var(--border);border-radius:14px;padding:28px;box-shadow:var(--shadow)}
.grid-2{display:grid;grid-template-columns:1fr 1fr;gap:28px}
.grid-3{display:grid;grid-template-columns:repeat(3,1fr);gap:24px}
.fade-in{opacity:0;transform:translateY(24px);transition:opacity .55s ease,transform .55s ease}
.fade-in.visible{opacity:1;transform:translateY(0)}

/* ── HEADER / NAV ─────────────────────────────────────────── */
#header{position:sticky;top:0;z-index:100;background:rgba(255,255,255,.96);backdrop-filter:blur(8px);border-bottom:1px solid var(--border);transition:box-shadow .2s}
#header.scrolled{box-shadow:var(--shadow)}
.nav-inner{display:flex;align-items:center;justify-content:space-between;height:68px}
.logo{display:flex;align-items:center;gap:10px}
.logo-hex{width:36px;height:36px}
.logo-text{font-family:'Space Grotesk',sans-serif;font-size:20px;font-weight:700;letter-spacing:-.01em}
.logo-text span.m{color:var(--navy)}
.logo-text span.r{color:var(--cyan)}
.logo-text span.i{color:var(--gray)}
.nav-links{display:flex;align-items:center;gap:32px}
.nav-links a{font-size:14px;font-weight:500;color:var(--muted);transition:color .15s}
.nav-links a:hover,.nav-links a.active{color:var(--navy)}
.nav-cta{display:flex;align-items:center;gap:12px}
.burger{display:none;flex-direction:column;gap:5px;background:none;padding:4px}
.burger span{width:22px;height:2px;background:var(--navy);border-radius:2px;transition:all .3s}
.mobile-menu{display:none;position:fixed;inset:0;background:#fff;z-index:200;flex-direction:column;padding:24px;gap:24px}
.mobile-menu.open{display:flex}
.mobile-close{align-self:flex-end;font-size:28px;background:none;color:var(--navy)}
.mobile-links{display:flex;flex-direction:column;gap:20px;margin-top:16px}
.mobile-links a{font-size:20px;font-weight:600;color:var(--navy)}

/* ── HERO ─────────────────────────────────────────────────── */
#hero{min-height:calc(100vh - 68px);display:flex;align-items:center;background:linear-gradient(135deg,#f0f6fc 0%,#e8f2fa 60%,#dff0fb 100%);position:relative;overflow:hidden}
.hero-bg-hex{position:absolute;right:-120px;top:50%;transform:translateY(-50%);opacity:.06;width:600px;height:600px}
.hero-inner{display:grid;grid-template-columns:1fr 1fr;gap:60px;align-items:center}
.hero-eyebrow{display:inline-flex;align-items:center;gap:8px;background:#fff;border:1px solid var(--border);border-radius:20px;padding:6px 14px;font-size:13px;font-weight:500;color:var(--navy);margin-bottom:24px}
.hero-eyebrow::before{content:'';width:8px;height:8px;border-radius:50%;background:var(--cyan);display:block}
.hero-title{font-family:'Space Grotesk',sans-serif;font-size:clamp(34px,5vw,58px);font-weight:700;color:var(--navy);line-height:1.08;margin-bottom:20px}
.hero-title em{font-style:normal;color:var(--cyan)}
.hero-sub{font-size:17px;color:var(--muted);line-height:1.7;margin-bottom:32px;max-width:480px}
.hero-btns{display:flex;gap:12px;flex-wrap:wrap}
.hero-visual{position:relative}
.hero-card-stack{display:flex;flex-direction:column;gap:14px}
.hcard{background:#fff;border-radius:14px;padding:20px 24px;box-shadow:var(--shadow-lg);border:1px solid var(--border);display:flex;align-items:center;gap:16px}
.hcard-icon{width:44px;height:44px;border-radius:10px;display:flex;align-items:center;justify-content:center;flex-shrink:0}
.hcard-icon.blue{background:#dbeeff}
.hcard-icon.cyan{background:#d6f1ff}
.hcard-icon.navy{background:#e6eef7}
.hcard-icon svg{width:22px;height:22px}
.hcard-title{font-weight:600;font-size:14px;color:var(--navy)}
.hcard-sub{font-size:12px;color:var(--muted);margin-top:2px}
.hero-badge{position:absolute;bottom:-16px;right:-16px;background:var(--navy);color:#fff;border-radius:12px;padding:14px 18px;font-size:13px;font-weight:600;box-shadow:var(--shadow-lg)}
.hero-badge span{display:block;font-size:22px;font-weight:700;color:var(--cyan)}

/* ── SERVICIOS ────────────────────────────────────────────── */
#servicios{background:#fff}
.services-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:20px;margin-top:48px}
.srv-card{background:#fff;border:1.5px solid var(--border);border-radius:14px;padding:28px;transition:all .25s;position:relative;overflow:hidden}
.srv-card::before{content:'';position:absolute;top:0;left:0;right:0;height:3px;background:var(--cyan);transform:scaleX(0);transition:transform .25s;transform-origin:left}
.srv-card:hover{box-shadow:var(--shadow-lg);transform:translateY(-4px);border-color:var(--cyan)}
.srv-card:hover::before{transform:scaleX(1)}
.srv-icon{width:48px;height:48px;border-radius:10px;background:var(--light);display:flex;align-items:center;justify-content:center;margin-bottom:16px}
.srv-icon svg{width:24px;height:24px;stroke:var(--navy)}
.srv-title{font-family:'Space Grotesk',sans-serif;font-size:17px;font-weight:700;color:var(--navy);margin-bottom:8px}
.srv-desc{font-size:14px;color:var(--muted);line-height:1.6}
.srv-tags{display:flex;flex-wrap:wrap;gap:6px;margin-top:14px}
.srv-tag{font-size:11px;padding:3px 10px;border-radius:20px;background:var(--light);color:var(--navy);font-weight:500}

/* ── PLANES ───────────────────────────────────────────────── */
#planes{background:var(--light)}
.planes-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:20px;margin-top:48px}
.plan-card{background:#fff;border:1.5px solid var(--border);border-radius:16px;padding:32px;transition:all .25s;position:relative}
.plan-card.featured{border-color:var(--cyan);box-shadow:0 0 0 4px rgba(0,155,226,.10)}
.plan-badge{position:absolute;top:-12px;left:50%;transform:translateX(-50%);background:var(--cyan);color:#fff;font-size:11px;font-weight:700;padding:4px 14px;border-radius:20px;letter-spacing:.05em;text-transform:uppercase}
.plan-name{font-family:'Space Grotesk',sans-serif;font-size:20px;font-weight:700;color:var(--navy);margin-bottom:6px}
.plan-desc{font-size:13px;color:var(--muted);margin-bottom:24px}
.plan-cta{display:block;text-align:center;padding:13px;border-radius:var(--radius);font-weight:600;font-size:14px;margin-top:24px;transition:all .2s}
.plan-cta.primary{background:var(--cyan);color:#fff}
.plan-cta.primary:hover{background:#007bbf}
.plan-cta.outline{border:1.5px solid var(--navy);color:var(--navy)}
.plan-cta.outline:hover{background:var(--navy);color:#fff}
.plan-feature{display:flex;align-items:flex-start;gap:10px;margin-bottom:12px;font-size:14px;color:var(--text)}
.plan-check{width:18px;height:18px;border-radius:50%;background:#d6f1ff;display:flex;align-items:center;justify-content:center;flex-shrink:0;margin-top:1px}
.plan-check svg{width:10px;height:10px;stroke:var(--cyan);fill:none}

/* ── COTIZADOR ────────────────────────────────────────────── */
#cotizador{background:#fff}
.quiz-wrap{max-width:700px;margin:48px auto 0;background:var(--light);border-radius:18px;padding:40px;border:1px solid var(--border)}
.quiz-step{display:none}
.quiz-step.active{display:block}
.quiz-progress{height:4px;background:var(--border);border-radius:4px;margin-bottom:32px}
.quiz-progress-bar{height:100%;background:var(--cyan);border-radius:4px;transition:width .4s ease}
.quiz-q{font-family:'Space Grotesk',sans-serif;font-size:20px;font-weight:700;color:var(--navy);margin-bottom:20px}
.quiz-options{display:flex;flex-direction:column;gap:10px}
.quiz-opt{background:#fff;border:1.5px solid var(--border);border-radius:10px;padding:14px 18px;font-size:14px;font-weight:500;color:var(--navy);text-align:left;transition:all .2s}
.quiz-opt:hover,.quiz-opt.selected{border-color:var(--cyan);background:#f0faff}
.quiz-nav{display:flex;justify-content:space-between;margin-top:24px}
.quiz-result{display:none;text-align:center}
.quiz-result-name{font-family:'Space Grotesk',sans-serif;font-size:28px;font-weight:700;color:var(--navy);margin:16px 0 8px}
.quiz-result-desc{color:var(--muted);margin-bottom:24px}

/* ── BLOG/VLOG ────────────────────────────────────────────── */
#blog{background:var(--light)}
.blog-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:24px;margin-top:48px}
.blog-card{background:#fff;border-radius:14px;overflow:hidden;border:1px solid var(--border);transition:all .25s}
.blog-card:hover{transform:translateY(-4px);box-shadow:var(--shadow-lg)}
.blog-thumb{height:180px;background:var(--light);display:flex;align-items:center;justify-content:center;position:relative;overflow:hidden}
.blog-thumb svg{width:48px;height:48px;stroke:var(--cyan)}
.blog-cat{position:absolute;top:12px;left:12px;background:var(--navy);color:#fff;font-size:11px;font-weight:600;padding:4px 10px;border-radius:20px}
.blog-body{padding:20px}
.blog-date{font-size:12px;color:var(--muted);margin-bottom:6px}
.blog-title{font-family:'Space Grotesk',sans-serif;font-size:16px;font-weight:700;color:var(--navy);margin-bottom:8px;line-height:1.3}
.blog-excerpt{font-size:13px;color:var(--muted);line-height:1.6}
.blog-link{display:inline-flex;align-items:center;gap:4px;margin-top:12px;font-size:13px;font-weight:600;color:var(--cyan)}

/* ── ANTES / DESPUÉS ──────────────────────────────────────── */
#antes-despues{background:#fff}
.compare-grid{display:grid;grid-template-columns:1fr 1fr;gap:20px;margin-top:48px}
.compare-card{border-radius:14px;overflow:hidden;border:1px solid var(--border)}
.compare-header{padding:14px 20px;font-weight:700;font-size:14px;display:flex;align-items:center;gap:8px}
.compare-header.before{background:#fce8e8;color:#9b1c1c}
.compare-header.after{background:#d6f1ff;color:var(--navy)}
.compare-body{padding:20px;background:#fff}
.compare-item{display:flex;align-items:center;gap:10px;margin-bottom:10px;font-size:14px;color:var(--text)}
.compare-icon{width:20px;height:20px;border-radius:50%;display:flex;align-items:center;justify-content:center;flex-shrink:0}
.compare-icon.bad{background:#fce8e8}
.compare-icon.good{background:#d6f1ff}
.compare-icon svg{width:11px;height:11px}

/* ── CLIENTES SATISFECHOS ─────────────────────────────────── */
#clientes{background:var(--light)}
.testimonial-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:20px;margin-top:48px}
.testimonial-card{background:#fff;border-radius:14px;padding:28px;border:1px solid var(--border);box-shadow:var(--shadow)}
.stars{color:var(--cyan);font-size:16px;margin-bottom:12px}
.testimonial-text{font-size:14px;color:var(--text);line-height:1.7;margin-bottom:20px;font-style:italic}
.testimonial-author{display:flex;align-items:center;gap:12px}
.author-avatar{width:40px;height:40px;border-radius:50%;background:var(--light);display:flex;align-items:center;justify-content:center;font-weight:700;font-size:15px;color:var(--navy);flex-shrink:0}
.author-name{font-weight:600;font-size:14px;color:var(--navy)}
.author-biz{font-size:12px;color:var(--muted)}

/* ── NOSOTROS ─────────────────────────────────────────────── */
#nosotros{background:#fff}
.about-inner{display:grid;grid-template-columns:1fr 1fr;gap:60px;align-items:center}
.about-visual{background:var(--light);border-radius:18px;height:420px;display:flex;align-items:center;justify-content:center;position:relative;overflow:hidden}
.about-hex-bg{position:absolute;opacity:.08}
.about-card-float{position:absolute;bottom:24px;left:24px;background:#fff;border-radius:12px;padding:16px 20px;box-shadow:var(--shadow-lg);border:1px solid var(--border)}
.about-values{display:grid;grid-template-columns:1fr 1fr;gap:16px;margin-top:32px}
.value-item{display:flex;align-items:flex-start;gap:10px}
.value-dot{width:8px;height:8px;border-radius:50%;background:var(--cyan);margin-top:6px;flex-shrink:0}
.value-text h4{font-weight:600;font-size:14px;color:var(--navy)}
.value-text p{font-size:13px;color:var(--muted);margin-top:2px}

/* ── GALERÍA ──────────────────────────────────────────────── */
#galeria{background:var(--light)}
.gallery-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:12px;margin-top:48px}
.gallery-item{border-radius:10px;background:var(--light);aspect-ratio:1;display:flex;align-items:center;justify-content:center;border:1px solid var(--border);overflow:hidden;position:relative;cursor:pointer;transition:all .25s}
.gallery-item:hover{transform:scale(1.03);box-shadow:var(--shadow-lg)}
.gallery-item svg{width:36px;height:36px;stroke:var(--muted)}
.gallery-item .gallery-label{position:absolute;bottom:0;left:0;right:0;background:rgba(16,43,76,.8);color:#fff;font-size:12px;font-weight:500;padding:8px 10px;transform:translateY(100%);transition:transform .25s}
.gallery-item:hover .gallery-label{transform:translateY(0)}
.gallery-add{background:#fff;border:1.5px dashed var(--cyan);cursor:pointer;flex-direction:column;gap:8px;font-size:13px;color:var(--cyan);font-weight:500}
.gallery-add svg{stroke:var(--cyan)}

/* ── FAQ ──────────────────────────────────────────────────── */
#faq{background:#fff}
.faq-list{max-width:760px;margin:48px auto 0}
.faq-item{border-bottom:1px solid var(--border)}
.faq-q{width:100%;text-align:left;background:none;padding:20px 0;display:flex;justify-content:space-between;align-items:center;font-size:16px;font-weight:600;color:var(--navy);gap:12px}
.faq-q svg{flex-shrink:0;transition:transform .25s;width:20px;height:20px;stroke:var(--cyan)}
.faq-q.open svg{transform:rotate(180deg)}
.faq-a{max-height:0;overflow:hidden;transition:max-height .3s ease,padding .3s}
.faq-a.open{max-height:300px;padding-bottom:20px}
.faq-a p{font-size:15px;color:var(--muted);line-height:1.7}

/* ── CONTACTO ─────────────────────────────────────────────── */
#contacto{background:var(--light)}
.contact-inner{display:grid;grid-template-columns:1fr 1fr;gap:48px;align-items:start}
.contact-info{display:flex;flex-direction:column;gap:20px}
.contact-item{display:flex;align-items:flex-start;gap:14px}
.contact-icon{width:44px;height:44px;border-radius:10px;background:#fff;border:1px solid var(--border);display:flex;align-items:center;justify-content:center;flex-shrink:0}
.contact-icon svg{width:20px;height:20px;stroke:var(--navy)}
.contact-label{font-size:12px;color:var(--muted);font-weight:500;margin-bottom:2px}
.contact-value{font-size:15px;font-weight:600;color:var(--navy)}
.contact-form{background:#fff;border-radius:16px;padding:36px;border:1px solid var(--border);box-shadow:var(--shadow)}
.form-group{margin-bottom:18px}
.form-group label{display:block;font-size:13px;font-weight:600;color:var(--navy);margin-bottom:6px}
.form-group input,.form-group select,.form-group textarea{width:100%;padding:12px 14px;border:1.5px solid var(--border);border-radius:var(--radius);font-size:14px;font-family:inherit;color:var(--text);transition:border-color .2s;background:#fff}
.form-group input:focus,.form-group select:focus,.form-group textarea:focus{outline:none;border-color:var(--cyan)}
.form-group textarea{height:120px;resize:vertical}
.form-submit{width:100%;padding:14px;background:var(--navy);color:#fff;border-radius:var(--radius);font-size:15px;font-weight:600;cursor:pointer;transition:all .2s}
.form-submit:hover{background:#0a1f38;transform:translateY(-1px)}
.form-success{display:none;text-align:center;padding:20px}
.map-placeholder{background:var(--light);border-radius:12px;height:220px;display:flex;align-items:center;justify-content:center;margin-top:24px;border:1px solid var(--border);font-size:14px;color:var(--muted);flex-direction:column;gap:8px}
.map-placeholder svg{width:32px;height:32px;stroke:var(--muted)}

/* ── FOOTER ───────────────────────────────────────────────── */
footer{background:var(--navy);color:#fff;padding:56px 0 28px}
.footer-inner{display:grid;grid-template-columns:2fr 1fr 1fr 1fr;gap:40px;margin-bottom:40px}
.footer-brand p{font-size:14px;color:rgba(255,255,255,.6);margin-top:12px;line-height:1.7}
.footer-col h4{font-family:'Space Grotesk',sans-serif;font-size:14px;font-weight:700;margin-bottom:16px;color:rgba(255,255,255,.9)}
.footer-col ul li{margin-bottom:10px}
.footer-col ul li a{font-size:14px;color:rgba(255,255,255,.55);transition:color .15s}
.footer-col ul li a:hover{color:#fff}
.footer-social{display:flex;gap:10px;margin-top:16px}
.footer-social a{width:36px;height:36px;border-radius:8px;border:1px solid rgba(255,255,255,.2);display:flex;align-items:center;justify-content:center;transition:all .15s}
.footer-social a:hover{border-color:var(--cyan);background:rgba(0,155,226,.15)}
.footer-social svg{width:16px;height:16px;stroke:#fff}
.footer-bottom{border-top:1px solid rgba(255,255,255,.1);padding-top:24px;display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:12px}
.footer-bottom p{font-size:13px;color:rgba(255,255,255,.4)}
.footer-legal{display:flex;gap:20px}
.footer-legal a{font-size:13px;color:rgba(255,255,255,.4);transition:color .15s}
.footer-legal a:hover{color:#fff}

/* ── LANG TOGGLE ─────────────────────────────────────────── */
.lang-toggle{display:flex;border:1.5px solid var(--border);border-radius:8px;overflow:hidden}
.lang-btn{padding:5px 12px;font-size:12px;font-weight:600;background:none;color:var(--muted);cursor:pointer;transition:all .15s}
.lang-btn.active{background:var(--navy);color:#fff}

/* ── RESPONSIVE ──────────────────────────────────────────── */
@media(max-width:900px){
.hero-inner,.about-inner,.contact-inner{grid-template-columns:1fr}
.services-grid,.planes-grid,.testimonial-grid,.blog-grid{grid-template-columns:1fr 1fr}
.footer-inner{grid-template-columns:1fr 1fr}
.gallery-grid{grid-template-columns:repeat(2,1fr)}
.hero-visual{display:none}
}
@media(max-width:600px){
.section{padding:56px 0}
.services-grid,.planes-grid,.testimonial-grid,.blog-grid,.compare-grid,.about-values{grid-template-columns:1fr}
.gallery-grid{grid-template-columns:repeat(2,1fr)}
.nav-links,.nav-cta .btn{display:none}
.burger{display:flex}
.footer-inner{grid-template-columns:1fr}
.hero-btns{flex-direction:column}
.grid-2{grid-template-columns:1fr}
}

/* ── LANGUAGE SWITCH ─────────────────────────────────────── */
[lang-es],[lang-en]{transition:opacity .2s}
body.lang-en [lang-es]{display:none}
body.lang-es [lang-en]{display:none}
body:not(.lang-en) [lang-en]{display:none}
body:not(.lang-es) [lang-en]{display:none}
</style>
</head>

<body class="lang-es">

<!-- ── MOBILE MENU ──────────────────────────────────────────────── -->
<div class="mobile-menu" id="mobileMenu">
<button class="mobile-close" onclick="closeMobile()">✕</button>
<nav class="mobile-links">
<a href="#servicios" onclick="closeMobile()">Servicios</a>
<a href="#planes" onclick="closeMobile()">Planes</a>
<a href="#blog" onclick="closeMobile()">Blog</a>
<a href="#clientes" onclick="closeMobile()">Clientes</a>
<a href="#nosotros" onclick="closeMobile()">Nosotros</a>
<a href="#faq" onclick="closeMobile()">FAQ</a>
<a href="#contacto" onclick="closeMobile()">Contacto</a>
</nav>
<a href="#contacto" class="btn btn-primary" onclick="closeMobile()" style="margin-top:16px">Solicitar diagnóstico gratis</a>
</div>

<!-- ── HEADER ───────────────────────────────────────────────────── -->
<header id="header">
<div class="container">
<nav class="nav-inner">
  <a href="#" class="logo">
    <svg class="logo-hex" viewBox="0 0 40 40" fill="none">
      <polygon points="20,2 36,11 36,29 20,38 4,29 4,11" fill="#102B4C"/>
      <polygon points="20,8 31,14.5 31,27.5 20,34 9,27.5 9,14.5" fill="none" stroke="#009BE2" stroke-width="1.5"/>
      <text x="20" y="23" text-anchor="middle" fill="#009BE2" font-size="8" font-family="Space Grotesk,sans-serif" font-weight="700">IT</text>
    </svg>
    <span class="logo-text"><span class="m">MAN</span>-<span class="r">RED</span>-<span class="i">IT</span></span>
  </a>

  <div class="nav-links">
    <a href="#servicios">Servicios</a>
    <a href="#planes">Planes</a>
    <a href="#blog">Blog</a>
    <a href="#clientes">Clientes</a>
    <a href="#nosotros">Nosotros</a>
    <a href="#faq">FAQ</a>
    <a href="#contacto">Contacto</a>
  </div>

  <div class="nav-cta">
    <div class="lang-toggle">
      <button class="lang-btn active" onclick="setLang('es')" id="btnEs">ES</button>
      <button class="lang-btn" onclick="setLang('en')" id="btnEn">EN</button>
    </div>
    <a href="#contacto" class="btn btn-primary" style="padding:9px 18px;font-size:13px">
      <lang-es>Diagnóstico gratis</lang-es><lang-en>Free diagnosis</lang-en>
    </a>
    <button class="burger" onclick="openMobile()" aria-label="Menú">
      <span></span><span></span><span></span>
    </button>
  </div>
</nav>
</div>
</header>

<!-- ── HERO ─────────────────────────────────────────────────────── -->
<section id="hero">
<svg class="hero-bg-hex" viewBox="0 0 600 600" fill="none">
<polygon points="300,20 540,155 540,445 300,580 60,445 60,155" fill="#102B4C"/>
</svg>
<div class="container">
<div class="hero-inner">
  <div class="fade-in">
    <div class="hero-eyebrow">
      <lang-es>Panamá · Colón · Soporte IT</lang-es>
      <lang-en>Panama · Colón · IT Support</lang-en>
    </div>
    <h1 class="hero-title">
      <lang-es>Menos problemas técnicos,<br><em>más resultados.</em></lang-es>
      <lang-en>Less tech problems,<br><em>more results.</em></lang-en>
    </h1>
    <p class="hero-sub">
      <lang-es>Soporte presencial y remoto para empresas y PYMES en Panamá. Mantenimiento, redes, impresoras y mucho más — con respuesta el mismo día.</lang-es>
      <lang-en>On-site and remote IT support for businesses in Panama. Maintenance, networks, printers and more — same-day response.</lang-en>
    </p>
    <div class="hero-btns">
      <a href="#cotizador" class="btn btn-primary">
        <svg width="16" height="16" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2"/></svg>
        <lang-es>Ver mi plan</lang-es><lang-en>Find my plan</lang-en>
      </a>
      <a href="#servicios" class="btn btn-outline">
        <lang-es>Ver servicios</lang-es><lang-en>See services</lang-en>
      </a>
    </div>
  </div>

  <div class="hero-visual fade-in">
    <div class="hero-card-stack">
      <div class="hcard">
        <div class="hcard-icon blue">
          <svg fill="none" stroke="#009BE2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.75 17L9 20l-1 1h8l-1-1-.75-3M3 13h18M5 17h14a2 2 0 002-2V5a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"/></svg>
        </div>
        <div>
          <div class="hcard-title"><lang-es>Mantenimiento preventivo</lang-es><lang-en>Preventive maintenance</lang-en></div>
          <div class="hcard-sub"><lang-es>Limpieza y diagnóstico completo</lang-es><lang-en>Full cleaning and diagnosis</lang-en></div>
        </div>
      </div>
      <div class="hcard">
        <div class="hcard-icon cyan">
          <svg fill="none" stroke="#009BE2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8.111 16.404a5.5 5.5 0 017.778 0M12 20h.01m-7.08-7.071c3.904-3.905 10.236-3.905 14.141 0M1.394 9.393c5.857-5.857 15.355-5.857 21.213 0"/></svg>
        </div>
        <div>
          <div class="hcard-title"><lang-es>Redes LAN / Wi-Fi</lang-es><lang-en>LAN / Wi-Fi Networks</lang-en></div>
          <div class="hcard-sub"><lang-es>Instalación y configuración</lang-es><lang-en>Installation and configuration</lang-en></div>
        </div>
      </div>
      <div class="hcard">
        <div class="hcard-icon navy">
          <svg fill="none" stroke="#102B4C" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 17h2a2 2 0 002-2v-4a2 2 0 00-2-2H5a2 2 0 00-2 2v4a2 2 0 002 2h2m2 4h6a2 2 0 002-2v-4a2 2 0 00-2-2H9a2 2 0 00-2 2v4a2 2 0 002 2zm8-12V5a2 2 0 00-2-2H9a2 2 0 00-2 2v4h10z"/></svg>
        </div>
        <div>
          <div class="hcard-title"><lang-es>Soporte de impresoras</lang-es><lang-en>Printer support</lang-en></div>
          <div class="hcard-sub"><lang-es>Diagnóstico y reparación</lang-es><lang-en>Diagnosis and repair</lang-en></div>
        </div>
      </div>
    </div>
    <div class="hero-badge">
      <span>+507</span>
      6784-9541
    </div>
  </div>
</div>
</div>
</section>

<!-- ── SERVICIOS ─────────────────────────────────────────────────── -->
<section id="servicios" class="section">
<div class="container">
  <div class="fade-in">
    <p class="section-label"><lang-es>Lo que hacemos</lang-es><lang-en>What we do</lang-en></p>
    <h2 class="section-title"><lang-es>Servicios IT para tu empresa</lang-es><lang-en>IT services for your business</lang-en></h2>
    <p class="section-sub"><lang-es>Atención presencial en Panamá y Colón. Respondemos el mismo día.</lang-es><lang-en>On-site service in Panama and Colón. Same-day response.</lang-en></p>
  </div>
  <div class="services-grid">
    <!-- Servicio 1 -->
    <div class="srv-card fade-in">
      <div class="srv-icon"><svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.75 17L9 20l-1 1h8l-1-1-.75-3M3 13h18M5 17h14a2 2 0 002-2V5a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"/></svg></div>
      <h3 class="srv-title"><lang-es>Mantenimiento preventivo</lang-es><lang-en>Preventive maintenance</lang-en></h3>
      <p class="srv-desc"><lang-es>Limpieza profunda, diagnóstico de componentes, actualización de drivers y optimización de rendimiento en laptops, desktops y servidores.</lang-es><lang-en>Deep cleaning, component diagnosis, driver updates and performance optimization for laptops, desktops and servers.</lang-en></p>
      <div class="srv-tags"><span class="srv-tag">Laptops</span><span class="srv-tag">Servidores</span><span class="srv-tag">Periféricos</span></div>
    </div>
    <!-- Servicio 2 -->
    <div class="srv-card fade-in">
      <div class="srv-icon"><svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8.111 16.404a5.5 5.5 0 017.778 0M12 20h.01m-7.08-7.071c3.904-3.905 10.236-3.905 14.141 0M1.394 9.393c5.857-5.857 15.355-5.857 21.213 0"/></svg></div>
      <h3 class="srv-title"><lang-es>Redes LAN / Wi-Fi</lang-es><lang-en>LAN / Wi-Fi Networks</lang-en></h3>
      <p class="srv-desc"><lang-es>Diseño e instalación de redes cableadas e inalámbricas. Configuración de routers MikroTik, switches y puntos de acceso.</lang-es><lang-en>Design and installation of wired and wireless networks. MikroTik router, switch and access point configuration.</lang-en></p>
      <div class="srv-tags"><span class="srv-tag">MikroTik</span><span class="srv-tag">LAN</span><span class="srv-tag">Cableado</span></div>
    </div>
    <!-- Servicio 3 -->
    <div class="srv-card fade-in">
      <div class="srv-icon"><svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 17h2a2 2 0 002-2v-4a2 2 0 00-2-2H5a2 2 0 00-2 2v4a2 2 0 002 2h2m2 4h6a2 2 0 002-2v-4a2 2 0 00-2-2H9a2 2 0 00-2 2v4a2 2 0 002 2zm8-12V5a2 2 0 00-2-2H9a2 2 0 00-2 2v4h10z"/></svg></div>
      <h3 class="srv-title"><lang-es>Impresoras y periféricos</lang-es><lang-en>Printers & peripherals</lang-en></h3>
      <p class="srv-desc"><lang-es>Diagnóstico, reparación y mantenimiento de impresoras Xerox y multifuncionales. Actualización de firmware y limpieza de componentes.</lang-es><lang-en>Diagnosis, repair and maintenance of Xerox and multifunction printers. Firmware updates and component cleaning.</lang-en></p>
      <div class="srv-tags"><span class="srv-tag">Xerox</span><span class="srv-tag">Firmware</span><span class="srv-tag">Drivers</span></div>
    </div>
    <!-- Servicio 4 -->
    <div class="srv-card fade-in">
      <div class="srv-icon"><svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 16v1a3 3 0 003 3h10a3 3 0 003-3v-1m-4-8l-4-4m0 0L8 8m4-4v12"/></svg></div>
      <h3 class="srv-title"><lang-es>Backup y OneDrive</lang-es><lang-en>Backup & OneDrive</lang-en></h3>
      <p class="srv-desc"><lang-es>Configuración de respaldos automáticos, migración a OneDrive y recuperación de datos. Solución para empresas sin sistema de backup.</lang-es><lang-en>Automatic backup setup, OneDrive migration and data recovery. Solution for businesses without a backup system.</lang-en></p>
      <div class="srv-tags"><span class="srv-tag">OneDrive</span><span class="srv-tag">Backup</span><span class="srv-tag">Recuperación</span></div>
    </div>
    <!-- Servicio 5 -->
    <div class="srv-card fade-in">
      <div class="srv-icon"><svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z"/></svg></div>
      <h3 class="srv-title"><lang-es>Software y licenciamientos</lang-es><lang-en>Software & licensing</lang-en></h3>
      <p class="srv-desc"><lang-es>Instalación de sistemas operativos, Office y software empresarial. Gestión de licencias para computadoras, escáneres y equipos.</lang-es><lang-en>OS installation, Office and business software. License management for computers, scanners and equipment.</lang-en></p>
      <div class="srv-tags"><span class="srv-tag">Windows</span><span class="srv-tag">Office</span><span class="srv-tag">Licencias</span></div>
    </div>
    <!-- Servicio 6 -->
    <div class="srv-card fade-in">
      <div class="srv-icon"><svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M18.364 5.636l-3.536 3.536m0 5.656l3.536 3.536M9.172 9.172L5.636 5.636m3.536 9.192l-3.536 3.536M21 12a9 9 0 11-18 0 9 9 0 0118 0zm-5 0a4 4 0 11-8 0 4 4 0 018 0z"/></svg></div>
      <h3 class="srv-title"><lang-es>Soporte presencial y remoto</lang-es><lang-en>On-site & remote support</lang-en></h3>
      <p class="srv-desc"><lang-es>Atendemos en tu oficina o de forma remota. Diagnóstico de logs, errores del sistema y resolución rápida de incidencias críticas.</lang-es><lang-en>We attend at your office or remotely. Log diagnosis, system errors and fast resolution of critical incidents.</lang-en></p>
      <div class="srv-tags"><span class="srv-tag">Presencial</span><span class="srv-tag">Remoto</span><span class="srv-tag">Mismo día</span></div>
    </div>
  </div>
</div>
</section>

<!-- ── PLANES ─────────────────────────────────────────────────────── -->
<section id="planes" class="section">
<div class="container">
  <div class="fade-in">
    <p class="section-label"><lang-es>Planes de servicio</lang-es><lang-en>Service plans</lang-en></p>
    <h2 class="section-title"><lang-es>Elige tu plan, sin contratos rígidos</lang-es><lang-en>Choose your plan, no rigid contracts</lang-en></h2>
    <p class="section-sub"><lang-es>Todos los planes incluyen diagnóstico inicial gratuito. Solicita cotización para tu empresa.</lang-es><lang-en>All plans include a free initial diagnosis. Request a quote for your business.</lang-en></p>
  </div>
  <div class="planes-grid">
    <!-- Plan Básico -->
    <div class="plan-card fade-in">
      <div class="plan-name"><lang-es>Básico</lang-es><lang-en>Basic</lang-en></div>
      <div class="plan-desc"><lang-es>Soporte esencial para oficinas pequeñas</lang-es><lang-en>Essential support for small offices</lang-en></div>
      <div class="plan-feature"><div class="plan-check"><svg viewBox="0 0 24 24" stroke-width="3"><polyline points="20 6 9 17 4 12"/></svg></div><lang-es>2 visitas programadas/mes</lang-es><lang-en>2 scheduled visits/month</lang-en></div>
      <div class="plan-feature"><div class="plan-check"><svg viewBox="0 0 24 24" stroke-width="3"><polyline points="20 6 9 17 4 12"/></svg></div><lang-es>Bolsa de 4 horas adicionales</lang-es><lang-en>4-hour additional pool</lang-en></div>
      <div class="plan-feature"><div class="plan-check"><svg viewBox="0 0 24 24" stroke-width="3"><polyline points="20 6 9 17 4 12"/></svg></div><lang-es>Respuesta en 8 horas hábiles</lang-es><lang-en>8 business-hour response</lang-en></div>
      <div class="plan-feature"><div class="plan-check"><svg viewBox="0 0 24 24" stroke-width="3"><polyline points="20 6 9 17 4 12"/></svg></div><lang-es>Mantenimiento preventivo</lang-es><lang-en>Preventive maintenance</lang-en></div>
      <div class="plan-feature"><div class="plan-check"><svg viewBox="0 0 24 24" stroke-width="3"><polyline points="20 6 9 17 4 12"/></svg></div><lang-es>Soporte remoto incluido</lang-es><lang-en>Remote support included</lang-en></div>
      <a href="#contacto" class="plan-cta outline"><lang-es>Cotizar plan</lang-es><lang-en>Get quote</lang-en></a>
    </div>
    <!-- Plan Estándar -->
    <div class="plan-card featured fade-in">
      <div class="plan-badge"><lang-es>Más popular</lang-es><lang-en>Most popular</lang-en></div>
      <div class="plan-name"><lang-es>Estándar</lang-es><lang-en>Standard</lang-en></div>
      <div class="plan-desc"><lang-es>Para empresas que no pueden parar</lang-es><lang-en>For businesses that can't stop</lang-en></div>
      <div class="plan-feature"><div class="plan-check"><svg viewBox="0 0 24 24" stroke-width="3"><polyline points="20 6 9 17 4 12"/></svg></div><lang-es>2 visitas programadas/mes</lang-es><lang-en>2 scheduled visits/month</lang-en></div>
      <div class="plan-feature"><div class="plan-check"><svg viewBox="0 0 24 24" stroke-width="3"><polyline points="20 6 9 17 4 12"/></svg></div><lang-es>Bolsa de 8 horas adicionales</lang-es><lang-en>8-hour additional pool</lang-en></div>
      <div class="plan-feature"><div class="plan-check"><svg viewBox="0 0 24 24" stroke-width="3"><polyline points="20 6 9 17 4 12"/></svg></div><lang-es>Respuesta rápida en 4 horas</lang-es><lang-en>Fast 4-hour response</lang-en></div>
      <div class="plan-feature"><div class="plan-check"><svg viewBox="0 0 24 24" stroke-width="3"><polyline points="20 6 9 17 4 12"/></svg></div><lang-es>Mantenimiento + redes</lang-es><lang-en>Maintenance + networks</lang-en></div>
      <div class="plan-feature"><div class="plan-check"><svg viewBox="0 0 24 24" stroke-width="3"><polyline points="20 6 9 17 4 12"/></svg></div><lang-es>Informe mensual de estado</lang-es><lang-en>Monthly status report</lang-en></div>
      <a href="#contacto" class="plan-cta primary"><lang-es>Cotizar plan</lang-es><lang-en>Get quote</lang-en></a>
    </div>
    <!-- Plan Completo -->
    <div class="plan-card fade-in">
      <div class="plan-name"><lang-es>Completo</lang-es><lang-en>Complete</lang-en></div>
      <div class="plan-desc"><lang-es>Máxima prioridad y cobertura total</lang-es><lang-en>Maximum priority and full coverage</lang-en></div>
      <div class="plan-feature"><div class="plan-check"><svg viewBox="0 0 24 24" stroke-width="3"><polyline points="20 6 9 17 4 12"/></svg></div><lang-es>2 visitas programadas/mes</lang-es><lang-en>2 scheduled visits/month</lang-en></div>
      <div class="plan-feature"><div class="plan-check"><svg viewBox="0 0 24 24" stroke-width="3"><polyline points="20 6 9 17 4 12"/></svg></div><lang-es>Bolsa de 16 horas adicionales</lang-es><lang-en>16-hour additional pool</lang-en></div>
      <div class="plan-feature"><div class="plan-check"><svg viewBox="0 0 24 24" stroke-width="3"><polyline points="20 6 9 17 4 12"/></svg></div><lang-es>Respuesta crítica en 2 horas</lang-es><lang-en>Critical 2-hour response</lang-en></div>
      <div class="plan-feature"><div class="plan-check"><svg viewBox="0 0 24 24" stroke-width="3"><polyline points="20 6 9 17 4 12"/></svg></div><lang-es>Cobertura completa IT</lang-es><lang-en>Full IT coverage</lang-en></div>
      <div class="plan-feature"><div class="plan-check"><svg viewBox="0 0 24 24" stroke-width="3"><polyline points="20 6 9 17 4 12"/></svg></div><lang-es>Prioridad máxima 24/7</lang-es><lang-en>Max priority 24/7</lang-en></div>
      <a href="#contacto" class="plan-cta outline"><lang-es>Cotizar plan</lang-es><lang-en>Get quote</lang-en></a>
    </div>
  </div>
</div>
</section>

<!-- ── COTIZADOR ──────────────────────────────────────────────────── -->
<section id="cotizador" class="section">
<div class="container">
  <div class="fade-in" style="text-align:center">
    <p class="section-label"><lang-es>Encuentra tu plan</lang-es><lang-en>Find your plan</lang-en></p>
    <h2 class="section-title" style="margin:0 auto"><lang-es>¿Cuál plan es para ti?</lang-es><lang-en>Which plan is for you?</lang-en></h2>
    <p class="section-sub" style="margin:12px auto 0"><lang-es>Responde 3 preguntas y te recomendamos el plan ideal.</lang-es><lang-en>Answer 3 questions and we'll recommend the ideal plan.</lang-en></p>
  </div>
  <div class="quiz-wrap fade-in">
    <div class="quiz-progress"><div class="quiz-progress-bar" id="qbar" style="width:0%"></div></div>

    <div class="quiz-step active" id="q1">
      <p class="quiz-q"><lang-es>¿Cuántas computadoras tiene tu empresa?</lang-es><lang-en>How many computers does your company have?</lang-en></p>
      <div class="quiz-options">
        <button class="quiz-opt" onclick="pickQ(1,'basic','1-5',this)"><lang-es>1 a 5 equipos</lang-es><lang-en>1 to 5 computers</lang-en></button>
        <button class="quiz-opt" onclick="pickQ(1,'estandar','6-15',this)"><lang-es>6 a 15 equipos</lang-es><lang-en>6 to 15 computers</lang-en></button>
        <button class="quiz-opt" onclick="pickQ(1,'completo','15+',this)"><lang-es>Más de 15 equipos</lang-es><lang-en>More than 15 computers</lang-en></button>
      </div>
    </div>

    <div class="quiz-step" id="q2">
      <p class="quiz-q"><lang-es>¿Con qué frecuencia tienen problemas técnicos?</lang-es><lang-en>How often do you have tech problems?</lang-en></p>
      <div class="quiz-options">
        <button class="quiz-opt" onclick="pickQ(2,'basic','raro',this)"><lang-es>Rara vez (menos de 1 vez al mes)</lang-es><lang-en>Rarely (less than once a month)</lang-en></button>
        <button class="quiz-opt" onclick="pickQ(2,'estandar','mensual',this)"><lang-es>Mensualmente</lang-es><lang-en>Monthly</lang-en></button>
        <button class="quiz-opt" onclick="pickQ(2,'completo','frecuente',this)"><lang-es>Con frecuencia (varias veces al mes)</lang-es><lang-en>Frequently (several times a month)</lang-en></button>
      </div>
    </div>

    <div class="quiz-step" id="q3">
      <p class="quiz-q"><lang-es>¿Qué tan crítica es la tecnología para tu operación?</lang-es><lang-en>How critical is technology to your operation?</lang-en></p>
      <div class="quiz-options">
        <button class="quiz-opt" onclick="showResult('basic',this)"><lang-es>Moderada — podemos esperar unas horas</lang-es><lang-en>Moderate — we can wait a few hours</lang-en></button>
        <button class="quiz-opt" onclick="showResult('estandar',this)"><lang-es>Alta — necesitamos respuesta ese mismo día</lang-es><lang-en>High — we need same-day response</lang-en></button>
        <button class="quiz-opt" onclick="showResult('completo',this)"><lang-es>Crítica — no podemos parar en ningún momento</lang-es><lang-en>Critical — we can't stop at any time</lang-en></button>
      </div>
    </div>

    <div class="quiz-result" id="qresult">
      <svg width="56" height="56" fill="none" stroke="#009BE2" viewBox="0 0 24 24" style="margin:0 auto"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
      <div class="quiz-result-name" id="resultName"></div>
      <div class="quiz-result-desc" id="resultDesc"></div>
      <div style="display:flex;gap:12px;justify-content:center;flex-wrap:wrap">
        <a href="#contacto" class="btn btn-primary"><lang-es>Cotizar este plan</lang-es><lang-en>Quote this plan</lang-en></a>
        <button class="btn btn-outline" onclick="resetQuiz()"><lang-es>Volver a responder</lang-es><lang-en>Answer again</lang-en></button>
      </div>
    </div>
  </div>
</div>
</section>

<!-- ── BLOG / VLOG ─────────────────────────────────────────────────── -->
<section id="blog" class="section">
<div class="container">
  <div style="display:flex;align-items:flex-end;justify-content:space-between;flex-wrap:wrap;gap:16px" class="fade-in">
    <div>
      <p class="section-label">Blog &amp; Vlog</p>
      <h2 class="section-title"><lang-es>Contenido que te ayuda</lang-es><lang-en>Content that helps you</lang-en></h2>
      <p class="section-sub"><lang-es>Tips reales, casos de servicio y novedades tecnológicas.</lang-es><lang-en>Real tips, service cases and tech news.</lang-en></p>
    </div>
    <a href="#blog" class="btn btn-outline" style="flex-shrink:0"><lang-es>Ver todos →</lang-es><lang-en>See all →</lang-en></a>
  </div>
  <div class="blog-grid">
    <div class="blog-card fade-in">
      <div class="blog-thumb">
        <svg fill="none" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M9.75 17L9 20l-1 1h8l-1-1-.75-3M3 13h18M5 17h14a2 2 0 002-2V5a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"/></svg>
        <span class="blog-cat"><lang-es>Mantenimiento</lang-es><lang-en>Maintenance</lang-en></span>
      </div>
      <div class="blog-body">
        <div class="blog-date">Junio 2025</div>
        <div class="blog-title"><lang-es>3 señales de que tu PC necesita mantenimiento urgente</lang-es><lang-en>3 signs your PC needs urgent maintenance</lang-en></div>
        <div class="blog-excerpt"><lang-es>Si tu computadora tarda más de 3 minutos en arrancar, se calienta sin motivo o muestra errores al abrir programas...</lang-es><lang-en>If your computer takes more than 3 minutes to boot, overheats for no reason or shows errors opening programs...</lang-en></div>
        <a class="blog-link" href="#">Leer más →</a>
      </div>
    </div>
    <div class="blog-card fade-in">
      <div class="blog-thumb">
        <svg fill="none" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M8.111 16.404a5.5 5.5 0 017.778 0M12 20h.01m-7.08-7.071c3.904-3.905 10.236-3.905 14.141 0M1.394 9.393c5.857-5.857 15.355-5.857 21.213 0"/></svg>
        <span class="blog-cat"><lang-es>Redes</lang-es><lang-en>Networks</lang-en></span>
      </div>
      <div class="blog-body">
        <div class="blog-date">Mayo 2025</div>
        <div class="blog-title"><lang-es>Cómo mejorar el Wi-Fi de tu oficina sin gastar de más</lang-es><lang-en>How to improve your office Wi-Fi without overspending</lang-en></div>
        <div class="blog-excerpt"><lang-es>La señal débil es uno de los problemas más comunes en oficinas panameñas. Aquí el paso a paso para diagnosticarlo...</lang-es><lang-en>Weak signal is one of the most common problems in Panamanian offices. Here's how to diagnose it...</lang-en></div>
        <a class="blog-link" href="#">Leer más →</a>
      </div>
    </div>
    <div class="blog-card fade-in">
      <div class="blog-thumb">
        <svg fill="none" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M4 16v1a3 3 0 003 3h10a3 3 0 003-3v-1m-4-8l-4-4m0 0L8 8m4-4v12"/></svg>
        <span class="blog-cat"><lang-es>Tips reales</lang-es><lang-en>Real tips</lang-en></span>
      </div>
      <div class="blog-body">
        <div class="blog-date">Abril 2025</div>
        <div class="blog-title"><lang-es>Backup automático paso a paso: nunca más pierdas información</lang-es><lang-en>Automatic backup step by step: never lose data again</lang-en></div>
        <div class="blog-excerpt"><lang-es>El 60% de las empresas que pierden datos críticos cierran en 6 meses. Configura tu respaldo en 15 minutos...</lang-es><lang-en>60% of businesses that lose critical data close within 6 months. Set up your backup in 15 minutes...</lang-en></div>
        <a class="blog-link" href="#">Leer más →</a>
      </div>
    </div>
  </div>
</div>
</section>

<!-- ── ANTES / DESPUÉS ─────────────────────────────────────────────── -->
<section id="antes-despues" class="section">
<div class="container">
  <div class="fade-in" style="text-align:center">
    <p class="section-label"><lang-es>Resultados reales</lang-es><lang-en>Real results</lang-en></p>
    <h2 class="section-title" style="margin:0 auto"><lang-es>Antes y después de MAN-RED-IT</lang-es><lang-en>Before and after MAN-RED-IT</lang-en></h2>
  </div>
  <div class="compare-grid" style="margin-top:48px">
    <div class="compare-card fade-in">
      <div class="compare-header before">
        <svg width="16" height="16" fill="none" stroke="currentColor" viewBox="0 0 24 24"><circle cx="12" cy="12" r="10"/><line x1="15" y1="9" x2="9" y2="15"/><line x1="9" y1="9" x2="15" y2="15"/></svg>
        <lang-es>Sin MAN-RED-IT</lang-es><lang-en>Without MAN-RED-IT</lang-en>
      </div>
      <div class="compare-body">
        <div class="compare-item"><div class="compare-icon bad"><svg fill="none" stroke="#9b1c1c" viewBox="0 0 24 24"><line x1="18" y1="6" x2="6" y2="18"/><line x1="6" y1="6" x2="18" y2="18"/></svg></div><lang-es>PC tarda 5+ minutos en arrancar</lang-es><lang-en>PC takes 5+ minutes to boot</lang-en></div>
        <div class="compare-item"><div class="compare-icon bad"><svg fill="none" stroke="#9b1c1c" viewBox="0 0 24 24"><line x1="18" y1="6" x2="6" y2="18"/><line x1="6" y1="6" x2="18" y2="18"/></svg></div><lang-es>Impresora sin conectividad de red</lang-es><lang-en>Printer with no network connectivity</lang-en></div>
        <div class="compare-item"><div class="compare-icon bad"><svg fill="none" stroke="#9b1c1c" viewBox="0 0 24 24"><line x1="18" y1="6" x2="6" y2="18"/><line x1="6" y1="6" x2="18" y2="18"/></svg></div><lang-es>Datos sin respaldo desde meses</lang-es><lang-en>Data without backup for months</lang-en></div>
        <div class="compare-item"><div class="compare-icon bad"><svg fill="none" stroke="#9b1c1c" viewBox="0 0 24 24"><line x1="18" y1="6" x2="6" y2="18"/><line x1="6" y1="6" x2="18" y2="18"/></svg></div><lang-es>Wi-Fi lento en toda la oficina</lang-es><lang-en>Slow Wi-Fi throughout the office</lang-en></div>
        <div class="compare-item"><div class="compare-icon bad"><svg fill="none" stroke="#9b1c1c" viewBox="0 0 24 24"><line x1="18" y1="6" x2="6" y2="18"/><line x1="6" y1="6" x2="18" y2="18"/></svg></div><lang-es>Drivers desactualizados con errores</lang-es><lang-en>Outdated drivers causing errors</lang-en></div>
      </div>
    </div>
    <div class="compare-card fade-in">
      <div class="compare-header after">
        <svg width="16" height="16" fill="none" stroke="currentColor" viewBox="0 0 24 24"><circle cx="12" cy="12" r="10"/><polyline points="9 12 11 14 15 10"/></svg>
        <lang-es>Con MAN-RED-IT</lang-es><lang-en>With MAN-RED-IT</lang-en>
      </div>
      <div class="compare-body">
        <div class="compare-item"><div class="compare-icon good"><svg fill="none" stroke="#009BE2" viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg></div><lang-es>Arranque en menos de 1 minuto</lang-es><lang-en>Boot in under 1 minute</lang-en></div>
        <div class="compare-item"><div class="compare-icon good"><svg fill="none" stroke="#009BE2" viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg></div><lang-es>Impresora funcionando en red estable</lang-es><lang-en>Printer running on stable network</lang-en></div>
        <div class="compare-item"><div class="compare-icon good"><svg fill="none" stroke="#009BE2" viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg></div><lang-es>Backup automático configurado</lang-es><lang-en>Automatic backup configured</lang-en></div>
        <div class="compare-item"><div class="compare-icon good"><svg fill="none" stroke="#009BE2" viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg></div><lang-es>Wi-Fi óptimo en toda la oficina</lang-es><lang-en>Optimal Wi-Fi throughout the office</lang-en></div>
        <div class="compare-item"><div class="compare-icon good"><svg fill="none" stroke="#009BE2" viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg></div><lang-es>Sistema actualizado sin errores</lang-es><lang-en>Updated system without errors</lang-en></div>
      </div>
    </div>
  </div>
</div>
</section>

<!-- ── CLIENTES ────────────────────────────────────────────────────── -->
<section id="clientes" class="section">
<div class="container">
  <div class="fade-in">
    <p class="section-label"><lang-es>Lo que dicen</lang-es><lang-en>What they say</lang-en></p>
    <h2 class="section-title"><lang-es>Clientes satisfechos</lang-es><lang-en>Happy clients</lang-en></h2>
    <p class="section-sub"><lang-es>Empresas en Panamá y Colón que confían en MAN-RED-IT.</lang-es><lang-en>Businesses in Panama and Colón that trust MAN-RED-IT.</lang-en></p>
  </div>
  <div class="testimonial-grid">
    <div class="testimonial-card fade-in">
      <div class="stars">★★★★★</div>
      <p class="testimonial-text"><lang-es>"Resolvieron el problema de nuestra red en menos de 2 horas. El equipo de impresoras que llevaba semanas fallando quedó funcionando perfectamente."</lang-es><lang-en>"They solved our network problem in under 2 hours. The printers that had been failing for weeks are now working perfectly."</lang-en></p>
      <div class="testimonial-author"><div class="author-avatar">JG</div><div><div class="author-name">Grupo Jurídico</div><div class="author-biz"><lang-es>Bufete de abogados · Panamá</lang-es><lang-en>Law firm · Panama</lang-en></div></div></div>
    </div>
    <div class="testimonial-card fade-in">
      <div class="stars">★★★★★</div>
      <p class="testimonial-text"><lang-es>"Configuraron toda la red de nuestra oficina desde cero. Profesionales, puntuales y con precios justos. Los recomiendo sin dudarlo."</lang-es><lang-en>"They configured our entire office network from scratch. Professional, punctual and fair prices. I recommend them without hesitation."</lang-en></p>
      <div class="testimonial-author"><div class="author-avatar">MC</div><div><div class="author-name">MC Distribuidora</div><div class="author-biz"><lang-es>Distribución · Colón</lang-es><lang-en>Distribution · Colón</lang-en></div></div></div>
    </div>
    <div class="testimonial-card fade-in">
      <div class="stars">★★★★★</div>
      <p class="testimonial-text"><lang-es>"El mantenimiento preventivo que hacen cada mes nos ha ahorrado mucho dinero. Ya no tenemos sorpresas con los equipos."</lang-es><lang-en>"The monthly preventive maintenance has saved us a lot of money. No more equipment surprises."</lang-en></p>
      <div class="testimonial-author"><div class="author-avatar">PA</div><div><div class="author-name"><lang-es>Pymé Activa</lang-es><lang-en>Active SME</lang-en></div><div class="author-biz"><lang-es>Comercio · Panamá</lang-es><lang-en>Commerce · Panama</lang-en></div></div></div>
    </div>
  </div>
  <div style="text-align:center;margin-top:32px" class="fade-in">
    <p style="font-size:14px;color:var(--muted);font-style:italic"><lang-es>¿Eres cliente? <a href="#contacto" style="color:var(--cyan);font-weight:600">Comparte tu experiencia →</a></lang-es><lang-en>Are you a client? <a href="#contacto" style="color:var(--cyan);font-weight:600">Share your experience →</a></lang-en></p>
  </div>
</div>
</section>

<!-- ── NOSOTROS ────────────────────────────────────────────────────── -->
<section id="nosotros" class="section">
<div class="container">
  <div class="about-inner">
    <div class="fade-in">
      <p class="section-label"><lang-es>Quiénes somos</lang-es><lang-en>Who we are</lang-en></p>
      <h2 class="section-title"><lang-es>Tecnología que no para. Servicio que llega.</lang-es><lang-en>Technology that doesn't stop. Service that arrives.</lang-en></h2>
      <p style="font-size:15px;color:var(--muted);line-height:1.8;margin-bottom:28px"><lang-es>MAN-RED-IT es una empresa de soporte IT con base en Colón y Ciudad de Panamá. Brindamos soluciones tecnológicas reales a empresas y PYMES que no pueden darse el lujo de esperar cuando algo falla.</lang-es><lang-en>MAN-RED-IT is an IT support company based in Colón and Panama City. We provide real technology solutions to businesses and SMEs that can't afford to wait when something fails.</lang-en></p>
      <div class="about-values">
        <div class="value-item"><div class="value-dot"></div><div class="value-text"><h4><lang-es>Respuesta el mismo día</lang-es><lang-en>Same-day response</lang-en></h4><p><lang-es>No días de espera</lang-es><lang-en>No waiting days</lang-en></p></div></div>
        <div class="value-item"><div class="value-dot"></div><div class="value-text"><h4><lang-es>Sin contratos rígidos</lang-es><lang-en>No rigid contracts</lang-en></h4><p><lang-es>Pagas lo que usas</lang-es><lang-en>Pay what you use</lang-en></p></div></div>
        <div class="value-item"><div class="value-dot"></div><div class="value-text"><h4><lang-es>Diagnóstico gratuito</lang-es><lang-en>Free diagnosis</lang-en></h4><p><lang-es>Sin compromiso inicial</lang-es><lang-en>No upfront commitment</lang-en></p></div></div>
        <div class="value-item"><div class="value-dot"></div><div class="value-text"><h4><lang-es>Presencia local</lang-es><lang-en>Local presence</lang-en></h4><p><lang-es>Panamá y Colón</lang-es><lang-en>Panama and Colón</lang-en></p></div></div>
      </div>
    </div>
    <div class="fade-in">
      <div class="about-visual">
        <svg class="about-hex-bg" width="300" height="300" viewBox="0 0 300 300"><polygon points="150,10 270,80 270,220 150,290 30,220 30,80" fill="#102B4C"/></svg>
        <div style="text-align:center;z-index:1">
          <svg width="80" height="80" fill="none" viewBox="0 0 80 80">
            <polygon points="40,4 72,22 72,58 40,76 8,58 8,22" fill="#102B4C"/>
            <polygon points="40,14 64,28 64,52 40,66 16,52 16,28" fill="none" stroke="#009BE2" stroke-width="2"/>
            <text x="40" y="44" text-anchor="middle" fill="#009BE2" font-size="16" font-family="Space Grotesk,sans-serif" font-weight="700">IT</text>
          </svg>
          <p style="font-family:'Space Grotesk',sans-serif;font-weight:700;font-size:22px;color:#102B4C;margin-top:12px">MAN-RED-IT</p>
          <p style="font-size:13px;color:var(--muted);margin-top:4px">IT Solutions · Panamá</p>
        </div>
        <div class="about-card-float">
          <p style="font-size:11px;font-weight:600;color:var(--muted);margin-bottom:2px">Cobertura</p>
          <p style="font-size:14px;font-weight:700;color:var(--navy)">Panamá · Colón</p>
        </div>
      </div>
    </div>
  </div>
</div>
</section>

<!-- ── GALERÍA ─────────────────────────────────────────────────────── -->
<section id="galeria" class="section">
<div class="container">
  <div class="fade-in">
    <p class="section-label"><lang-es>Nuestro trabajo</lang-es><lang-en>Our work</lang-en></p>
    <h2 class="section-title"><lang-es>Galería de proyectos</lang-es><lang-en>Project gallery</lang-en></h2>
    <p class="section-sub"><lang-es>Instalaciones, mantenimientos y redes completadas.</lang-es><lang-en>Completed installations, maintenance and networks.</lang-en></p>
  </div>
  <div class="gallery-grid" style="margin-top:48px">
    <div class="gallery-item fade-in">
      <svg fill="none" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M8.111 16.404a5.5 5.5 0 017.778 0M12 20h.01m-7.08-7.071c3.904-3.905 10.236-3.905 14.141 0M1.394 9.393c5.857-5.857 15.355-5.857 21.213 0"/></svg>
      <span class="gallery-label"><lang-es>Instalación de red</lang-es><lang-en>Network installation</lang-en></span>
    </div>
    <div class="gallery-item fade-in">
      <svg fill="none" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M9.75 17L9 20l-1 1h8l-1-1-.75-3M3 13h18M5 17h14a2 2 0 002-2V5a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"/></svg>
      <span class="gallery-label"><lang-es>Mantenimiento PC</lang-es><lang-en>PC maintenance</lang-en></span>
    </div>
    <div class="gallery-item fade-in">
      <svg fill="none" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M17 17h2a2 2 0 002-2v-4a2 2 0 00-2-2H5a2 2 0 00-2 2v4a2 2 0 002 2h2m2 4h6a2 2 0 002-2v-4a2 2 0 00-2-2H9a2 2 0 00-2 2v4a2 2 0 002 2zm8-12V5a2 2 0 00-2-2H9a2 2 0 00-2 2v4h10z"/></svg>
      <span class="gallery-label"><lang-es>Impresora reparada</lang-es><lang-en>Printer repaired</lang-en></span>
    </div>
    <div class="gallery-item gallery-add fade-in" onclick="alert('Próximamente: sube fotos reales de tus trabajos.')">
      <svg fill="none" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M12 4v16m8-8H4"/></svg>
      <span><lang-es>Agregar foto</lang-es><lang-en>Add photo</lang-en></span>
    </div>
  </div>
  <p style="text-align:center;font-size:13px;color:var(--muted);margin-top:20px;font-style:italic"><lang-es>Sección activa — agrega fotos reales de tus trabajos para mayor impacto.</lang-es><lang-en>Active section — add real work photos for greater impact.</lang-en></p>
</div>
</section>

<!-- ── FAQ ────────────────────────────────────────────────────────── -->
<section id="faq" class="section">
<div class="container">
  <div class="fade-in" style="text-align:center">
    <p class="section-label">FAQ</p>
    <h2 class="section-title" style="margin:0 auto"><lang-es>Preguntas frecuentes</lang-es><lang-en>Frequently asked questions</lang-en></h2>
  </div>
  <div class="faq-list fade-in">
    <div class="faq-item">
      <button class="faq-q" onclick="toggleFaq(this)">
        <span><lang-es>¿Cuánto cuesta una revisión?</lang-es><lang-en>How much does a review cost?</lang-en></span>
        <svg fill="none" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"/></svg>
      </button>
      <div class="faq-a"><p><lang-es>El diagnóstico inicial es 100% gratuito y sin compromiso. El costo de la revisión completa depende del tipo de equipo y los servicios necesarios. Contáctanos para una cotización exacta para tu empresa.</lang-es><lang-en>The initial diagnosis is 100% free with no commitment. The full review cost depends on equipment type and services needed. Contact us for an exact quote for your business.</lang-en></p></div>
    </div>
    <div class="faq-item">
      <button class="faq-q" onclick="toggleFaq(this)">
        <span><lang-es>¿Atienden a domicilio?</lang-es><lang-en>Do you provide on-site service?</lang-en></span>
        <svg fill="none" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"/></svg>
      </button>
      <div class="faq-a"><p><lang-es>Sí. Atendemos directamente en tu oficina o empresa en Panamá y Colón. No necesitas trasladar tus equipos — nosotros vamos donde estás. También ofrecemos soporte remoto para problemas de software.</lang-es><lang-en>Yes. We attend directly at your office in Panama and Colón. You don't need to move your equipment — we come to you. We also offer remote support for software issues.</lang-en></p></div>
    </div>
    <div class="faq-item">
      <button class="faq-q" onclick="toggleFaq(this)">
        <span><lang-es>¿Cuánto tarda una reparación?</lang-es><lang-en>How long does a repair take?</lang-en></span>
        <svg fill="none" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"/></svg>
      </button>
      <div class="faq-a"><p><lang-es>La mayoría de los problemas se resuelven en la misma visita (1-2 horas). Para reparaciones más complejas que requieren piezas, el tiempo promedio es de 24-48 horas hábiles. Nunca te dejamos sin respuesta.</lang-es><lang-en>Most problems are resolved in the same visit (1-2 hours). For more complex repairs requiring parts, the average time is 24-48 business hours. We never leave you without an answer.</lang-en></p></div>
    </div>
    <div class="faq-item">
      <button class="faq-q" onclick="toggleFaq(this)">
        <span><lang-es>¿Trabajan con empresas o también con particulares?</lang-es><lang-en>Do you work with businesses or individuals too?</lang-en></span>
        <svg fill="none" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"/></svg>
      </button>
      <div class="faq-a"><p><lang-es>Principalmente atendemos a empresas, PYMES y corporaciones. Sin embargo, también ayudamos a profesionales independientes y personas con equipos de trabajo. Contáctanos y evaluamos tu caso.</lang-es><lang-en>We primarily serve businesses, SMEs and corporations. However, we also help independent professionals and individuals with work equipment. Contact us and we'll evaluate your case.</lang-en></p></div>
    </div>
    <div class="faq-item">
      <button class="faq-q" onclick="toggleFaq(this)">
        <span><lang-es>¿Tienen contratos obligatorios?</lang-es><lang-en>Do you have mandatory contracts?</lang-en></span>
        <svg fill="none" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"/></svg>
      </button>
      <div class="faq-a"><p><lang-es>No. Nuestros planes son flexibles — puedes elegir visitas programadas, bolsas de horas bajo demanda, o simplemente llamarnos cuando necesitas ayuda. Sin compromisos de permanencia.</lang-es><lang-en>No. Our plans are flexible — you can choose scheduled visits, on-demand hour pools, or simply call us when you need help. No commitment periods.</lang-en></p></div>
    </div>
  </div>
</div>
</section>

<!-- ── CONTACTO ────────────────────────────────────────────────────── -->
<section id="contacto" class="section">
<div class="container">
  <div class="fade-in">
    <p class="section-label"><lang-es>Hablemos</lang-es><lang-en>Let's talk</lang-en></p>
    <h2 class="section-title"><lang-es>Solicita tu diagnóstico gratuito</lang-es><lang-en>Request your free diagnosis</lang-en></h2>
    <p class="section-sub"><lang-es>Te respondemos por WhatsApp en menos de 1 hora hábil.</lang-es><lang-en>We reply via WhatsApp within 1 business hour.</lang-en></p>
  </div>
  <div class="contact-inner" style="margin-top:48px">
    <div>
      <div class="contact-info fade-in">
        <div class="contact-item">
          <div class="contact-icon"><svg fill="none" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"/></svg></div>
          <div><div class="contact-label">WhatsApp</div><div class="contact-value">+507 6784-9541</div></div>
        </div>
        <div class="contact-item">
          <div class="contact-icon"><svg fill="none" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"/></svg></div>
          <div><div class="contact-label">Email</div><div class="contact-value">ian@manred.it</div></div>
        </div>
        <div class="contact-item">
          <div class="contact-icon"><svg fill="none" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"/><circle cx="12" cy="11" r="3"/></svg></div>
          <div><div class="contact-label"><lang-es>Cobertura</lang-es><lang-en>Coverage</lang-en></div><div class="contact-value"><lang-es>Panamá · Colón</lang-es><lang-en>Panama · Colón</lang-en></div></div>
        </div>
      </div>
      <div class="map-placeholder fade-in" style="margin-top:28px">
        <svg fill="none" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M9 20l-5.447-2.724A1 1 0 013 16.382V5.618a1 1 0 011.447-.894L9 7m0 13l6-3m-6 3V7m6 10l4.553 2.276A1 1 0 0021 18.382V7.618a1 1 0 00-.553-.894L15 4m0 13V4m0 0L9 7"/></svg>
        <span><lang-es>Mapa de cobertura: Panamá y Colón</lang-es><lang-en>Coverage map: Panama and Colón</lang-en></span>
        <span style="font-size:12px"><lang-es>Agrega tu API key de Google Maps aquí</lang-es><lang-en>Add your Google Maps API key here</lang-en></span>
      </div>
    </div>

    <div class="contact-form fade-in">
      <form id="contactForm" onsubmit="submitForm(event)">
        <div class="form-group">
          <label><lang-es>Nombre y empresa</lang-es><lang-en>Name and company</lang-en></label>
          <input type="text" required placeholder="Ej: Juan García — Empresa XYZ">
        </div>
        <div class="form-group">
          <label>WhatsApp / Teléfono</label>
          <input type="tel" required placeholder="+507 6000-0000">
        </div>
        <div class="form-group">
          <label><lang-es>¿Qué necesitas?</lang-es><lang-en>What do you need?</lang-en></label>
          <select>
            <option value=""><lang-es>Selecciona un servicio</lang-es><lang-en>Select a service</lang-en></option>
            <option><lang-es>Mantenimiento preventivo</lang-es><lang-en>Preventive maintenance</lang-en></option>
            <option><lang-es>Redes LAN / Wi-Fi</lang-es><lang-en>LAN / Wi-Fi Networks</lang-en></option>
            <option><lang-es>Soporte de impresoras</lang-es><lang-en>Printer support</lang-en></option>
            <option><lang-es>Backup y almacenamiento</lang-es><lang-en>Backup and storage</lang-en></option>
            <option><lang-es>Software y licencias</lang-es><lang-en>Software and licenses</lang-en></option>
            <option><lang-es>Otro</lang-es><lang-en>Other</lang-en></option>
          </select>
        </div>
        <div class="form-group">
          <label><lang-es>Cuéntame más (opcional)</lang-es><lang-en>Tell me more (optional)</lang-en></label>
          <textarea placeholder="Ej: Tenemos 5 equipos, una impresora Xerox y la red está fallando..."></textarea>
        </div>
        <button type="submit" class="form-submit"><lang-es>Enviar y recibir diagnóstico gratis</lang-es><lang-en>Send and get free diagnosis</lang-en></button>
      </form>
      <div class="form-success" id="formSuccess">
        <svg width="48" height="48" fill="none" stroke="#009BE2" viewBox="0 0 24 24" style="margin:0 auto"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
        <h3 style="font-family:'Space Grotesk',sans-serif;font-size:20px;color:var(--navy);margin:12px 0 8px"><lang-es>¡Mensaje enviado!</lang-es><lang-en>Message sent!</lang-en></h3>
        <p style="font-size:14px;color:var(--muted)"><lang-es>Te escribimos por WhatsApp en menos de 1 hora hábil.</lang-es><lang-en>We'll message you on WhatsApp within 1 business hour.</lang-en></p>
        <a href="https://wa.me/50767849541" target="_blank" class="btn btn-cyan" style="margin-top:16px">WhatsApp directo →</a>
      </div>
    </div>
  </div>
</div>
</section>

<!-- ── FOOTER ─────────────────────────────────────────────────────── -->
<footer>
<div class="container">
  <div class="footer-inner">
    <div class="footer-brand">
      <div style="display:flex;align-items:center;gap:10px;margin-bottom:8px">
        <svg width="32" height="32" viewBox="0 0 40 40" fill="none"><polygon points="20,2 36,11 36,29 20,38 4,29 4,11" fill="#102B4C"/><polygon points="20,8 31,14.5 31,27.5 20,34 9,27.5 9,14.5" fill="none" stroke="#009BE2" stroke-width="1.5"/><text x="20" y="23" text-anchor="middle" fill="#009BE2" font-size="8" font-family="Space Grotesk,sans-serif" font-weight="700">IT</text></svg>
        <span style="font-family:'Space Grotesk',sans-serif;font-size:18px;font-weight:700;color:#fff">MAN-RED-IT</span>
      </div>
      <p><lang-es>Menos problemas técnicos, más resultados.</lang-es><lang-en>Less tech problems, more results.</lang-en><br><lang-es>Soporte IT en Panamá y Colón.</lang-es><lang-en>IT support in Panama and Colón.</lang-en></p>
      <div class="footer-social">
        <a href="#" aria-label="Instagram"><svg viewBox="0 0 24 24"><rect x="2" y="2" width="20" height="20" rx="5" ry="5"/><path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"/><line x1="17.5" y1="6.5" x2="17.51" y2="6.5"/></svg></a>
        <a href="https://wa.me/50767849541" aria-label="WhatsApp"><svg viewBox="0 0 24 24"><path d="M21 11.5a8.38 8.38 0 0 1-.9 3.8 8.5 8.5 0 0 1-7.6 4.7 8.38 8.38 0 0 1-3.8-.9L3 21l1.9-5.7a8.38 8.38 0 0 1-.9-3.8 8.5 8.5 0 0 1 4.7-7.6 8.38 8.38 0 0 1 3.8-.9h.5a8.48 8.48 0 0 1 8 8v.5z"/></svg></a>
      </div>
    </div>
    <div class="footer-col">
      <h4><lang-es>Servicios</lang-es><lang-en>Services</lang-en></h4>
      <ul>
        <li><a href="#servicios"><lang-es>Mantenimiento</lang-es><lang-en>Maintenance</lang-en></a></li>
        <li><a href="#servicios"><lang-es>Redes LAN/Wi-Fi</lang-es><lang-en>LAN/Wi-Fi Networks</lang-en></a></li>
        <li><a href="#servicios"><lang-es>Impresoras</lang-es><lang-en>Printers</lang-en></a></li>
        <li><a href="#servicios">Backup / OneDrive</a></li>
        <li><a href="#servicios">Software</a></li>
      </ul>
    </div>
    <div class="footer-col">
      <h4><lang-es>Empresa</lang-es><lang-en>Company</lang-en></h4>
      <ul>
        <li><a href="#nosotros"><lang-es>Nosotros</lang-es><lang-en>About us</lang-en></a></li>
        <li><a href="#planes"><lang-es>Planes</lang-es><lang-en>Plans</lang-en></a></li>
        <li><a href="#blog">Blog</a></li>
        <li><a href="#clientes"><lang-es>Clientes</lang-es><lang-en>Clients</lang-en></a></li>
        <li><a href="#faq">FAQ</a></li>
      </ul>
    </div>
    <div class="footer-col">
      <h4><lang-es>Contacto</lang-es><lang-en>Contact</lang-en></h4>
      <ul>
        <li><a href="https://wa.me/50767849541">+507 6784-9541</a></li>
        <li><a href="mailto:ian@manred.it">ian@manred.it</a></li>
        <li><a href="#contacto"><lang-es>Diagnóstico gratis</lang-es><lang-en>Free diagnosis</lang-en></a></li>
      </ul>
    </div>
  </div>
  <div class="footer-bottom">
    <p>© 2025 MAN-RED-IT · IT Solutions Panama</p>
    <div class="footer-legal">
      <a href="#"><lang-es>Política de privacidad</lang-es><lang-en>Privacy policy</lang-en></a>
      <a href="#"><lang-es>Términos de uso</lang-es><lang-en>Terms of use</lang-en></a>
    </div>
  </div>
</div>
</footer>

<script>
// ── LANG SWITCH ────────────────────────────────────────────────
function setLang(l){
  document.body.className=document.body.className.replace(/lang-\w+/g,'')+" lang-"+l;
  document.getElementById('btnEs').className='lang-btn'+(l==='es'?' active':'');
  document.getElementById('btnEn').className='lang-btn'+(l==='en'?' active':'');
  // toggle all lang elements
  document.querySelectorAll('lang-es,lang-en').forEach(el=>{
    el.style.display=(el.tagName.toLowerCase()==='lang-'+l)?'':'none';
  });
}
// init display
setLang('es');

// ── SCROLL HEADER ──────────────────────────────────────────────
window.addEventListener('scroll',()=>{
  document.getElementById('header').classList.toggle('scrolled',scrollY>20);
});

// ── FADE IN ON SCROLL ──────────────────────────────────────────
const obs=new IntersectionObserver(entries=>{
  entries.forEach(e=>{if(e.isIntersecting)e.target.classList.add('visible')});
},{threshold:.12});
document.querySelectorAll('.fade-in').forEach(el=>obs.observe(el));

// ── MOBILE MENU ────────────────────────────────────────────────
function openMobile(){document.getElementById('mobileMenu').classList.add('open')}
function closeMobile(){document.getElementById('mobileMenu').classList.remove('open')}

// ── FAQ ────────────────────────────────────────────────────────
function toggleFaq(btn){
  const a=btn.nextElementSibling;
  const isOpen=a.classList.contains('open');
  document.querySelectorAll('.faq-a').forEach(x=>x.classList.remove('open'));
  document.querySelectorAll('.faq-q').forEach(x=>x.classList.remove('open'));
  if(!isOpen){a.classList.add('open');btn.classList.add('open');}
}

// ── QUIZ ───────────────────────────────────────────────────────
let answers={score:{basic:0,estandar:0,completo:0}};
function pickQ(step,plan,val,btn){
  btn.closest('.quiz-options').querySelectorAll('.quiz-opt').forEach(b=>b.classList.remove('selected'));
  btn.classList.add('selected');
  answers.score[plan]++;
  setTimeout(()=>nextQ(step),320);
}
function nextQ(step){
  document.getElementById('q'+step).classList.remove('active');
  if(step<3){
    document.getElementById('q'+(step+1)).classList.add('active');
    document.getElementById('qbar').style.width=(step/3*100)+'%';
  }
}
function showResult(plan,btn){
  btn.closest('.quiz-options').querySelectorAll('.quiz-opt').forEach(b=>b.classList.remove('selected'));
  btn.classList.add('selected');
  document.getElementById('q3').classList.remove('active');
  document.getElementById('qbar').style.width='100%';
  const plans={
    basic:{name:'Plan Básico',desc:'Ideal para tu empresa. 2 visitas mensuales + 4 horas adicionales con respuesta en 8 horas hábiles.'},
    estandar:{name:'Plan Estándar',desc:'El más popular. 2 visitas + 8 horas adicionales con respuesta rápida en 4 horas. Incluye informe mensual.'},
    completo:{name:'Plan Completo',desc:'Máxima cobertura. 2 visitas + 16 horas adicionales con respuesta crítica en 2 horas y prioridad 24/7.'}
  };
  document.getElementById('resultName').textContent=plans[plan].name;
  document.getElementById('resultDesc').textContent=plans[plan].desc;
  document.getElementById('qresult').style.display='block';
}
function resetQuiz(){
  document.getElementById('qresult').style.display='none';
  document.querySelectorAll('.quiz-step').forEach(s=>s.classList.remove('active'));
  document.querySelectorAll('.quiz-opt').forEach(b=>b.classList.remove('selected'));
  document.getElementById('q1').classList.add('active');
  document.getElementById('qbar').style.width='0%';
  answers={score:{basic:0,estandar:0,completo:0}};
}

// ── FORM ───────────────────────────────────────────────────────
function submitForm(e){
  e.preventDefault();
  document.getElementById('contactForm').style.display='none';
  document.getElementById('formSuccess').style.display='block';
}
</script>
</body>
</html>
