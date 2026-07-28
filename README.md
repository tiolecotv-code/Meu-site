frames inviteShift{0%,100%{background-position:0% 50%;}50%{background-position:100% 50%;}}
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
tr.highlight
