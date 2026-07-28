<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Grêmio Notícias — Leco TV Sports | Tio Leco</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,400;9..144,600;9..144,700;9..144,900&family=Oswald:wght@400;500;600;700&family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<style>
  :root{
    --navy:#101425; --navy-deep:#0a0d18; --sky:#29b6f6; --sky-soft:#7dd3fc;
    --gremio-blue:#1c4e9c; --paper:#f7f5ef; --ink:#14161c; --ink-soft:#4a4d57;
    --line:#dedad0; --red:#c1272d; --green-live:#2e9e5b;
  }
  *{margin:0;padding:0;box-sizing:border-box;}
  html{scroll-behavior:smooth;}
  body{background:var(--paper);color:var(--ink);font-family:'Inter',sans-serif;}
  a{color:inherit;text-decoration:none;}
  ::selection{background:var(--sky);color:#fff;}
  img{display:block;max-width:100%;}
  .eyebrow{font-family:'Oswald',sans-serif;text-transform:uppercase;letter-spacing:.16em;font-size:.7rem;font-weight:600;color:var(--sky);}
  h1,h2,h3,h4{font-family:'Fraunces',serif;font-weight:700;letter-spacing:-.01em;line-height:1.05;color:var(--ink);}

  .topbar{background:var(--navy-deep);color:#cfd2dd;font-family:'Oswald',sans-serif;font-size:.72rem;letter-spacing:.05em;display:flex;justify-content:space-between;align-items:center;padding:7px 6vw;}
  .topbar .date{opacity:.7;}
  .topbar .live{display:flex;align-items:center;gap:8px;color:var(--sky-soft);font-weight:600;}
  .topbar .live i{width:7px;height:7px;background:var(--red);border-radius:50%;display:inline-block;animation:pulse 1.4s infinite;}
  @keyframes pulse{0%,100%{opacity:1;}50%{opacity:.3;}}

  .masthead{background:var(--navy);border-bottom:3px solid var(--sky);padding:22px 6vw 18px;box-shadow:0 8px 24px rgba(0,0,0,.2);}
  .masthead-row{display:flex;align-items:center;justify-content:space-between;gap:20px;flex-wrap:wrap;}
  .brand{display:flex;align-items:center;gap:14px;}
  .brand img{width:54px;height:54px;border-radius:50%;}
  .brand-word{font-family:'Fraunces',serif;font-weight:900;font-size:1.7rem;color:var(--paper);line-height:1;}
  .brand-word span{display:block;font-family:'Oswald',sans-serif;font-weight:600;font-size:.62rem;letter-spacing:.3em;color:var(--sky-soft);margin-top:5px;text-transform:uppercase;}
  nav{display:flex;gap:22px;}
  nav a{font-family:'Oswald',sans-serif;font-size:.8rem;letter-spacing:.06em;text-transform:uppercase;color:#cfd2dd;opacity:.8;}
  nav a:hover{opacity:1;color:var(--sky-soft);}
  @media(max-width:860px){nav{display:none;}}

  .ticker-wrap{background:var(--sky);overflow:hidden;white-space:nowrap;position:relative;}
  .ticker-tag{position:absolute;left:0;top:0;bottom:0;background:var(--navy-deep);color:var(--sky-soft);font-family:'Oswald',sans-serif;font-weight:700;font-size:.68rem;letter-spacing:.14em;display:flex;align-items:center;padding:0 16px;z-index:2;}
  .ticker-tag::after{content:'';position:absolute;right:-12px;top:0;bottom:0;width:12px;background:var(--navy-deep);clip-path:polygon(0 0,100% 50%,0 100%);}
  .ticker-track{display:inline-flex;padding-left:130px;animation:scrollT 38s linear infinite;}
  .ticker-track span{padding:7px 36px 7px 0;font-family:'Oswald',sans-serif;font-size:.8rem;color:var(--navy-deep);font-weight:500;}
  .ticker-track span b{font-weight:700;}
  @keyframes scrollT{0%{transform:translateX(0);}100%{transform:translateX(-50%);}}

  /* SPONSOR STRIP */
  .sponsor-strip{
    background:
      repeating-linear-gradient(45deg, rgba(41,182,246,.08) 0 2px, transparent 2px 18px),
      linear-gradient(135deg, #0a0d18, #101425 55%, #0a1e33);
    border-top:2px solid var(--sky);border-bottom:2px solid var(--sky);
    padding:14px 6vw;
  }
  .sponsor-strip-inner{
    max-width:1180px;margin:0 auto;display:flex;align-items:center;gap:16px;flex-wrap:nowrap;justify-content:center;
    overflow-x:auto;
  }
  .sponsor-heading{display:flex;flex-direction:column;align-items:flex-start;gap:2px;margin-right:4px;flex-shrink:0;}
  .sponsor-label{
    font-family:'Oswald',sans-serif;font-weight:700;font-size:.7rem;letter-spacing:.14em;text-transform:uppercase;
    color:#fff;background:linear-gradient(120deg,var(--sky),var(--gremio-blue));padding:5px 14px;border-radius:20px;white-space:nowrap;
    box-shadow:0 0 14px rgba(41,182,246,.55);
    display:flex;align-items:center;gap:7px;
  }
  .sponsor-label i{width:6px;height:6px;background:#fff;border-radius:50%;display:inline-block;animation:pulse 1.2s infinite;}
  .sponsor-sub{font-family:'Oswald',sans-serif;font-size:.56rem;letter-spacing:.05em;color:#8fb8d9;text-transform:uppercase;white-space:nowrap;}
  .sponsor-logos{display:flex;align-items:center;gap:10px;flex-wrap:nowrap;justify-content:center;}
  .sponsor-card{
    background:#fff;border-radius:8px;padding:6px;
    display:flex;align-items:center;justify-content:center;
    width:96px;height:48px;flex-shrink:0;
    box-shadow:0 6px 14px rgba(0,0,0,.35);
    transition:transform .2s ease;
    border:2px solid var(--sky);
    animation:sponsorGlow 1.6s ease-in-out infinite;
  }
  .sponsor-card.sponsor-combined{width:100%;max-width:640px;height:auto;padding:8px;}
  .sponsor-card:nth-child(2){animation-delay:.3s;}
  .sponsor-card:nth-child(3){animation-delay:.6s;}
  .sponsor-card:hover{transform:translateY(-3px) scale(1.03);}
  .sponsor-card img{max-width:100%;max-height:100%;width:auto;height:auto;object-fit:contain;}
  @keyframes sponsorGlow{
    0%,100%{border-color:var(--sky);box-shadow:0 6px 14px rgba(0,0,0,.35), 0 0 5px rgba(41,182,246,.3);}
    50%{border-color:#bfe9ff;box-shadow:0 6px 14px rgba(0,0,0,.35), 0 0 18px rgba(41,182,246,.9);}
  }

  .radio-announce{background:linear-gradient(90deg, var(--navy-deep), #1a2036 60%, var(--navy-deep));border-bottom:1px solid rgba(41,182,246,.3);padding:14px 6vw;display:flex;align-items:center;justify-content:center;gap:16px;flex-wrap:wrap;}
  .radio-announce .live-dot{display:flex;align-items:center;gap:8px;font-family:'Oswald',sans-serif;font-weight:700;font-size:.72rem;letter-spacing:.1em;color:#fff;background:var(--green-live);padding:5px 12px;border-radius:20px;text-transform:uppercase;}
  .radio-announce .live-dot i{width:7px;height:7px;background:#fff;border-radius:50%;display:inline-block;animation:pulse 1.2s infinite;}
  .radio-announce p{color:#e7e9f0;font-size:.9rem;font-family:'Oswald',sans-serif;text-align:center;}
  .top-player{display:flex;align-items:center;width:100%;max-width:280px;}
  .top-player audio{height:34px;width:100%;}
  audio::-webkit-media-controls-timeline{display:none;}
  audio{max-width:100%;}

  /* COMPACT TOP SCOREBOARD */
  .top-score{background:#0b3a7a;border-bottom:2px solid var(--sky);}
  .top-score-inner{
    max-width:1180px;margin:0 auto;padding:10px 6vw;
    display:flex;align-items:center;justify-content:center;gap:16px;flex-wrap:wrap;
  }
  .top-score-comp{font-family:'Oswald',sans-serif;font-size:.66rem;letter-spacing:.1em;text-transform:uppercase;color:#bcd0f2;white-space:nowrap;}
  .top-score-match{display:flex;align-items:center;gap:10px;font-family:'Oswald',sans-serif;color:#fff;}
  .ts-team{display:flex;align-items:center;gap:6px;font-size:.86rem;font-weight:600;white-space:nowrap;}
  .ts-dot{width:9px;height:9px;border-radius:50%;display:inline-block;}
  .ts-dot.mir{background:#2fae62;}
  .ts-dot.gre{background:#29b6f6;}
  .ts-num{font-family:'Fraunces',serif;font-weight:900;font-size:1.2rem;}
  .ts-x{opacity:.5;font-size:.8rem;}
  .top-score-status{font-family:'Oswald',sans-serif;font-size:.64rem;letter-spacing:.1em;text-transform:uppercase;color:#bcd0f2;background:rgba(255,255,255,.12);padding:3px 10px;border-radius:20px;white-space:nowrap;}

  /* WEEKEND HIGHLIGHT BANNER */
  .weekend-highlight{
    background:linear-gradient(90deg, #2a1608, #1a0f06 60%, #2a1608);
    border-top:1px solid rgba(41,182,246,.4);border-bottom:1px solid rgba(41,182,246,.4);
    padding:12px 6vw;display:flex;align-items:center;justify-content:center;gap:14px;flex-wrap:wrap;
  }
  .wh-badge{font-family:'Oswald',sans-serif;font-weight:700;font-size:.68rem;letter-spacing:.1em;text-transform:uppercase;color:var(--navy-deep);background:var(--sky);padding:5px 12px;border-radius:20px;white-space:nowrap;}
  .weekend-highlight p{color:#f2e6d8;font-size:.86rem;line-height:1.5;text-align:center;max-width:760px;}
  .weekend-highlight p b{color:var(--sky-soft);}
  .weekend-highlight.breaking{background:linear-gradient(90deg, #3a0e0e, #1a0606 55%, #3a0e0e);border-color:rgba(193,39,45,.5);}

  /* PROMO BANNER (uploaded match graphic) */
  .promo-banner{
    padding:14px 6vw;background:var(--navy-deep);border-top:2px solid var(--sky);border-bottom:2px solid var(--sky);
  }
  .promo-banner img{
    max-width:1000px;margin:0 auto;border-radius:8px;display:block;
    border:2px solid var(--sky);
    box-shadow:0 0 24px rgba(41,182,246,.5);
    animation:sponsorGlow 2s ease-in-out infinite;
  }

  /* TEAM FEATURE */
  .team-feature{
    background:var(--navy);border-radius:12px;overflow:hidden;margin-bottom:36px;
    border:1px solid rgba(41,182,246,.3);box-shadow:0 14px 30px rgba(16,20,37,.18);
    display:grid;grid-template-columns:1fr 1.2fr;
  }
  @media(max-width:700px){.team-feature{grid-template-columns:1fr;}}
  .team-photo{position:relative;min-height:220px;}
  .team-photo img{width:100%;height:100%;object-fit:cover;position:absolute;inset:0;}
  .team-copy{padding:26px;display:flex;flex-direction:column;justify-content:center;}

  /* RADIO INVITE BANNER */
  .radio-invite{
    background:linear-gradient(100deg, var(--gremio-blue), var(--navy-deep) 55%, var(--sky));
    background-size:180% 180%;
    animation:inviteShift 6s ease-in-out infinite;
    padding:18px 6vw;display:flex;align-items:center;gap:20px;flex-wrap:wrap;justify-content:center;
    border-top:2px solid var(--sky-soft);border-bottom:2px solid var(--sky-soft);
  }
  @keyframes inviteShift{0%,100%{background-position:0% 50%;}50%{background-position:100% 50%;}}
  .ri-icon{
    width:52px;height:52px;border-radius:50%;background:rgba(255,255,255,.12);border:2px solid rgba(255,255,255,.5);
    display:flex;align-items:center;justify-content:center;flex-shrink:0;
  }
  .ri-eq{display:flex;align-items:flex-end;gap:3px;height:22px;}
  .ri-eq span{width:4px;background:#fff;display:block;border-radius:2px;animation:eq 1s infinite ease-in-out;}
  .ri-eq span:nth-child(1){height:40%;}
  .ri-eq span:nth-child(2){height:100%;animation-delay:.15s;}
  .ri-eq span:nth-child(3){height:65%;animation-delay:.3s;}
  .ri-eq span:nth-child(4){height:85%;animation-delay:.45s;}
  .ri-copy{max-width:600px;}
  .ri-tag{
    display:inline-flex;align-items:center;gap:7px;font-family:'Oswald',sans-serif;font-weight:700;font-size:.68rem;
    letter-spacing:.14em;text-transform:uppercase;color:var(--navy-deep);background:#fff;padding:5px 14px;border-radius:20px;margin-bottom:8px;
  }
  .ri-tag i{width:6px;height:6px;background:var(--red);border-radius:50%;display:inline-block;animation:pulse 1.1s infinite;}
  .ri-copy p{color:#fff;font-size:.94rem;line-height:1.55;font-family:'Inter',sans-serif;}
  .ri-copy p b{color:#fff;text-decoration:underline;text-decoration-color:var(--sky-soft);text-underline-offset:3px;}
  .ri-cta{
    font-family:'Oswald',sans-serif;font-weight:700;font-size:.8rem;letter-spacing:.06em;text-transform:uppercase;
    background:#fff;color:var(--navy-deep);padding:12px 24px;border-radius:4px;white-space:nowrap;flex-shrink:0;
    box-shadow:0 8px 20px rgba(0,0,0,.25);transition:transform .2s ease;
  }
  .ri-cta:hover{transform:translateY(-2px);}

  .breaking-badge{background:var(--red);color:#fff;display:inline-flex;align-items:center;gap:7px;}
  .bk-dot{width:7px;height:7px;background:#fff;border-radius:50%;display:inline-block;animation:pulse 1.1s infinite;}

  .wrap{max-width:1180px;margin:0 auto;padding:44px 6vw;}
  .layout{display:grid;grid-template-columns:1fr 320px;gap:44px;align-items:start;}
  @media(max-width:900px){.layout{grid-template-columns:1fr;}}

  /* SCOREBOARD HERO */
  .hero-story{border-bottom:1px solid var(--line);padding-bottom:36px;margin-bottom:36px;}
  .scoreboard{
    background:linear-gradient(135deg,#0e2c5c,#101425 55%,#075985);
    border-radius:10px;padding:30px 26px;margin-bottom:22px;color:#fff;position:relative;overflow:hidden;
    box-shadow:0 20px 40px rgba(16,20,37,.25);
  }
  .scoreboard::before{
    content:'';position:absolute;inset:-40% -10% auto -10%;height:140%;
    background:radial-gradient(circle at 30% 20%, rgba(41,182,246,.35), transparent 55%),
               radial-gradient(circle at 80% 80%, rgba(28,78,156,.35), transparent 55%);
    pointer-events:none;
  }
  .scoreboard > *{position:relative;z-index:1;}
  .scoreboard .comp{font-family:'Oswald',sans-serif;font-size:.68rem;letter-spacing:.14em;text-transform:uppercase;color:var(--sky-soft);text-align:center;margin-bottom:18px;}
  .score-row{display:flex;align-items:center;justify-content:center;gap:22px;}
  .team{display:flex;flex-direction:column;align-items:center;gap:8px;width:130px;}
  .crest{width:56px;height:56px;border-radius:50%;display:flex;align-items:center;justify-content:center;font-family:'Fraunces',serif;font-weight:900;font-size:1.3rem;color:#fff;border:2px solid rgba(255,255,255,.5);}
  .crest.mir{background:#0a5c2e;}
  .crest.gre{background:#1c4e9c;}
  .crest-img{width:64px;height:64px;object-fit:contain;background:#fff;border-radius:50%;padding:6px;box-shadow:0 4px 14px rgba(0,0,0,.25);}
  .team-name{font-family:'Oswald',sans-serif;font-size:.78rem;letter-spacing:.05em;text-transform:uppercase;text-align:center;}
  .score-num{font-family:'Fraunces',serif;font-weight:900;font-size:3rem;line-height:1;}
  .score-sep{font-family:'Oswald',sans-serif;font-size:1.4rem;opacity:.5;}
  .scoreboard .meta{text-align:center;margin-top:18px;font-family:'Oswald',sans-serif;font-size:.72rem;color:#c7cad4;letter-spacing:.03em;}
  .match-facts{display:flex;gap:10px;flex-wrap:wrap;margin-bottom:18px;}
  .mf{background:#fff;border:1px solid var(--line);border-radius:8px;padding:8px 14px;flex:1;min-width:140px;text-align:center;}
  .mf-label{display:block;font-family:'Oswald',sans-serif;font-size:.6rem;letter-spacing:.1em;text-transform:uppercase;color:var(--ink-soft);margin-bottom:3px;}
  .mf-value{display:block;font-family:'Oswald',sans-serif;font-size:.82rem;font-weight:600;color:var(--gremio-blue);}
  .hero-story h2{font-size:clamp(1.7rem,3.2vw,2.4rem);margin-bottom:14px;}
  .hero-story .dek{font-size:1.02rem;color:var(--ink-soft);line-height:1.6;max-width:660px;margin-bottom:14px;}
  .byline{font-family:'Oswald',sans-serif;font-size:.78rem;color:var(--ink-soft);}
  .byline b{color:var(--ink);}

  .section-label{display:flex;align-items:center;gap:14px;margin:0 0 22px;}
  .section-label h3{font-size:1.25rem;}
  .section-label::after{content:'';flex:1;height:1px;background:var(--line);}

  .pitch-wrap{background:var(--navy);border-radius:14px;padding:22px;margin-bottom:36px;border:1px solid rgba(41,182,246,.3);box-shadow:0 14px 30px rgba(16,20,37,.18);}
  .pitch-header{display:flex;justify-content:space-between;align-items:center;margin-bottom:14px;flex-wrap:wrap;gap:8px;}
  .pitch-coach{font-family:'Oswald',sans-serif;font-size:.82rem;color:#c7cad4;}
  .pitch-coach b{color:var(--sky-soft);}
  .pitch-formation{font-family:'Oswald',sans-serif;font-weight:700;font-size:.78rem;letter-spacing:.08em;color:var(--navy-deep);background:var(--sky-soft);padding:4px 12px;border-radius:20px;}
  .pitch{
    position:relative;width:100%;max-width:420px;margin:0 auto;aspect-ratio:2/3;border-radius:10px;overflow:hidden;
    background:
      repeating-linear-gradient(180deg, rgba(255,255,255,.05) 0 15%, transparent 15% 30%),
      linear-gradient(180deg,#1c7a3e,#156a34);
    border:2px solid rgba(255,255,255,.6);
  }
  .pitch-halfline{position:absolute;top:50%;left:0;right:0;height:2px;background:rgba(255,255,255,.55);}
  .pitch-circle{position:absolute;top:50%;left:50%;width:26%;aspect-ratio:1;border:2px solid rgba(255,255,255,.55);border-radius:50%;transform:translate(-50%,-50%);}
  .pitch-box{position:absolute;left:50%;width:56%;height:13%;border:2px solid rgba(255,255,255,.55);transform:translateX(-50%);}
  .pitch-box.top{top:0;border-top:none;}
  .pitch-box.bottom{bottom:0;border-bottom:none;}
  .pitch-arc{position:absolute;left:50%;width:22%;aspect-ratio:2/1;border:2px solid rgba(255,255,255,.55);border-radius:0 0 50% 50%;transform:translateX(-50%);}
  .pitch-arc.top{top:13%;border-top:none;transform:translateX(-50%) rotate(180deg);}
  .pitch-arc.bottom{bottom:13%;border-bottom:none;}
  .pt{position:absolute;transform:translate(-50%,-50%);display:flex;flex-direction:column;align-items:center;gap:3px;width:78px;z-index:2;}
  .pt .dot{
    width:32px;height:32px;border-radius:50%;background:var(--navy);border:2px solid var(--sky-soft);
    display:flex;align-items:center;justify-content:center;font-family:'Oswald',sans-serif;font-weight:700;font-size:.56rem;color:#fff;
    box-shadow:0 4px 10px rgba(0,0,0,.4);
  }
  .pt .dot.gk{background:var(--sky);border-color:#fff;color:var(--navy-deep);}
  .pt .nm{font-family:'Oswald',sans-serif;font-size:.6rem;color:#fff;text-shadow:0 1px 4px rgba(0,0,0,.7);text-align:center;line-height:1.15;white-space:nowrap;}
  .pitch-note{margin-top:16px;padding-top:14px;border-top:1px solid rgba(255,255,255,.15);font-size:.82rem;color:#a8acb8;line-height:1.55;}

  .standings-table-wrap{background:#fff;border:1px solid var(--line);border-radius:10px;overflow:hidden;margin-bottom:36px;box-shadow:0 10px 24px rgba(16,20,37,.06);}

  /* FEATURED VIDEOS */
  .video-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:22px;margin-bottom:36px;}
  @media(max-width:640px){.video-grid{grid-template-columns:1fr;}}
  .video-card{
    background:var(--navy);border-radius:10px;overflow:hidden;border:1px solid rgba(41,182,246,.3);
    box-shadow:0 14px 30px rgba(16,20,37,.18);
    aspect-ratio:9/14.5;
    display:flex;align-items:center;justify-content:center;
  }
  .video-card iframe{width:100%;height:100%;border:none;}
  .standings-table{width:100%;border-collapse:collapse;font-family:'Oswald',sans-serif;}
  .standings-table thead th{
    background:var(--navy);color:var(--sky-soft);font-size:.66rem;letter-spacing:.1em;text-transform:uppercase;
    text-align:left;padding:10px 14px;font-weight:600;
  }
  .standings-table thead th:nth-child(3), .standings-table thead th:nth-child(4), .standings-table thead th:nth-child(5){text-align:center;}
  .standings-table tbody td{padding:10px 14px;font-size:.86rem;color:var(--ink);border-bottom:1px solid var(--line);}
  .standings-table tbody tr:last-child td{border-bottom:none;}
  .standings-table tbody td:nth-child(3), .standings-table tbody td:nth-child(4){text-align:center;color:var(--ink-soft);}
  .standings-table tbody td:nth-child(5){text-align:center;font-weight:700;}
  .standings-table tbody tr.highlight td{background:rgba(28,78,156,.08);font-weight:700;}
  .standings-table tbody tr.highlight td:first-child{border-left:3px solid var(--gremio-blue);}
  .standings-table tbody tr.z4 td{background:rgba(193,39,45,.05);}
  .standings-legend{display:flex;align-items:center;gap:8px;padding:10px 14px;font-family:'Oswald',sans-serif;font-size:.68rem;color:var(--ink-soft);border-top:1px solid var(--line);}
  .standings-legend .dot{width:8px;height:8px;border-radius:50%;background:var(--red);display:inline-block;}

  .quote-block{background:#fff;border-left:4px solid var(--sky);border-radius:6px;padding:18px 22px;margin-bottom:18px;box-shadow:0 8px 20px rgba(16,20,37,.06);}
  .quote-block .who{font-family:'Oswald',sans-serif;font-size:.72rem;letter-spacing:.08em;text-transform:uppercase;color:var(--ink-soft);margin-bottom:8px;}
  .quote-block p{font-family:'Fraunces',serif;font-size:1.05rem;font-style:italic;color:var(--ink);line-height:1.5;}
  .quote-b
