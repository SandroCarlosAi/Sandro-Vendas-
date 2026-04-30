<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AquaMais — Máquina de Vendas</title>
<script src="https://cdn.jsdelivr.net/npm/chart.js@4.4.0/dist/chart.umd.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/xlsx@0.18.5/dist/xlsx.full.min.js"></script>
<style>
:root{--aqua:#0097a7;--wave:#1565c0;--coral:#e8521a;--gold:#c4870a;--dark:#f0f5f9;--darker:#e2edf5;--card:#ffffff;--border:rgba(0,130,150,0.2);--green:#00956a;--t1:#1e3445;--t2:#4a7090;--t3:#8aaabb}
*{margin:0;padding:0;box-sizing:border-box}
body{font-family:'Segoe UI',system-ui,sans-serif;background:var(--dark);color:var(--t1);display:flex;min-height:100vh}
.sidebar{width:230px;background:var(--darker);border-right:1px solid var(--border);display:flex;flex-direction:column;position:fixed;top:0;left:0;height:100vh;z-index:100;overflow-y:auto}
.sidebar-logo{padding:18px 16px;border-bottom:1px solid var(--border)}
.brand{font-size:19px;font-weight:800;color:var(--aqua)}
.sub{font-size:9px;color:var(--t3);letter-spacing:2px;text-transform:uppercase;margin-top:2px}
.nav-section{padding:10px 0}
.nav-label{font-size:9px;font-weight:700;letter-spacing:2px;text-transform:uppercase;color:var(--t3);padding:0 14px 6px}
.nav-item{display:flex;align-items:center;gap:10px;padding:9px 14px;cursor:pointer;font-size:13px;color:var(--t2);border-left:3px solid transparent;transition:.15s}
.nav-item:hover{background:rgba(0,130,150,0.08);color:var(--t1)}
.nav-item.active{background:rgba(0,130,150,0.13);color:var(--aqua);border-left-color:var(--aqua)}
.nav-badge{margin-left:auto;background:var(--coral);color:#fff;font-size:9px;font-weight:700;padding:2px 6px;border-radius:100px}
.sidebar-bottom{margin-top:auto;padding:14px;border-top:1px solid var(--border)}
.meta-box{background:rgba(0,130,150,0.07);border:1px solid var(--border);border-radius:10px;padding:12px}
.meta-box .lbl{font-size:10px;color:var(--t2);text-transform:uppercase;letter-spacing:1px;margin-bottom:4px}
.meta-box .val{font-size:22px;font-weight:800;color:var(--aqua)}
.prog{height:4px;background:rgba(0,0,0,0.1);border-radius:2px;margin-top:8px}
.prog-bar{height:4px;background:linear-gradient(90deg,var(--aqua),var(--wave));border-radius:2px;transition:.5s}
.main{margin-left:230px;flex:1;display:flex;flex-direction:column}
.topbar{background:#fff;border-bottom:1px solid var(--border);padding:12px 22px;display:flex;align-items:center;justify-content:space-between;position:sticky;top:0;z-index:50;box-shadow:0 1px 3px rgba(0,0,0,0.06)}
.topbar-title{font-size:15px;font-weight:700;color:var(--t1)}
.topbar-right{display:flex;align-items:center;gap:10px}
.btn{padding:7px 14px;border-radius:7px;border:none;cursor:pointer;font-size:12px;font-weight:600;transition:.15s;line-height:1}
.btn-primary{background:var(--aqua);color:#fff}
.btn-primary:hover{background:#00afc2}
.btn-outline{background:transparent;color:var(--aqua);border:1px solid var(--aqua)}
.btn-outline:hover{background:rgba(0,130,150,0.08)}
.btn-coral{background:var(--coral);color:#fff}
.btn-coral:hover{background:#f0622a}
.btn-danger{background:rgba(232,82,26,0.1);color:var(--coral);border:1px solid rgba(232,82,26,0.3)}
.btn-danger:hover{background:rgba(232,82,26,0.2)}
.btn-gold{background:rgba(196,135,10,0.1);color:var(--gold);border:1px solid rgba(196,135,10,0.3)}
.btn-green{background:rgba(0,149,106,0.1);color:var(--green);border:1px solid rgba(0,149,106,0.3)}
.btn-sm{padding:4px 10px;font-size:11px}
.live-badge{display:flex;align-items:center;gap:5px;background:rgba(0,149,106,0.1);border:1px solid var(--green);border-radius:100px;padding:4px 10px;font-size:11px;font-weight:600;color:var(--green)}
.live-badge span{width:5px;height:5px;background:var(--green);border-radius:50%;animation:pulse 1.5s infinite}
@keyframes pulse{0%,100%{opacity:1;transform:scale(1)}50%{opacity:.4;transform:scale(1.6)}}
.content{padding:20px;flex:1}
.page{display:none}.page.active{display:block}
.grid-2{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:14px;margin-bottom:16px}
.grid-3{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:14px;margin-bottom:16px}
.grid-4{display:grid;grid-template-columns:repeat(auto-fit,minmax(170px,1fr));gap:10px;margin-bottom:16px}
.card{background:var(--card);border:1px solid var(--border);border-radius:14px;padding:18px;box-shadow:0 1px 4px rgba(0,0,0,0.06)}
.card-header{display:flex;align-items:center;justify-content:space-between;margin-bottom:14px;gap:8px;flex-wrap:wrap}
.card-title{font-size:12px;font-weight:700;color:var(--t2);text-transform:uppercase;letter-spacing:.5px}
.kpi-card{background:var(--card);border:1px solid var(--border);border-radius:12px;padding:16px;position:relative;overflow:hidden;box-shadow:0 1px 4px rgba(0,0,0,0.07)}
.kpi-label{font-size:11px;color:var(--t2);text-transform:uppercase;letter-spacing:1px;margin-bottom:5px}
.kpi-val{font-size:28px;font-weight:800;line-height:1}
.kpi-sub{font-size:11px;color:var(--t2);margin-top:3px}
.kpi-trend{font-size:11px;font-weight:600;margin-top:6px}
.trend-up{color:var(--green)}.trend-ok{color:var(--gold)}
.kprog{height:3px;background:rgba(0,0,0,0.08);border-radius:2px;margin-top:8px}
.kprog-bar{height:3px;border-radius:2px;transition:.5s}
.kpi-edit-btn{position:absolute;top:10px;right:10px;background:rgba(0,130,150,0.1);border:1px solid var(--border);border-radius:5px;padding:3px 7px;cursor:pointer;font-size:11px;color:var(--aqua);transition:.15s;line-height:1}
.kpi-edit-btn:hover{background:rgba(0,130,150,0.2)}
.sec-tag{font-size:10px;font-weight:700;letter-spacing:2.5px;text-transform:uppercase;color:var(--aqua);margin-bottom:5px}
.sec-title{font-size:20px;font-weight:800;color:var(--t1)}
.sec-sub{font-size:13px;color:var(--t2);margin-top:3px}
.sec-header{margin-bottom:18px}
.funnel-bar{height:34px;border-radius:5px;display:flex;align-items:center;padding:0 12px;font-size:12px;font-weight:600;transition:.5s;margin-bottom:6px}
table{width:100%;border-collapse:collapse;font-size:13px}
th{text-align:left;padding:9px 12px;background:rgba(0,130,150,0.07);color:var(--aqua);font-weight:600;font-size:11px;letter-spacing:.5px;text-transform:uppercase;white-space:nowrap}
td{padding:10px 12px;border-bottom:1px solid rgba(0,0,0,0.05);color:var(--t1);vertical-align:middle}
tr:hover td{background:rgba(0,0,0,0.02)}
.table-wrap{overflow-x:auto}
.badge-s{padding:2px 9px;border-radius:100px;font-size:11px;font-weight:600;white-space:nowrap}
.s-novo{background:rgba(21,101,192,0.12);color:var(--wave)}
.s-quente{background:rgba(232,82,26,0.12);color:var(--coral)}
.s-abordagem{background:rgba(196,135,10,0.12);color:var(--gold)}
.s-fechado{background:rgba(0,149,106,0.12);color:var(--green)}
.s-perdido{background:rgba(100,100,100,0.1);color:#777}
.kanban{display:grid;grid-template-columns:repeat(5,1fr);gap:10px;min-width:860px}
.kcol{background:rgba(0,0,0,0.02);border:1px solid var(--border);border-radius:12px;padding:10px}
.kcol-hdr{display:flex;align-items:center;justify-content:space-between;margin-bottom:10px;padding-bottom:8px;border-bottom:1px solid var(--border)}
.kcol-title{font-size:11px;font-weight:700;text-transform:uppercase;letter-spacing:.5px}
.kcount{background:rgba(0,0,0,0.07);border-radius:100px;padding:1px 7px;font-size:11px;color:var(--t2)}
.kcard{background:#fff;border:1px solid var(--border);border-radius:9px;padding:10px;margin-bottom:7px;transition:.15s;box-shadow:0 1px 3px rgba(0,0,0,0.06)}
.kcard:hover{border-color:var(--aqua);box-shadow:0 2px 8px rgba(0,130,150,0.15)}
.kcard .kname{font-size:13px;font-weight:600;margin-bottom:3px;color:var(--t1)}
.kcard .kinfo{font-size:11px;color:var(--t2);line-height:1.5}
.kcard .ktel{font-size:12px;color:var(--aqua);margin-top:4px;font-weight:600}
.kcard .kactions{display:flex;gap:4px;margin-top:7px;flex-wrap:wrap}
input,select,textarea{background:#f5f9fc;border:1px solid var(--border);border-radius:7px;color:var(--t1);padding:8px 12px;font-size:13px;width:100%;outline:none;font-family:inherit;transition:.15s}
input:focus,select:focus,textarea:focus{border-color:var(--aqua);background:#fff;box-shadow:0 0 0 3px rgba(0,130,150,0.08)}
select option{background:#fff;color:var(--t1)}
label{font-size:11px;color:var(--t2);font-weight:600;margin-bottom:3px;display:block}
.fg{margin-bottom:12px}
.fr{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:12px}
.modal-overlay{position:fixed;inset:0;background:rgba(0,0,0,0.45);z-index:300;display:none;align-items:center;justify-content:center;padding:20px}
.modal-overlay.open{display:flex}
.modal{background:#fff;border:1px solid var(--border);border-radius:16px;padding:24px;width:100%;max-width:480px;max-height:90vh;overflow-y:auto;box-shadow:0 8px 32px rgba(0,0,0,0.14)}
.modal-lg{max-width:640px}
.modal-header{display:flex;align-items:center;justify-content:space-between;margin-bottom:18px}
.modal-title{font-size:17px;font-weight:800;color:var(--t1)}
.modal-close{cursor:pointer;background:none;border:none;color:var(--t2);font-size:18px;padding:2px 6px}
.modal-close:hover{color:var(--coral)}
.tab-row{display:flex;gap:2px;background:rgba(0,0,0,0.06);border-radius:8px;padding:3px;margin-bottom:18px}
.tab-btn{flex:1;padding:7px;border:none;background:none;cursor:pointer;border-radius:6px;font-size:12px;font-weight:600;color:var(--t2);transition:.15s}
.tab-btn.active{background:#fff;color:var(--aqua);box-shadow:0 1px 4px rgba(0,0,0,0.1)}
.ranking-item{display:flex;align-items:center;gap:10px;padding:10px 0;border-bottom:1px solid rgba(0,0,0,0.05)}
.ranking-item:last-child{border:none}
.rank-pos{width:26px;height:26px;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:11px;font-weight:800;flex-shrink:0}
.r1{background:rgba(196,135,10,0.15);color:var(--gold);border:1px solid var(--gold)}
.r2{background:rgba(160,160,160,0.12);color:#888;border:1px solid #bbb}
.r3{background:rgba(160,90,40,0.12);color:#b06030;border:1px solid #cd7f32}
.rn{background:rgba(0,0,0,0.05);color:var(--t2);border:1px solid var(--border)}
.script-card{background:var(--card);border:1px solid var(--border);border-radius:12px;margin-bottom:12px;overflow:hidden;box-shadow:0 1px 3px rgba(0,0,0,0.05)}
.script-hdr{display:flex;align-items:center;gap:10px;padding:14px 18px;border-bottom:1px solid var(--border);cursor:pointer}
.script-hdr .stitle{font-weight:700;font-size:14px;flex:1;color:var(--t1)}
.script-hdr .schan{font-size:11px;color:var(--t2);text-transform:uppercase;letter-spacing:1px}
.script-body{padding:18px;display:none}
.script-body.open{display:block}
.script-txt{background:rgba(0,130,150,0.04);border-left:3px solid var(--aqua);border-radius:0 9px 9px 0;padding:14px 18px;font-size:13px;color:var(--t1);line-height:1.8;font-style:italic;margin-bottom:10px;white-space:pre-wrap}
.copy-btn{display:inline-flex;align-items:center;gap:5px;background:rgba(0,130,150,0.08);border:1px solid var(--border);border-radius:7px;padding:7px 12px;cursor:pointer;font-size:11px;font-weight:600;color:var(--aqua);transition:.15s}
.copy-btn:hover{background:rgba(0,130,150,0.15)}
.plan-card{background:var(--card);border:1px solid var(--border);border-radius:14px;margin-bottom:12px;overflow:hidden;box-shadow:0 1px 3px rgba(0,0,0,0.05)}
.plan-hdr{display:flex;align-items:center;gap:12px;padding:16px 18px;cursor:pointer;border-bottom:1px solid var(--border);flex-wrap:wrap}
.plan-body{padding:18px;display:none}
.plan-body.open{display:block}
.ci{display:flex;align-items:flex-start;gap:10px;padding:8px 0;border-bottom:1px solid rgba(0,0,0,0.04);cursor:pointer}
.ci:last-child{border:none}
.cbox{width:17px;height:17px;border:2px solid var(--border);border-radius:4px;flex-shrink:0;display:flex;align-items:center;justify-content:center;transition:.15s;margin-top:2px;font-size:10px}
.cbox.chk{background:var(--green);border-color:var(--green);color:#fff}
.ci.done .ctext{text-decoration:line-through;color:var(--t3)}
.ctext{font-size:13px;color:var(--t1);line-height:1.5}
.tl{position:relative;padding-left:34px}
.tl::before{content:'';position:absolute;left:9px;top:0;bottom:0;width:2px;background:linear-gradient(180deg,var(--aqua),var(--coral))}
.tl-item{position:relative;margin-bottom:26px}
.tl-dot{position:absolute;left:-29px;top:4px;width:13px;height:13px;border-radius:50%;border:2px solid var(--aqua);background:var(--dark)}
.tl-dot.done{background:var(--green);border-color:var(--green)}
.tl-dot.active{background:var(--coral);border-color:var(--coral);box-shadow:0 0 0 4px rgba(232,82,26,0.15)}
.tl-week{font-size:10px;font-weight:700;letter-spacing:2px;text-transform:uppercase;color:var(--aqua);margin-bottom:3px}
.tl-title{font-weight:700;font-size:14px;margin-bottom:3px;color:var(--t1)}
.tl-desc{font-size:12px;color:var(--t2);line-height:1.6}
.alert-card{background:var(--card);border:1px solid var(--border);border-radius:12px;padding:16px;margin-bottom:10px;display:flex;gap:14px;align-items:flex-start;box-shadow:0 1px 3px rgba(0,0,0,0.05)}
.alert-card.ok{border-color:rgba(0,149,106,0.3);background:rgba(0,149,106,0.03)}
.alert-card.warn{border-color:rgba(196,135,10,0.35);background:rgba(196,135,10,0.03)}
.alert-card.danger{border-color:rgba(232,82,26,0.35);background:rgba(232,82,26,0.03)}
.pill{padding:3px 10px;border-radius:100px;font-size:10px;font-weight:700}
.pill-ok{background:rgba(0,149,106,0.12);color:var(--green);border:1px solid rgba(0,149,106,0.3)}
.pill-warn{background:rgba(196,135,10,0.12);color:var(--gold);border:1px solid rgba(196,135,10,0.3)}
.pill-danger{background:rgba(232,82,26,0.12);color:var(--coral);border:1px solid rgba(232,82,26,0.3)}
.ref-tier{background:var(--card);border:1px solid var(--border);border-radius:10px;padding:14px;text-align:center;box-shadow:0 1px 3px rgba(0,0,0,0.05)}
.tier-amt{font-size:26px;font-weight:800;color:var(--gold)}
.tier-nm{font-size:11px;color:var(--t2);text-transform:uppercase;letter-spacing:1px;margin:3px 0}
.tier-cd{font-size:10px;color:var(--t3)}
.chart-wrap{position:relative;height:210px}
.chart-wrap-lg{position:relative;height:280px}
::-webkit-scrollbar{width:4px;height:4px}
::-webkit-scrollbar-thumb{background:rgba(0,130,150,0.25);border-radius:2px}
.sep{height:1px;background:linear-gradient(90deg,transparent,var(--border),transparent);margin:18px 0}
.import-drop{border:2px dashed var(--border);border-radius:12px;padding:28px;text-align:center;cursor:pointer;transition:.15s;margin-bottom:12px;background:rgba(0,130,150,0.02)}
.import-drop:hover,.import-drop.drag{border-color:var(--aqua);background:rgba(0,130,150,0.05)}
.import-drop .di{font-size:32px;margin-bottom:8px}
.import-drop p{font-size:13px;color:var(--t2)}
.import-drop small{font-size:11px;color:var(--t3)}
.preview-table{max-height:200px;overflow-y:auto;margin:10px 0}
.preview-table table{font-size:11px}
.preview-table th{font-size:10px;padding:6px 8px}
.preview-table td{padding:5px 8px}
.swot-grid{display:grid;grid-template-columns:1fr 1fr;gap:14px;margin-bottom:20px}
.swot-quad{background:var(--card);border:1px solid var(--border);border-radius:14px;padding:18px;box-shadow:0 1px 3px rgba(0,0,0,0.05)}
.swot-quad-title{font-size:11px;font-weight:700;letter-spacing:2px;text-transform:uppercase;margin-bottom:14px;display:flex;align-items:center;gap:8px}
.swot-F .swot-quad-title{color:var(--green)}.swot-W .swot-quad-title{color:var(--coral)}
.swot-O .swot-quad-title{color:var(--aqua)}.swot-T .swot-quad-title{color:var(--gold)}
.swot-item{padding:10px 0;border-bottom:1px solid rgba(0,0,0,0.05)}
.swot-item:last-child{border:none}
.swot-item-hdr{display:flex;gap:10px;align-items:flex-start}
.swot-item-icon{font-size:18px;flex-shrink:0;margin-top:1px}
.swot-item-title{font-size:13px;font-weight:600;margin-bottom:2px;color:var(--t1)}
.swot-item-desc{font-size:12px;color:var(--t2);line-height:1.5}
.swot-plano-toggle{font-size:11px;font-weight:600;color:var(--aqua);cursor:pointer;margin-top:6px;display:inline-flex;align-items:center;gap:4px;background:rgba(0,130,150,0.07);border:1px solid var(--border);border-radius:5px;padding:3px 8px}
.swot-plano-toggle:hover{background:rgba(0,130,150,0.15)}
.swot-plano{display:none;margin-top:8px;background:rgba(0,130,150,0.04);border-left:3px solid var(--aqua);border-radius:0 8px 8px 0;padding:10px 14px}
.swot-plano.open{display:block}
.swot-plano ul{list-style:none;display:flex;flex-direction:column;gap:5px}
.swot-plano li{font-size:12px;color:var(--t1);line-height:1.5;display:flex;gap:6px}
.swot-plano li::before{content:'→';color:var(--aqua);flex-shrink:0}
.health-bar-wrap{background:var(--card);border:1px solid var(--border);border-radius:14px;padding:20px;margin-bottom:20px;box-shadow:0 1px 4px rgba(0,0,0,0.06)}
.conn-status{display:inline-flex;align-items:center;gap:6px;padding:4px 12px;border-radius:100px;font-size:12px;font-weight:600}
.conn-ok{background:rgba(0,149,106,0.1);color:var(--green);border:1px solid rgba(0,149,106,0.3)}
.conn-err{background:rgba(232,82,26,0.1);color:var(--coral);border:1px solid rgba(232,82,26,0.3)}
.conn-idle{background:rgba(0,0,0,0.06);color:var(--t2);border:1px solid var(--border)}
.conn-dot{width:7px;height:7px;border-radius:50%;background:currentColor}
.log-box{background:#f5f9fc;border:1px solid var(--border);border-radius:8px;padding:12px;font-size:11px;font-family:monospace;color:var(--t2);max-height:140px;overflow-y:auto;line-height:1.8}
@media print{.sidebar,.topbar,.btn,.swot-plano-toggle{display:none!important}.main{margin-left:0!important}.swot-plano{display:block!important}}
</style>
</head>
<body>

<aside class="sidebar">
  <div class="sidebar-logo">
    <div class="brand">🌊 AquaMais</div>
    <div class="sub">Máquina de Vendas V4</div>
  </div>
  <div class="nav-section">
    <div class="nav-label">Principal</div>
    <div class="nav-item active" onclick="go('dashboard',this)"><span>📊</span> Dashboard</div>
    <div class="nav-item" onclick="go('pipeline',this)"><span>🎯</span> Pipeline CRM <span class="nav-badge" id="badge-leads">0</span></div>
    <div class="nav-item" onclick="go('time',this)"><span>👥</span> Time de Vendas</div>
    <div class="nav-item" onclick="go('indicacoes',this)"><span>💰</span> Indicações PIX</div>
  </div>
  <div class="nav-section">
    <div class="nav-label">Execução</div>
    <div class="nav-item" onclick="go('metas',this)"><span>🎯</span> Metas</div>
    <div class="nav-item" onclick="go('planos',this)"><span>📋</span> 7 Planos de Ação</div>
    <div class="nav-item" onclick="go('scripts',this)"><span>📜</span> Scripts de Venda</div>
    <div class="nav-item" onclick="go('cronograma',this)"><span>📅</span> Cronograma 30d</div>
    <div class="nav-item" onclick="go('alertas',this)"><span>⚠️</span> Alertas <span class="nav-badge">3</span></div>
  </div>
  <div class="nav-section">
    <div class="nav-label">Relatórios</div>
    <div class="nav-item" onclick="go('swot',this)"><span>📊</span> Análise SWOT</div>
  </div>
  <div class="nav-section">
    <div class="nav-label">Integração</div>
    <div class="nav-item" onclick="go('conector',this)"><span>🔌</span> Conector API</div>
  </div>
  <div class="sidebar-bottom">
    <div class="meta-box">
      <div class="lbl">Meta do Mês</div>
      <div class="val" id="sb-val">0</div>
      <div style="font-size:11px;color:var(--t3);margin-top:2px">/ <span id="sb-meta">1000</span> cotas</div>
      <div class="prog"><div class="prog-bar" id="sb-bar" style="width:0%"></div></div>
    </div>
  </div>
</aside>

<div class="main">
<div class="topbar">
  <div class="topbar-title" id="topbar-title">Dashboard</div>
  <div class="topbar-right">
    <div class="live-badge"><span></span> Ao Vivo</div>
    <button class="btn btn-primary" onclick="openModal('m-lead')">+ Novo Lead</button>
  </div>
</div>
<div class="content">

<!-- ═══ DASHBOARD ═══ -->
<div class="page active" id="page-dashboard">
  <div class="sec-header">
    <div class="sec-tag">Visão Geral</div>
    <div class="sec-title">Máquina de 1.000 Vendas/Mês</div>
  </div>
  <div class="grid-4">
    <div class="kpi-card"><button class="kpi-edit-btn" onclick="openKpiEdit('vendas')" title="Editar manualmente">✏️ Editar</button><div class="kpi-label">Cotas Vendidas</div><div class="kpi-val" style="color:var(--aqua)" id="kpi-v">347</div><div class="kpi-sub" id="kpi-v-sub">Meta: 1.000/mês</div><div class="kpi-trend trend-up">↑ +23% vs semana anterior</div><div class="kprog"><div class="kprog-bar" id="kprog-v" style="background:var(--aqua)"></div></div></div>
    <div class="kpi-card"><button class="kpi-edit-btn" onclick="openKpiEdit('leads')" title="Editar manualmente">✏️ Editar</button><div class="kpi-label">Leads Captados</div><div class="kpi-val" style="color:var(--coral)" id="kpi-l">11.430</div><div class="kpi-sub" id="kpi-l-sub">Meta: 33.000/mês</div><div class="kpi-trend trend-up">↑ +18% vs semana anterior</div><div class="kprog"><div class="kprog-bar" id="kprog-l" style="background:var(--coral)"></div></div></div>
    <div class="kpi-card"><div class="kpi-label">Custo por Lead</div><div class="kpi-val" style="color:var(--gold)" id="kpi-cpl">R$11</div><div class="kpi-sub" id="kpi-cpl-sub">Meta: R$8–15</div><div class="kpi-trend trend-ok">✓ Dentro da meta</div><div class="kprog"><div class="kprog-bar" style="width:70%;background:var(--gold)"></div></div></div>
    <div class="kpi-card"><div class="kpi-label">Via Indicação</div><div class="kpi-val" style="color:var(--green)" id="kpi-ind">89</div><div class="kpi-sub" id="kpi-ind-sub">Meta: 300/mês</div><div class="kpi-trend trend-up">↑ +41% vs semana anterior</div><div class="kprog"><div class="kprog-bar" id="kprog-ind" style="background:var(--green)"></div></div></div>
  </div>
  <div class="grid-2">
    <div class="card">
      <div class="card-header"><div class="card-title">Funil de Conversão</div></div>
      <div id="funnel-v"></div>
    </div>
    <div class="card">
      <div class="card-header"><div class="card-title">Vendas Diárias — Últimos 14 dias</div></div>
      <div class="chart-wrap"><canvas id="c-vendas"></canvas></div>
    </div>
  </div>
  <div class="grid-2">
    <div class="card">
      <div class="card-header"><div class="card-title">Origem das Vendas</div></div>
      <div style="display:grid;grid-template-columns:1fr 1fr;gap:10px;align-items:center">
        <div class="chart-wrap" style="height:170px"><canvas id="c-canais"></canvas></div>
        <div id="canais-leg" style="font-size:12px;display:flex;flex-direction:column;gap:6px"></div>
      </div>
    </div>
    <div class="card">
      <div class="card-header"><div class="card-title">Top Indicadores</div></div>
      <div id="dash-ranking"></div>
    </div>
  </div>
  <div class="card">
    <div class="card-header"><div class="card-title">KPIs Semana Atual vs Meta</div></div>
    <div class="table-wrap"><table><thead><tr><th>KPI</th><th>Real Semana</th><th>Meta Semana</th><th>% Meta</th><th>Status</th></tr></thead><tbody id="kpi-table"></tbody></table></div>
  </div>
</div>

<!-- ═══ PIPELINE CRM ═══ -->
<div class="page" id="page-pipeline">
  <div class="sec-header">
    <div class="sec-tag">CRM</div>
    <div class="sec-title">Pipeline de Leads</div>
  </div>
  <div style="display:flex;gap:8px;margin-bottom:16px;flex-wrap:wrap">
    <button class="btn btn-primary" onclick="openModal('m-lead')">+ Novo Lead</button>
    <button class="btn btn-outline" onclick="openModal('m-import')">📥 Importar Excel/CSV</button>
    <input id="s-leads" type="text" placeholder="Buscar..." style="max-width:220px" oninput="renderKanban();renderLeadTable()">
    <select id="f-status" style="max-width:140px" onchange="renderKanban();renderLeadTable()">
      <option value="">Todos</option><option>Novo</option><option>Quente</option><option>Abordagem</option><option>Fechado</option><option>Perdido</option>
    </select>
  </div>
  <div class="tab-row">
    <button class="tab-btn active" onclick="setPipeTab('kanban',this)">🗂 Kanban</button>
    <button class="tab-btn" onclick="setPipeTab('lista',this)">📋 Lista</button>
  </div>
  <div id="pipe-kanban"><div style="overflow-x:auto"><div class="kanban" id="kanban"></div></div></div>
  <div id="pipe-lista" style="display:none">
    <div class="card"><div class="table-wrap"><table><thead><tr><th>Nome</th><th>Telefone</th><th>Origem</th><th>Status</th><th>Vendedor</th><th>Obs</th><th>Ações</th></tr></thead><tbody id="leads-table"></tbody></table></div></div>
  </div>
</div>

<!-- ═══ TIME DE VENDAS ═══ -->
<div class="page" id="page-time">
  <div class="sec-header">
    <div class="sec-tag">Equipe Comercial</div>
    <div class="sec-title">Gestão do Time</div>
  </div>
  <div class="tab-row">
    <button class="tab-btn active" onclick="setTimeTab('sdrs',this)">⚡ SDRs</button>
    <button class="tab-btn" onclick="setTimeTab('closers',this)">🏆 Closers</button>
    <button class="tab-btn" onclick="setTimeTab('ranking',this)">🥇 Ranking</button>
  </div>
  <div id="time-sdrs">
    <div class="card">
      <div class="card-header"><div class="card-title">SDRs Ativos</div><button class="btn btn-primary" onclick="openAddMembro('SDR')">+ Novo SDR</button></div>
      <div class="table-wrap"><table><thead><tr><th>Nome</th><th>Telefone</th><th>Abordagens/dia</th><th>Meta/dia</th><th>Taxa Conv.</th><th>% Meta</th><th>Ações</th></tr></thead><tbody id="sdr-table"></tbody></table></div>
    </div>
  </div>
  <div id="time-closers" style="display:none">
    <div class="card">
      <div class="card-header"><div class="card-title">Closers Ativos</div><button class="btn btn-primary" onclick="openAddMembro('Closer')">+ Novo Closer</button></div>
      <div class="table-wrap"><table><thead><tr><th>Nome</th><th>Telefone</th><th>Fechamentos</th><th>Meta mês</th><th>Taxa</th><th>% Meta</th><th>Ações</th></tr></thead><tbody id="closer-table"></tbody></table></div>
    </div>
  </div>
  <div id="time-ranking" style="display:none">
    <div class="grid-2">
      <div class="card">
        <div class="card-header"><div class="card-title">Ranking Geral</div></div>
        <div id="ranking-time"></div>
      </div>
      <div class="card">
        <div class="card-header"><div class="card-title">Performance por Vendedor</div></div>
        <div class="chart-wrap-lg"><canvas id="c-time"></canvas></div>
      </div>
    </div>
  </div>
</div>

<!-- ═══ INDICAÇÕES PIX ═══ -->
<div class="page" id="page-indicacoes">
  <div class="sec-header">
    <div class="sec-tag">Programa de Afiliados</div>
    <div class="sec-title">Indicações PIX</div>
  </div>
  <div class="grid-4" style="margin-bottom:16px">
    <div class="ref-tier"><div class="tier-amt">R$50</div><div class="tier-nm">Bronze</div><div class="tier-cd">1ª indicação</div></div>
    <div class="ref-tier"><div class="tier-amt">R$80</div><div class="tier-nm">Silver</div><div class="tier-cd">2ª a 5ª</div></div>
    <div class="ref-tier"><div class="tier-amt">R$120</div><div class="tier-nm">Gold</div><div class="tier-cd">6ª ou mais</div></div>
    <div class="ref-tier"><div class="tier-amt">R$500</div><div class="tier-nm">Platinum</div><div class="tier-cd">10+ no mês</div></div>
  </div>
  <div class="grid-4" style="margin-bottom:16px">
    <div class="kpi-card"><div class="kpi-label">Afiliados Ativos</div><div class="kpi-val" style="color:var(--aqua)" id="aff-ativos">0</div></div>
    <div class="kpi-card"><div class="kpi-label">Cotas via Indicação</div><div class="kpi-val" style="color:var(--green)" id="aff-cotas">0</div></div>
    <div class="kpi-card"><div class="kpi-label">PIX Pagos</div><div class="kpi-val" style="color:var(--gold)" id="aff-pix">R$0</div></div>
    <div class="kpi-card"><div class="kpi-label" style="color:var(--coral)">PIX Pendentes</div><div class="kpi-val" style="color:var(--coral)" id="aff-pend">R$0</div></div>
  </div>
  <div class="card">
    <div class="card-header"><div class="card-title">Todos os Afiliados</div><button class="btn btn-primary" onclick="openModal('m-afiliado')">+ Nova Indicação</button></div>
    <div class="table-wrap"><table><thead><tr><th>Nome</th><th>Cotas</th><th>Nível</th><th>PIX Valor</th><th>Status Pgto</th><th>Telefone</th><th>Ações</th></tr></thead><tbody id="aff-table"></tbody></table></div>
  </div>
</div>

<!-- ═══ METAS ═══ -->
<div class="page" id="page-metas">
  <div class="sec-header">
    <div class="sec-tag">Gestão de Metas</div>
    <div class="sec-title">Metas da Operação</div>
    <div class="sec-sub">Defina e acompanhe as metas de cada indicador</div>
  </div>
  <div style="display:flex;justify-content:flex-end;margin-bottom:14px">
    <button class="btn btn-primary" onclick="openModal('m-meta')">+ Nova Meta</button>
  </div>
  <div class="card">
    <div class="table-wrap"><table><thead><tr><th>Indicador</th><th>Meta Mensal</th><th>Meta Semanal</th><th>Real Atual</th><th>% Atingida</th><th>Cor</th><th>Ações</th></tr></thead><tbody id="metas-table"></tbody></table></div>
  </div>
  <div class="sep"></div>
  <div class="grid-2">
    <div class="card"><div class="card-header"><div class="card-title">Progresso das Metas</div></div><div class="chart-wrap-lg"><canvas id="c-metas"></canvas></div></div>
    <div class="card"><div class="card-header"><div class="card-title">% de Atingimento</div></div><div id="metas-prog-list"></div></div>
  </div>
</div>

<!-- ═══ PLANOS ═══ -->
<div class="page" id="page-planos">
  <div class="sec-header"><div class="sec-tag">Execução</div><div class="sec-title">7 Máquinas de Venda</div></div>
  <div class="grid-4" id="planos-kpis" style="margin-bottom:16px"></div>
  <div id="planos-list"></div>
</div>

<!-- ═══ SCRIPTS ═══ -->
<div class="page" id="page-scripts">
  <div class="sec-header">
    <div class="sec-tag">Biblioteca</div>
    <div class="sec-title">Scripts de Venda</div>
    <div class="sec-sub">Crie e edite scripts para cada canal e público</div>
  </div>
  <div style="display:flex;justify-content:flex-end;margin-bottom:14px">
    <button class="btn btn-primary" onclick="openNewScript()">+ Novo Script</button>
  </div>
  <div id="scripts-list"></div>
</div>

<!-- ═══ CRONOGRAMA ═══ -->
<div class="page" id="page-cronograma">
  <div class="sec-header"><div class="sec-tag">Plano 30 Dias</div><div class="sec-title">Semana a Semana: do Zero a 1.000</div></div>
  <div class="grid-2">
    <div class="card"><div class="card-header"><div class="card-title">Linha do Tempo</div></div><div class="tl" id="tl-list"></div></div>
    <div class="card"><div class="card-header"><div class="card-title">Real vs Meta por Semana</div></div><div class="chart-wrap-lg"><canvas id="c-crono"></canvas></div></div>
  </div>
</div>

<!-- ═══ ALERTAS ═══ -->
<div class="page" id="page-alertas">
  <div class="sec-header"><div class="sec-tag">Monitoramento</div><div class="sec-title">Alertas Estratégicos</div></div>
  <div id="alerts-list"></div>
</div>

<!-- ═══ SWOT ═══ -->
<div class="page" id="page-swot">
  <div class="sec-header">
    <div class="sec-tag">Análise Estratégica</div>
    <div class="sec-title">Relatório SWOT da Operação</div>
    <div class="sec-sub">Gerado automaticamente com base nos dados reais do app</div>
  </div>
  <div style="display:flex;gap:8px;margin-bottom:20px;flex-wrap:wrap;align-items:center">
    <button class="btn btn-primary" onclick="buildSWOT()">🔄 Gerar / Atualizar Relatório</button>
    <button class="btn btn-outline" onclick="window.print()">🖨️ Imprimir</button>
    <div id="swot-date" style="margin-left:auto;font-size:12px;color:var(--t3)"></div>
  </div>
  <div id="swot-health" style="display:none"></div>
  <div id="swot-content" style="display:none">
    <div class="swot-grid">
      <div class="swot-quad swot-F"><div class="swot-quad-title">💪 Forças — O que está funcionando</div><div id="sq-F"></div></div>
      <div class="swot-quad swot-W"><div class="swot-quad-title">⚠️ Fraquezas — O que precisa melhorar</div><div id="sq-W"></div></div>
      <div class="swot-quad swot-O"><div class="swot-quad-title">🚀 Oportunidades — O que pode ser explorado</div><div id="sq-O"></div></div>
      <div class="swot-quad swot-T"><div class="swot-quad-title">🚨 Ameaças — O que pode travar a operação</div><div id="sq-T"></div></div>
    </div>
    <div id="swot-action-plan"></div>
  </div>
  <div id="swot-placeholder" style="text-align:center;padding:60px 20px;color:var(--t3)">
    <div style="font-size:52px;margin-bottom:14px">📊</div>
    <div style="font-size:16px;font-weight:700;margin-bottom:6px;color:var(--t2)">Análise SWOT não gerada ainda</div>
    <div style="font-size:13px;margin-bottom:20px">Clique abaixo para analisar toda a operação automaticamente</div>
    <button class="btn btn-primary" onclick="buildSWOT()">🔄 Gerar Relatório Agora</button>
  </div>
</div>

<!-- ═══ CONECTOR API ═══ -->
<div class="page" id="page-conector">
  <div class="sec-header">
    <div class="sec-tag">Integração</div>
    <div class="sec-title">Conector de Dados</div>
    <div class="sec-sub">Conecte um sistema externo para alimentar os KPIs automaticamente</div>
  </div>
  <div class="grid-2" style="margin-bottom:16px">
    <div class="card">
      <div class="card-header"><div class="card-title">Status da Conexão</div><span id="conn-status-badge" class="conn-status conn-idle"><span class="conn-dot"></span>Não configurado</span></div>
      <div style="font-size:13px;color:var(--t2);margin-bottom:14px">Última sincronização: <strong id="conn-last-sync" style="color:var(--t1)">—</strong></div>
      <div style="display:flex;gap:8px;flex-wrap:wrap">
        <button class="btn btn-primary" onclick="connSync()">🔄 Sincronizar Agora</button>
        <button class="btn btn-outline" onclick="openModal_conector()">⚙️ Configurar</button>
        <button class="btn btn-outline" onclick="connTest()">🧪 Testar Conexão</button>
      </div>
      <div style="margin-top:14px">
        <label style="display:flex;align-items:center;gap:8px;cursor:pointer;font-size:13px;font-weight:600;color:var(--t1)">
          <input type="checkbox" id="conn-auto-toggle" onchange="toggleAutoSync(this.checked)" style="width:auto;accent-color:var(--aqua)">
          Sincronização automática
        </label>
        <div style="font-size:11px;color:var(--t3);margin-top:4px">Intervalo: <span id="conn-interval-display">—</span></div>
      </div>
    </div>
    <div class="card">
      <div class="card-header"><div class="card-title">Configuração Atual</div></div>
      <div id="conn-config-display" style="font-size:13px;color:var(--t2)">
        <div style="text-align:center;padding:20px;color:var(--t3)">Nenhuma configuração salva.<br>Clique em "Configurar" para começar.</div>
      </div>
    </div>
  </div>
  <div class="card">
    <div class="card-header"><div class="card-title">Log de Sincronização</div><button class="btn btn-outline btn-sm" onclick="clearConnLog()">Limpar</button></div>
    <div class="log-box" id="conn-log">Aguardando sincronização...</div>
  </div>
  <div class="card" style="margin-top:16px">
    <div class="card-header"><div class="card-title">Como funciona</div></div>
    <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:16px;font-size:13px">
      <div style="padding:14px;background:var(--dark);border-radius:10px;border:1px solid var(--border)"><div style="font-size:20px;margin-bottom:8px">1️⃣</div><strong style="color:var(--t1)">Configure o endpoint</strong><div style="color:var(--t2);margin-top:4px">Informe a URL da API do seu sistema (CRM, planilha, ERP).</div></div>
      <div style="padding:14px;background:var(--dark);border-radius:10px;border:1px solid var(--border)"><div style="font-size:20px;margin-bottom:8px">2️⃣</div><strong style="color:var(--t1)">Mapeie os campos</strong><div style="color:var(--t2);margin-top:4px">Defina qual campo da API corresponde a Cotas e Leads (ex: <code>data.sales</code>).</div></div>
      <div style="padding:14px;background:var(--dark);border-radius:10px;border:1px solid var(--border)"><div style="font-size:20px;margin-bottom:8px">3️⃣</div><strong style="color:var(--t1)">Sincronize</strong><div style="color:var(--t2);margin-top:4px">Manualmente ou ative a sincronização automática por intervalo.</div></div>
      <div style="padding:14px;background:var(--dark);border-radius:10px;border:1px solid var(--border)"><div style="font-size:20px;margin-bottom:8px">4️⃣</div><strong style="color:var(--t1)">Dados atualizados</strong><div style="color:var(--t2);margin-top:4px">O Dashboard reflete os valores do sistema externo em tempo real.</div></div>
    </div>
  </div>
</div>

</div><!-- /content -->
</div><!-- /main -->

<!-- ═══ MODALS ═══ -->

<!-- KPI Quick Edit -->
<div class="modal-overlay" id="m-kpi-edit">
<div class="modal">
  <div class="modal-header"><div class="modal-title" id="m-kpi-edit-title">✏️ Editar KPI</div><button class="modal-close" onclick="closeModal('m-kpi-edit')">✕</button></div>
  <input type="hidden" id="kpi-edit-key">
  <div class="fg"><label id="kpi-edit-label">Valor Atual</label><input type="number" id="kpi-edit-val" placeholder="0" min="0"></div>
  <div class="fg"><label>Meta Mensal</label><input type="number" id="kpi-edit-meta" placeholder="0" min="0"></div>
  <div style="background:var(--dark);border-radius:8px;padding:10px;font-size:12px;color:var(--t2);margin-bottom:14px">
    💡 A edição manual sobrescreve o valor atual. O sistema parará o incremento automático por 5 minutos após salvar.
  </div>
  <div style="display:flex;gap:8px">
    <button class="btn btn-primary" style="flex:1" onclick="saveKpiEdit()">Salvar</button>
    <button class="btn btn-outline" onclick="closeModal('m-kpi-edit')">Cancelar</button>
  </div>
</div>
</div>

<!-- Conector Config -->
<div class="modal-overlay" id="m-conector">
<div class="modal modal-lg">
  <div class="modal-header"><div class="modal-title">⚙️ Configurar Conector</div><button class="modal-close" onclick="closeModal('m-conector')">✕</button></div>
  <div class="fg"><label>URL do Endpoint (GET)</label><input id="conn-url" placeholder="https://api.seusis tema.com/vendas/resumo" type="url"></div>
  <div class="fr">
    <div class="fg"><label>Chave de API (Authorization)</label><input id="conn-apikey" placeholder="Bearer seu-token-aqui" type="password"></div>
    <div class="fg"><label>Intervalo Auto-Sync</label>
      <select id="conn-interval">
        <option value="0">Desativado</option>
        <option value="60">1 minuto</option>
        <option value="300">5 minutos</option>
        <option value="600">10 minutos</option>
        <option value="1800">30 minutos</option>
        <option value="3600">1 hora</option>
      </select>
    </div>
  </div>
  <div style="margin-bottom:14px"><div class="card-title" style="margin-bottom:10px">Mapeamento de Campos (caminho no JSON da resposta)</div>
    <div class="fr">
      <div class="fg"><label>Cotas Vendidas</label><input id="conn-map-cotas" placeholder="data.sales_count"></div>
      <div class="fg"><label>Leads Captados</label><input id="conn-map-leads" placeholder="data.leads_total"></div>
    </div>
    <div class="fr">
      <div class="fg"><label>Cotas via Indicação (opcional)</label><input id="conn-map-ind" placeholder="data.referrals"></div>
      <div class="fg"><label>Leads Qualificados (opcional)</label><input id="conn-map-qlf" placeholder="data.qualified_leads"></div>
    </div>
  </div>
  <div style="background:var(--dark);border-radius:8px;padding:10px;font-size:12px;color:var(--t2);margin-bottom:14px">
    <strong>Exemplo de resposta esperada:</strong><br>
    <code style="color:var(--aqua)">{"data":{"sales_count":347,"leads_total":11430,"referrals":89}}</code><br>
    Use notação de ponto para campos aninhados: <code style="color:var(--aqua)">data.sales_count</code>
  </div>
  <div style="display:flex;gap:8px">
    <button class="btn btn-primary" style="flex:1" onclick="saveConnConfig()">Salvar Configuração</button>
    <button class="btn btn-outline" onclick="connTest()">🧪 Testar</button>
    <button class="btn btn-outline" onclick="closeModal('m-conector')">Cancelar</button>
  </div>
</div>
</div>

<!-- Lead -->
<div class="modal-overlay" id="m-lead">
<div class="modal">
  <div class="modal-header"><div class="modal-title" id="m-lead-title">+ Novo Lead</div><button class="modal-close" onclick="closeModal('m-lead')">✕</button></div>
  <input type="hidden" id="lead-edit-id">
  <div class="fr"><div class="fg"><label>Nome</label><input id="l-nome" placeholder="Nome completo"></div><div class="fg"><label>Telefone (WhatsApp)</label><input id="l-tel" placeholder="(31) 99999-9999"></div></div>
  <div class="fr"><div class="fg"><label>Origem</label><select id="l-origem"><option>Meta Ads</option><option>Google Ads</option><option>Indicação</option><option>Instagram</option><option>Live</option><option>Evento</option><option>Orgânico</option><option>B2B</option></select></div><div class="fg"><label>Status</label><select id="l-status"><option>Novo</option><option>Quente</option><option>Abordagem</option><option>Fechado</option><option>Perdido</option></select></div></div>
  <div class="fr"><div class="fg"><label>Vendedor</label><select id="l-vend"></select></div><div class="fg"><label>Data</label><input type="date" id="l-data"></div></div>
  <div class="fg"><label>Observação</label><textarea id="l-obs" rows="2" placeholder="Interesse, objeções..."></textarea></div>
  <div style="display:flex;gap:8px;margin-top:8px">
    <button class="btn btn-primary" style="flex:1" onclick="saveLead()">Salvar</button>
    <button class="btn btn-outline" onclick="closeModal('m-lead')">Cancelar</button>
  </div>
</div>
</div>

<!-- Importar Leads -->
<div class="modal-overlay" id="m-import">
<div class="modal modal-lg">
  <div class="modal-header"><div class="modal-title">📥 Importar Leads — Excel / CSV</div><button class="modal-close" onclick="closeModal('m-import')">✕</button></div>
  <div class="import-drop" id="drop-zone" onclick="document.getElementById('file-import').click()" ondragover="ev.preventDefault();this.classList.add('drag')" ondragleave="this.classList.remove('drag')" ondrop="handleDrop(event)">
    <div class="di">📂</div>
    <p>Clique ou arraste o arquivo aqui</p>
    <small>Suporta .xlsx, .xls, .csv — Colunas: nome, telefone, origem, status</small>
  </div>
  <input type="file" id="file-import" accept=".xlsx,.xls,.csv" style="display:none" onchange="handleFileImport(this)">
  <div id="import-preview" style="display:none">
    <p style="font-size:13px;color:var(--t2);margin-bottom:8px">Prévia (<span id="preview-count">0</span> leads detectados):</p>
    <div class="preview-table" id="preview-table-wrap"></div>
    <div class="fg">
      <label>Status padrão (se não detectado na planilha)</label>
      <select id="import-default-status"><option>Novo</option><option>Quente</option><option>Abordagem</option></select>
    </div>
  </div>
  <div style="display:flex;gap:8px;margin-top:10px">
    <button class="btn btn-primary" style="flex:1" onclick="confirmImport()" id="btn-import-confirm" disabled>Importar Leads</button>
    <button class="btn btn-outline" onclick="closeModal('m-import')">Cancelar</button>
  </div>
</div>
</div>

<!-- Membro Time -->
<div class="modal-overlay" id="m-membro">
<div class="modal">
  <div class="modal-header"><div class="modal-title" id="m-membro-title">+ Novo SDR</div><button class="modal-close" onclick="closeModal('m-membro')">✕</button></div>
  <input type="hidden" id="membro-edit-id">
  <input type="hidden" id="membro-tipo">
  <div class="fr"><div class="fg"><label>Nome</label><input id="mb-nome" placeholder="Nome completo"></div><div class="fg"><label>Telefone</label><input id="mb-tel" placeholder="(31) 99999-0000"></div></div>
  <div class="fr"><div class="fg"><label>Abordagens/Fechamentos por dia</label><input id="mb-meta-d" type="number" placeholder="100"></div><div class="fg"><label>Meta Mensal (cotas)</label><input id="mb-meta-m" type="number" placeholder="50"></div></div>
  <div class="fr"><div class="fg"><label>Taxa de Conversão (%)</label><input id="mb-taxa" type="number" placeholder="28"></div><div class="fg"><label>Atividade Atual (hoje)</label><input id="mb-atual" type="number" placeholder="0"></div></div>
  <div style="display:flex;gap:8px;margin-top:8px">
    <button class="btn btn-primary" style="flex:1" onclick="saveMembro()">Salvar</button>
    <button class="btn btn-outline" onclick="closeModal('m-membro')">Cancelar</button>
  </div>
</div>
</div>

<!-- Afiliado -->
<div class="modal-overlay" id="m-afiliado">
<div class="modal">
  <div class="modal-header"><div class="modal-title" id="m-aff-title">+ Nova Indicação</div><button class="modal-close" onclick="closeModal('m-afiliado')">✕</button></div>
  <input type="hidden" id="aff-edit-id">
  <div class="fr"><div class="fg"><label>Nome do Sócio</label><input id="af-nome" placeholder="Nome completo"></div><div class="fg"><label>Telefone</label><input id="af-tel" placeholder="(31) 99999-0000"></div></div>
  <div class="fr"><div class="fg"><label>Cotas Indicadas</label><input id="af-cotas" type="number" placeholder="1"></div><div class="fg"><label>Nível</label><select id="af-nivel"><option>Bronze</option><option>Silver</option><option>Gold</option><option>Platinum</option></select></div></div>
  <div class="fr"><div class="fg"><label>Valor PIX (R$)</label><input id="af-pix" type="number" placeholder="50"></div><div class="fg"><label>Status do Pagamento</label><select id="af-status"><option value="pago">Pago ✅</option><option value="pendente">Pendente ⏳</option></select></div></div>
  <div style="display:flex;gap:8px;margin-top:8px">
    <button class="btn btn-primary" style="flex:1" onclick="saveAfiliado()">Salvar</button>
    <button class="btn btn-outline" onclick="closeModal('m-afiliado')">Cancelar</button>
  </div>
</div>
</div>

<!-- Script -->
<div class="modal-overlay" id="m-script">
<div class="modal modal-lg">
  <div class="modal-header"><div class="modal-title" id="m-script-title">+ Novo Script</div><button class="modal-close" onclick="closeModal('m-script')">✕</button></div>
  <input type="hidden" id="script-edit-id">
  <div class="fr">
    <div class="fg"><label>Emoji / Ícone</label><input id="sc-emoji" placeholder="📱" style="max-width:80px"></div>
    <div class="fg"><label>Canal / Público</label><input id="sc-canal" placeholder="Ex: WhatsApp — B2B Empresas"></div>
  </div>
  <div class="fg"><label>Título do Script</label><input id="sc-titulo" placeholder="Ex: Abordagem para RH de Empresas"></div>
  <div class="fg"><label>Texto do Script</label><textarea id="sc-txt" rows="10" placeholder="Escreva aqui o script completo. Use [nome], [empresa], etc. como variáveis..."></textarea></div>
  <div style="display:flex;gap:8px;margin-top:8px">
    <button class="btn btn-primary" style="flex:1" onclick="saveScript()">Salvar Script</button>
    <button class="btn btn-outline" onclick="closeModal('m-script')">Cancelar</button>
  </div>
</div>
</div>

<!-- Meta -->
<div class="modal-overlay" id="m-meta">
<div class="modal">
  <div class="modal-header"><div class="modal-title" id="m-meta-title">+ Nova Meta</div><button class="modal-close" onclick="closeModal('m-meta')">✕</button></div>
  <input type="hidden" id="meta-edit-id">
  <div class="fg"><label>Nome do Indicador</label><input id="mt-nome" placeholder="Ex: Cotas Vendidas"></div>
  <div class="fr"><div class="fg"><label>Meta Mensal</label><input id="mt-mensal" type="number" placeholder="1000"></div><div class="fg"><label>Meta Semanal</label><input id="mt-semanal" type="number" placeholder="250"></div></div>
  <div class="fr"><div class="fg"><label>Real Atual</label><input id="mt-real" type="number" placeholder="0"></div><div class="fg"><label>Cor</label><select id="mt-cor"><option value="aqua">Azul (aqua)</option><option value="coral">Coral</option><option value="gold">Dourado</option><option value="green">Verde</option><option value="wave">Azul escuro</option></select></div></div>
  <div style="display:flex;gap:8px;margin-top:8px">
    <button class="btn btn-primary" style="flex:1" onclick="saveMeta()">Salvar</button>
    <button class="btn btn-outline" onclick="closeModal('m-meta')">Cancelar</button>
  </div>
</div>
</div>

<script>
// ─── STORAGE ───────────────────────────────────────────
const SK = 'aquamais_v2';
function load(){try{return JSON.parse(localStorage.getItem(SK))||{};}catch{return {};}}
function save(){localStorage.setItem(SK,JSON.stringify(S));}
let S = load();

// ─── DEFAULT STATE ──────────────────────────────────────
if(!S.nextId) S.nextId=20;
if(!S.leads) S.leads=[
  {id:1,nome:'Roberto Alves',tel:'(31)98765-4321',origem:'Meta Ads',status:'Quente',vendedor:'Carlos Silva',data:'2026-04-28',obs:'Perguntou sobre clube parceiro'},
  {id:2,nome:'Fernanda Lima',tel:'(31)99876-5432',origem:'Indicação',status:'Abordagem',vendedor:'Marina Torres',data:'2026-04-27',obs:'Indicada pela sócia #47'},
  {id:3,nome:'Marcos Souza',tel:'(31)97654-3210',origem:'Live',status:'Fechado',vendedor:'Rafael Nobre',data:'2026-04-26',obs:'Comprou na live de domingo'},
  {id:4,nome:'Ana Costa',tel:'(31)96543-2109',origem:'Google Ads',status:'Novo',vendedor:'Paulo Mendes',data:'2026-04-28',obs:''},
  {id:5,nome:'Diego Santos',tel:'(31)95432-1098',origem:'Instagram',status:'Perdido',vendedor:'Juliana Costa',data:'2026-04-25',obs:'Quer esperar inaugurar'},
  {id:6,nome:'Patrícia Rocha',tel:'(31)94321-0987',origem:'Evento',status:'Quente',vendedor:'Carlos Silva',data:'2026-04-28',obs:'Esteve na Noite do Fundador'},
  {id:7,nome:'Eduardo Ferreira',tel:'(31)93210-9876',origem:'Meta Ads',status:'Abordagem',vendedor:'Marina Torres',data:'2026-04-27',obs:'Pediu mais infos sobre lote'},
  {id:8,nome:'Camila Nunes',tel:'(31)92109-8765',origem:'Indicação',status:'Fechado',vendedor:'Rafael Nobre',data:'2026-04-26',obs:'Indicou 2 amigos'},
];
if(!S.sdrs) S.sdrs=[
  {id:1,nome:'Carlos Silva',tel:'(31)99100-1001',metaDia:100,metaMes:0,taxa:29.8,atual:94},
  {id:2,nome:'Marina Torres',tel:'(31)99100-1002',metaDia:100,metaMes:0,taxa:27.6,atual:87},
  {id:3,nome:'Paulo Mendes',tel:'(31)99100-1003',metaDia:100,metaMes:0,taxa:30.4,atual:102},
  {id:4,nome:'Juliana Costa',tel:'(31)99100-1004',metaDia:100,metaMes:0,taxa:26.9,atual:78},
  {id:5,nome:'Rafael Nobre',tel:'(31)99100-1005',metaDia:100,metaMes:0,taxa:29.7,atual:91},
];
if(!S.closers) S.closers=[
  {id:1,nome:'Ricardo Vaz',tel:'(31)99200-2001',metaDia:10,metaMes:50,taxa:23.7,atual:9},
  {id:2,nome:'Simone Dias',tel:'(31)99200-2002',metaDia:8,metaMes:50,taxa:21.9,atual:7},
  {id:3,nome:'Henrique Luz',tel:'(31)99200-2003',metaDia:12,metaMes:60,taxa:24.4,atual:10},
];
if(!S.afiliados) S.afiliados=[
  {id:1,nome:'Gilberto Costa',tel:'(31)98100-1111',cotas:14,nivel:'Platinum',pix:1180,status:'pago'},
  {id:2,nome:'Sandra Oliveira',tel:'(31)98100-2222',cotas:11,nivel:'Platinum',pix:920,status:'pago'},
  {id:3,nome:'Marcos Freitas',tel:'(31)98100-3333',cotas:9,nivel:'Gold',pix:880,status:'pago'},
  {id:4,nome:'Carla Vieira',tel:'(31)98100-4444',cotas:7,nivel:'Gold',pix:600,status:'pendente'},
  {id:5,nome:'João Batista',tel:'(31)98100-5555',cotas:6,nivel:'Gold',pix:480,status:'pendente'},
];
if(!S.metas) S.metas=[
  {id:1,nome:'Cotas Vendidas',mensal:1000,semanal:250,real:347,cor:'aqua'},
  {id:2,nome:'Leads Captados',mensal:33000,semanal:8250,real:11430,cor:'coral'},
  {id:3,nome:'Cotas via Indicação',mensal:300,semanal:75,real:89,cor:'green'},
  {id:4,nome:'Leads Qualificados',mensal:16000,semanal:4000,real:5800,cor:'wave'},
  {id:5,nome:'PIX de Indicação pagos',mensal:300,semanal:70,real:89,cor:'gold'},
];
if(!S.planos) S.planos={};
if(!S.scripts) S.scripts=[
  {id:1,e:'📱',c:'WhatsApp — SDR',t:'Primeiro Contato',txt:`"Oi [nome]! Aqui é o [nome] do AquaMais 🌊 Vi que você se interessou em conhecer o projeto.\n\nVocê sabia que o AquaMais será o maior parque aquático de MG — na sua região, a 30 min de BH?\n\nHoje a gente tem uma condição especial de fundador: você garante a cota pagando só R$10 na primeira parcela, e já pode usar clubes parceiros na sua cidade enquanto o parque fica pronto.\n\nPosso te mandar o vídeo completo do projeto e os detalhes da oferta? É rápido 🙏"`},
  {id:2,e:'📞',c:'Ligação — Closer',t:'Objeção: "Ainda não inaugurou"',txt:`"Entendo sua pergunta — faz todo sentido. Mas deixa eu te mostrar uma perspectiva diferente: foi exatamente por não ter inaugurado ainda que você tem acesso ao menor preço que o AquaMais vai ter na história.\n\nQuem comprou apartamento na planta pagou menos. Os sócios que garantiram hoje já estão usando os clubes parceiros — então o benefício é REAL agora.\n\nE quando o parque abrir em 2026, você vai estar lá como fundador, com área VIP, sem pagar preço de balcão.\n\nQual seria o melhor dia para a sua família aproveitar o clube parceiro mais próximo essa semana?"`},
  {id:3,e:'💰',c:'WhatsApp — Sócio',t:'Script de Indicação para Sócios',txt:`"Ei [nome]! Acabei de garantir minha cota de fundador no AquaMais — aquele parque aquático que vai ser o Copacabana de Minas aqui em Betim! 🏝️\n\nEntrei por R$10 na primeira parcela e já recebi acesso ao clube aqui perto. Quando o parque abrir, tenho área VIP garantida.\n\nSe você usar meu link pra entrar hoje, eu recebo um PIX e você garante o mesmo preço que eu paguei (amanhã já sobe de lote). Aqui está: [LINK]\n\nQualquer dúvida, fala comigo! 🌊"`},
  {id:4,e:'🔥',c:'WhatsApp — Nutrição Dia 2',t:'Urgência de Lote',txt:`"⚠️ [nome], AVISO IMPORTANTE:\n\nO lote atual tem apenas 120 cotas restantes. Quando esgotar, o próximo começa em R$347/mês — uma diferença de R$50 todo mês.\n\nIsso significa que quem entrar no próximo lote vai pagar R$600 a mais por ano. Por 5 anos = R$3.000 de diferença só por esperar.\n\nVocê ainda pode garantir o preço atual 👇\n[LINK DA OFERTA]"`},
  {id:5,e:'🏊',c:'WhatsApp — Nutrição Dia 3',t:'Benefício Imediato (Clube Parceiro)',txt:`"[nome], uma coisa que pouca gente sabe:\n\nComo Platinum do AquaMais, você já pode usar os clubes parceiros AGORA mesmo antes de o parque abrir! 🏊\n\nSão 5 clubes aquáticos na região de BH disponíveis pra você, sua família e seus filhos aproveitarem ainda esse fim de semana.\n\nQuer saber quais clubes ficam perto da sua casa? Me manda seu bairro 📍"`},
  {id:6,e:'🎯',c:'Ligação — Closer',t:'Fechamento com Urgência',txt:`"[nome], vou ser direto porque só tenho autorização pra isso agora.\n\nConsigo garantir o preço do lote anterior para você — que está R$50 menor do que o atual.\n\nPreciso só de uma confirmação agora. O pagamento é de R$10 hoje, o restante em parcelas que cabem no seu bolso.\n\nVocê prefere pagar pelo link ou gero o Pix na hora?"`},
  {id:7,e:'🤝',c:'E-mail / Apresentação — B2B',t:'Script Corporativo (RH e Empresas)',txt:`"Olá [Nome do RH/Diretor],\n\nMeu nome é [seu nome] e represento o AquaMais — o maior parque aquático em construção em Minas Gerais, a 30 minutos de BH.\n\nEstamos lançando um programa exclusivo para empresas parceiras: o Benefício Corporativo AquaMais.\n\n✅ O que sua empresa ganha:\n• Cotas Platinum VIP para seus colaboradores com preço de fundador (condição especial para grupos)\n• Acesso imediato a clubes aquáticos parceiros na região — benefício ativo ainda hoje\n• Desconto progressivo: 20+ cotas = preço do lote anterior garantido\n• Área VIP corporativa reservada para o dia da inauguração (2026)\n\n📊 Exemplo prático:\n• Empresa com 50 colaboradores → R$297/mês por cota (vs R$397 no preço de varejo)\n• 50 cotas = economia de R$5.000/mês na folha de benefícios vs clubes convencionais\n\n🎯 Próximos passos:\nPosso apresentar o projeto em uma reunião de 30 minutos, na sua empresa ou online. Sem compromisso.\n\nQuando teria 30 minutos esta semana?\n\nAtt,\n[Seu nome] | AquaMais Parque\n[telefone] | [link de calendário]"`},
];
let importRows=[];

// ─── CORES ─────────────────────────────────────────────
const COLORS={aqua:'#00c9d4',coral:'#ff6b35',gold:'#f0a500',green:'#00d084',wave:'#1e88e5'};

// ─── NAVIGATION ────────────────────────────────────────
function go(id,el){
  document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
  document.querySelectorAll('.nav-item').forEach(n=>n.classList.remove('active'));
  document.getElementById('page-'+id).classList.add('active');
  el.classList.add('active');
  const titles={dashboard:'Dashboard',pipeline:'Pipeline CRM',time:'Time de Vendas',indicacoes:'Indicações PIX',metas:'Metas',planos:'7 Planos de Ação',scripts:'Scripts de Venda',cronograma:'Cronograma 30d',alertas:'Alertas',swot:'Análise SWOT',conector:'Conector API'};
  document.getElementById('topbar-title').textContent=titles[id]||id;
  if(id==='pipeline'){renderKanban();renderLeadTable();}
  if(id==='time'){renderSDR();renderCloser();renderTimeRanking();}
  if(id==='indicacoes')renderAfiliados();
  if(id==='metas'){renderMetas();setTimeout(renderMetasChart,100);}
  if(id==='planos')renderPlanos();
  if(id==='scripts')renderScripts();
  if(id==='cronograma')setTimeout(renderCrono,100);
  if(id==='alertas')renderAlertas();
  if(id==='conector'){renderConnConfig();}
}

// ─── MODALS ────────────────────────────────────────────
function openModal(id){document.getElementById(id).classList.add('open');}
function closeModal(id){document.getElementById(id).classList.remove('open');}
document.querySelectorAll('.modal-overlay').forEach(m=>m.addEventListener('click',e=>{if(e.target===m)m.classList.remove('open');}));

// ─── SIDEBAR UPDATE ────────────────────────────────────
function updateSidebar(){
  const metaCotas=S.metas.find(m=>m.nome==='Cotas Vendidas');
  const meta=metaCotas?metaCotas.mensal:1000;
  const real=metaCotas?metaCotas.real:347;
  const extras=S.leads.filter(l=>l.status==='Fechado').length;
  const total=real+extras;
  document.getElementById('sb-val').textContent=total;
  document.getElementById('sb-meta').textContent=meta;
  document.getElementById('sb-bar').style.width=Math.min(100,total/meta*100)+'%';
  document.getElementById('badge-leads').textContent=S.leads.filter(l=>l.status==='Novo'||l.status==='Quente').length;
}

// ─── VENDEDOR SELECT ───────────────────────────────────
function populateVendedorSelect(){
  const sel=document.getElementById('l-vend');
  sel.innerHTML=[...S.sdrs,...S.closers].map(v=>`<option>${v.nome}</option>`).join('');
}

// ─── LEADS ─────────────────────────────────────────────
function openEditLead(id){
  const l=S.leads.find(x=>x.id===id);if(!l)return;
  document.getElementById('m-lead-title').textContent='✏️ Editar Lead';
  document.getElementById('lead-edit-id').value=id;
  document.getElementById('l-nome').value=l.nome;
  document.getElementById('l-tel').value=l.tel||'';
  document.getElementById('l-obs').value=l.obs||'';
  document.getElementById('l-data').value=l.data||'';
  populateVendedorSelect();
  document.getElementById('l-origem').value=l.origem||'Meta Ads';
  document.getElementById('l-status').value=l.status||'Novo';
  setTimeout(()=>{try{document.getElementById('l-vend').value=l.vendedor;}catch(e){}},50);
  openModal('m-lead');
}
function openNewLead(){
  document.getElementById('m-lead-title').textContent='+ Novo Lead';
  document.getElementById('lead-edit-id').value='';
  document.getElementById('l-nome').value='';document.getElementById('l-tel').value='';
  document.getElementById('l-obs').value='';document.getElementById('l-data').value=new Date().toISOString().split('T')[0];
  populateVendedorSelect();openModal('m-lead');
}
function saveLead(){
  const nome=document.getElementById('l-nome').value.trim();if(!nome){alert('Informe o nome!');return;}
  const editId=parseInt(document.getElementById('lead-edit-id').value)||0;
  const obj={nome,tel:document.getElementById('l-tel').value,origem:document.getElementById('l-origem').value,status:document.getElementById('l-status').value,vendedor:document.getElementById('l-vend').value,data:document.getElementById('l-data').value,obs:document.getElementById('l-obs').value};
  if(editId){Object.assign(S.leads.find(x=>x.id===editId),obj);}
  else{obj.id=S.nextId++;S.leads.push(obj);}
  save();closeModal('m-lead');updateSidebar();renderKanban();renderLeadTable();
}
function deleteLead(id){if(!confirm('Excluir este lead?'))return;S.leads=S.leads.filter(x=>x.id!==id);save();updateSidebar();renderKanban();renderLeadTable();}
function setLeadStatus(id,s){const l=S.leads.find(x=>x.id===id);if(l){l.status=s;save();updateSidebar();renderKanban();renderLeadTable();}}

const SC={Novo:'s-novo',Quente:'s-quente',Abordagem:'s-abordagem',Fechado:'s-fechado',Perdido:'s-perdido'};
const CC={Novo:'var(--wave)',Quente:'var(--coral)',Abordagem:'var(--gold)',Fechado:'var(--green)',Perdido:'#555'};

function filteredLeads(){
  const s=(document.getElementById('s-leads')||{}).value||'';
  const f=(document.getElementById('f-status')||{}).value||'';
  return S.leads.filter(l=>(!s||l.nome.toLowerCase().includes(s.toLowerCase())||( l.tel&&l.tel.includes(s)))&&(!f||l.status===f));
}

function renderKanban(){
  const cols=['Novo','Quente','Abordagem','Fechado','Perdido'];
  const leads=filteredLeads();
  document.getElementById('kanban').innerHTML=cols.map(col=>{
    const items=leads.filter(l=>l.status===col);
    return`<div class="kcol">
      <div class="kcol-hdr"><div class="kcol-title" style="color:${CC[col]}">${col}</div><div class="kcount">${items.length}</div></div>
      ${items.map(l=>`<div class="kcard">
        <div class="kname">${l.nome}</div>
        <div class="kinfo">${l.origem} · ${l.data||''}</div>
        <div class="kinfo">${l.vendedor||''}</div>
        ${l.tel?`<div class="ktel">📞 ${l.tel}</div>`:''}
        ${l.obs?`<div class="kinfo" style="font-style:italic;margin-top:2px">${l.obs}</div>`:''}
        <div class="kactions">
          ${col!=='Fechado'?`<button class="btn btn-green btn-sm" onclick="setLeadStatus(${l.id},'Fechado')">✓ Fechar</button>`:''}
          ${col==='Novo'?`<button class="btn btn-gold btn-sm" onclick="setLeadStatus(${l.id},'Quente')">🔥</button>`:''}
          <button class="btn btn-outline btn-sm" onclick="openEditLead(${l.id})">✏️</button>
          <button class="btn btn-danger btn-sm" onclick="deleteLead(${l.id})">🗑</button>
        </div>
      </div>`).join('')}
    </div>`;
  }).join('');
}

function renderLeadTable(){
  const leads=filteredLeads();
  document.getElementById('leads-table').innerHTML=leads.map(l=>`<tr>
    <td><strong>${l.nome}</strong></td>
    <td>${l.tel?`<a href="tel:${l.tel}" style="color:var(--aqua)">${l.tel}</a>`:''}</td>
    <td>${l.origem||''}</td>
    <td><span class="badge-s ${SC[l.status]||''}">${l.status}</span></td>
    <td>${l.vendedor||''}</td>
    <td style="font-size:12px;color:var(--t3)">${l.obs||''}</td>
    <td>
      <div style="display:flex;gap:4px">
        <button class="btn btn-outline btn-sm" onclick="openEditLead(${l.id})">✏️</button>
        <button class="btn btn-danger btn-sm" onclick="deleteLead(${l.id})">🗑</button>
      </div>
    </td>
  </tr>`).join('');
}

// ─── IMPORT EXCEL/CSV ──────────────────────────────────
function handleDrop(ev){ev.preventDefault();document.getElementById('drop-zone').classList.remove('drag');const f=ev.dataTransfer.files[0];if(f)processFile(f);}
function handleFileImport(inp){if(inp.files[0])processFile(inp.files[0]);}
function processFile(file){
  const reader=new FileReader();
  reader.onload=function(e){
    let rows=[];
    try{
      const wb=XLSX.read(e.target.result,{type:'binary'});
      const ws=wb.Sheets[wb.SheetNames[0]];
      rows=XLSX.utils.sheet_to_json(ws,{defval:''});
    }catch(err){alert('Erro ao ler arquivo: '+err);return;}
    if(!rows.length){alert('Nenhum dado encontrado!');return;}
    // map columns
    const map=col=>rows[0]&&Object.keys(rows[0]).find(k=>k.toLowerCase().replace(/\s/g,'').includes(col));
    const nomCol=map('nome')||map('name')||map('cliente')||Object.keys(rows[0])[0];
    const telCol=map('tel')||map('phone')||map('celular')||map('whatsapp')||map('fone');
    const oriCol=map('origem')||map('source')||map('canal')||map('origem');
    const staCol=map('status')||map('etapa')||map('stage');
    importRows=rows.map(r=>({
      nome:(r[nomCol]||'').toString().trim(),
      tel:telCol?(r[telCol]||'').toString().trim():'',
      origem:oriCol?(r[oriCol]||'').toString().trim()||'Importado':'Importado',
      status:staCol?mapStatus((r[staCol]||'').toString().trim()):'',
    })).filter(r=>r.nome);
    showImportPreview(importRows);
  };
  reader.readAsBinaryString(file);
}
function mapStatus(s){
  const sl=s.toLowerCase();
  if(sl.includes('quet')||sl.includes('hot')||sl.includes('interest'))return'Quente';
  if(sl.includes('abord')||sl.includes('contact'))return'Abordagem';
  if(sl.includes('fech')||sl.includes('clos')||sl.includes('vend')||sl.includes('won'))return'Fechado';
  if(sl.includes('perd')||sl.includes('lost'))return'Perdido';
  if(sl.includes('nov')||sl.includes('new')||sl.includes('fresh'))return'Novo';
  return '';
}
function showImportPreview(rows){
  document.getElementById('preview-count').textContent=rows.length;
  document.getElementById('preview-table-wrap').innerHTML=`<table><thead><tr><th>Nome</th><th>Telefone</th><th>Origem</th><th>Status</th></tr></thead><tbody>${rows.slice(0,10).map(r=>`<tr><td>${r.nome}</td><td>${r.tel}</td><td>${r.origem}</td><td>${r.status||'(padrão)'}</td></tr>`).join('')}${rows.length>10?`<tr><td colspan="4" style="color:var(--t3)">...e mais ${rows.length-10} leads</td></tr>`:''}</tbody></table>`;
  document.getElementById('import-preview').style.display='block';
  document.getElementById('btn-import-confirm').disabled=false;
}
function confirmImport(){
  const defaultSt=document.getElementById('import-default-status').value;
  importRows.forEach(r=>{S.leads.push({id:S.nextId++,nome:r.nome,tel:r.tel,origem:r.origem,status:r.status||defaultSt,vendedor:'',data:new Date().toISOString().split('T')[0],obs:'Importado'});});
  save();closeModal('m-import');updateSidebar();renderKanban();renderLeadTable();
  document.getElementById('import-preview').style.display='none';
  document.getElementById('btn-import-confirm').disabled=true;
  importRows=[];alert(`✅ ${importRows.length||'Leads'} importados com sucesso!`);
}

// ─── PIPELINE TABS ─────────────────────────────────────
function setPipeTab(tab,btn){
  document.querySelectorAll('#page-pipeline .tab-btn').forEach(b=>b.classList.remove('active'));btn.classList.add('active');
  document.getElementById('pipe-kanban').style.display=tab==='kanban'?'block':'none';
  document.getElementById('pipe-lista').style.display=tab==='lista'?'block':'none';
}

// ─── TIME DE VENDAS ────────────────────────────────────
function setTimeTab(tab,btn){
  document.querySelectorAll('#page-time .tab-btn').forEach(b=>b.classList.remove('active'));btn.classList.add('active');
  ['sdrs','closers','ranking'].forEach(t=>document.getElementById('time-'+t).style.display=t===tab?'block':'none');
  if(tab==='ranking')setTimeout(renderTimeChart,100);
}
function openAddMembro(tipo){
  document.getElementById('m-membro-title').textContent=`+ Novo ${tipo}`;
  document.getElementById('membro-tipo').value=tipo;
  document.getElementById('membro-edit-id').value='';
  ['mb-nome','mb-tel','mb-meta-d','mb-meta-m','mb-taxa','mb-atual'].forEach(id=>document.getElementById(id).value='');
  openModal('m-membro');
}
function openEditMembro(tipo,id){
  const list=tipo==='SDR'?S.sdrs:S.closers;
  const m=list.find(x=>x.id===id);if(!m)return;
  document.getElementById('m-membro-title').textContent=`✏️ Editar ${tipo}`;
  document.getElementById('membro-tipo').value=tipo;
  document.getElementById('membro-edit-id').value=id;
  document.getElementById('mb-nome').value=m.nome;
  document.getElementById('mb-tel').value=m.tel||'';
  document.getElementById('mb-meta-d').value=m.metaDia||'';
  document.getElementById('mb-meta-m').value=m.metaMes||'';
  document.getElementById('mb-taxa').value=m.taxa||'';
  document.getElementById('mb-atual').value=m.atual||'';
  openModal('m-membro');
}
function saveMembro(){
  const nome=document.getElementById('mb-nome').value.trim();if(!nome){alert('Informe o nome!');return;}
  const tipo=document.getElementById('membro-tipo').value;
  const editId=parseInt(document.getElementById('membro-edit-id').value)||0;
  const obj={nome,tel:document.getElementById('mb-tel').value,metaDia:+document.getElementById('mb-meta-d').value||100,metaMes:+document.getElementById('mb-meta-m').value||50,taxa:+document.getElementById('mb-taxa').value||28,atual:+document.getElementById('mb-atual').value||0};
  const list=tipo==='SDR'?S.sdrs:S.closers;
  if(editId){Object.assign(list.find(x=>x.id===editId),obj);}else{obj.id=S.nextId++;list.push(obj);}
  save();closeModal('m-membro');populateVendedorSelect();
  if(tipo==='SDR')renderSDR();else renderCloser();
}
function deleteMembro(tipo,id){if(!confirm('Excluir?'))return;if(tipo==='SDR')S.sdrs=S.sdrs.filter(x=>x.id!==id);else S.closers=S.closers.filter(x=>x.id!==id);save();if(tipo==='SDR')renderSDR();else renderCloser();}

function renderSDR(){
  document.getElementById('sdr-table').innerHTML=S.sdrs.map(s=>{
    const pct=Math.min(100,Math.round(s.atual/(s.metaDia||100)*100));
    const cor=pct>=90?'var(--green)':pct>=60?'var(--gold)':'var(--coral)';
    return`<tr><td><strong>${s.nome}</strong></td><td>${s.tel?`<a href="tel:${s.tel}" style="color:var(--aqua)">${s.tel}</a>`:''}</td><td style="color:${cor};font-weight:700">${s.atual}</td><td>${s.metaDia}/dia</td><td>${s.taxa}%</td><td><div style="display:flex;align-items:center;gap:6px"><div style="flex:1;height:5px;background:rgba(0,0,0,0.08);border-radius:3px"><div style="width:${pct}%;height:5px;background:${cor};border-radius:3px"></div></div><span style="font-size:11px;color:${cor}">${pct}%</span></div></td><td><div style="display:flex;gap:4px"><button class="btn btn-outline btn-sm" onclick="openEditMembro('SDR',${s.id})">✏️</button><button class="btn btn-danger btn-sm" onclick="deleteMembro('SDR',${s.id})">🗑</button></div></td></tr>`;
  }).join('');
}
function renderCloser(){
  document.getElementById('closer-table').innerHTML=S.closers.map(c=>{
    const pct=Math.min(100,Math.round(c.atual/(c.metaDia||10)*100*4));
    const cor=pct>=90?'var(--green)':pct>=60?'var(--gold)':'var(--coral)';
    return`<tr><td><strong>${c.nome}</strong></td><td>${c.tel?`<a href="tel:${c.tel}" style="color:var(--aqua)">${c.tel}</a>`:''}</td><td style="color:var(--green);font-weight:700">${c.atual}</td><td>${c.metaMes} cotas</td><td>${c.taxa}%</td><td><div style="display:flex;align-items:center;gap:6px"><div style="flex:1;height:5px;background:rgba(0,0,0,0.08);border-radius:3px"><div style="width:${pct}%;height:5px;background:${cor};border-radius:3px"></div></div><span style="font-size:11px;color:${cor}">${pct}%</span></div></td><td><div style="display:flex;gap:4px"><button class="btn btn-outline btn-sm" onclick="openEditMembro('Closer',${c.id})">✏️</button><button class="btn btn-danger btn-sm" onclick="deleteMembro('Closer',${c.id})">🗑</button></div></td></tr>`;
  }).join('');
}
function renderTimeRanking(){
  const all=[...S.sdrs.map(s=>({nome:s.nome,val:s.atual,tipo:'SDR'})),...S.closers.map(c=>({nome:c.nome,val:c.atual*5,tipo:'Closer'}))].sort((a,b)=>b.val-a.val);
  document.getElementById('ranking-time').innerHTML=all.map((p,i)=>`<div class="ranking-item"><div class="rank-pos ${['r1','r2','r3'][i]||'rn'}">${i+1}</div><div style="flex:1"><div style="font-size:13px;font-weight:600">${p.nome}</div><div style="font-size:11px;color:var(--t3)">${p.tipo}</div></div><div style="font-size:18px;font-weight:800;color:var(--aqua)">${p.val}</div></div>`).join('');
}

// ─── AFILIADOS ─────────────────────────────────────────
function openEditAfiliado(id){
  const a=S.afiliados.find(x=>x.id===id);if(!a)return;
  document.getElementById('m-aff-title').textContent='✏️ Editar Indicação';
  document.getElementById('aff-edit-id').value=id;
  document.getElementById('af-nome').value=a.nome;
  document.getElementById('af-tel').value=a.tel||'';
  document.getElementById('af-cotas').value=a.cotas;
  document.getElementById('af-nivel').value=a.nivel;
  document.getElementById('af-pix').value=a.pix;
  document.getElementById('af-status').value=a.status;
  openModal('m-afiliado');
}
function saveAfiliado(){
  const nome=document.getElementById('af-nome').value.trim();if(!nome){alert('Informe o nome!');return;}
  const editId=parseInt(document.getElementById('aff-edit-id').value)||0;
  const obj={nome,tel:document.getElementById('af-tel').value,cotas:+document.getElementById('af-cotas').value||1,nivel:document.getElementById('af-nivel').value,pix:+document.getElementById('af-pix').value||50,status:document.getElementById('af-status').value};
  if(editId){Object.assign(S.afiliados.find(x=>x.id===editId),obj);}else{obj.id=S.nextId++;S.afiliados.push(obj);}
  save();closeModal('m-afiliado');
  document.getElementById('aff-edit-id').value='';
  document.getElementById('m-aff-title').textContent='+ Nova Indicação';
  renderAfiliados();
}
function deleteAfiliado(id){if(!confirm('Excluir indicação?'))return;S.afiliados=S.afiliados.filter(x=>x.id!==id);save();renderAfiliados();}
function renderAfiliados(){
  const sorted=[...S.afiliados].sort((a,b)=>b.cotas-a.cotas);
  const totalPix=sorted.filter(a=>a.status==='pago').reduce((s,a)=>s+a.pix,0);
  const pendPix=sorted.filter(a=>a.status==='pendente').reduce((s,a)=>s+a.pix,0);
  document.getElementById('aff-ativos').textContent=sorted.length;
  document.getElementById('aff-cotas').textContent=sorted.reduce((s,a)=>s+a.cotas,0);
  document.getElementById('aff-pix').textContent='R$'+totalPix.toLocaleString('pt-BR');
  document.getElementById('aff-pend').textContent='R$'+pendPix.toLocaleString('pt-BR');
  document.getElementById('aff-table').innerHTML=sorted.map((a,i)=>`<tr>
    <td><strong>${i+1}. ${a.nome}</strong></td>
    <td><strong style="color:var(--aqua)">${a.cotas}</strong></td>
    <td><span class="badge-s" style="background:rgba(240,165,0,0.15);color:var(--gold);border:1px solid rgba(240,165,0,0.3)">${a.nivel}</span></td>
    <td style="color:var(--gold);font-weight:700">R$${a.pix.toLocaleString('pt-BR')}</td>
    <td><span class="badge-s ${a.status==='pago'?'s-fechado':'s-quente'}">${a.status==='pago'?'✅ Pago':'⏳ Pendente'}</span></td>
    <td>${a.tel?`<a href="tel:${a.tel}" style="color:var(--aqua)">${a.tel}</a>`:''}</td>
    <td><div style="display:flex;gap:4px">
      ${a.status==='pendente'?`<button class="btn btn-green btn-sm" onclick="pagarPix(${a.id})">💸 Pagar</button>`:''}
      <button class="btn btn-outline btn-sm" onclick="openEditAfiliado(${a.id})">✏️</button>
      <button class="btn btn-danger btn-sm" onclick="deleteAfiliado(${a.id})">🗑</button>
    </div></td>
  </tr>`).join('');
}
function pagarPix(id){const a=S.afiliados.find(x=>x.id===id);if(a){a.status='pago';save();renderAfiliados();}}

// ─── METAS ─────────────────────────────────────────────
function openEditMeta(id){
  const m=S.metas.find(x=>x.id===id);if(!m)return;
  document.getElementById('m-meta-title').textContent='✏️ Editar Meta';
  document.getElementById('meta-edit-id').value=id;
  document.getElementById('mt-nome').value=m.nome;
  document.getElementById('mt-mensal').value=m.mensal;
  document.getElementById('mt-semanal').value=m.semanal;
  document.getElementById('mt-real').value=m.real;
  document.getElementById('mt-cor').value=m.cor;
  openModal('m-meta');
}
function saveMeta(){
  const nome=document.getElementById('mt-nome').value.trim();if(!nome){alert('Informe o nome!');return;}
  const editId=parseInt(document.getElementById('meta-edit-id').value)||0;
  const obj={nome,mensal:+document.getElementById('mt-mensal').value||0,semanal:+document.getElementById('mt-semanal').value||0,real:+document.getElementById('mt-real').value||0,cor:document.getElementById('mt-cor').value};
  if(editId){Object.assign(S.metas.find(x=>x.id===editId),obj);}else{obj.id=S.nextId++;S.metas.push(obj);}
  save();closeModal('m-meta');document.getElementById('meta-edit-id').value='';document.getElementById('m-meta-title').textContent='+ Nova Meta';
  renderMetas();renderMetasChart();updateSidebar();updateDashKpis();
}
function deleteMeta(id){if(!confirm('Excluir meta?'))return;S.metas=S.metas.filter(x=>x.id!==id);save();renderMetas();renderMetasChart();updateDashKpis();}
function renderMetas(){
  document.getElementById('metas-table').innerHTML=S.metas.map(m=>{
    const pct=m.mensal?Math.round(m.real/m.mensal*100):0;
    const cor=pct>=80?'var(--green)':pct>=50?'var(--gold)':'var(--coral)';
    return`<tr>
      <td><strong>${m.nome}</strong></td>
      <td><strong style="color:${COLORS[m.cor]||'var(--aqua)'}">${m.mensal.toLocaleString('pt-BR')}</strong></td>
      <td>${m.semanal.toLocaleString('pt-BR')}</td>
      <td>${m.real.toLocaleString('pt-BR')}</td>
      <td><div style="display:flex;align-items:center;gap:8px"><div style="flex:1;height:5px;background:rgba(0,0,0,0.08);border-radius:3px"><div style="width:${Math.min(100,pct)}%;height:5px;background:${cor};border-radius:3px"></div></div><span style="color:${cor};font-weight:700;font-size:12px">${pct}%</span></div></td>
      <td><div style="width:14px;height:14px;border-radius:50%;background:${COLORS[m.cor]||'var(--aqua)'}"></div></td>
      <td><div style="display:flex;gap:4px"><button class="btn btn-outline btn-sm" onclick="openEditMeta(${m.id})">✏️</button><button class="btn btn-danger btn-sm" onclick="deleteMeta(${m.id})">🗑</button></div></td>
    </tr>`;
  }).join('');
  document.getElementById('metas-prog-list').innerHTML=S.metas.map(m=>{
    const pct=m.mensal?Math.min(100,Math.round(m.real/m.mensal*100)):0;
    const cor=COLORS[m.cor]||'var(--aqua)';
    return`<div style="margin-bottom:14px"><div style="display:flex;justify-content:space-between;margin-bottom:4px"><span style="font-size:13px">${m.nome}</span><span style="font-size:13px;font-weight:700;color:${cor}">${pct}%</span></div><div style="height:6px;background:rgba(0,0,0,0.08);border-radius:3px"><div style="width:${pct}%;height:6px;background:${cor};border-radius:3px;transition:.5s"></div></div><div style="font-size:11px;color:var(--t3);margin-top:3px">${m.real.toLocaleString('pt-BR')} / ${m.mensal.toLocaleString('pt-BR')}</div></div>`;
  }).join('');
}

// ─── CHARTS MAP ────────────────────────────────────────
let charts={};
function dc(id){if(charts[id]){charts[id].destroy();delete charts[id];}}

function renderMetasChart(){
  dc('metas');
  if(!document.getElementById('c-metas'))return;
  charts['metas']=new Chart(document.getElementById('c-metas'),{
    type:'bar',
    data:{labels:S.metas.map(m=>m.nome.split(' ').slice(0,2).join(' ')),datasets:[{label:'Real',data:S.metas.map(m=>m.real),backgroundColor:S.metas.map(m=>COLORS[m.cor]+'99'||'rgba(0,201,212,0.6)'),borderRadius:4},{label:'Meta',data:S.metas.map(m=>m.mensal),backgroundColor:'rgba(0,0,0,0.07)',borderRadius:4}]},
    options:{responsive:true,maintainAspectRatio:false,plugins:{legend:{labels:{color:'#4a7090',font:{size:11}}}},scales:{x:{ticks:{color:'#4a7090',font:{size:10}},grid:{color:'rgba(0,0,0,0.04)'}},y:{ticks:{color:'#4a7090'},grid:{color:'rgba(0,0,0,0.05)'}}}}
  });
}

// ─── DASHBOARD ─────────────────────────────────────────
function updateDashKpis(){
  const mv=S.metas.find(m=>m.nome==='Cotas Vendidas')||{mensal:1000,real:347};
  const ml=S.metas.find(m=>m.nome==='Leads Captados')||{mensal:33000,real:11430};
  const mi=S.metas.find(m=>m.nome==='Cotas via Indicação')||{mensal:300,real:89};
  document.getElementById('kpi-v').textContent=mv.real;
  document.getElementById('kpi-v-sub').textContent='Meta: '+mv.mensal.toLocaleString('pt-BR')+'/mês';
  document.getElementById('kprog-v').style.width=Math.min(100,mv.real/mv.mensal*100)+'%';
  document.getElementById('kpi-l').textContent=ml.real.toLocaleString('pt-BR');
  document.getElementById('kpi-l-sub').textContent='Meta: '+ml.mensal.toLocaleString('pt-BR')+'/mês';
  document.getElementById('kprog-l').style.width=Math.min(100,ml.real/ml.mensal*100)+'%';
  document.getElementById('kpi-ind').textContent=mi.real;
  document.getElementById('kpi-ind-sub').textContent='Meta: '+mi.mensal+'/mês';
  document.getElementById('kprog-ind').style.width=Math.min(100,mi.real/mi.mensal*100)+'%';
}

function initDashCharts(){
  // Funil
  const funnelData=[{label:'🌊 Alcance',val:'54k',w:100,bg:'rgba(0,201,212,0.2)',c:'var(--aqua)'},{label:'🎯 Leads',val:'11.4k',w:75,bg:'rgba(30,136,229,0.2)',c:'var(--wave)'},{label:'🔥 Quentes',val:'5.8k',w:52,bg:'rgba(240,165,0,0.2)',c:'var(--gold)'},{label:'📞 Abordagem',val:'1.8k',w:30,bg:'rgba(255,107,53,0.2)',c:'var(--coral)'},{label:'✅ Vendas',val:'347',w:12,bg:'rgba(0,208,132,0.2)',c:'var(--green)'}];
  document.getElementById('funnel-v').innerHTML=funnelData.map(f=>`<div style="display:flex;align-items:center;gap:10px;margin-bottom:7px"><div style="flex:1"><div class="funnel-bar" style="width:${f.w}%;background:${f.bg};color:${f.c}">${f.label}</div></div><div style="width:55px;text-align:right;font-size:16px;font-weight:800;color:${f.c}">${f.val}</div></div>`).join('');
  // Vendas
  dc('vendas');
  const days=['15/04','16/04','17/04','18/04','19/04','20/04','21/04','22/04','23/04','24/04','25/04','26/04','27/04','28/04'];
  const vals=[18,22,19,31,28,14,8,25,29,33,27,38,35,21];
  charts['vendas']=new Chart(document.getElementById('c-vendas'),{type:'bar',data:{labels:days,datasets:[{label:'Cotas',data:vals,backgroundColor:vals.map(v=>v>=30?'rgba(0,208,132,0.7)':v>=20?'rgba(0,201,212,0.6)':'rgba(30,136,229,0.5)'),borderRadius:4,borderSkipped:false}]},options:{responsive:true,maintainAspectRatio:false,plugins:{legend:{display:false}},scales:{x:{ticks:{color:'#4a7090',font:{size:10}},grid:{color:'rgba(0,0,0,0.04)'}},y:{ticks:{color:'#4a7090'},grid:{color:'rgba(0,0,0,0.05)'}}}}});
  // Canais
  dc('canais');
  const cd={labels:['Meta Ads','Indicação','Google Ads','Live','Evento','Orgânico','B2B'],data:[142,89,63,31,14,8,5]};
  const clrs=['#1e88e5','#f0a500','#00c9d4','#ff6b35','#00d084','#6c757d','#9c27b0'];
  charts['canais']=new Chart(document.getElementById('c-canais'),{type:'doughnut',data:{labels:cd.labels,datasets:[{data:cd.data,backgroundColor:clrs,borderWidth:0,hoverOffset:4}]},options:{responsive:true,maintainAspectRatio:false,plugins:{legend:{display:false}},cutout:'65%'}});
  document.getElementById('canais-leg').innerHTML=cd.labels.map((l,i)=>`<div style="display:flex;align-items:center;gap:5px;font-size:11px"><div style="width:8px;height:8px;border-radius:50%;background:${clrs[i]};flex-shrink:0"></div>${l} <strong style="margin-left:auto">${cd.data[i]}</strong></div>`).join('');
  // Ranking dash
  const sorted=[...S.afiliados].sort((a,b)=>b.cotas-a.cotas);
  document.getElementById('dash-ranking').innerHTML=sorted.slice(0,5).map((a,i)=>`<div class="ranking-item"><div class="rank-pos ${['r1','r2','r3'][i]||'rn'}">${i+1}</div><div style="flex:1"><div style="font-size:13px;font-weight:600">${a.nome}</div><div style="font-size:11px;color:var(--t3)">${a.nivel}</div></div><div style="font-size:18px;font-weight:800;color:var(--aqua)">${a.cotas}</div></div>`).join('');
  // KPI table
  document.getElementById('kpi-table').innerHTML=S.metas.map(m=>{
    const pct=m.semanal?Math.round(m.real/m.mensal*100):0;
    const cor=pct>=80?'var(--green)':pct>=50?'var(--gold)':'var(--coral)';
    const wkReal=Math.round(m.real/4);
    return`<tr><td>${m.nome}</td><td><strong style="color:var(--aqua)">${wkReal.toLocaleString('pt-BR')}</strong></td><td>${m.semanal.toLocaleString('pt-BR')}</td><td style="color:${cor};font-weight:700">${Math.round(wkReal/m.semanal*100)||0}%</td><td><span class="badge-s" style="background:rgba(${pct>=80?'0,208,132':pct>=50?'240,165,0':'255,107,53'},0.15);color:${cor};border:1px solid ${cor}">${pct>=80?'✅ OK':pct>=50?'⚠ Atenção':'❌ Crítico'}</span></td></tr>`;
  }).join('');
}

function renderTimeChart(){
  dc('time');
  if(!document.getElementById('c-time'))return;
  charts['time']=new Chart(document.getElementById('c-time'),{type:'bar',data:{labels:[...S.closers.map(c=>c.nome.split(' ')[0]),...S.sdrs.slice(0,4).map(s=>s.nome.split(' ')[0])],datasets:[{label:'Atividade',data:[...S.closers.map(c=>c.atual),...S.sdrs.slice(0,4).map(s=>s.atual)],backgroundColor:'rgba(0,149,106,0.6)',borderRadius:4},{label:'Meta',data:[...S.closers.map(c=>c.metaDia),...S.sdrs.slice(0,4).map(s=>s.metaDia)],backgroundColor:'rgba(0,0,0,0.07)',borderRadius:4}]},options:{responsive:true,maintainAspectRatio:false,plugins:{legend:{labels:{color:'#4a7090',font:{size:11}}}},scales:{x:{ticks:{color:'#4a7090',font:{size:10}},grid:{color:'rgba(0,0,0,0.04)'}},y:{ticks:{color:'#4a7090'},grid:{color:'rgba(0,0,0,0.05)'}}}}});
}

// ─── PLANOS ─────────────────────────────────────────────
const PLANOS=[
  {id:'p1',e:'🔴',t:'PLANO 1 — Máquina de Indicação (PIX Viral)',itens:['Estruturar 3 tiers de recompensa com PIX automático','Criar landing page de afiliado com link único por sócio','WhatsApp broadcast semanal para base de sócios','Criar stories kit para sócios postarem com link próprio','Ativar ranking público de top indicadores (gamificação)','Challenge mensal: quem indica 5 ganha convite VIP']},
  {id:'p2',e:'📱',t:'PLANO 2 — Lives de Conversão no Instagram',itens:['Live "Bastidores da Obra" semanal com drone no canteiro','Live "Sócio Fundador do Mês" com depoimento ao vivo','Live com oferta de 24h + contador regressivo no bio','Live "Família Fundadora" nos clubes parceiros','Contatar 5 micro-influenciadores locais de BH/Betim']},
  {id:'p3',e:'🎯',t:'PLANO 3 — Meta Ads: Funil de Performance',itens:['Campanha topo de funil — vídeo emocional 15s','Campanha meio de funil — carrossel de benefícios','Campanha fundo de funil — depoimento + oferta R$10','Criativo de urgência dinâmica com contador de lotes','Google Ads com keywords de intenção de compra']},
  {id:'p4',e:'🤝',t:'PLANO 4 — Clube de Empresas e RH (B2B)',itens:['Mapear 200 maiores empregadoras de Betim e contorno','Criar proposta corporativa com desconto progressivo','Realizar "AquaMais Business Day" com 15 empresas','Contatar sindicatos e associações de classe da região','Apresentação em reuniões de condomínio/associações']},
  {id:'p5',e:'🏅',t:'PLANO 5 — Descontos Progressivos (Efeito Manada)',itens:['Criar "Turma de Fundadores" — grupos de 10–20 pessoas','Publicar tabela de preços por lote publicamente','Programa "Fundador traz Fundador" — 5% desconto permanente','Campanha "Família Fundadora" — benefício para 3+ cotas']},
  {id:'p6',e:'🎪',t:'PLANO 6 — Eventos Presenciais de Conversão',itens:['"Noite do Fundador" semanal — meta 20+ cotas/evento','Pop-up em shoppings de Betim e BH — meta 30/fim de semana','Visita guiada à obra — closer no ônibus de volta','Parceria com escolas para pais de alunos']},
  {id:'p7',e:'🤖',t:'PLANO 7 — Automação de Nutrição (N8N + WhatsApp)',itens:['Dia 0: Sequência imediata — vídeo + oferta R$10','Dia 1: Prova social com depoimentos de sócios','Dia 2: Urgência de preço — cotas do lote restantes','Dia 3: Benefício imediato — clubes parceiros','Dia 5: SDR humano entra com mensagem personalizada','Dia 7: Última chance com calculadora de economia']},
];
function renderPlanos(){
  let total=0,done=0;
  PLANOS.forEach(p=>{total+=p.itens.length;done+=(S.planos[p.id]||[]).length;});
  document.getElementById('planos-kpis').innerHTML=`<div class="kpi-card"><div class="kpi-label">Total de Ações</div><div class="kpi-val" style="color:var(--aqua)">${total}</div></div><div class="kpi-card"><div class="kpi-label">Concluídas</div><div class="kpi-val" style="color:var(--green)">${done}</div></div><div class="kpi-card"><div class="kpi-label">Progresso</div><div class="kpi-val" style="color:var(--gold)">${Math.round(done/total*100)}%</div></div><div class="kpi-card"><div class="kpi-label">Pendentes</div><div class="kpi-val" style="color:var(--coral)">${total-done}</div></div>`;
  document.getElementById('planos-list').innerHTML=PLANOS.map(p=>{
    const d=S.planos[p.id]||[];const pct=Math.round(d.length/p.itens.length*100);
    return`<div class="plan-card"><div class="plan-hdr" onclick="togglePlan('pb-${p.id}')"><span style="font-size:22px">${p.e}</span><div style="flex:1;font-weight:700;font-size:14px">${p.t}</div><div style="display:flex;align-items:center;gap:8px"><div style="width:55px;height:3px;background:rgba(0,0,0,0.08);border-radius:2px"><div style="width:${pct}%;height:3px;background:${pct===100?'var(--green)':'var(--aqua)'};border-radius:2px"></div></div><span style="font-size:11px;color:${pct===100?'var(--green)':'var(--t3)'}">${pct}%</span></div></div><div class="plan-body" id="pb-${p.id}">${p.itens.map((item,i)=>{const chk=d.includes(i);return`<div class="ci ${chk?'done':''}" onclick="toggleCheck('${p.id}',${i})"><div class="cbox ${chk?'chk':''}">${chk?'✓':''}</div><div class="ctext">${item}</div></div>`;}).join('')}</div></div>`;
  }).join('');
}
function togglePlan(id){document.getElementById(id).classList.toggle('open');}
function toggleCheck(pid,idx){if(!S.planos[pid])S.planos[pid]=[];const a=S.planos[pid];const pos=a.indexOf(idx);if(pos>=0)a.splice(pos,1);else a.push(idx);save();renderPlanos();}

// ─── SCRIPTS CRUD ──────────────────────────────────────
function openNewScript(){
  document.getElementById('m-script-title').textContent='+ Novo Script';
  document.getElementById('script-edit-id').value='';
  document.getElementById('sc-emoji').value='📝';
  document.getElementById('sc-canal').value='';
  document.getElementById('sc-titulo').value='';
  document.getElementById('sc-txt').value='';
  openModal('m-script');
}
function openEditScript(id){
  const s=S.scripts.find(x=>x.id===id);if(!s)return;
  document.getElementById('m-script-title').textContent='✏️ Editar Script';
  document.getElementById('script-edit-id').value=id;
  document.getElementById('sc-emoji').value=s.e||'📝';
  document.getElementById('sc-canal').value=s.c||'';
  document.getElementById('sc-titulo').value=s.t||'';
  document.getElementById('sc-txt').value=s.txt||'';
  openModal('m-script');
}
function saveScript(){
  const t=document.getElementById('sc-titulo').value.trim();
  if(!t){alert('Informe o título do script!');return;}
  const editId=parseInt(document.getElementById('script-edit-id').value)||0;
  const obj={e:document.getElementById('sc-emoji').value||'📝',c:document.getElementById('sc-canal').value||'Geral',t,txt:document.getElementById('sc-txt').value};
  if(editId){Object.assign(S.scripts.find(x=>x.id===editId),obj);}
  else{obj.id=S.nextId++;S.scripts.push(obj);}
  save();closeModal('m-script');renderScripts();
}
function deleteScript(id){
  if(!confirm('Excluir este script?'))return;
  S.scripts=S.scripts.filter(x=>x.id!==id);
  save();renderScripts();
}
function renderScripts(){
  document.getElementById('scripts-list').innerHTML=S.scripts.map((s,i)=>`
    <div class="script-card">
      <div class="script-hdr" onclick="document.getElementById('ssb-${s.id}').classList.toggle('open')">
        <span style="font-size:18px">${s.e||'📝'}</span>
        <div style="flex:1">
          <div class="stitle">${s.t}</div>
          <div class="schan">${s.c}</div>
        </div>
        <div style="display:flex;align-items:center;gap:6px">
          <button class="btn btn-outline btn-sm" onclick="event.stopPropagation();openEditScript(${s.id})">✏️</button>
          <button class="btn btn-danger btn-sm" onclick="event.stopPropagation();deleteScript(${s.id})">🗑</button>
          <span style="color:var(--t3)">▼</span>
        </div>
      </div>
      <div class="script-body" id="ssb-${s.id}">
        <div class="script-txt">${(s.txt||'').replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;').replace(/\n/g,'<br>')}</div>
        <button class="copy-btn" onclick="copyScript(${s.id})">📋 Copiar Script</button>
      </div>
    </div>`).join('');
}
function copyScript(id){
  const s=S.scripts.find(x=>x.id===id);
  if(!s)return;
  navigator.clipboard.writeText(s.txt).then(()=>{
    const btn=document.querySelector(`[onclick="copyScript(${id})"]`);
    if(btn){btn.textContent='✅ Copiado!';setTimeout(()=>{btn.innerHTML='📋 Copiar Script';},2000);}
  });
}

// ─── CRONOGRAMA ────────────────────────────────────────
const TL=[
  {w:'Dias 1–2',t:'🚀 Ativação de Emergência',d:'Reunião com equipe, auditoria de campanhas, mapear sócios, configurar links rastreáveis.',m:0,r:0,dot:'done'},
  {w:'Semana 1 — Dias 3–9',t:'🔥 Lançamento da Máquina',d:'Landing page, N8N, Meta Ads 3 campanhas, Live de lançamento, Noite do Fundador, broadcast sócios.',m:150,r:147,dot:'done'},
  {w:'Semana 2 — Dias 10–16',t:'📊 Otimização e B2B',d:'Análise de CPL, 20 contatos B2B, pop-up shopping, Live com drone, visitas guiadas à obra.',m:220,r:89,dot:'active'},
  {w:'Semana 3 — Dias 17–23',t:'📈 Aceleração de Indicações',d:'Top 10 indicadores publicados, challenge ativado, micro-influenciadores, Live com depoimento.',m:280,r:0,dot:''},
  {w:'Semana 4 — Dias 24–30',t:'🎯 Fechamento Agressivo',d:'Última chance para leads frios, live de encerramento de lote, Business Day, review do mês.',m:350,r:0,dot:''},
];
function renderCrono(){
  document.getElementById('tl-list').innerHTML=TL.map(t=>`<div class="tl-item"><div class="tl-dot ${t.dot}"></div><div class="tl-week">${t.w}</div><div class="tl-title">${t.t}</div><div class="tl-desc">${t.d}</div>${t.m?`<div style="margin-top:8px;height:4px;background:rgba(0,0,0,0.08);border-radius:2px"><div style="width:${Math.min(100,t.r/t.m*100)||0}%;height:4px;background:linear-gradient(90deg,var(--aqua),var(--wave));border-radius:2px"></div></div><div style="display:flex;justify-content:space-between;font-size:11px;color:var(--t3);margin-top:3px"><span>${t.r}/${t.m} cotas</span><span>${Math.round(t.r/t.m*100)||0}%</span></div>`:''}</div>`).join('');
  dc('crono');
  charts['crono']=new Chart(document.getElementById('c-crono'),{type:'bar',data:{labels:['Sem 1','Sem 2','Sem 3','Sem 4'],datasets:[{label:'Real',data:[147,89,0,0],backgroundColor:['rgba(0,208,132,0.7)','rgba(240,165,0,0.7)','rgba(0,201,212,0.3)','rgba(0,201,212,0.3)'],borderRadius:5},{label:'Meta',data:[150,220,280,350],backgroundColor:'rgba(0,0,0,0.07)',borderRadius:5}]},options:{responsive:true,maintainAspectRatio:false,plugins:{legend:{labels:{color:'#4a7090'}}},scales:{x:{ticks:{color:'#4a7090'},grid:{color:'rgba(0,0,0,0.04)'}},y:{ticks:{color:'#4a7090'},grid:{color:'rgba(0,0,0,0.05)'}}}}});
}

// ─── ALERTAS ───────────────────────────────────────────
const ALERTAS=[
  {t:'danger',i:'🚨',title:'PIX de Indicação Pendente',desc:'R$1.080 em PIX pendentes há mais de 48h. Pagar hoje para não matar o programa.',s:'Crítico'},
  {t:'warn',i:'⚠️',title:'CPL acima da meta — campanha #3',desc:'Meta Ads "Lote Família" com CPL de R$18 vs meta de R$15. Revisar criativos.',s:'Atenção'},
  {t:'warn',i:'⚠️',title:'Taxa SDR→Closer abaixo da meta',desc:'28% atual vs meta de 30%. 2 SDRs com taxa abaixo de 27%. Revisar script.',s:'Atenção'},
  {t:'warn',i:'⚠️',title:'8 dias sem atualização visual da obra',desc:'Recomendado pelo menos 1 vídeo/foto da obra por semana para reduzir cancelamentos.',s:'Atenção'},
  {t:'ok',i:'✅',title:'Clube Parceiro funcionando normalmente',desc:'Nenhuma reclamação de acesso nos últimos 7 dias.',s:'OK'},
  {t:'ok',i:'✅',title:'Google Ads dentro do orçamento',desc:'CPC médio R$2,10 com CTR de 3,8%.',s:'OK'},
  {t:'ok',i:'✅',title:'Sequência N8N ativa e funcionando',desc:'Automação disparando para 100% dos leads novos. Taxa de abertura: 68%.',s:'OK'},
  {t:'ok',i:'✅',title:'CRM atualizado diariamente',desc:'Todos os leads com status atualizado nas últimas 24h.',s:'OK'},
];
function renderAlertas(){
  document.getElementById('alerts-list').innerHTML=ALERTAS.map(a=>`<div class="alert-card ${a.t}"><div style="font-size:22px;flex-shrink:0">${a.i}</div><div style="flex:1"><div style="font-weight:700;font-size:14px;margin-bottom:3px">${a.title}</div><div style="font-size:13px;color:var(--t2);line-height:1.5">${a.desc}</div></div><div style="flex-shrink:0"><div class="pill pill-${a.t==='ok'?'ok':a.t==='warn'?'warn':'danger'}">${a.s}</div></div></div>`).join('');
}

// ─── SWOT ──────────────────────────────────────────────
function generateSWOT(){
  const F=[],W=[],O=[],T=[];
  S.metas.forEach(m=>{
    const pct=m.mensal>0?(m.real/m.mensal*100):0;
    if(pct>=70) F.push({i:'🎯',t:`${m.nome} em ritmo forte`,d:`${m.real.toLocaleString('pt-BR')} / ${m.mensal.toLocaleString('pt-BR')} — ${Math.round(pct)}% da meta mensal atingida.`});
    else if(pct<50){const nd=Math.round((m.mensal-m.real)/14);W.push({i:'📉',t:`${m.nome} abaixo da meta (${Math.round(pct)}%)`,d:`Apenas ${m.real.toLocaleString('pt-BR')} de ${m.mensal.toLocaleString('pt-BR')}. Precisa de ${nd}/dia para recuperar no mês.`,p:[`Aumentar cadência para ${nd} unidades/dia nas próximas 2 semanas`,`Identificar o canal com melhor ROI e alocar mais verba nele`,`Daily de 15 min com o time para diagnosticar gargalos`,`Ativar campanha de urgência "últimas vagas do lote" imediatamente`]});}
  });
  const tot=S.leads.length||1;
  const perdidos=S.leads.filter(l=>l.status==='Perdido').length;
  const quentes=S.leads.filter(l=>l.status==='Quente').length;
  const fechados=S.leads.filter(l=>l.status==='Fechado').length;
  const emAbord=S.leads.filter(l=>l.status==='Abordagem').length;
  if(fechados>0&&fechados/tot>=0.2) F.push({i:'✅',t:`Taxa de fechamento de ${Math.round(fechados/tot*100)}% no CRM`,d:`${fechados} leads convertidos de ${tot} — performance acima de 20%.`});
  if(quentes>0) O.push({i:'🔥',t:`${quentes} lead(s) quente(s) sem fechar`,d:`Interesse já demonstrado. Conversão imediata possível com o script certo.`,p:[`Contatar todos os ${quentes} leads quentes hoje — prioridade máxima`,`Usar script de urgência de lote (variação de preço iminente)`,`Atribuir ao Closer com maior taxa de conversão`]});
  if(emAbord>0) O.push({i:'📋',t:`${emAbord} lead(s) em abordagem para acelerar`,d:`Estão no meio do funil — com follow-up correto, parte fecha essa semana.`,p:[`Ligar com condição especial por tempo limitado`,`Enviar vídeo da obra + depoimento de sócio`,`Criar urgência: "lote fecha sexta"`]});
  if(perdidos/tot>0.25) T.push({i:'😞',t:`${Math.round(perdidos/tot*100)}% de leads marcados como perdidos`,d:`${perdidos} de ${tot} perdidos — acima de 25%. Indica falha de script ou qualidade de lead.`,p:[`Mapear as 3 objeções mais frequentes dos leads perdidos`,`Revisar script de contorno com todo o time esta semana`,`Criar sequência N8N de re-engajamento para perdidos há 7-14 dias`,`Testar nova segmentação de público nas campanhas pagas`]});
  if(S.sdrs.length){
    const ab=S.sdrs.filter(s=>s.taxa<28),ac=S.sdrs.filter(s=>s.taxa>=30);
    if(ac.length) F.push({i:'⚡',t:`${ac.length} SDR(s) acima de 30% de conversão`,d:`${ac.map(s=>s.nome).join(', ')} — acima da meta. Compartilhar práticas com o restante do time.`});
    if(ab.length) W.push({i:'👥',t:`${ab.length} SDR(s) abaixo de 28% de conversão`,d:`${ab.map(s=>`${s.nome} (${s.taxa}%)`).join(', ')} — reduzindo volume para os Closers.`,p:[`Roleplay semanal com foco nas objeções mais comuns`,`Rever qualidade dos leads atribuídos a cada SDR`,`Feedback imediato nas 10 primeiras abordagens do dia`,`Realocar leads de qualidade para SDRs com maior taxa temporariamente`]});
  }
  if(S.closers.length){
    const bom=S.closers.filter(c=>c.atual>=c.metaDia),bx=S.closers.filter(c=>c.atual<c.metaDia*0.7);
    if(bom.length) F.push({i:'🏆',t:`${bom.length} Closer(s) batendo meta diária`,d:`${bom.map(c=>c.nome).join(', ')} — base sólida de fechamento.`});
    if(bx.length) W.push({i:'📞',t:`${bx.length} Closer(s) abaixo de 70% da meta`,d:`${bx.map(c=>`${c.nome} (${c.atual}/${c.metaDia}/dia)`).join(', ')} — impacto direto no faturamento.`,p:[`Escutar gravações das últimas 5 ligações de cada closer abaixo`,`Identificar onde a conversa quebra no processo de fechamento`,`Simulação de fechamento com script de urgência`,`Verificar se os leads recebidos estão qualificados o suficiente`]});
  }
  if(S.afiliados.length){
    const plat=S.afiliados.filter(a=>a.nivel==='Platinum'||a.cotas>=10);
    const pend=S.afiliados.filter(a=>a.status==='pendente');
    const pixPend=pend.reduce((s,a)=>s+(a.pix||0),0);
    if(plat.length) F.push({i:'💎',t:`${plat.length} afiliado(s) Platinum ativos`,d:`${plat.map(a=>a.nome).join(', ')} — gerando volume consistente via indicação.`});
    if(pend.length) T.push({i:'💸',t:`R$${pixPend.toLocaleString('pt-BR')} em PIX pendentes`,d:`${pend.length} afiliado(s) sem receber: ${pend.map(a=>a.nome).join(', ')}. Atrasos matam o programa de indicações.`,p:[`Pagar HOJE os PIX de ${pend.map(a=>a.nome).join(', ')}`,`Enviar comprovante via WhatsApp para cada afiliado imediatamente`,`Publicar print do pagamento para motivar outros afiliados`,`Regra interna: PIX deve ser pago em no máximo 24h após conversão confirmada`]});
    if(S.afiliados.length<15) O.push({i:'📣',t:'Expandir a base de afiliados',d:`Apenas ${S.afiliados.length} afiliados cadastrados. Meta recomendada: 50+ para gerar 300 cotas/mês via indicação.`,p:[`Recrutar afiliados entre os sócios mais engajados`,`Bônus extra para quem recrutar 3+ novos afiliados este mês`,`Criar grupo exclusivo de afiliados no WhatsApp com conteúdo de suporte`]});
  }
  const b2b=S.leads.filter(l=>l.origem==='B2B').length;
  O.push({i:'🤝',t:`Canal B2B${b2b>0?` — ${b2b} empresa(s) no pipeline`:' ainda subexplorado'}`,d:'1 cliente B2B = 20-50 cotas fechadas. Alto ROI com volume garantido e sem CPL.',p:[`Mapear 20 empresas com 100+ funcionários em 30km de Betim`,`Enviar script corporativo para RH via LinkedIn e e-mail`,`Meta: 2 reuniões B2B por semana`,`Business Day: visita à obra + apresentação para a equipe da empresa`]});
  const mc=S.metas.find(m=>m.nome==='Cotas Vendidas');
  if(mc){
    const dp=16,dr=30-dp,ra=mc.real/dp,rn=(mc.mensal-mc.real)/dr;
    if(rn>ra*1.15) T.push({i:'⏰',t:'Ritmo atual insuficiente para bater a meta mensal',d:`Vendendo ${ra.toFixed(1)}/dia, mas precisa de ${rn.toFixed(1)}/dia. Faltam ${mc.mensal-mc.real} cotas em ${dr} dias.`,p:[`Lançar campanha "Último Lote" nos próximos 3 dias`,`Dobrar follow-up com todos os leads em abordagem`,`Live de vendas com oferta exclusiva esta semana`,`Business Day para fechar empresas em grupo`,`Mobilizar afiliados Platinum com bônus extra até dia 30`]});
  }
  let score=50+F.length*8-W.length*7+O.length*3-T.length*6;
  score=Math.max(5,Math.min(100,score));
  return{F,W,O,T,score};
}

function buildSWOT(){
  const d=generateSWOT();
  const sc=d.score>=70?'var(--green)':d.score>=40?'var(--gold)':'var(--coral)';
  const sl=d.score>=70?'Operação Saudável':d.score>=40?'Atenção Necessária':'Risco Alto — Ação Imediata';
  document.getElementById('swot-health').innerHTML=`<div class="health-bar-wrap"><div style="display:flex;align-items:center;gap:24px;flex-wrap:wrap"><div><div style="font-size:11px;color:var(--t3);text-transform:uppercase;letter-spacing:1px;margin-bottom:4px">Score de Saúde Operacional</div><div style="font-size:52px;font-weight:900;color:${sc};line-height:1">${d.score}<span style="font-size:22px;color:var(--t3)">/100</span></div><div style="font-size:14px;font-weight:700;color:${sc};margin-top:6px">${sl}</div></div><div style="flex:1;min-width:200px"><div style="height:10px;background:rgba(0,0,0,0.08);border-radius:5px;margin-bottom:14px"><div style="width:${d.score}%;height:10px;background:${sc};border-radius:5px;transition:.8s"></div></div><div style="display:grid;grid-template-columns:repeat(4,1fr);gap:8px;text-align:center"><div style="background:rgba(0,208,132,0.08);border:1px solid rgba(0,208,132,0.2);border-radius:8px;padding:10px"><div style="font-size:22px;font-weight:800;color:var(--green)">${d.F.length}</div><div style="font-size:10px;color:var(--t3);margin-top:2px">Forças</div></div><div style="background:rgba(255,107,53,0.08);border:1px solid rgba(255,107,53,0.2);border-radius:8px;padding:10px"><div style="font-size:22px;font-weight:800;color:var(--coral)">${d.W.length}</div><div style="font-size:10px;color:var(--t3);margin-top:2px">Fraquezas</div></div><div style="background:rgba(0,201,212,0.08);border:1px solid rgba(0,201,212,0.2);border-radius:8px;padding:10px"><div style="font-size:22px;font-weight:800;color:var(--aqua)">${d.O.length}</div><div style="font-size:10px;color:var(--t3);margin-top:2px">Oportunidades</div></div><div style="background:rgba(240,165,0,0.08);border:1px solid rgba(240,165,0,0.2);border-radius:8px;padding:10px"><div style="font-size:22px;font-weight:800;color:var(--gold)">${d.T.length}</div><div style="font-size:10px;color:var(--t3);margin-top:2px">Ameaças</div></div></div></div></div></div>`;
  document.getElementById('swot-health').style.display='block';
  function ri(items,pfx,showP){
    if(!items.length)return`<div style="text-align:center;padding:16px;color:var(--t3);font-size:13px">Nenhum item identificado ✓</div>`;
    return items.map((it,i)=>{const k=pfx+'_'+i;return`<div class="swot-item"><div class="swot-item-hdr"><div class="swot-item-icon">${it.i}</div><div style="flex:1"><div class="swot-item-title">${it.t}</div><div class="swot-item-desc">${it.d}</div>${it.p&&showP?`<span class="swot-plano-toggle" onclick="toggleSP('${k}')">📋 Plano de Ação ▼</span><div class="swot-plano" id="sp-${k}"><ul>${it.p.map(a=>`<li>${a}</li>`).join('')}</ul></div>`:''}</div></div></div>`;}).join('');
  }
  document.getElementById('sq-F').innerHTML=ri(d.F,'F',false);
  document.getElementById('sq-W').innerHTML=ri(d.W,'W',true);
  document.getElementById('sq-O').innerHTML=ri(d.O,'O',true);
  document.getElementById('sq-T').innerHTML=ri(d.T,'T',true);
  const probs=[...d.W,...d.T].filter(p=>p.p);
  document.getElementById('swot-action-plan').innerHTML=probs.length?`<div class="card" style="margin-top:6px"><div class="card-header"><div class="card-title">🎯 Plano de Ação Consolidado — Prioridades Imediatas</div></div><div style="display:flex;flex-direction:column;gap:12px">${probs.map((p,i)=>`<div style="background:var(--dark);border:1px solid var(--border);border-radius:10px;padding:14px"><div style="display:flex;align-items:center;gap:8px;margin-bottom:10px"><div style="width:24px;height:24px;background:rgba(0,201,212,0.15);border:1px solid var(--aqua);border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:11px;font-weight:800;color:var(--aqua);flex-shrink:0">${i+1}</div><div style="font-weight:700;font-size:13px">${p.i} ${p.t}</div></div><div style="display:flex;flex-direction:column;gap:6px;padding-left:32px">${p.p.map((a,j)=>`<div style="display:flex;gap:8px;font-size:12px;color:var(--t1)"><span style="color:var(--aqua);font-weight:700;flex-shrink:0">${j+1}.</span><span>${a}</span></div>`).join('')}</div></div>`).join('')}</div></div>`:'';
  document.getElementById('swot-content').style.display='block';
  document.getElementById('swot-placeholder').style.display='none';
  document.getElementById('swot-date').textContent='Gerado em '+new Date().toLocaleString('pt-BR');
}

function toggleSP(k){const el=document.getElementById('sp-'+k);if(el)el.classList.toggle('open');}

// ─── KPI QUICK EDIT ────────────────────────────────────
let kpiPausedUntil=0;
function openKpiEdit(key){
  const labels={vendas:'Cotas Vendidas',leads:'Leads Captados'};
  const metaNames={vendas:'Cotas Vendidas',leads:'Leads Captados'};
  const m=S.metas.find(x=>x.nome===metaNames[key]);
  document.getElementById('kpi-edit-key').value=key;
  document.getElementById('m-kpi-edit-title').textContent='✏️ Editar — '+(labels[key]||key);
  document.getElementById('kpi-edit-label').textContent='Valor Atual ('+labels[key]+')';
  document.getElementById('kpi-edit-val').value=m?m.real:0;
  document.getElementById('kpi-edit-meta').value=m?m.mensal:0;
  openModal('m-kpi-edit');
}
function saveKpiEdit(){
  const key=document.getElementById('kpi-edit-key').value;
  const val=+document.getElementById('kpi-edit-val').value||0;
  const meta=+document.getElementById('kpi-edit-meta').value||0;
  const metaNames={vendas:'Cotas Vendidas',leads:'Leads Captados'};
  const m=S.metas.find(x=>x.nome===metaNames[key]);
  if(m){m.real=val;if(meta>0)m.mensal=meta;}
  save();closeModal('m-kpi-edit');
  kpiPausedUntil=Date.now()+300000;
  updateDashKpis();updateSidebar();
}

// ─── CONECTOR API ───────────────────────────────────────
let connTimer=null;
if(!S.connConfig)S.connConfig={url:'',apiKey:'',interval:0,mapCotas:'',mapLeads:'',mapInd:'',mapQlf:''};

function getNestedVal(obj,path){
  if(!path)return undefined;
  return path.split('.').reduce((o,k)=>o&&o[k]!==undefined?o[k]:undefined,obj);
}
function connLog(msg){
  const el=document.getElementById('conn-log');
  if(!el)return;
  const t=new Date().toLocaleTimeString('pt-BR');
  el.innerHTML=`[${t}] ${msg}\n`+el.innerHTML;
}
function clearConnLog(){const el=document.getElementById('conn-log');if(el)el.innerHTML='Log limpo.';}
function setConnStatus(state,txt){
  const el=document.getElementById('conn-status-badge');
  if(!el)return;
  el.className='conn-status '+(state==='ok'?'conn-ok':state==='err'?'conn-err':'conn-idle');
  el.innerHTML=`<span class="conn-dot"></span>${txt}`;
}
function renderConnConfig(){
  const el=document.getElementById('conn-config-display');if(!el)return;
  const c=S.connConfig;
  if(!c.url){el.innerHTML='<div style="text-align:center;padding:20px;color:var(--t3)">Nenhuma configuração salva.<br>Clique em "Configurar" para começar.</div>';return;}
  el.innerHTML=`
    <div style="display:flex;flex-direction:column;gap:8px;font-size:13px">
      <div><strong style="color:var(--t2)">URL:</strong> <span style="word-break:break-all">${c.url}</span></div>
      <div><strong style="color:var(--t2)">Auth:</strong> ${c.apiKey?'••••••••••':'Não configurado'}</div>
      <div><strong style="color:var(--t2)">Cotas →</strong> ${c.mapCotas||'—'}</div>
      <div><strong style="color:var(--t2)">Leads →</strong> ${c.mapLeads||'—'}</div>
      ${c.mapInd?`<div><strong style="color:var(--t2)">Indicações →</strong> ${c.mapInd}</div>`:''}
      ${c.mapQlf?`<div><strong style="color:var(--t2)">Qualificados →</strong> ${c.mapQlf}</div>`:''}
      <div><strong style="color:var(--t2)">Auto-sync:</strong> ${c.interval>0?(c.interval/60)+' min':'Desativado'}</div>
    </div>`;
  const intEl=document.getElementById('conn-interval-display');
  if(intEl)intEl.textContent=c.interval>0?(c.interval/60)+' minuto(s)':'Desativado';
  const tog=document.getElementById('conn-auto-toggle');
  if(tog)tog.checked=c.interval>0;
}
function openModal_conector(){
  const c=S.connConfig;
  document.getElementById('conn-url').value=c.url||'';
  document.getElementById('conn-apikey').value=c.apiKey||'';
  document.getElementById('conn-interval').value=c.interval||0;
  document.getElementById('conn-map-cotas').value=c.mapCotas||'';
  document.getElementById('conn-map-leads').value=c.mapLeads||'';
  document.getElementById('conn-map-ind').value=c.mapInd||'';
  document.getElementById('conn-map-qlf').value=c.mapQlf||'';
  openModal('m-conector');
}
function saveConnConfig(){
  S.connConfig={
    url:document.getElementById('conn-url').value.trim(),
    apiKey:document.getElementById('conn-apikey').value.trim(),
    interval:+document.getElementById('conn-interval').value||0,
    mapCotas:document.getElementById('conn-map-cotas').value.trim(),
    mapLeads:document.getElementById('conn-map-leads').value.trim(),
    mapInd:document.getElementById('conn-map-ind').value.trim(),
    mapQlf:document.getElementById('conn-map-qlf').value.trim(),
  };
  save();closeModal('m-conector');renderConnConfig();
  setupAutoSync();
  connLog('✅ Configuração salva.');
  setConnStatus('idle','Configurado');
}
function toggleAutoSync(on){
  S.connConfig.interval=on?300:0;save();
  setupAutoSync();renderConnConfig();
  connLog(on?'🔄 Auto-sync ativado.':'⏹ Auto-sync desativado.');
}
function setupAutoSync(){
  if(connTimer){clearInterval(connTimer);connTimer=null;}
  const iv=S.connConfig.interval;
  if(iv>0)connTimer=setInterval(connSync,iv*1000);
}
async function connSync(){
  const c=S.connConfig;
  if(!c.url){connLog('⚠️ Configure o endpoint primeiro.');return;}
  connLog('🔄 Sincronizando...');setConnStatus('idle','Sincronizando…');
  try{
    const headers={'Content-Type':'application/json'};
    if(c.apiKey)headers['Authorization']=c.apiKey;
    const res=await fetch(c.url,{headers,mode:'cors'});
    if(!res.ok)throw new Error('HTTP '+res.status);
    const data=await res.json();
    let updated=[];
    if(c.mapCotas){const v=getNestedVal(data,c.mapCotas);if(v!==undefined){const m=S.metas.find(x=>x.nome==='Cotas Vendidas');if(m){m.real=+v;updated.push('Cotas='+v);}}}
    if(c.mapLeads){const v=getNestedVal(data,c.mapLeads);if(v!==undefined){const m=S.metas.find(x=>x.nome==='Leads Captados');if(m){m.real=+v;updated.push('Leads='+v);}}}
    if(c.mapInd){const v=getNestedVal(data,c.mapInd);if(v!==undefined){const m=S.metas.find(x=>x.nome==='Cotas via Indicação');if(m){m.real=+v;updated.push('Indicações='+v);}}}
    if(c.mapQlf){const v=getNestedVal(data,c.mapQlf);if(v!==undefined){const m=S.metas.find(x=>x.nome==='Leads Qualificados');if(m){m.real=+v;updated.push('Qualif.='+v);}}}
    save();kpiPausedUntil=Date.now()+300000;
    updateDashKpis();updateSidebar();
    const ts=new Date().toLocaleString('pt-BR');
    const el=document.getElementById('conn-last-sync');if(el)el.textContent=ts;
    connLog('✅ Sucesso — '+( updated.length?updated.join(', '):'nenhum campo mapeado'));
    setConnStatus('ok','Conectado');
  }catch(e){
    connLog('❌ Erro: '+e.message);
    setConnStatus('err','Erro de conexão');
  }
}
async function connTest(){
  const url=(document.getElementById('conn-url')||{value:''}).value||S.connConfig.url;
  const key=(document.getElementById('conn-apikey')||{value:''}).value||S.connConfig.apiKey;
  if(!url){alert('Informe a URL do endpoint.');return;}
  connLog('🧪 Testando conexão...');
  try{
    const headers={'Content-Type':'application/json'};
    if(key)headers['Authorization']=key;
    const res=await fetch(url,{headers,mode:'cors'});
    const txt=await res.text();
    connLog(`🧪 Resposta HTTP ${res.status}: ${txt.slice(0,200)}`);
    if(res.ok)setConnStatus('ok','Teste OK');else setConnStatus('err','Teste falhou ('+res.status+')');
  }catch(e){
    connLog('❌ Teste falhou: '+e.message+' (verifique CORS e URL)');
    setConnStatus('err','Falhou');
  }
}

// ─── LIVE UPDATE ───────────────────────────────────────
function liveUpdate(){
  if(Date.now()<kpiPausedUntil)return;
  const mv=S.metas.find(m=>m.nome==='Cotas Vendidas');
  const ml=S.metas.find(m=>m.nome==='Leads Captados');
  if(mv&&Math.random()>.6){mv.real++;save();updateDashKpis();updateSidebar();}
  if(ml&&Math.random()>.5){ml.real+=Math.floor(Math.random()*3)+1;save();updateDashKpis();}
}

// ─── INIT ──────────────────────────────────────────────
document.addEventListener('DOMContentLoaded',()=>{
  populateVendedorSelect();
  updateSidebar();
  updateDashKpis();
  setTimeout(initDashCharts,120);
  setInterval(liveUpdate,5000);
  renderScripts();
  renderPlanos();
  renderConnConfig();
  setupAutoSync();
  document.querySelector('.btn-primary[onclick*="m-lead"]').onclick=openNewLead;
});
</script>
</body>
</html>
