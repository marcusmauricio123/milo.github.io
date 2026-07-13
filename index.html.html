<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>HUB Franquias</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
  :root{
    --navy:#21295C;
    --navy-2:#2C3768;
    --deepblue:#065A82;
    --teal:#1C7293;
    --mint:#5FC9BF;
    --offwhite:#F5F8FA;
    --white:#FFFFFF;
    --ink:#1B222B;
    --muted:#6B7684;
    --ice:#CADCFC;
  }
  *{box-sizing:border-box;}
  html,body{
    margin:0;padding:0;height:100%;overflow:hidden;
    font-family:Calibri,'Segoe UI',Arial,sans-serif;
    background:#0d1330;
  }
  h1,h2,h3{font-family:Cambria,Georgia,'Times New Roman',serif;margin:0;}

  .deck{position:relative;width:100vw;height:100vh;}

  .slide{
    position:absolute;inset:0;
    display:flex;flex-direction:column;justify-content:center;
    opacity:0;visibility:hidden;
    transform:translateX(40px) scale(0.98);
    transition:opacity .55s ease, transform .55s ease, visibility .55s;
    pointer-events:none;
  }
  .slide.active{
    opacity:1;visibility:visible;transform:translateX(0) scale(1);
    pointer-events:auto;
    z-index:2;
  }
  .slide.prevslide{transform:translateX(-40px) scale(0.98);}

  .slide-inner{width:100%;height:100%;position:relative;padding:70px 90px;}

  /* ---------- reveal animation for children ---------- */
  .reveal{opacity:0;transform:translateY(26px);transition:opacity .6s ease, transform .6s ease;}
  .slide.active .reveal{opacity:1;transform:translateY(0);}
  .slide.active .r1{transition-delay:.05s;}
  .slide.active .r2{transition-delay:.15s;}
  .slide.active .r3{transition-delay:.25s;}
  .slide.active .r4{transition-delay:.35s;}
  .slide.active .r5{transition-delay:.45s;}
  .slide.active .r6{transition-delay:.55s;}
  .slide.active .r7{transition-delay:.65s;}

  .scalein{opacity:0;transform:scale(.7);transition:opacity .55s ease, transform .55s cubic-bezier(.34,1.56,.64,1);}
  .slide.active .scalein{opacity:1;transform:scale(1);}

  /* -------- backgrounds -------- */
  .bg-navy{background:radial-gradient(circle at 85% 0%, #16407a 0%, var(--navy) 45%, var(--navy) 100%);color:var(--white);}
  .bg-light{background:var(--offwhite);color:var(--ink);}
  .bg-white{background:var(--white);color:var(--ink);}

  .blob{position:absolute;border-radius:50%;pointer-events:none;}

  /* -------- generic bits -------- */
  .eyebrow{
    font-size:14px;font-weight:700;letter-spacing:2px;color:var(--mint);
    text-transform:uppercase;margin-bottom:10px;
  }
  .title-xl{font-size:46px;font-weight:700;color:var(--navy);}
  .bg-navy .title-xl{color:var(--white);}
  .subtitle{font-size:15px;color:var(--muted);margin-top:14px;max-width:820px;line-height:1.5;}
  .bg-navy .subtitle{color:var(--ice);}

  .footer{
    position:absolute;left:90px;bottom:34px;font-size:12px;font-style:italic;color:var(--muted);
  }
  .footer-r{
    position:absolute;right:90px;bottom:34px;font-size:12px;color:var(--muted);
  }
  .bg-navy .footer, .bg-navy .footer-r{color:#9AA6C4;}

  .icon-circle{
    border-radius:50%;display:flex;align-items:center;justify-content:center;
    flex-shrink:0;
  }

  /* -------- cards (slide 2) -------- */
  .card-row{display:flex;gap:16px;margin-top:50px;}
  .card{
    background:var(--white);border-radius:14px;padding:22px 14px;flex:1;
    text-align:center;box-shadow:0 14px 30px rgba(20,30,60,.10);
    transition:transform .35s ease, box-shadow .35s ease;
  }
  .card:hover{transform:translateY(-8px);box-shadow:0 20px 40px rgba(20,30,60,.16);}
  .card .icon-circle{width:60px;height:60px;font-size:26px;margin:0 auto 16px;}
  .card h3{font-size:14px;color:var(--navy);line-height:1.25;}
  .card p{font-size:10.5px;color:var(--muted);margin-top:10px;line-height:1.4;}

  /* -------- split slide (slide 3) -------- */
  .split{display:flex;height:100%;}
  .split-left{
    width:36%;background:var(--deepblue);color:var(--white);
    display:flex;flex-direction:column;align-items:center;justify-content:center;
    padding:40px;text-align:center;position:relative;
  }
  .split-left .icon-circle{width:110px;height:110px;font-size:52px;background:var(--mint);margin-bottom:26px;}
  .split-left h2{font-size:26px;line-height:1.2;}
  .split-left p{font-size:13px;color:var(--ice);margin-top:16px;line-height:1.5;}
  .split-right{width:64%;padding:90px 70px;display:flex;flex-direction:column;justify-content:center;gap:44px;}
  .split-item{display:flex;align-items:flex-start;gap:26px;}
  .split-item .icon-circle{width:64px;height:64px;font-size:26px;background:var(--teal);color:#fff;}
  .split-item h3{font-size:20px;color:var(--navy);margin-bottom:8px;}
  .split-item p{font-size:14px;color:var(--muted);line-height:1.5;max-width:640px;}

  /* -------- slide 4 grid + stat -------- */
  .stat-box{
    position:absolute;top:70px;right:90px;background:var(--navy);border-radius:12px;
    padding:20px 34px;color:#fff;text-align:center;min-width:200px;
  }
  .stat-box .num{font-size:44px;font-weight:700;color:var(--mint);font-family:Cambria,serif;}
  .stat-box .lbl{font-size:11px;margin-top:4px;line-height:1.3;}
  .grid2x2{display:grid;grid-template-columns:1fr 1fr;gap:22px;margin-top:60px;}
  .row-card{
    background:var(--white);border-radius:12px;padding:26px 28px;display:flex;gap:20px;align-items:flex-start;
    box-shadow:0 10px 26px rgba(20,30,60,.08);
  }
  .row-card .icon-circle{width:60px;height:60px;font-size:24px;background:var(--deepblue);color:#fff;flex-shrink:0;}
  .row-card h3{font-size:16px;color:var(--navy);}
  .row-card p{font-size:12px;color:var(--muted);margin-top:8px;line-height:1.4;}

  /* -------- process flow (slide 5) -------- */
  .flow{display:flex;align-items:stretch;justify-content:center;gap:0;margin-top:70px;}
  .flow-step{
    background:var(--navy-2);border:1px solid #3E4A82;border-radius:12px;
    width:190px;padding:22px 16px;text-align:center;position:relative;margin-right:34px;
  }
  .flow-step .num{position:absolute;top:12px;left:16px;font-family:Cambria,serif;font-size:20px;font-weight:700;color:var(--mint);}
  .flow-step .icon-circle{width:64px;height:64px;font-size:26px;background:var(--deepblue);margin:20px auto 18px;color:#fff;}
  .flow-step h4{font-size:13px;color:#fff;line-height:1.3;}
  .flow-arrow{
    align-self:center;color:var(--mint);font-size:26px;font-weight:700;margin-right:34px;margin-top:-40px;
  }

  /* -------- slide 6 five cards -------- */
  .card5-row{display:flex;gap:20px;margin-top:56px;}
  .card5{
    background:var(--white);border-radius:12px;padding:24px 14px;flex:1;text-align:center;
    box-shadow:0 10px 24px rgba(20,30,60,.08);
  }
  .card5 .icon-circle{width:64px;height:64px;font-size:26px;background:var(--deepblue);color:#fff;margin:0 auto 16px;}
  .card5 h3{font-size:14px;color:var(--navy);}
  .card5 p{font-size:10.5px;color:var(--muted);margin-top:10px;line-height:1.35;}

  /* -------- slide 7 education -------- */
  .edu-header{
    background:var(--teal);color:#fff;padding:60px 90px 40px;position:relative;
  }
  .edu-header .icon-circle{
    position:absolute;right:90px;top:40px;width:96px;height:96px;font-size:42px;background:var(--mint);
  }
  .edu-body{padding:50px 90px;}
  .grid2x2-edu{display:grid;grid-template-columns:1fr 1fr;gap:26px;}
  .edu-card{
    background:var(--offwhite);border-radius:10px;padding:24px 26px;display:flex;gap:20px;align-items:flex-start;
  }
  .edu-card .icon-circle{width:60px;height:60px;font-size:24px;background:var(--teal);color:#fff;flex-shrink:0;}
  .edu-card h3{font-size:16px;color:var(--navy);}
  .edu-card p{font-size:12px;color:var(--muted);margin-top:8px;line-height:1.4;}

  /* -------- slide 8 repasse -------- */
  .rep-cols{display:flex;gap:22px;margin-top:56px;}
  .rep-col{
    background:#fff;border-radius:12px;padding:28px 26px;flex:1;
    box-shadow:0 10px 26px rgba(20,30,60,.08);
  }
  .rep-head{display:flex;align-items:center;gap:16px;margin-bottom:22px;}
  .rep-col .icon-circle{width:52px;height:52px;font-size:22px;color:#fff;}
  .rep-col h3{font-size:17px;color:var(--navy);}
  .rep-col ul{margin:0;padding:0;list-style:none;}
  .rep-col li{
    font-size:13px;color:var(--ink);padding:9px 0 9px 22px;position:relative;line-height:1.4;
  }
  .rep-col li:before{
    content:"";position:absolute;left:0;top:17px;width:6px;height:6px;border-radius:50%;background:var(--teal);
  }

  /* -------- slide 9 closing -------- */
  .closing{display:flex;flex-direction:column;align-items:center;text-align:center;justify-content:center;height:100%;}
  .closing .icon-circle{width:100px;height:100px;font-size:44px;background:var(--mint);margin-bottom:36px;}
  .closing h2{font-size:36px;color:#fff;max-width:900px;line-height:1.3;}
  .closing p{font-size:15px;color:var(--ice);max-width:720px;margin-top:22px;line-height:1.5;}
  .tags{display:flex;gap:14px;margin-top:44px;row-gap:14px;}
  .tag{
    background:var(--navy-2);border-radius:30px;padding:14px 26px;font-size:13px;font-weight:700;color:var(--mint);
  }

  /* -------- nav controls -------- */
  .progress{position:fixed;top:0;left:0;height:4px;background:var(--mint);z-index:10;transition:width .4s ease;}
  .navbar{
    position:fixed;bottom:22px;left:50%;transform:translateX(-50%);
    display:flex;align-items:center;gap:18px;z-index:10;
    background:rgba(10,15,35,.55);backdrop-filter:blur(6px);
    padding:10px 20px;border-radius:40px;
  }
  .navbtn{
    width:36px;height:36px;border-radius:50%;border:none;background:rgba(255,255,255,.12);
    color:#fff;font-size:16px;cursor:pointer;display:flex;align-items:center;justify-content:center;
    transition:background .25s ease;
  }
  .navbtn:hover{background:var(--mint);color:var(--navy);}
  .dots{display:flex;gap:9px;}
  .dot{width:8px;height:8px;border-radius:50%;background:rgba(255,255,255,.35);cursor:pointer;transition:all .25s ease;}
  .dot.active{background:var(--mint);width:22px;border-radius:5px;}
  .counter{color:#fff;font-size:12px;min-width:42px;text-align:center;letter-spacing:.5px;}

  @media (max-width:900px){
    .slide-inner{padding:34px 26px;}
    .title-xl{font-size:28px;}
    .card-row,.card5-row{flex-wrap:wrap;}
    .split{flex-direction:column;}
    .split-left,.split-right{width:100%;}
    .grid2x2,.grid2x2-edu,.rep-cols{grid-template-columns:1fr;flex-direction:column;}
    .flow{flex-wrap:wrap;}
  }
</style>
</head>
<body>

<div class="progress" id="progress"></div>

<div class="deck" id="deck">

  <!-- SLIDE 1 : TITLE -->
  <section class="slide bg-navy" data-index="0">
    <div class="blob" style="width:420px;height:420px;top:-140px;right:-60px;background:rgba(6,90,130,.55);"></div>
    <div class="blob" style="width:260px;height:260px;top:-30px;right:120px;background:rgba(28,114,147,.55);"></div>
    <div class="blob" style="width:320px;height:320px;bottom:-160px;left:-140px;background:rgba(6,90,130,.55);"></div>
    <div class="slide-inner">
      <div class="icon-circle scalein" style="width:90px;height:90px;font-size:38px;background:var(--mint);margin-bottom:34px;">🧩</div>
      <h1 class="title-xl reveal r1" style="font-size:56px;letter-spacing:1px;">HUB FRANQUIAS</h1>
      <p class="subtitle reveal r2" style="font-size:18px;max-width:680px;">O ecossistema que estrutura, vende, formata,
        treina e repassa franquias — do zero à expansão nacional.</p>
      <p class="reveal r3" style="margin-top:70px;font-size:11px;font-weight:700;letter-spacing:1px;color:var(--mint);max-width:900px;line-height:1.7;">
        DYNAMIS &nbsp;·&nbsp; FAZ FRANQUIA FRANCHISING &nbsp;·&nbsp; NEGÓCIO E FRANQUIA &nbsp;·&nbsp; FAZ FRANQUIA CONSULTORIA &nbsp;·&nbsp; FAZ EDUCAÇÃO &nbsp;·&nbsp; REPASSE FRANCHISING
      </p>
    </div>
  </section>

  <!-- SLIDE 2 : OVERVIEW -->
  <section class="slide bg-light" data-index="1">
    <div class="slide-inner">
      <div class="eyebrow reveal r1">Visão geral</div>
      <h2 class="title-xl reveal r1">Um ecossistema, seis empresas</h2>
      <p class="subtitle reveal r2">O HUB Franquias reúne seis empresas que, juntas, cobrem todo o ciclo de vida de uma rede de franquias.</p>
      <div class="card-row">
        <div class="card reveal r3"><div class="icon-circle" style="background:var(--navy);color:#fff;">🏢</div><h3>Dynamis</h3><p>Gestão e estratégia de negócios</p></div>
        <div class="card reveal r3"><div class="icon-circle" style="background:var(--deepblue);color:#fff;">🚀</div><h3>Faz Franquia Franchising</h3><p>Vendas e aceleração de franquias</p></div>
        <div class="card reveal r4"><div class="icon-circle" style="background:var(--teal);color:#fff;">📰</div><h3>Negócio e Franquia</h3><p>Notícias, leads, eventos e conteúdo</p></div>
        <div class="card reveal r5"><div class="icon-circle" style="background:var(--deepblue);color:#fff;">📋</div><h3>Faz Franquia Consultoria</h3><p>Formatação, operação e gestão</p></div>
        <div class="card reveal r6"><div class="icon-circle" style="background:var(--teal);color:#fff;">🎓</div><h3>Faz Educação</h3><p>Treinamento e plataforma educacional</p></div>
        <div class="card reveal r7"><div class="icon-circle" style="background:var(--deepblue);color:#fff;">🔄</div><h3>Repasse Franchising</h3><p>Plataforma de repasse de franquias</p></div>
      </div>
      <div class="footer">Visão geral do ecossistema</div>
      <div class="footer-r">HUB Franquias</div>
    </div>
  </section>

  <!-- SLIDE 3 : FAZ FRANQUIA FRANCHISING -->
  <section class="slide bg-white" data-index="2">
    <div class="split">
      <div class="split-left">
        <div class="icon-circle scalein">🚀</div>
        <h2 class="reveal r1">Faz Franquia<br>Franchising</h2>
        <p class="reveal r2">A frente comercial: leva a marca ao mercado e acelera o crescimento da rede.</p>
      </div>
      <div class="split-right">
        <div class="split-item reveal r2">
          <div class="icon-circle">🤝</div>
          <div><h3>Vendas</h3><p>Condução comercial do processo de venda de novas unidades franqueadas.</p></div>
        </div>
        <div class="split-item reveal r4">
          <div class="icon-circle">📈</div>
          <div><h3>Aceleração de franquias</h3><p>Estratégias e ações para acelerar a expansão e a captação de franqueados.</p></div>
        </div>
      </div>
    </div>
    <div class="footer">Faz Franquia Franchising</div>
    <div class="footer-r">HUB Franquias</div>
  </section>

  <!-- SLIDE 4 : NEGÓCIO E FRANQUIA -->
  <section class="slide bg-light" data-index="3">
    <div class="slide-inner">
      <h2 class="title-xl reveal r1">Negócio e Franquia</h2>
      <p class="subtitle reveal r2">Conteúdo, relacionamento e geração de demanda para o setor de franquias.</p>
      <div class="stat-box scalein">
        <div class="num">24</div>
        <div class="lbl">eventos por ano<br>em capitais</div>
      </div>
      <div class="grid2x2">
        <div class="row-card reveal r3"><div class="icon-circle">📰</div><div><h3>Notícias</h3><p>Cobertura editorial do mercado de franquias.</p></div></div>
        <div class="row-card reveal r4"><div class="icon-circle">👥</div><div><h3>Geração de Leads</h3><p>Captação de interessados para redes franqueadoras.</p></div></div>
        <div class="row-card reveal r5"><div class="icon-circle">📣</div><div><h3>Conteúdo Digital</h3><p>Produção de conteúdo para presença digital das marcas.</p></div></div>
        <div class="row-card reveal r6"><div class="icon-circle">🧑‍🏫</div><div><h3>Assessoria de Marketing</h3><p>Marketing terceirizado para franqueadores.</p></div></div>
      </div>
      <div class="footer">Negócio e Franquia</div>
      <div class="footer-r">HUB Franquias</div>
    </div>
  </section>

  <!-- SLIDE 5 : FORMATAÇÃO -->
  <section class="slide bg-navy" data-index="4">
    <div class="slide-inner">
      <div class="eyebrow reveal r1">Faz Franquia Consultoria</div>
      <h2 class="title-xl reveal r1">Formatação do negócio</h2>
      <p class="subtitle reveal r2">Cinco etapas para transformar um negócio próprio em uma franquia formatada e pronta para operar.</p>
      <div class="flow">
        <div class="flow-step reveal r3"><div class="num">1</div><div class="icon-circle">📋</div><h4>Elaboração do modelo de negócios</h4></div>
        <div class="flow-arrow reveal r3">›</div>
        <div class="flow-step reveal r4"><div class="num">2</div><div class="icon-circle">🖋️</div><h4>Registro no INPI</h4></div>
        <div class="flow-arrow reveal r4">›</div>
        <div class="flow-step reveal r5"><div class="num">3</div><div class="icon-circle">📄</div><h4>Desenvolvimento da COF</h4></div>
        <div class="flow-arrow reveal r5">›</div>
        <div class="flow-step reveal r6"><div class="num">4</div><div class="icon-circle">⚖️</div><h4>Desenvolvimento do Contrato</h4></div>
        <div class="flow-arrow reveal r6">›</div>
        <div class="flow-step reveal r7" style="margin-right:0;"><div class="num">5</div><div class="icon-circle">💻</div><h4>Manuais</h4></div>
      </div>
      <div class="footer">Faz Franquia Consultoria · Formatação</div>
      <div class="footer-r">HUB Franquias</div>
    </div>
  </section>

  <!-- SLIDE 6 : OPERAÇÃO E GESTÃO -->
  <section class="slide bg-light" data-index="5">
    <div class="slide-inner">
      <div class="eyebrow reveal r1" style="color:var(--teal);">Faz Franquia Consultoria</div>
      <h2 class="title-xl reveal r1">Operação, gestão e registro</h2>
      <p class="subtitle reveal r2">Depois de formatada, a franquia é implantada, gerida e regularizada perante o mercado.</p>
      <div class="card5-row">
        <div class="card5 reveal r3"><div class="icon-circle">⚙️</div><h3>Operações</h3><p>Padronização e suporte às operações da rede franqueada.</p></div>
        <div class="card5 reveal r4"><div class="icon-circle">🚀</div><h3>Implantação</h3><p>Abertura e implantação de novas unidades franqueadas.</p></div>
        <div class="card5 reveal r5"><div class="icon-circle">📣</div><h3>Marketing</h3><p>Estratégia de marketing para a marca franqueadora.</p></div>
        <div class="card5 reveal r6"><div class="icon-circle">📋</div><h3>Gestão</h3><p>Gestão contínua da rede e dos processos internos.</p></div>
        <div class="card5 reveal r7"><div class="icon-circle">🖋️</div><h3>Registro na ABF</h3><p>Regularização da marca junto à Associação Brasileira de Franchising.</p></div>
      </div>
      <div class="footer">Faz Franquia Consultoria · Operação e gestão</div>
      <div class="footer-r">HUB Franquias</div>
    </div>
  </section>

  <!-- SLIDE 7 : FAZ EDUCAÇÃO -->
  <section class="slide bg-white" data-index="6">
    <div class="edu-header">
      <h2 class="reveal r1" style="font-size:34px;">Faz Educação</h2>
      <p class="reveal r2" style="font-size:14px;margin-top:10px;max-width:640px;">Formação e capacitação contínua para franqueados, franqueadores e equipes.</p>
      <div class="icon-circle scalein">🎓</div>
    </div>
    <div class="edu-body">
      <div class="grid2x2-edu">
        <div class="edu-card reveal r3"><div class="icon-circle">💻</div><div><h3>CCD Online</h3><p>Curso de Certificação e Desenvolvimento em formato 100% online.</p></div></div>
        <div class="edu-card reveal r4"><div class="icon-circle">🧑‍🏫</div><div><h3>CCD Presencial</h3><p>Curso de Certificação e Desenvolvimento com turmas presenciais.</p></div></div>
        <div class="edu-card reveal r5"><div class="icon-circle">👥</div><div><h3>CCD Treinamentos</h3><p>Treinamentos complementares dentro do programa CCD.</p></div></div>
        <div class="edu-card reveal r6"><div class="icon-circle">🌐</div><div><h3>Plataforma Educacional</h3><p>Ambiente digital que centraliza todo o conteúdo de ensino.</p></div></div>
      </div>
    </div>
    <div class="footer">Faz Educação</div>
    <div class="footer-r">HUB Franquias</div>
  </section>

  <!-- SLIDE 8 : REPASSE FRANCHISING -->
  <section class="slide bg-light" data-index="7">
    <div class="slide-inner">
      <h2 class="title-xl reveal r1">Repasse Franchising</h2>
      <p class="subtitle reveal r2">Plataforma de repasse de franquias — conecta franqueado, franqueador e interessado em um único fluxo, com aderência total à COF.</p>
      <div class="rep-cols">
        <div class="rep-col reveal r3">
          <div class="rep-head"><div class="icon-circle" style="background:var(--deepblue);">🤝</div><h3>Franqueado</h3></div>
          <ul>
            <li>Segue rigorosamente a COF</li>
            <li>Facilidade de acompanhamento do processo</li>
          </ul>
        </div>
        <div class="rep-col reveal r4">
          <div class="rep-head"><div class="icon-circle" style="background:var(--teal);">📋</div><h3>Cadastro Franqueador</h3></div>
          <ul>
            <li>Perfil do comprador</li>
            <li>Marca</li>
            <li>Tipo de franquia</li>
            <li>Vantagens para negociações feitas na plataforma</li>
          </ul>
        </div>
        <div class="rep-col reveal r5">
          <div class="rep-head"><div class="icon-circle" style="background:var(--deepblue);">📍</div><h3>Interessado</h3></div>
          <ul>
            <li>Local (CEP e endereço)</li>
            <li>Segmento</li>
            <li>Tipo de franquia</li>
            <li>Valor</li>
          </ul>
        </div>
      </div>
      <div class="footer">Repasse Franchising</div>
      <div class="footer-r">HUB Franquias</div>
    </div>
  </section>

  <!-- SLIDE 9 : CLOSING -->
  <section class="slide bg-navy" data-index="8">
    <div class="blob" style="width:380px;height:380px;top:-160px;left:-140px;background:rgba(6,90,130,.5);"></div>
    <div class="blob" style="width:340px;height:340px;bottom:-160px;right:-120px;background:rgba(28,114,147,.5);"></div>
    <div class="closing">
      <div class="icon-circle scalein">🧩</div>
      <h2 class="reveal r1">Do franqueado ao franqueador,<br>um único ecossistema</h2>
      <p class="reveal r2">O HUB Franquias integra Dynamis, franchising, consultoria, educação e repasse em uma jornada só — da ideia à expansão nacional.</p>
      <div class="tags" style="flex-wrap:wrap;justify-content:center;max-width:820px;">
        <div class="tag reveal r3">Dynamis</div>
        <div class="tag reveal r3">Faz Franquia Franchising</div>
        <div class="tag reveal r4">Negócio e Franquia</div>
        <div class="tag reveal r5">Faz Franquia Consultoria</div>
        <div class="tag reveal r6">Faz Educação</div>
        <div class="tag reveal r6">Repasse Franchising</div>
      </div>
    </div>
  </section>

</div>

<div class="navbar">
  <button class="navbtn" id="prevBtn">‹</button>
  <div class="dots" id="dots"></div>
  <div class="counter" id="counter">1 / 9</div>
  <button class="navbtn" id="nextBtn">›</button>
</div>

<script>
  const slides = Array.from(document.querySelectorAll('.slide'));
  const total = slides.length;
  let current = 0;

  const dotsWrap = document.getElementById('dots');
  slides.forEach((_, i) => {
    const d = document.createElement('div');
    d.className = 'dot' + (i === 0 ? ' active' : '');
    d.addEventListener('click', () => goTo(i));
    dotsWrap.appendChild(d);
  });
  const dots = Array.from(dotsWrap.children);
  const counter = document.getElementById('counter');
  const progress = document.getElementById('progress');

  function render(){
    slides.forEach((s, i) => {
      s.classList.remove('active','prevslide');
      if(i === current) s.classList.add('active');
      else if(i < current) s.classList.add('prevslide');
    });
    dots.forEach((d,i) => d.classList.toggle('active', i === current));
    counter.textContent = (current+1) + ' / ' + total;
    progress.style.width = ((current+1)/total*100) + '%';
  }

  function goTo(i){
    current = Math.max(0, Math.min(total-1, i));
    render();
  }
  function next(){ if(current < total-1){ current++; render(); } }
  function prev(){ if(current > 0){ current--; render(); } }

  document.getElementById('nextBtn').addEventListener('click', next);
  document.getElementById('prevBtn').addEventListener('click', prev);

  window.addEventListener('keydown', (e) => {
    if(['ArrowRight','ArrowDown','PageDown',' '].includes(e.key)){ e.preventDefault(); next(); }
    if(['ArrowLeft','ArrowUp','PageUp'].includes(e.key)){ e.preventDefault(); prev(); }
    if(e.key === 'Home'){ goTo(0); }
    if(e.key === 'End'){ goTo(total-1); }
  });

  // basic touch swipe support
  let touchX = null;
  window.addEventListener('touchstart', e => touchX = e.touches[0].clientX);
  window.addEventListener('touchend', e => {
    if(touchX === null) return;
    const dx = e.changedTouches[0].clientX - touchX;
    if(dx > 60) prev();
    if(dx < -60) next();
    touchX = null;
  });

  // mouse wheel navigation (throttled)
  let wheelLock = false;
  window.addEventListener('wheel', (e) => {
    if(wheelLock) return;
    if(Math.abs(e.deltaY) < 30) return;
    wheelLock = true;
    if(e.deltaY > 0) next(); else prev();
    setTimeout(() => wheelLock = false, 700);
  });

  render();
</script>
</body>
</html>
