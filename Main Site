# Site-Fiu-0.885
Site de estudo para a minha academia
<!DOCTYPE html>
<html lang="pt-BR" data-theme="dark">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>FIU Capoeira — Gestão</title>
<link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700;900&family=Barlow:ital,wght@0,300;0,400;0,500;0,600;0,700;1,400&family=Barlow+Condensed:wght@500;700;900&display=swap" rel="stylesheet"/>
<style>
/* ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ */
:root{
  --g1:#079d28; --g2:#4ebe6a; --g3:#d4f5da;
  --y1:#c89a00; --y2:#f9d441; --y3:#fef9d0;
  --b1:#073e8e; --b2:#4a7acc; --b3:#dde8f8;
  --r1:#b83530; --r2:#e06060;
}

/* DARK */
[data-theme="dark"]{
  --bg:    #07090a;
  --bg2:   #0c1210;
  --surf:  #111916;
  --surf2: #192220;
  --bord:  #213028;
  --bord2: #2d4038;
  --txt:   #eef4ef;
  --txt2:  #b0c4b8;
  --mute:  #6a8872;
  --acc:   #f9d441;
  --acc2:  #4ebe6a;
  --ok-bg: rgba(7,157,40,.12); --ok-bd:rgba(78,190,106,.3);  --ok-tx:#4ebe6a;
  --wn-bg: rgba(200,154,0,.12);--wn-bd:rgba(249,212,65,.28); --wn-tx:#f9d441;
  --er-bg: rgba(184,53,48,.12);--er-bd:rgba(224,96,96,.28);  --er-tx:#e06060;
  --in-bg: rgba(7,62,142,.12); --in-bd:rgba(74,122,204,.28); --in-tx:#4a7acc;
  --shad:  rgba(0,0,0,.4);
  --shad2: rgba(0,0,0,.65);
  --over:  rgba(7,9,10,.88);
  --scrl:  #2d4038;
}
/* LIGHT */
[data-theme="light"]{
  --bg:    #f2f5f2;
  --bg2:   #e8ede8;
  --surf:  #ffffff;
  --surf2: #edf3ed;
  --bord:  #ccd8cc;
  --bord2: #b0c8b4;
  --txt:   #162018;
  --txt2:  #3a5040;
  --mute:  #6a8870;
  --acc:   #b08800;
  --acc2:  #079d28;
  --ok-bg: rgba(7,157,40,.08); --ok-bd:rgba(7,157,40,.22);  --ok-tx:#079d28;
  --wn-bg: rgba(200,154,0,.08);--wn-bd:rgba(200,154,0,.25); --wn-tx:#a07800;
  --er-bg: rgba(184,53,48,.08);--er-bd:rgba(184,53,48,.22); --er-tx:#b83530;
  --in-bg: rgba(7,62,142,.08); --in-bd:rgba(7,62,142,.2);   --in-tx:#073e8e;
  --shad:  rgba(0,0,0,.08);
  --shad2: rgba(0,0,0,.14);
  --over:  rgba(242,245,242,.92);
  --scrl:  #b0c8b4;
}

/* ━━━━━━━━━━━━━━━━━━━━ RESET ━━━━━━━━━━━━━━━━━━━━ */
*,*::before,*::after{margin:0;padding:0;box-sizing:border-box;}
html{scroll-behavior:smooth;}
body{
  font-family:'Barlow',sans-serif;
  background:var(--bg);color:var(--txt);
  min-height:100vh;transition:background .25s,color .25s;
}
*::-webkit-scrollbar{width:5px;height:5px;}
*::-webkit-scrollbar-track{background:transparent;}
*::-webkit-scrollbar-thumb{background:var(--scrl);border-radius:4px;}

/* ━━━━━━━━━━━━━━━━━━━━ NAV ━━━━━━━━━━━━━━━━━━━━ */
/* ━━━━━━━━━━━━━━━━━━━━ SIDEBAR ━━━━━━━━━━━━━━━━━━━━ */
.sidebar{
  position:fixed;top:0;left:0;bottom:0;z-index:300;
  width:222px;background:var(--surf);border-right:1px solid var(--bord);
  display:flex;flex-direction:column;
  transition:width .22s,transform .25s,background .25s,border-color .25s;
  box-shadow:2px 0 16px var(--shad);
}
body.sidebar-collapsed .sidebar{width:64px;}
.sidebar-head{
  display:flex;align-items:center;justify-content:space-between;gap:6px;
  padding:14px 12px;border-bottom:1px solid var(--bord);flex-shrink:0;min-height:60px;
}
body.sidebar-collapsed .sidebar-head{padding:14px 8px;}
.nav-brand{
  display:flex;align-items:center;gap:9px;
  text-decoration:none;flex-shrink:1;overflow:hidden;min-width:0;
}
.nav-brand img{
  width:36px;height:36px;object-fit:contain;border-radius:50%;flex-shrink:0;
  border:1.5px solid rgba(7,157,40,.35);
  box-shadow:0 0 10px rgba(7,157,40,.2);
  transition:box-shadow .2s;
}
.nav-brand:hover img{box-shadow:0 0 18px rgba(7,157,40,.4);}
.nav-brand-text{overflow:hidden;white-space:nowrap;transition:opacity .15s;}
body.sidebar-collapsed .nav-brand-text{display:none;}
.nb-name{
  font-family:'Cinzel',serif;font-size:.8rem;font-weight:700;
  color:var(--acc);letter-spacing:.05em;line-height:1.2;
}
.nb-sub{
  font-size:.5rem;letter-spacing:.2em;text-transform:uppercase;
  color:var(--acc2);font-weight:600;margin-top:1px;
}
.sidebar-collapse-btn{
  width:26px;height:26px;border-radius:7px;flex-shrink:0;
  background:var(--surf2);border:1px solid var(--bord);color:var(--txt2);
  display:flex;align-items:center;justify-content:center;cursor:pointer;transition:all .18s;
}
.sidebar-collapse-btn:hover{border-color:var(--acc);color:var(--acc);}
.sidebar-collapse-btn svg{width:13px;height:13px;transition:transform .22s;display:block;}
body.sidebar-collapsed .sidebar-collapse-btn svg{transform:rotate(180deg);}
.nav-tabs{
  flex:1;display:flex;flex-direction:column;gap:2px;
  padding:10px;overflow-y:auto;overflow-x:hidden;scrollbar-width:none;
}
.nav-tabs::-webkit-scrollbar{display:none;}
.nav-divider{width:auto;height:1px;background:var(--bord2);flex-shrink:0;margin:6px 6px;}
.ntab{
  display:flex;align-items:center;gap:11px;
  padding:10px 12px;height:auto;border-radius:9px;width:100%;text-align:left;
  font-size:.7rem;font-weight:700;letter-spacing:.05em;text-transform:uppercase;
  border:none;background:transparent;color:var(--mute);
  cursor:pointer;transition:all .18s;white-space:nowrap;position:relative;
}
body.sidebar-collapsed .ntab{justify-content:center;padding:10px 0;}
.ntab:hover{background:var(--surf2);color:var(--txt);}
.ntab.active{
  background:linear-gradient(135deg,var(--g1) 0%,var(--b1) 100%);
  color:#fff;box-shadow:0 2px 10px rgba(7,157,40,.28);
}
.ntab-ic{
  width:16px;height:16px;flex-shrink:0;
  display:inline-flex;align-items:center;justify-content:center;
  opacity:.85;position:relative;
}
.ntab-ic svg{width:100%;height:100%;display:block;}
.ntab.active .ntab-ic{opacity:1;}
.ntab-label{overflow:hidden;text-overflow:ellipsis;}
body.sidebar-collapsed .ntab-label{display:none;}
body.sidebar-collapsed .notif-badge{top:-3px;right:-3px;}
.sidebar-toggle-mobile{
  display:none;width:36px;height:36px;border-radius:8px;flex-shrink:0;
  background:var(--surf2);border:1px solid var(--bord);color:var(--txt2);
  align-items:center;justify-content:center;cursor:pointer;
}
.sidebar-overlay{display:none;position:fixed;inset:0;background:rgba(0,0,0,.5);z-index:290;}
.sidebar-overlay.show{display:block;}

/* ━━━━━━━━━━━━━━━━━━━━ TOPBAR + MAIN WRAP ━━━━━━━━━━━━━━━━━━━━ */
.main-wrap{margin-left:222px;min-height:100vh;transition:margin-left .22s;}
body.sidebar-collapsed .main-wrap{margin-left:64px;}
.topbar{
  height:60px;display:flex;align-items:center;justify-content:space-between;gap:10px;
  padding:0 20px;background:var(--surf);border-bottom:1px solid var(--bord);
  position:sticky;top:0;z-index:200;box-shadow:0 2px 16px var(--shad);
  transition:background .25s,border-color .25s;
}
.topbar-title{
  font-family:'Cinzel',serif;font-size:1rem;font-weight:700;color:var(--txt);
  display:flex;align-items:center;gap:10px;min-width:0;
}
.nav-right{display:flex;align-items:center;gap:7px;margin-left:auto;flex-shrink:0;}
.icon-btn{
  width:34px;height:34px;border-radius:8px;
  background:var(--surf2);border:1px solid var(--bord);
  color:var(--txt2);cursor:pointer;font-size:.95rem;
  transition:all .18s;display:flex;align-items:center;justify-content:center;
}
.icon-btn svg{width:18px;height:18px;display:block;}
.icon-btn:hover{border-color:var(--acc);color:var(--acc);}
.role-pill{
  display:flex;align-items:center;gap:6px;
  padding:5px 11px;border-radius:20px;
  background:var(--surf2);border:1px solid var(--bord2);
  font-size:.66rem;font-weight:700;letter-spacing:.07em;text-transform:uppercase;
  color:var(--txt2);cursor:pointer;transition:all .18s;white-space:nowrap;
}
.role-pill:hover{border-color:var(--r2);color:var(--r2);}
.rdot{width:7px;height:7px;border-radius:50%;flex-shrink:0;}

/* ━━━━━━━━━━━━━━━━━━━━ NOTIFICAÇÕES ━━━━━━━━━━━━━━━━━━━━ */
/* ━━━━━━━━━━━━━━━━━━━━ ÍCONE DE CORDA (nav) ━━━━━━━━━━━━━━━━━━━━ */
.corda-icon{
  display:inline-flex;align-items:center;justify-content:center;
  width:15px;height:15px;flex-shrink:0;
  --corda-c1:#c8b878;--corda-c2:#b0a060;
  filter:drop-shadow(0 1px 1px rgba(0,0,0,.25));
}
.corda-icon svg{display:block;width:100%;height:100%;}
.corda-icon .rope-strand-a{fill:var(--corda-c1);}
.corda-icon .rope-strand-b{fill:var(--corda-c2);}

.notif-wrap{position:relative;}
.notif-badge{
  position:absolute;top:-4px;right:-4px;
  min-width:16px;height:16px;padding:0 3px;border-radius:9px;
  background:var(--r1);border:1.5px solid var(--surf);
  color:#fff;font-size:.58rem;font-weight:900;
  display:flex;align-items:center;justify-content:center;
  line-height:1;font-family:'Barlow Condensed',sans-serif;
}
.notif-badge.hidden{display:none;}
.notif-panel{
  position:absolute;top:46px;right:0;z-index:400;
  width:360px;max-width:92vw;max-height:78vh;
  background:var(--surf);border:1px solid var(--bord2);border-radius:14px;
  box-shadow:0 16px 50px var(--shad2);
  display:flex;flex-direction:column;overflow:hidden;
  opacity:0;transform:translateY(-8px) scale(.97);pointer-events:none;
  transition:opacity .18s,transform .18s;
}
.notif-panel.open{opacity:1;transform:translateY(0) scale(1);pointer-events:all;}
.notif-head{
  padding:16px 18px 12px;border-bottom:1px solid var(--bord);
  display:flex;align-items:flex-start;justify-content:space-between;
}
.notif-head-title{
  font-family:'Cinzel',serif;font-size:.92rem;font-weight:900;
  letter-spacing:.08em;text-transform:uppercase;color:var(--txt);
  display:flex;align-items:center;gap:7px;
}
.notif-head-sub{font-size:.64rem;letter-spacing:.1em;text-transform:uppercase;color:var(--mute);margin-top:2px;}
.notif-close{background:none;border:none;color:var(--mute);cursor:pointer;font-size:1.05rem;line-height:1;padding:2px;transition:color .15s;}
.notif-close:hover{color:var(--txt);}
.notif-actions{
  display:flex;align-items:center;gap:8px;
  padding:11px 18px;border-bottom:1px solid var(--bord);
}
.notif-newbtn{
  flex:1;display:flex;align-items:center;justify-content:center;gap:6px;
  padding:9px 12px;border-radius:9px;
  background:linear-gradient(135deg,var(--g1),#0a7820);border:1px solid var(--g2);
  color:#fff;font-family:'Barlow Condensed',sans-serif;font-size:.74rem;font-weight:900;
  letter-spacing:.1em;text-transform:uppercase;cursor:pointer;transition:all .2s;
}
.notif-newbtn:hover{filter:brightness(1.1);transform:translateY(-1px);}
.notif-iconbtn{
  width:34px;height:34px;border-radius:8px;flex-shrink:0;
  background:var(--surf2);border:1px solid var(--bord);color:var(--txt2);
  display:flex;align-items:center;justify-content:center;cursor:pointer;
  font-size:.85rem;transition:all .15s;
}
.notif-iconbtn:hover{border-color:var(--acc);color:var(--acc);}
.notif-list{flex:1;overflow-y:auto;max-height:420px;}
.notif-item{
  display:flex;gap:11px;padding:13px 18px;border-bottom:1px solid var(--bord);
  cursor:pointer;transition:background .15s;position:relative;
}
.notif-item:hover{background:var(--surf2);}
.notif-item:last-child{border-bottom:none;}
.notif-item.unread::before{
  content:'';position:absolute;left:6px;top:50%;transform:translateY(-50%);
  width:6px;height:6px;border-radius:50%;background:var(--acc2);box-shadow:0 0 6px var(--acc2);
}
.notif-ic{
  width:38px;height:38px;border-radius:9px;flex-shrink:0;
  display:flex;align-items:center;justify-content:center;font-size:1.05rem;
}
.notif-body{flex:1;min-width:0;}
.notif-title{font-size:.82rem;font-weight:700;color:var(--txt);line-height:1.3;}
.notif-sub{font-size:.74rem;color:var(--txt2);margin-top:1px;line-height:1.35;}
.notif-time{font-size:.62rem;color:var(--mute);letter-spacing:.05em;text-transform:uppercase;margin-top:5px;}
.notif-del{
  background:none;border:none;color:var(--bord2);cursor:pointer;font-size:.85rem;
  padding:2px 4px;flex-shrink:0;opacity:0;transition:opacity .15s,color .15s;align-self:center;
}
.notif-item:hover .notif-del{opacity:1;}
.notif-del:hover{color:var(--er-tx);}
.notif-empty{text-align:center;padding:40px 20px;color:var(--mute);}
.notif-empty .ne-icon{width:36px;height:36px;margin:0 auto 8px;opacity:.35;}
.notif-empty .ne-icon svg{width:100%;height:100%;display:block;}
@media(max-width:640px){
  .notif-panel{position:fixed;top:64px;right:8px;left:8px;width:auto;}
}

/* ━━━━━━━━━━━━━━━━━━━━ LAYOUT ━━━━━━━━━━━━━━━━━━━━ */
.app{min-height:calc(100vh - 60px);}
.page{display:none;padding:26px 28px 80px;animation:fadeUp .22s ease;}
.page.active{display:block;}
@keyframes fadeUp{from{opacity:0;transform:translateY(8px);}to{opacity:1;transform:translateY(0);}}

/* ━━━━━━━━━━━━━━━━━━━━ COMPONENTS ━━━━━━━━━━━━━━━━━━━━ */
/* Page header */
.ph{
  display:flex;align-items:flex-start;justify-content:space-between;
  flex-wrap:wrap;gap:10px;margin-bottom:22px;
  padding-bottom:16px;border-bottom:1px solid var(--bord);
}
.ph-left h1{
  font-family:'Cinzel',serif;font-size:1.5rem;font-weight:900;color:var(--txt);
}
.ph-left h1 span{
  background:linear-gradient(90deg,var(--g1),var(--y2));
  -webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;
}
.ph-left p{font-size:.8rem;color:var(--mute);margin-top:3px;}
.ph-right{display:flex;gap:6px;align-items:center;flex-wrap:wrap;}

/* Card */
.card{
  background:var(--surf);border:1px solid var(--bord);border-radius:10px;
  padding:18px;box-shadow:0 2px 8px var(--shad);transition:background .25s,border-color .25s;
}
.card-tit{
  font-family:'Barlow Condensed',sans-serif;font-size:.66rem;font-weight:900;
  letter-spacing:.2em;text-transform:uppercase;color:var(--mute);
  margin-bottom:12px;padding-bottom:9px;border-bottom:1px solid var(--bord);
}

/* Buttons */
.btn{
  display:inline-flex;align-items:center;gap:5px;
  padding:8px 15px;border-radius:7px;
  font-family:'Barlow',sans-serif;font-size:.7rem;font-weight:700;
  letter-spacing:.07em;text-transform:uppercase;
  border:1px solid transparent;cursor:pointer;transition:all .2s;white-space:nowrap;
}
.btn-g{background:linear-gradient(135deg,var(--g1),#0a7820);border-color:var(--g2);color:#fff;box-shadow:0 2px 8px rgba(7,157,40,.22);}
.btn-g:hover{filter:brightness(1.12);transform:translateY(-1px);box-shadow:0 4px 14px rgba(7,157,40,.3);}
.btn-y{background:linear-gradient(135deg,var(--y1),#a07800);border-color:var(--y2);color:#fff;box-shadow:0 2px 8px rgba(200,154,0,.2);}
.btn-y:hover{filter:brightness(1.1);transform:translateY(-1px);}
.btn-b{background:linear-gradient(135deg,var(--b1),#0a3070);border-color:var(--b2);color:#fff;}
.btn-b:hover{filter:brightness(1.12);transform:translateY(-1px);}
.btn-ghost{background:transparent;border-color:var(--bord2);color:var(--txt2);}
.btn-ghost:hover{border-color:var(--acc);color:var(--acc);}
.btn-red{background:var(--er-bg);border-color:var(--er-bd);color:var(--er-tx);}
.btn-red:hover{background:rgba(184,53,48,.22);}
.btn-sm{padding:5px 11px;font-size:.64rem;}
.btn-xs{padding:3px 8px;font-size:.6rem;}

/* Inputs */
.fg{margin-bottom:12px;}
.fg label{display:block;font-size:.64rem;font-weight:700;letter-spacing:.1em;text-transform:uppercase;color:var(--txt2);margin-bottom:4px;}
.inp{
  width:100%;padding:9px 11px;
  background:var(--bg2);border:1.5px solid var(--bord);border-radius:7px;
  color:var(--txt);font-family:'Barlow',sans-serif;font-size:.87rem;
  outline:none;transition:border-color .2s,box-shadow .2s;
}
.inp:focus{border-color:var(--y2);box-shadow:0 0 0 3px rgba(249,212,65,.07);}
.inp::placeholder{color:var(--mute);}
.inp option{background:var(--surf);}
.g2{display:grid;grid-template-columns:1fr 1fr;gap:10px;}
.g3{display:grid;grid-template-columns:1fr 1fr 1fr;gap:10px;}

/* Pills */
.pill{
  display:inline-flex;align-items:center;gap:3px;
  padding:2px 8px;border-radius:20px;
  font-size:.6rem;font-weight:700;letter-spacing:.07em;text-transform:uppercase;
}
.p-ok  {background:var(--ok-bg);border:1px solid var(--ok-bd);color:var(--ok-tx);}
.p-warn{background:var(--wn-bg);border:1px solid var(--wn-bd);color:var(--wn-tx);}
.p-err {background:var(--er-bg);border:1px solid var(--er-bd);color:var(--er-tx);}
.p-info{background:var(--in-bg);border:1px solid var(--in-bd);color:var(--in-tx);}
.p-mute{background:var(--surf2);border:1px solid var(--bord);color:var(--mute);}

/* Stat boxes */
.stat-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(110px,1fr));gap:8px;}
.sbox{
  background:var(--surf2);border:1px solid var(--bord);border-radius:8px;
  padding:12px;text-align:center;transition:all .18s;
}
.sbox:hover{border-color:var(--bord2);transform:translateY(-1px);}
.snum{font-family:'Cinzel',serif;font-size:1.5rem;font-weight:900;line-height:1;color:var(--acc);}
.slbl{font-size:.58rem;letter-spacing:.1em;text-transform:uppercase;color:var(--mute);margin-top:4px;}

/* Progress bar */
.pbar-wrap{margin-bottom:7px;}
.pbar-row{display:flex;justify-content:space-between;font-size:.65rem;color:var(--txt2);margin-bottom:3px;}
.pbar{height:5px;background:var(--bord);border-radius:3px;overflow:hidden;}
.pbar-fill{height:100%;border-radius:3px;transition:width .5s;}

/* Modal */
.modal-ov{
  position:fixed;inset:0;z-index:500;
  background:var(--over);backdrop-filter:blur(5px);
  display:flex;align-items:center;justify-content:center;
  opacity:0;pointer-events:none;transition:opacity .2s;
}
.modal-ov.open{opacity:1;pointer-events:all;}
.modal{
  background:var(--surf);border:1px solid var(--bord2);border-radius:12px;
  padding:26px;width:90%;max-width:500px;max-height:90vh;overflow-y:auto;
  box-shadow:0 20px 60px var(--shad2);
  transform:translateY(16px) scale(.97);transition:all .22s;
}
.modal-ov.open .modal{transform:translateY(0) scale(1);}
.modal h2{font-family:'Cinzel',serif;font-size:1.05rem;font-weight:900;color:var(--acc);margin-bottom:16px;}
.modal-act{display:flex;gap:8px;justify-content:flex-end;margin-top:16px;}

/* Toast */
.toast-el{
  position:fixed;bottom:22px;right:22px;z-index:600;
  padding:10px 18px;border-radius:8px;
  font-size:.78rem;font-weight:600;color:#fff;
  transform:translateY(50px);opacity:0;transition:all .3s;pointer-events:none;
  box-shadow:0 4px 20px rgba(0,0,0,.3);
  background:var(--g1);border:1px solid var(--g2);
}
.toast-el.show{transform:translateY(0);opacity:1;}
.toast-el.warn{background:var(--y1);border-color:var(--y2);}
.toast-el.err {background:var(--r1);border-color:var(--r2);}

/* ━━━━━━━━━━━━━━━━━━━━ PRESENÇA ━━━━━━━━━━━━━━━━━━━━ */
.pres-grid{display:grid;grid-template-columns:268px 1fr;gap:14px;align-items:start;}
.aluno-list{display:flex;flex-direction:column;gap:3px;max-height:calc(100vh - 228px);overflow-y:auto;}
.aitem{
  display:flex;align-items:center;gap:9px;
  padding:9px 11px;border-radius:8px;cursor:pointer;
  border:1.5px solid transparent;background:var(--bg2);transition:all .15s;
}
.aitem:hover{background:var(--surf2);border-color:var(--bord);}
.aitem.sel{background:var(--surf2);border-color:var(--g1);}
.av{
  width:34px;height:34px;border-radius:50%;
  display:flex;align-items:center;justify-content:center;
  font-family:'Cinzel',serif;font-size:.78rem;font-weight:900;
  color:#fff;flex-shrink:0;
}
.a-name{font-size:.84rem;font-weight:700;color:var(--txt);}
.a-cord{font-size:.61rem;letter-spacing:.06em;text-transform:uppercase;margin-top:1px;}

/* attend cols */
.att-cols{display:grid;grid-template-columns:1fr 310px;gap:12px;align-items:start;}
.right-col{display:flex;flex-direction:column;gap:10px;}

/* Calendar */
.cal-wrap{border-radius:10px;overflow:hidden;border:1px solid var(--bord);}
.cal-head{
  display:flex;align-items:center;justify-content:space-between;
  padding:11px 15px;background:var(--surf);border-bottom:1px solid var(--bord);
}
.cal-lbl{font-family:'Cinzel',serif;font-size:.92rem;font-weight:700;color:var(--acc);}
.cal-btn{
  width:28px;height:28px;border-radius:6px;
  background:var(--surf2);border:1px solid var(--bord);
  color:var(--txt2);cursor:pointer;font-size:.78rem;transition:all .15s;
}
.cal-btn:hover{border-color:var(--acc);color:var(--acc);}
.cal-body{background:var(--surf);padding:10px;}
.cal-grid{display:grid;grid-template-columns:repeat(7,1fr);gap:2px;}
.cal-dow{font-size:.57rem;font-weight:700;letter-spacing:.08em;text-transform:uppercase;color:var(--mute);text-align:center;padding:3px 0;}
.cday{
  aspect-ratio:1;display:flex;flex-direction:column;
  align-items:center;justify-content:center;
  font-size:.74rem;font-weight:600;border-radius:6px;
  cursor:pointer;border:1.5px solid transparent;transition:all .13s;
  color:var(--txt2);gap:1px;
}
.cday:hover:not(.emp):not(.fut){background:var(--surf2);border-color:var(--bord);}
.cday.emp,.cday.fut{cursor:default;color:var(--bord2);}
.cday.has-p{background:var(--ok-bg);border-color:var(--ok-bd);}
.cday.has-p .cdn{color:var(--ok-tx);}
.cday.has-a{background:var(--er-bg);border-color:var(--er-bd);}
.cday.has-a .cdn{color:var(--er-tx);}
.cday.has-m{background:var(--wn-bg);border-color:var(--wn-bd);}
.cday.has-m .cdn{color:var(--wn-tx);}
.cday.tod{box-shadow:0 0 0 2px var(--acc);}
.cday.tod .cdn{color:var(--acc);}
.cdn{line-height:1;}
.cdots{display:flex;gap:2px;flex-wrap:wrap;justify-content:center;max-width:22px;}
.cdot{width:3px;height:3px;border-radius:50%;}

/* Dia panel */
.dia-panel{
  background:var(--surf);border:1px solid var(--bord);border-radius:10px;
  padding:15px;margin-top:10px;
}
.dia-head{display:flex;align-items:center;justify-content:space-between;margin-bottom:10px;flex-wrap:wrap;gap:6px;}
.dia-ttl{font-family:'Cinzel',serif;font-size:.88rem;font-weight:700;}
.dia-ttl span{color:var(--acc);}
.aulas-list{display:flex;flex-direction:column;gap:4px;margin-bottom:10px;}
.aula-row{
  display:flex;align-items:center;gap:8px;
  padding:8px 11px;border-radius:7px;
  background:var(--bg2);border:1px solid var(--bord);transition:border-color .13s;
}
.aula-row:hover{border-color:var(--bord2);}
.aula-hora{font-family:'Barlow Condensed',sans-serif;font-size:.88rem;font-weight:900;color:var(--txt);min-width:82px;white-space:nowrap;}
.mod-badge{display:inline-block;padding:2px 8px;border-radius:5px;font-size:.62rem;font-weight:700;letter-spacing:.06em;text-transform:uppercase;}
.sp{padding:3px 9px;border-radius:5px;font-size:.62rem;font-weight:700;letter-spacing:.06em;text-transform:uppercase;cursor:pointer;transition:all .13s;white-space:nowrap;}
.sp-p{background:var(--ok-bg);border:1px solid var(--ok-bd);color:var(--ok-tx);}
.sp-a{background:var(--er-bg);border:1px solid var(--er-bd);color:var(--er-tx);}
.sp-n{background:var(--surf2);border:1px solid var(--bord2);color:var(--mute);}
.sp-p:hover,.sp-n:hover{background:var(--ok-bg);border-color:var(--ok-bd);color:var(--ok-tx);}
.sp-a:hover{background:rgba(184,53,48,.22);}
.adel{background:transparent;border:none;color:var(--bord2);cursor:pointer;font-size:.88rem;padding:2px 3px;transition:color .13s;}
.adel:hover{color:var(--er-tx);}
.log-list{display:flex;flex-direction:column;gap:3px;max-height:170px;overflow-y:auto;}
.lrow{display:flex;align-items:center;gap:6px;padding:5px 8px;background:var(--bg2);border-radius:5px;font-size:.72rem;}
.ldot{width:5px;height:5px;border-radius:50%;flex-shrink:0;}
.ldate{color:var(--txt2);min-width:66px;}
.ltime{color:var(--mute);min-width:72px;font-family:'Barlow Condensed',sans-serif;}
.lmod{flex:1;color:var(--mute);}
.lst{font-weight:700;}

/* ━━━━━━━━━━━━━━━━━━━━ ALUNOS GRID ━━━━━━━━━━━━━━━━━━━━ */
.alunos-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(255px,1fr));gap:12px;}
.acard{
  background:var(--surf);border:1px solid var(--bord);border-radius:10px;
  padding:16px;transition:all .2s;position:relative;overflow:hidden;
}
.acard::before{content:'';position:absolute;top:0;left:0;right:0;height:3px;background:var(--card-grad,linear-gradient(90deg,var(--g1),var(--y2)));}
.acard:hover{box-shadow:0 6px 24px var(--shad2);transform:translateY(-2px);}
.acard-top{display:flex;align-items:center;gap:10px;margin-bottom:12px;}
.acard-av{width:44px;height:44px;border-radius:50%;display:flex;align-items:center;justify-content:center;font-family:'Cinzel',serif;font-size:.9rem;font-weight:900;color:#fff;flex-shrink:0;}
.acard-name{font-family:'Cinzel',serif;font-size:.88rem;font-weight:700;color:var(--txt);}
.acard-meta{font-size:.66rem;color:var(--mute);margin-top:2px;}
.acard-pills{display:flex;gap:3px;flex-wrap:wrap;margin-bottom:9px;}
.acard-acts{display:flex;gap:4px;flex-wrap:wrap;margin-top:10px;}

/* ━━━━━━━━━━━━━━━━━━━━ PAGAMENTOS ━━━━━━━━━━━━━━━━━━━━ */
.pag-layout{display:grid;grid-template-columns:1fr 330px;gap:14px;align-items:start;}
.pag-filters{display:flex;gap:4px;margin-bottom:12px;flex-wrap:wrap;}
.ptab{padding:6px 14px;border-radius:6px;font-size:.66rem;font-weight:700;letter-spacing:.08em;text-transform:uppercase;border:1px solid var(--bord);background:transparent;color:var(--mute);cursor:pointer;font-family:'Barlow',sans-serif;transition:all .18s;}
.ptab:hover{border-color:var(--bord2);color:var(--txt);}
.ptab.active{background:linear-gradient(135deg,var(--y1),#8a6600);border-color:var(--y2);color:#fff;}
.ptable{width:100%;border-collapse:collapse;}
.ptable th{font-family:'Barlow Condensed',sans-serif;font-size:.64rem;font-weight:900;letter-spacing:.16em;text-transform:uppercase;color:var(--mute);padding:8px 13px;text-align:left;border-bottom:2px solid var(--bord);background:var(--surf2);}
.ptable td{padding:9px 13px;font-size:.8rem;border-bottom:1px solid var(--bord);color:var(--txt2);vertical-align:middle;}
.ptable tr:hover td{background:var(--surf2);}
.ptable tr.pok td{border-left:3px solid var(--g1);}
.ptable tr.pwn td{border-left:3px solid var(--y2);}
.ptable tr.per td{border-left:3px solid var(--r1);}
.pag-right{display:flex;flex-direction:column;gap:10px;}
.pres-boxes{display:grid;grid-template-columns:1fr 1fr;gap:7px;}
.pbox{background:var(--surf2);border:1px solid var(--bord);border-radius:8px;padding:12px;text-align:center;}
.pbox-num{font-family:'Cinzel',serif;font-size:1.4rem;font-weight:900;line-height:1;}
.pbox-lbl{font-size:.58rem;letter-spacing:.1em;text-transform:uppercase;color:var(--mute);margin-top:4px;}
.inadim{
  display:flex;align-items:center;gap:9px;padding:11px 14px;border-radius:8px;
  background:var(--er-bg);border:1px solid var(--er-bd);margin-bottom:12px;
  position:relative;overflow:hidden;
}
.inadim::before{content:'';position:absolute;left:0;top:0;bottom:0;width:3px;background:var(--r1);}

/* ━━━━━━━━━━━━━━━━━━━━ MENSAGENS (CHAT) ━━━━━━━━━━━━━━━━━━━━ */
.chat-layout{display:grid;grid-template-columns:280px 1fr;gap:14px;align-items:start;height:calc(100vh - 190px);min-height:420px;}
.chat-list-card{height:100%;display:flex;flex-direction:column;overflow:hidden;}
.chat-lista{flex:1;overflow-y:auto;display:flex;flex-direction:column;gap:3px;margin-top:9px;}
.chat-item{
  display:flex;align-items:center;gap:9px;padding:9px 10px;border-radius:8px;cursor:pointer;
  border:1.5px solid transparent;background:var(--bg2);transition:all .15s;position:relative;
}
.chat-item:hover{background:var(--surf2);border-color:var(--bord);}
.chat-item.sel{background:var(--surf2);border-color:var(--g1);}
.chat-item.inadimplente{border-left:3px solid var(--r1);}
.chat-item-info{flex:1;min-width:0;}
.chat-item-name{font-size:.82rem;font-weight:700;color:var(--txt);display:flex;align-items:center;gap:5px;}
.chat-item-preview{font-size:.68rem;color:var(--mute);white-space:nowrap;overflow:hidden;text-overflow:ellipsis;margin-top:1px;}
.chat-item-unread{
  min-width:17px;height:17px;padding:0 4px;border-radius:9px;background:var(--r1);color:#fff;
  font-size:.6rem;font-weight:900;display:flex;align-items:center;justify-content:center;flex-shrink:0;
}
.chat-thread-card{height:100%;display:flex;flex-direction:column;padding:0;overflow:hidden;}
.chat-thread-header{
  padding:14px 18px;border-bottom:1px solid var(--bord);display:flex;align-items:center;gap:11px;flex-shrink:0;
}
.chat-thread-title{font-family:'Cinzel',serif;font-size:.92rem;font-weight:700;color:var(--txt);}
.chat-thread-sub{font-size:.7rem;color:var(--mute);margin-top:1px;}
.chat-messages{flex:1;overflow-y:auto;padding:16px 18px;display:flex;flex-direction:column;gap:10px;}
.chat-bubble-row{display:flex;flex-direction:column;max-width:72%;}
.chat-bubble-row.mine{align-self:flex-end;align-items:flex-end;}
.chat-bubble-row.theirs{align-self:flex-start;align-items:flex-start;}
.chat-bubble{
  padding:9px 13px;border-radius:14px;font-size:.83rem;line-height:1.5;word-break:break-word;
}
.chat-bubble-row.mine .chat-bubble{background:linear-gradient(135deg,var(--g1),#0a7820);color:#fff;border-bottom-right-radius:4px;}
.chat-bubble-row.theirs .chat-bubble{background:var(--surf2);border:1px solid var(--bord);color:var(--txt);border-bottom-left-radius:4px;}
.chat-bubble-meta{font-size:.6rem;color:var(--mute);margin-top:3px;padding:0 3px;}
.chat-receipt{
  width:230px;border-radius:12px;overflow:hidden;
  background:var(--surf2);border:1px solid var(--ok-bd);
  box-shadow:0 2px 10px rgba(0,0,0,.15);
}
.chat-receipt-head{
  background:linear-gradient(135deg,var(--g1),#0a7820);color:#fff;
  padding:10px 13px;display:flex;align-items:center;gap:7px;
}
.chat-receipt-head .cr-ic{font-size:1rem;}
.chat-receipt-head .cr-lbl{font-family:'Barlow Condensed',sans-serif;font-size:.68rem;font-weight:900;letter-spacing:.06em;text-transform:uppercase;}
.chat-receipt-value{
  padding:13px;text-align:center;border-bottom:1px dashed var(--bord2);
}
.chat-receipt-value .cr-num{font-family:'Cinzel',serif;font-size:1.3rem;font-weight:900;color:var(--ok-tx);line-height:1;}
.chat-receipt-value .cr-sub{font-size:.6rem;color:var(--mute);letter-spacing:.08em;text-transform:uppercase;margin-top:3px;}
.chat-receipt-body{padding:10px 13px;display:flex;flex-direction:column;gap:5px;}
.chat-receipt-row{display:flex;justify-content:space-between;font-size:.7rem;}
.chat-receipt-row span:first-child{color:var(--mute);}
.chat-receipt-row span:last-child{color:var(--txt);font-weight:600;text-align:right;}
.chat-input-row{display:flex;gap:8px;padding:13px 16px;border-top:1px solid var(--bord);flex-shrink:0;}
.chat-input-row input{flex:1;}
.chat-quick-btn{
  padding:4px 10px;border-radius:6px;font-size:.64rem;font-weight:700;letter-spacing:.04em;
  border:1px solid var(--er-bd);background:var(--er-bg);color:var(--er-tx);cursor:pointer;
  transition:all .15s;white-space:nowrap;display:inline-flex;align-items:center;gap:4px;
}
.chat-quick-btn:hover{background:rgba(184,53,48,.22);}
@media(max-width:960px){
  .chat-layout{grid-template-columns:1fr;height:auto;}
  .chat-list-card{max-height:280px;}
  .chat-thread-card{height:60vh;}
}

/* ━━━━━━━━━━━━━━━━━━━━ PERMISSÕES ━━━━━━━━━━━━━━━━━━━━ */
.perm-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(245px,1fr));gap:12px;}
.perm-card{background:var(--surf);border:1px solid var(--bord);border-radius:10px;padding:15px;transition:border-color .18s;}
.perm-card:hover{border-color:var(--bord2);}
.perm-top{display:flex;align-items:center;gap:10px;margin-bottom:10px;}
.perm-row{display:flex;align-items:center;justify-content:space-between;padding:5px 9px;background:var(--surf2);border-radius:6px;font-size:.76rem;margin-bottom:4px;}

/* ━━━━━━━━━━━━━━━━━━━━ GRADE ━━━━━━━━━━━━━━━━━━━━ */
.grade-layout{display:grid;grid-template-columns:1fr 275px;gap:14px;align-items:start;}
.gtable{width:100%;border-collapse:collapse;}
.gtable th{font-family:'Barlow Condensed',sans-serif;font-size:.64rem;font-weight:900;letter-spacing:.16em;text-transform:uppercase;color:var(--mute);padding:8px 13px;text-align:left;border-bottom:2px solid var(--bord);background:var(--surf2);}
.gtable td{padding:8px 13px;font-size:.8rem;border-bottom:1px solid var(--bord);color:var(--txt2);vertical-align:middle;}
.gtable tr:hover td{background:var(--surf2);}
.dchip{display:inline-block;padding:2px 7px;border-radius:4px;font-size:.6rem;font-weight:700;background:var(--surf2);border:1px solid var(--bord);color:var(--mute);margin:1px;}

/* ━━━━━━━━━━━━━━━━━━━━ CORDAS — lista compacta ━━━━━━━━━━━━━━━━━━━━ */
.cordas-wrap{max-width:720px;}
.nivel-hdr{
  display:flex;align-items:center;gap:9px;
  padding:9px 16px;border-radius:8px;
  margin:26px 0 8px;
  position:sticky;top:60px;z-index:10;
  backdrop-filter:blur(14px);-webkit-backdrop-filter:blur(14px);
}
.corda-row{
  display:flex;align-items:center;gap:14px;
  padding:13px 8px;border-bottom:1px solid var(--bord);
  cursor:pointer;transition:background .15s;
  position:relative;
}
.corda-row:hover{background:var(--surf2);}
.corda-row:last-child{border-bottom:none;}
.cr-circle{
  width:40px;height:40px;border-radius:50%;flex-shrink:0;
  box-shadow:0 2px 8px rgba(0,0,0,.22),inset 0 1px 0 rgba(255,255,255,.18);
  border:1.5px solid rgba(255,255,255,.12);
  position:relative;overflow:hidden;
}
.cr-circle::after{
  content:'';position:absolute;top:4px;left:6px;
  width:12px;height:5px;border-radius:50%;
  background:rgba(255,255,255,.2);transform:rotate(-30deg);
}
.cr-info{flex:1;min-width:0;}
.cr-name{font-family:'Cinzel',serif;font-size:.88rem;font-weight:900;letter-spacing:.01em;line-height:1.25;color:var(--txt);}
.cr-meta{font-size:.72rem;color:var(--mute);display:flex;align-items:center;gap:5px;flex-wrap:wrap;margin-top:2px;}
.cr-sim{color:var(--acc);font-style:italic;}
.cr-right{display:flex;align-items:center;gap:9px;flex-shrink:0;}
.cr-chevron{
  font-size:.7rem;color:var(--bord2);transition:transform .2s;flex-shrink:0;
}
.corda-row.open .cr-chevron{transform:rotate(90deg);color:var(--acc);}
.cr-detail{
  display:none;
  margin:0 0 8px 62px;padding:9px 13px;
  background:var(--surf2);border:1px solid var(--bord);border-radius:8px;
  font-size:.78rem;color:var(--txt2);line-height:1.6;
  animation:fadeUp .18s ease;
}
.corda-row.open + .cr-detail{display:block;}
.cr-detail .cr-chips{display:flex;gap:3px;flex-wrap:wrap;margin-top:8px;padding-top:8px;border-top:1px solid var(--bord);}

/* misc */
.empty-st{text-align:center;padding:44px 20px;color:var(--mute);}
.empty-icon{font-size:2.2rem;margin-bottom:10px;opacity:.28;}
.divider{height:1px;background:var(--bord);margin:11px 0;}


/* ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
   PRESENÇA VISUAL (integrada com grade)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ */
.pres-hero{
  background:linear-gradient(135deg,var(--g1) 0%,var(--b1) 100%);
  border-radius:12px;padding:24px 28px;margin-bottom:20px;
  display:flex;align-items:center;justify-content:space-between;
  flex-wrap:wrap;gap:14px;position:relative;overflow:hidden;
}
.pres-hero::before{
  content:'';position:absolute;top:-40px;right:-40px;
  width:200px;height:200px;border-radius:50%;
  background:rgba(255,255,255,.07);pointer-events:none;
}
.pres-hero::after{
  content:'';position:absolute;bottom:-30px;right:60px;
  width:120px;height:120px;border-radius:50%;
  background:rgba(255,255,255,.05);pointer-events:none;
}
.ph-left-info{position:relative;z-index:1;}
.ph-greeting{font-size:.72rem;letter-spacing:.18em;text-transform:uppercase;color:rgba(255,255,255,.7);margin-bottom:4px;}
.ph-username{font-family:'Cinzel',serif;font-size:1.5rem;font-weight:900;color:#fff;line-height:1.1;}
.ph-date{font-size:.82rem;color:rgba(255,255,255,.75);margin-top:5px;}
.ph-stats-mini{display:flex;gap:12px;flex-wrap:wrap;position:relative;z-index:1;}
.phsm{text-align:center;background:rgba(255,255,255,.12);border-radius:8px;padding:10px 16px;backdrop-filter:blur(8px);}
.phsm-num{font-family:'Cinzel',serif;font-size:1.4rem;font-weight:900;color:#fff;line-height:1;}
.phsm-lbl{font-size:.58rem;letter-spacing:.1em;text-transform:uppercase;color:rgba(255,255,255,.7);margin-top:3px;}

/* Hoje grid */
.hoje-grid{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:20px;}
@media(max-width:600px){.hoje-grid{grid-template-columns:1fr;}}

.aula-card-hoje{
  background:var(--surf);border:1px solid var(--bord);border-radius:10px;
  padding:16px;transition:all .2s;position:relative;overflow:hidden;
  cursor:default;
}
.aula-card-hoje::before{
  content:'';position:absolute;left:0;top:0;bottom:0;width:4px;
}
.aula-card-hoje:hover{box-shadow:0 4px 16px var(--shad2);transform:translateY(-1px);}
.ach-time{font-family:'Barlow Condensed',sans-serif;font-size:.82rem;font-weight:700;color:var(--mute);letter-spacing:.06em;margin-bottom:5px;}
.ach-mod{font-family:'Cinzel',serif;font-size:1rem;font-weight:700;color:var(--txt);margin-bottom:4px;}
.ach-turma{font-size:.72rem;color:var(--mute);}
.ach-status{
  display:flex;align-items:center;justify-content:space-between;
  margin-top:10px;padding-top:10px;border-top:1px solid var(--bord);
}
.ach-mark-btn{
  padding:5px 12px;border-radius:6px;font-size:.65rem;font-weight:700;
  letter-spacing:.07em;text-transform:uppercase;border:1px solid transparent;
  cursor:pointer;transition:all .18s;font-family:'Barlow',sans-serif;
}
.ach-p{background:var(--ok-bg);border-color:var(--ok-bd);color:var(--ok-tx);}
.ach-a{background:var(--er-bg);border-color:var(--er-bd);color:var(--er-tx);}
.ach-n{background:var(--surf2);border-color:var(--bord2);color:var(--mute);}
.ach-n:hover{background:var(--wn-bg);border-color:var(--wn-bd);color:var(--wn-tx);}

.empty-hoje{
  grid-column:1/-1;text-align:center;padding:36px;
  background:var(--surf);border:1px dashed var(--bord2);border-radius:10px;
  color:var(--mute);
}

/* Weekly mini view */
.week-strip{
  background:var(--surf);border:1px solid var(--bord);border-radius:10px;
  padding:16px;margin-bottom:20px;
}
.week-grid{display:grid;grid-template-columns:repeat(7,1fr);gap:4px;margin-top:12px;}
.wday{text-align:center;}
.wday-label{font-size:.6rem;font-weight:700;letter-spacing:.08em;text-transform:uppercase;color:var(--mute);margin-bottom:4px;}
.wday-num{
  width:32px;height:32px;border-radius:8px;margin:0 auto;
  display:flex;align-items:center;justify-content:center;
  font-size:.8rem;font-weight:700;color:var(--txt2);
  border:1.5px solid transparent;cursor:pointer;transition:all .15s;
}
.wday-num:hover{background:var(--surf2);}
.wday-num.today{background:linear-gradient(135deg,var(--g1),var(--b1));color:#fff;border:none;}
.wday-num.has-p{border-color:var(--ok-bd);color:var(--ok-tx);}
.wday-num.has-a{border-color:var(--er-bd);color:var(--er-tx);}
.wday-num.has-m{border-color:var(--wn-bd);color:var(--wn-tx);}
.wday-num.no-class{color:var(--bord2);cursor:default;}
.wday-dots{display:flex;gap:2px;justify-content:center;margin-top:2px;min-height:6px;}
.wdot{width:4px;height:4px;border-radius:50%;}

/* ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
   GRADE VISUAL — editor semanal
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ */
.grade-visual{margin-top:4px;}
.gv-week{
  display:grid;
  grid-template-columns:60px repeat(7,1fr);
  gap:0;border:1px solid var(--bord);border-radius:10px;overflow:hidden;
}
.gv-header{
  background:var(--surf2);border-bottom:2px solid var(--bord);
  display:contents;
}
.gv-col-head{
  padding:10px 6px;text-align:center;
  font-family:'Barlow Condensed',sans-serif;font-size:.72rem;
  font-weight:900;letter-spacing:.1em;text-transform:uppercase;color:var(--mute);
  border-right:1px solid var(--bord);background:var(--surf2);
}
.gv-col-head.today-col{background:linear-gradient(135deg,rgba(7,157,40,.15),rgba(7,62,142,.1));color:var(--txt);}
.gv-col-head:last-child{border-right:none;}
.gv-time-col{
  padding:8px 4px;text-align:right;
  font-family:'Barlow Condensed',sans-serif;font-size:.62rem;
  font-weight:700;color:var(--mute);border-right:1px solid var(--bord);
  background:var(--surf2);display:flex;flex-direction:column;
  justify-content:center;white-space:nowrap;
}
.gv-cell{
  border-right:1px solid var(--bord);border-bottom:1px solid var(--bord);
  min-height:52px;position:relative;background:var(--surf);
  transition:background .15s;cursor:pointer;padding:3px;
}
.gv-cell:hover{background:var(--surf2);}
.gv-cell:last-child{border-right:none;}
.gv-cell.today-col{background:rgba(7,157,40,.04);}
.gv-cell.today-col:hover{background:rgba(7,157,40,.09);}
.gv-add-hint{
  position:absolute;inset:0;display:flex;align-items:center;justify-content:center;
  font-size:1.2rem;color:var(--bord2);opacity:0;transition:opacity .15s;
}
.gv-cell:hover .gv-add-hint{opacity:1;}
.gv-aula{
  border-radius:6px;padding:5px 7px;margin-bottom:3px;
  font-size:.67rem;cursor:pointer;transition:all .18s;position:relative;
  border:1px solid transparent;
}
.gv-aula:hover{filter:brightness(1.08);transform:scale(1.02);}
.gv-aula-time{
  font-family:'Barlow Condensed',sans-serif;font-size:.65rem;
  font-weight:700;opacity:.8;line-height:1;margin-bottom:2px;
}
.gv-aula-mod{font-weight:700;line-height:1.2;}
.gv-aula-turma{opacity:.75;font-size:.6rem;margin-top:1px;}
.gv-aula-del{
  position:absolute;top:3px;right:4px;
  background:rgba(0,0,0,.2);border:none;border-radius:3px;
  color:rgba(255,255,255,.8);cursor:pointer;font-size:.7rem;
  width:16px;height:16px;display:flex;align-items:center;justify-content:center;
  opacity:0;transition:opacity .15s;
}
.gv-aula:hover .gv-aula-del{opacity:1;}

/* quick add inline form */
.quick-add-form{
  background:var(--surf2);border:1.5px solid var(--bord2);border-radius:8px;
  padding:12px;margin-top:8px;display:none;animation:fadeUp .18s ease;
}
.quick-add-form.open{display:block;}

/* presença chamada massa */
.chamada-card{
  background:var(--surf);border:1px solid var(--bord);border-radius:10px;
  padding:16px;margin-bottom:10px;
}
.chamada-card-head{display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:8px;margin-bottom:12px;}
.chamada-card-title{font-family:'Cinzel',serif;font-size:.9rem;font-weight:700;}
.aluno-chamada-row{
  display:flex;align-items:center;gap:8px;
  padding:7px 10px;border-radius:7px;border:1px solid var(--bord);
  background:var(--bg2);margin-bottom:4px;
}
.aluno-chamada-name{flex:1;font-size:.82rem;font-weight:600;color:var(--txt);}
.chamada-btns{display:flex;gap:4px;}
.cbtn{
  padding:3px 10px;border-radius:5px;font-size:.63rem;font-weight:700;
  letter-spacing:.06em;text-transform:uppercase;border:1px solid transparent;
  cursor:pointer;transition:all .13s;font-family:'Barlow',sans-serif;
}
.cbtn-p{background:var(--ok-bg);border-color:var(--ok-bd);color:var(--ok-tx);}
.cbtn-p.active,.cbtn-p:hover{background:var(--g1);border-color:var(--g2);color:#fff;}
.cbtn-a{background:var(--er-bg);border-color:var(--er-bd);color:var(--er-tx);}
.cbtn-a.active,.cbtn-a:hover{background:var(--r1);border-color:var(--r2);color:#fff;}

@media(max-width:960px){
  .page{padding:16px 12px 60px;}
  .pres-grid,.att-cols,.pag-layout,.grade-layout{grid-template-columns:1fr;}
  .sidebar{
    transform:translateX(-100%);width:240px;
  }
  body.sidebar-collapsed .sidebar{width:240px;} /* em mobile, colapsar não se aplica — sempre expandida quando aberta */
  .sidebar.mobile-open{transform:translateX(0);}
  .main-wrap{margin-left:0 !important;}
  .sidebar-collapse-btn{display:none;}
  .sidebar-toggle-mobile{display:flex;}
  .topbar{padding:0 12px;}
}
</style>
</head>
<body>

<!-- NAV -->
<nav>
  <a class="nav-brand" href="#">
    <img id="nav-logo" src="data:image/png;base64,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" alt="FIU"/>
    <div><div class="nb-name">Família Irmãos Unidos</div><div class="nb-sub">Capoeira</div></div>
  </a>
  <div class="nav-tabs" id="nav-tabs">
    <button class="ntab active" onclick="showPage('presenca',this)"><span class="ntab-ic"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 5H7a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h10a2 2 0 0 0 2-2V7a2 2 0 0 0-2-2h-2"/><rect x="9" y="3" width="6" height="4" rx="1"/><path d="m9 14 2 2 4-4"/></svg></span> Presença</button>
    <button class="ntab"        onclick="showPage('alunos',this)"><span class="ntab-ic"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M16 21v-2a4 4 0 0 0-4-4H6a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M22 21v-2a4 4 0 0 0-3-3.87"/><path d="M16 3.13a4 4 0 0 1 0 7.75"/></svg></span> Alunos</button>
    <button class="ntab" id="ntab-mensagens" style="position:relative" onclick="showPage('mensagens',this)"><span class="ntab-ic"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2Z"/></svg></span> Mensagens<span class="notif-badge hidden" id="chat-nav-badge" style="position:absolute;top:-4px;right:-4px">0</span></button>
    <span class="nav-divider"></span>
    <button class="ntab"        onclick="showPage('pagamentos',this)"><span class="ntab-ic"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 12V7a2 2 0 0 0-2-2H5a2 2 0 0 0-2 2v10a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-3"/><path d="M17 12a1 1 0 0 0 0 2h4v-2Z"/></svg></span> Pagamentos</button>
    <button class="ntab"        onclick="showPage('permissoes',this)"><span class="ntab-ic"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="7.5" cy="15.5" r="5.5"/><path d="m21 2-9.6 9.6"/><path d="m15.5 7.5 3 3L22 7l-3-3"/></svg></span> Permissões</button>
    <span class="nav-divider"></span>
    <button class="ntab"        onclick="showPage('grade',this)"><span class="ntab-ic"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="9"/><path d="M12 7v5l3 2"/></svg></span> Grade</button>
    <button class="ntab" id="ntab-cordas" onclick="showPage('cordas',this)"><span class="corda-icon" id="corda-nav-icon"><svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
      <path class="rope-strand-a" d="M9 1.5 C9 1.5 16 4.5 16 8 C16 11.5 8 12.5 8 16 C8 19.5 15 22.5 15 22.5 L13.2 22.5 C13.2 22.5 6.8 19.5 6.8 16 C6.8 12.5 14.8 11.5 14.8 8 C14.8 4.5 7.8 1.5 7.8 1.5 Z"/>
      <path class="rope-strand-b" d="M15 1.5 C15 1.5 8 4.5 8 8 C8 11.5 16 12.5 16 16 C16 19.5 9 22.5 9 22.5 L10.8 22.5 C10.8 22.5 17.2 19.5 17.2 16 C17.2 12.5 9.2 11.5 9.2 8 C9.2 4.5 16.2 1.5 16.2 1.5 Z"/>
    </svg></span> Cordas</button>
  </div>
  <div class="nav-right">
    <button class="role-pill" id="user-badge" onclick="doLogout()" title="Clique para sair" style="display:none">
      <span class="rdot"></span>
      <span id="user-badge-name"></span>
    </button>
    <div class="notif-wrap">
      <button class="icon-btn" id="notif-btn" onclick="toggleNotifPanel()" title="Notificações">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M6 8a6 6 0 0 1 12 0c0 7 3 9 3 9H3s3-2 3-9"/><path d="M10.3 21a1.94 1.94 0 0 0 3.4 0"/></svg><span class="notif-badge hidden" id="notif-badge">0</span>
      </button>
      <div class="notif-panel" id="notif-panel">
        <div class="notif-head">
          <div>
            <div class="notif-head-title"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" style="width:15px;height:15px;vertical-align:-3px;margin-right:4px"><path d="M6 8a6 6 0 0 1 12 0c0 7 3 9 3 9H3s3-2 3-9"/><path d="M10.3 21a1.94 1.94 0 0 0 3.4 0"/></svg> Notificações</div>
            <div class="notif-head-sub" id="notif-head-sub">Tudo em dia</div>
          </div>
          <button class="notif-close" onclick="toggleNotifPanel(false)">×</button>
        </div>
        <div class="notif-actions">
          <button class="notif-newbtn" onclick="openModal('modal-nova-msg')">✉ Nova Mensagem</button>
          <button class="notif-iconbtn" onclick="marcarTodasLidas()" title="Marcar todas como lidas">✓✓</button>
          <button class="notif-iconbtn" onclick="limparNotificacoes()" title="Limpar todas">🗑</button>
        </div>
        <div class="notif-list" id="notif-list"></div>
      </div>
    </div>
    <button class="icon-btn" id="theme-btn" onclick="toggleTheme()" title="Alternar tema"></button>
  </div>
</nav>

<div class="app">
<!-- PRESENÇA -->
<div class="page active" id="page-presenca">
  <!-- Hero -->
  <div class="pres-hero" id="pres-hero">
    <div class="ph-left-info">
      <div class="ph-greeting">Bem-vindo(a) de volta</div>
      <div class="ph-username" id="ph-username">FIU Capoeira</div>
      <div class="ph-date" id="ph-date"></div>
    </div>
    <div class="ph-stats-mini" id="ph-stats-mini"></div>
  </div>

  <!-- Visão aluno -->
  <div id="pres-aluno-view">
    <!-- Aulas de hoje -->
    <div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:12px;flex-wrap:wrap;gap:8px">
      <div>
        <div class="card-tit" style="border:none;padding:0;margin:0;font-size:.7rem">Aulas de Hoje</div>
        <div id="hoje-subtitle" style="font-size:.72rem;color:var(--mute)"></div>
      </div>
      <div id="pres-prof-actions" style="display:none">
        <button class="btn btn-ghost btn-sm" onclick="showPage('grade',document.querySelectorAll('.ntab')[4])">⚙ Editar Grade</button>
      </div>
    </div>
    <div class="hoje-grid" id="hoje-grid">
      <div class="empty-hoje"><div class="empty-icon">🤸</div><p>Carregando...</p></div>
    </div>

    <!-- Strip semanal -->
    <div class="week-strip" id="week-strip">
      <div style="display:flex;align-items:center;justify-content:space-between">
        <div class="card-tit" style="border:none;padding:0;margin:0">Semana Atual</div>
        <div id="week-range" style="font-size:.7rem;color:var(--mute)"></div>
      </div>
      <div class="week-grid" id="week-grid"></div>
    </div>

    <!-- Painel aluno selecionado (prof/mestre) -->
    <div id="pres-detail-panel"></div>
  </div>

  <!-- Seletor de aluno (prof/mestre) -->
  <div id="pres-prof-view" style="display:none">
    <div class="pres-grid">
      <div>
        <div class="card" style="margin-bottom:10px">
          <div class="card-tit">Turma</div>
          <input id="search-aluno" class="inp" style="margin-bottom:9px" placeholder="🔍 Buscar aluno..." oninput="renderAlunoList()"/>
          <div class="aluno-list" id="aluno-list"></div>
        </div>
        <button class="btn btn-g btn-sm" style="width:100%" id="btn-add-aluno" onclick="openModal('modal-add-aluno')">+ Novo Aluno</button>
      </div>
      <div id="attend-panel"><div class="empty-st"><div class="empty-icon">🤸</div><p>Selecione um aluno para ver e registrar presenças.</p></div></div>
    </div>
  </div>
</div>
<!-- ALUNOS -->
<div class="page" id="page-alunos">
  <div class="ph">
    <div class="ph-left"><h1>Gestão de <span>Alunos</span></h1><p>Progresso, cordas e frequência</p></div>
    <div class="ph-right"><button class="btn btn-g btn-sm" onclick="openModal('modal-add-aluno')">+ Novo Aluno</button></div>
  </div>
  <div class="alunos-grid" id="alunos-grid"></div>
</div>

<!-- MENSAGENS (CHAT) -->
<div class="page" id="page-mensagens">
  <div class="ph">
    <div class="ph-left"><h1>Mensagens com <span>Alunos</span></h1><p>Converse com alunos, especialmente os inadimplentes</p></div>
  </div>

  <!-- Visão staff: lista + conversa -->
  <div id="chat-staff-view" class="chat-layout" style="display:none">
    <div class="card chat-list-card">
      <input id="chat-search" class="inp" style="margin-bottom:9px" placeholder="🔍 Buscar aluno..." oninput="renderChatLista()"/>
      <div class="chat-lista" id="chat-lista"></div>
    </div>
    <div class="card chat-thread-card" id="chat-thread-wrap">
      <div class="empty-st"><div class="empty-icon">💬</div><p>Selecione um aluno para ver a conversa.</p></div>
    </div>
  </div>

  <!-- Visão aluno: conversa direta com a academia -->
  <div id="chat-aluno-view" style="display:none">
    <div class="card chat-thread-card" id="chat-thread-aluno-wrap" style="height:calc(100vh - 210px)"></div>
  </div>
</div>

<!-- PAGAMENTOS -->
<div class="page" id="page-pagamentos">
  <div class="ph">
    <div class="ph-left"><h1>Controle de <span>Pagamentos</span></h1><p>Mensalidades e histórico financeiro</p></div>
    <div class="ph-right">
      <button class="btn btn-g btn-sm" onclick="openModal('modal-reg-pag')">+ Registrar</button>
      <button class="btn btn-ghost btn-sm" onclick="openModal('modal-config-pag')">⚙ Config</button>
    </div>
  </div>
  <div class="pag-layout">
    <div>
      <div id="inadim-banner"></div>
      <div class="pag-filters">
        <button class="ptab active" onclick="setPagTab('todos',this)">Todos</button>
        <button class="ptab" onclick="setPagTab('em_dia',this)">✓ Em Dia</button>
        <button class="ptab" onclick="setPagTab('pendente',this)">⏳ Pendente</button>
        <button class="ptab" onclick="setPagTab('atrasado',this)">⚠ Atrasado</button>
      </div>
      <div class="card"><table class="ptable"><thead><tr><th>Aluno</th><th>Corda</th><th>Plano</th><th>Venc.</th><th>Último Pag.</th><th>Status</th><th></th></tr></thead><tbody id="pag-tbody"></tbody></table></div>
    </div>
    <div class="pag-right">
      <div class="card"><div class="card-tit">Resumo do Mês</div><div class="pres-boxes"><div class="pbox"><div class="pbox-num" id="pr-emdia" style="color:var(--g2)">—</div><div class="pbox-lbl">Em Dia</div></div><div class="pbox"><div class="pbox-num" id="pr-pendente" style="color:var(--y2)">—</div><div class="pbox-lbl">Pendente</div></div><div class="pbox"><div class="pbox-num" id="pr-atrasado" style="color:var(--r2)">—</div><div class="pbox-lbl">Atrasado</div></div><div class="pbox"><div class="pbox-num" id="pr-receita" style="color:var(--acc)">—</div><div class="pbox-lbl">Receita</div></div></div></div>
      <div class="card"><div class="card-tit">Planos Ativos</div><div id="pag-planos-resumo"></div></div>
      <div class="card"><div class="card-tit">Últimos Pagamentos</div><div style="max-height:280px;overflow-y:auto" id="pag-historico"></div></div>
    </div>
  </div>
</div>

<!-- PERMISSÕES -->
<div class="page" id="page-permissoes">
  <div class="ph">
    <div class="ph-left"><h1>Tags de <span>Permissão</span></h1><p>Acesso baseado em pagamento e graduação</p></div>
    <div class="ph-right"><button class="btn btn-g btn-sm" onclick="openModal('modal-add-tag')">+ Nova Tag</button></div>
  </div>
  <div class="card" style="margin-bottom:14px">
    <div class="card-tit">Como funciona</div>
    <div style="display:grid;grid-template-columns:repeat(auto-fill,minmax(170px,1fr));gap:7px">
      <div style="padding:9px;background:var(--surf2);border-radius:7px;border:1px solid var(--bord)"><div class="pill p-ok" style="margin-bottom:5px">✓ Em Dia</div><div style="font-size:.74rem;color:var(--txt2)">Acesso completo ao plano.</div></div>
      <div style="padding:9px;background:var(--surf2);border-radius:7px;border:1px solid var(--bord)"><div class="pill p-warn" style="margin-bottom:5px">⏳ Pendente</div><div style="font-size:.74rem;color:var(--txt2)">Apenas aulas básicas.</div></div>
      <div style="padding:9px;background:var(--surf2);border-radius:7px;border:1px solid var(--bord)"><div class="pill p-err" style="margin-bottom:5px">⚠ Atrasado</div><div style="font-size:.74rem;color:var(--txt2)">Sem acesso a aulas.</div></div>
      <div style="padding:9px;background:var(--surf2);border-radius:7px;border:1px solid var(--bord)"><div class="pill p-info" style="margin-bottom:5px">🏷 Custom</div><div style="font-size:.74rem;color:var(--txt2)">Tags personalizadas.</div></div>
    </div>
  </div>
  <div class="perm-grid" id="perm-grid"></div>
</div>

<!-- GRADE -->
<div class="page" id="page-grade">
  <div class="ph">
    <div class="ph-left"><h1>Grade de <span>Aulas</span></h1><p>Gerencie os horários da semana — clique em qualquer célula para adicionar uma aula</p></div>
    <div class="ph-right">
      <button class="btn btn-g btn-sm" onclick="openModal('modal-add-aula-grade')">+ Nova Aula</button>
      <button class="btn btn-ghost btn-sm" onclick="toggleGradeView()" id="btn-grade-view">📋 Chamada</button>
    </div>
  </div>

  <!-- Grade Visual Semanal -->
  <div id="grade-visual-section">
    <div class="card" style="margin-bottom:16px;overflow-x:auto">
      <div class="gv-week" id="gv-week"></div>
    </div>
    <!-- Lista compacta -->
    <div class="card">
      <div class="card-tit">Todas as aulas cadastradas</div>
      <table class="gtable"><thead><tr><th>Dias</th><th>Horário</th><th>Duração</th><th>Modalidade</th><th>Turma</th><th></th></tr></thead>
      <tbody id="grade-tbody"></tbody></table>
    </div>
  </div>

  <!-- Chamada em massa (alternar) -->
  <div id="grade-chamada-section" style="display:none">
    <div style="margin-bottom:14px;display:flex;align-items:center;gap:10px;flex-wrap:wrap">
      <div class="fg" style="margin:0;flex:1;min-width:160px">
        <label style="font-size:.64rem;font-weight:700;letter-spacing:.1em;text-transform:uppercase;color:var(--txt2);display:block;margin-bottom:4px">Data da chamada</label>
        <input type="date" id="chamada-data" class="inp" style="max-width:200px"/>
      </div>
      <div class="fg" style="margin:0;flex:1;min-width:160px">
        <label style="font-size:.64rem;font-weight:700;letter-spacing:.1em;text-transform:uppercase;color:var(--txt2);display:block;margin-bottom:4px">Aula</label>
        <select id="chamada-aula-sel" class="inp" style="max-width:280px"></select>
      </div>
      <button class="btn btn-g btn-sm" onclick="renderChamada()">Carregar Turma</button>
    </div>
    <div id="chamada-container"></div>
  </div>
</div>
<!-- CORDAS -->
<div class="page" id="page-cordas">
  <div class="ph">
    <div class="ph-left"><h1>Sistema de <span>Cordas</span></h1><p>Graduação Família Irmãos Unidos · Mestre Sidney</p></div>
  </div>
  <div class="cordas-wrap" id="cordas-list"></div>
</div>
</div><!-- /app -->

<!-- MODAIS -->
<div class="modal-ov" id="modal-add-aluno"><div class="modal"><h2>Novo Aluno</h2><div class="fg"><label>Nome completo</label><input id="add-nome" class="inp" placeholder="Nome do aluno"/></div><div class="g2"><div class="fg"><label>Data de início</label><input type="date" id="add-inicio" class="inp"/></div><div class="fg"><label>Corda atual</label><select id="add-corda" class="inp"></select></div></div><div class="g2"><div class="fg"><label>Plano</label><select id="add-plano" class="inp"><option value="basico">Básico</option><option value="intermediario">Intermediário</option><option value="completo">Completo</option><option value="bolsista">Bolsista</option></select></div><div class="fg"><label>Vencimento</label><select id="add-venc" class="inp"><option value="5">Dia 5</option><option value="10">Dia 10</option><option value="15">Dia 15</option><option value="20">Dia 20</option></select></div></div><div class="modal-act"><button class="btn btn-ghost" onclick="closeModal('modal-add-aluno')">Cancelar</button><button class="btn btn-g" onclick="addAluno()">Salvar</button></div></div></div>
<div class="modal-ov" id="modal-promover"><div class="modal"><h2>Promover Aluno</h2><p style="font-size:.82rem;color:var(--mute);margin-bottom:13px" id="promover-info"></p><div class="g2"><div class="fg"><label>Nova corda</label><select id="promover-corda" class="inp"></select></div><div class="fg"><label>Data</label><input type="date" id="promover-data" class="inp"/></div></div><div class="modal-act"><button class="btn btn-ghost" onclick="closeModal('modal-promover')">Cancelar</button><button class="btn btn-y" onclick="promoverAluno()">Confirmar</button></div></div></div>
<div class="modal-ov" id="modal-reg-pag"><div class="modal"><h2>Registrar Pagamento</h2><div class="fg"><label>Aluno</label><select id="pag-aluno-sel" class="inp"></select></div><div class="g3"><div class="fg"><label>Valor (R$)</label><input type="number" id="pag-valor" class="inp" step="0.01"/></div><div class="fg"><label>Data</label><input type="date" id="pag-data" class="inp"/></div><div class="fg"><label>Mês ref.</label><input type="month" id="pag-mes" class="inp"/></div></div><div class="g2"><div class="fg"><label>Forma</label><select id="pag-forma" class="inp"><option>Pix</option><option>Dinheiro</option><option>Cartão Débito</option><option>Cartão Crédito</option><option>Transferência</option></select></div><div class="fg"><label>Status</label><select id="pag-status-sel" class="inp"><option value="pago">✓ Pago</option><option value="pendente">⏳ Pendente</option></select></div></div><div class="fg"><label>Observação</label><input id="pag-obs" class="inp" placeholder="Opcional..."/></div><div class="modal-act"><button class="btn btn-ghost" onclick="closeModal('modal-reg-pag')">Cancelar</button><button class="btn btn-g" onclick="regPag()">Salvar</button></div></div></div>
<div class="modal-ov" id="modal-config-pag"><div class="modal"><h2>Configurar Planos</h2><div class="g2"><div class="fg"><label>Básico (R$)</label><input type="number" id="cfg-basico" class="inp" step="0.01"/></div><div class="fg"><label>Intermediário (R$)</label><input type="number" id="cfg-intermediario" class="inp" step="0.01"/></div></div><div class="g2"><div class="fg"><label>Completo (R$)</label><input type="number" id="cfg-completo" class="inp" step="0.01"/></div><div class="fg"><label>Tolerância (dias)</label><input type="number" id="cfg-tolerancia" class="inp" value="5"/></div></div><div class="modal-act"><button class="btn btn-ghost" onclick="closeModal('modal-config-pag')">Cancelar</button><button class="btn btn-y" onclick="salvarConfig()">Salvar</button></div></div></div>
<div class="modal-ov" id="modal-add-tag"><div class="modal"><h2>Nova Tag</h2><div class="fg"><label>Aluno</label><select id="tag-aluno-sel" class="inp"></select></div><div class="g2"><div class="fg"><label>Tag</label><input id="tag-nome" class="inp" placeholder="Ex: Instrutor..."/></div><div class="fg"><label>Cor</label><select id="tag-cor" class="inp"><option value="p-ok">Verde</option><option value="p-info">Azul</option><option value="p-warn">Amarelo</option><option value="p-mute">Cinza</option></select></div></div><div class="fg"><label>Permissão</label><input id="tag-perm" class="inp" placeholder="Ex: Acesso sala avançada..."/></div><div class="modal-act"><button class="btn btn-ghost" onclick="closeModal('modal-add-tag')">Cancelar</button><button class="btn btn-g" onclick="addTag()">Criar</button></div></div></div>
<div class="modal-ov" id="modal-add-aula-grade"><div class="modal"><h2>Nova Aula na Grade</h2><div class="fg"><label>Dias da semana</label><div style="display:flex;gap:4px;flex-wrap:wrap" id="dias-check"></div></div><div class="g2"><div class="fg"><label>Início</label><input type="time" id="ag-inicio" class="inp" value="09:00"/></div><div class="fg"><label>Fim</label><input type="time" id="ag-fim" class="inp" value="10:00"/></div></div><div class="g2"><div class="fg"><label>Modalidade</label><select id="ag-mod" class="inp"><option>Capoeira Regional</option><option>Capoeira Angola</option><option>Maculelê</option><option>Musicalidade</option><option>Acrobacia</option><option>Infantil</option><option>Juvenil</option><option>Roda</option><option>Treino Livre</option></select></div><div class="fg"><label>Turma</label><input id="ag-turma" class="inp" placeholder="Ex: Avançado..."/></div></div><div class="modal-act"><button class="btn btn-ghost" onclick="closeModal('modal-add-aula-grade')">Cancelar</button><button class="btn btn-g" onclick="addAulaGrade()">Salvar</button></div></div></div>
<div class="modal-ov" id="modal-add-aula-dia"><div class="modal"><h2>Adicionar Aula</h2><p style="font-size:.78rem;color:var(--mute);margin-bottom:12px" id="add-aula-dia-info"></p><div class="g2"><div class="fg"><label>Início</label><input type="time" id="ad-inicio" class="inp" value="09:00"/></div><div class="fg"><label>Fim</label><input type="time" id="ad-fim" class="inp" value="10:00"/></div></div><div class="g2"><div class="fg"><label>Modalidade</label><select id="ad-mod" class="inp"><option>Capoeira Regional</option><option>Capoeira Angola</option><option>Maculelê</option><option>Musicalidade</option><option>Acrobacia</option><option>Infantil</option><option>Juvenil</option><option>Roda</option><option>Treino Livre</option></select></div><div class="fg"><label>Status</label><select id="ad-status" class="inp"><option value="P">✓ Presente</option><option value="A">✗ Falta</option><option value="">— Não definido</option></select></div></div><div class="modal-act"><button class="btn btn-ghost" onclick="closeModal('modal-add-aula-dia')">Cancelar</button><button class="btn btn-g" onclick="addAulaDia()">Adicionar</button></div></div></div>
<div class="modal-ov" id="modal-nova-msg"><div class="modal"><h2>✉ Nova Mensagem</h2><div class="fg"><label>Para</label><select id="msg-destino" class="inp"><option value="todos">📢 Todos (mural geral)</option><option value="professores">👨‍🏫 Professores e Mestres</option></select></div><div class="fg"><label>Assunto</label><input id="msg-assunto" class="inp" placeholder="Ex: Aviso sobre o evento de sábado..."/></div><div class="fg"><label>Mensagem</label><textarea id="msg-texto" class="inp" rows="4" style="resize:vertical;font-family:inherit" placeholder="Escreva sua mensagem..."></textarea></div><div class="modal-act"><button class="btn btn-ghost" onclick="closeModal('modal-nova-msg')">Cancelar</button><button class="btn btn-g" onclick="enviarMensagem()">Enviar</button></div></div></div>

<div class="toast-el" id="toast"></div>
<script>
// ── THEME ──
const ICON_MOON='<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79Z"/></svg>';
const ICON_SUN='<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="4"/><path d="M12 2v2M12 20v2M4.93 4.93l1.41 1.41M17.66 17.66l1.41 1.41M2 12h2M20 12h2M6.34 17.66l-1.41 1.41M19.07 4.93l-1.41 1.41"/></svg>';
function toggleTheme(){
  const b=document.documentElement;
  const d=b.getAttribute('data-theme')==='dark';
  b.setAttribute('data-theme',d?'light':'dark');
  document.getElementById('theme-btn').innerHTML=d?ICON_MOON:ICON_SUN;
  localStorage.setItem('fiu_theme',d?'light':'dark');
}
(function(){
  const t=localStorage.getItem('fiu_theme')||'dark';
  document.documentElement.setAttribute('data-theme',t);
  document.body.style.display=''; // prevent FOUC
  const btn=document.getElementById('theme-btn');
  if(btn)btn.innerHTML=t==='dark'?ICON_MOON:ICON_SUN;
})();

// ── NAV ──
function showPage(id,btn){
  document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
  document.querySelectorAll('.ntab').forEach(t=>t.classList.remove('active'));
  document.getElementById('page-'+id).classList.add('active');
  if(btn)btn.classList.add('active');
  if(id==='presenca')renderPresenca();
  if(id==='alunos')renderAlunosGrid();
  if(id==='mensagens')renderMensagens();
  if(id==='pagamentos')renderPagamentos();
  if(id==='permissoes')renderPermissoes();
  if(id==='grade')renderGrade();
  if(id==='cordas')renderCordas();
}

// ── MODAL ──
function openModal(id){
  if(id==='modal-add-aluno'){document.getElementById('add-nome').value='';document.getElementById('add-inicio').value=today();populateSel('add-corda',0);}
  if(id==='modal-reg-pag'){populateAlunoSel('pag-aluno-sel');document.getElementById('pag-data').value=today();const n=new Date();document.getElementById('pag-mes').value=`${n.getFullYear()}-${String(n.getMonth()+1).padStart(2,'0')}`;document.getElementById('pag-aluno-sel').onchange=()=>{const a=getAluno(parseInt(document.getElementById('pag-aluno-sel').value));if(a&&S.config[a.plano])document.getElementById('pag-valor').value=S.config[a.plano];};}
  if(id==='modal-config-pag'){document.getElementById('cfg-basico').value=S.config.basico;document.getElementById('cfg-intermediario').value=S.config.intermediario;document.getElementById('cfg-completo').value=S.config.completo;document.getElementById('cfg-tolerancia').value=S.config.tolerancia;}
  if(id==='modal-add-tag'){populateAlunoSel('tag-aluno-sel');document.getElementById('tag-nome').value='';document.getElementById('tag-perm').value='';}
  if(id==='modal-add-aula-grade')renderDiasCheck();
  if(id==='modal-nova-msg'){document.getElementById('msg-destino').value='todos';document.getElementById('msg-assunto').value='';document.getElementById('msg-texto').value='';}
  document.getElementById(id).classList.add('open');
}
function closeModal(id){document.getElementById(id).classList.remove('open');}
document.querySelectorAll('.modal-ov').forEach(o=>o.addEventListener('click',e=>{if(e.target===o)o.classList.remove('open');}));
function populateSel(id,sel){document.getElementById(id).innerHTML=CORDAS.map((c,i)=>`<option value="${i}"${i===sel?' selected':''}>${c.n}. ${c.nome}</option>`).join('');}
function populateAlunoSel(id){document.getElementById(id).innerHTML=S.alunos.map(a=>`<option value="${a.id}">${a.nome}</option>`).join('');}

// ── TOAST ──
function toast(msg,tipo=''){const t=document.getElementById('toast');t.textContent=msg;t.className='toast-el show'+(tipo?' '+tipo:'');clearTimeout(t._t);t._t=setTimeout(()=>t.className='toast-el',2800);}

// ── DATA ──
const CORDAS=[
  // Cores EXATAS das fotos do documento (Mestre Sidney / Família Irmãos Unidos)
  {id:0, n:1, nome:'Crua',              c1:'#c8b878',c2:'#b0a060',sim:'Universo',          desc:'A corda de todo iniciante e o ingresso para o mundo da Capoeira.',                                                                           min:6, max:12, nivel:'iniciante'},
  {id:1, n:2, nome:'Crua e Verde',      c1:'#c8b878',c2:'#1a9a30',sim:'Transição',         desc:'Corda de transição — a junção do universo com o oxigênio. Seu significado é a junção das duas cores que a compõem.',                         min:6, max:12, nivel:'iniciante'},
  {id:2, n:3, nome:'Verde',             c1:'#1a9a30',c2:'#157825',sim:'Oxigênio',          desc:'Quando o aluno passa a ganhar mais resistência durante os treinos. Transmite harmonia e equilíbrio.',                                        min:6, max:12, nivel:'iniciante'},
  {id:3, n:4, nome:'Verde e Laranja',   c1:'#1a9a30',c2:'#d06010',sim:'Transição',         desc:'Corda de transição entre o oxigênio e o despertar do sol.',                                                                                  min:6, max:12, nivel:'basico'},
  {id:4, n:5, nome:'Laranja',           c1:'#d06010',c2:'#b85010',sim:'Despertar do Sol',  desc:'Quando o aluno desperta seus sentimentos pela Capoeira, seus reflexos e sua vontade. Transmite agilidade mental e corporal, encorajamento e dedicação.', min:8,max:14,nivel:'basico'},
  {id:5, n:6, nome:'Laranja e Amarelo', c1:'#d06010',c2:'#e8c010',sim:'Transição',         desc:'Corda de transição entre o despertar do sol e o ouro.',                                                                                      min:8, max:14, nivel:'basico'},
  {id:6, n:7, nome:'Amarelo',           c1:'#e8c010',c2:'#c8a808',sim:'Ouro',              desc:'Quando o aluno começa a valorizar seu aprendizado, a se valorizar como capoeirista e a valorizar seu mestre e seu grupo. Transmite energia e muita atenção.', min:10,max:16,nivel:'intermediario'},
  {id:7, n:8, nome:'Amarelo e Azul',    c1:'#e8c010',c2:'#1040a0',sim:'Monitor/a',         desc:'Corda de Monitor/a — transição entre o ouro e a imensidão do mar.',                                                                          min:12, max:18, nivel:'intermediario'},
  {id:8, n:9, nome:'Azul',             c1:'#1a50c0',c2:'#0c3890',sim:'Imensidão do Mar',   desc:'O aluno olha para trás e vê o caminho percorrido; para frente vê o tanto que tem que percorrer. Transmite tranquilidade, sinceridade e confiança. (Instrutor/a)', min:24,max:36,nivel:'instrutor'},
  {id:9, n:10,nome:'Azul e Roxa',       c1:'#1a50c0',c2:'#7030a0',sim:'Instrutor/a 2º Grau',desc:'Instrutor/a de segundo grau — domínio profundo da arte.',                                                                                  min:24, max:36, nivel:'instrutor'},
  {id:10,n:11,nome:'Roxa',              c1:'#7030a0',c2:'#5a2080',sim:'Pedras Preciosas',   desc:'O capoeirista é uma pedra lapidada de muito valor. Professor/a que acompanha o grupo de 10 a 13 anos. Transmite respeito, dignidade, devoção e sinceridade.', min:24,max:36,nivel:'professor'},
  {id:11,n:12,nome:'Roxa e Marrom',     c1:'#7030a0',c2:'#7a3818',sim:'Professor/a 2º Grau',desc:'Professor/a de segundo grau.',                                                                                                              min:24, max:36, nivel:'professor'},
  {id:12,n:13,nome:'Marrom',            c1:'#8a4018',c2:'#6a2e10',sim:'Terra',              desc:'O capoeirista começa a plantar suas primeiras raízes. Transmite respeito, maturidade, consciência e responsabilidade. (Contra Mestre/a)',    min:24, max:48, nivel:'contramestre'},
  {id:13,n:14,nome:'Marrom e Preto',    c1:'#8a4018',c2:'#1a1a1a',sim:'Contra Mestre 2º',  desc:'Contra Mestre de segundo grau.',                                                                                                             min:24, max:48, nivel:'contramestre'},
  {id:14,n:15,nome:'Preta',             c1:'#2a2a2a',c2:'#101010',sim:'Minérios e Negros Criadores', desc:'Simboliza os criadores da Capoeira. O mestre passou por muitas dificuldades e experiências. Transmite respeito, autoridade e maturidade. (Mestre/a)', min:36,max:60,nivel:'mestre'},
  {id:15,n:16,nome:'Preta e Branca',    c1:'#2a2a2a',c2:'#e8e4d8',sim:'Mestre de 2º Grau', desc:'Mestre de segundo grau — a junção da escuridão com a luz.',                                                                                 min:36, max:60, nivel:'mestre'},
  {id:16,n:17,nome:'Branca',            c1:'#e8e4d8',c2:'#d0ccbc',sim:'Luz',               desc:'A última etapa — transformação de todos os caminhos no universo da Capoeira. A mistura de todas as cores. Grão Mestre da Capoeira.',          min:48,max:999,nivel:'grandmestre'},
];
const NIVEL_COR={
  iniciante:{bg:'rgba(7,157,40,.12)',bd:'rgba(7,157,40,.3)',tx:'#4ebe6a'},
  basico:{bg:'rgba(184,96,16,.13)',bd:'rgba(208,96,0,.3)',tx:'#e08040'},
  intermediario:{bg:'rgba(249,212,65,.12)',bd:'rgba(249,212,65,.28)',tx:'#f9d441'},
  avancado:{bg:'rgba(7,62,142,.13)',bd:'rgba(7,62,142,.28)',tx:'#4a7acc'},
  instrutor:{bg:'rgba(16,140,140,.12)',bd:'rgba(16,140,140,.28)',tx:'#40b8b8'},
  professor:{bg:'rgba(122,56,184,.1)',bd:'rgba(122,56,184,.24)',tx:'#a878d0'},
  contramestre:{bg:'rgba(184,76,48,.13)',bd:'rgba(184,76,48,.3)',tx:'#d4704a'},
  mestre:{bg:'rgba(122,56,184,.13)',bd:'rgba(122,56,184,.28)',tx:'#9060d0'},
  grandmestre:{bg:'rgba(238,244,239,.1)',bd:'rgba(238,244,239,.2)',tx:'#f0f0e4'},
};

const CORD_IMGS = [
  'data:image/png;base64,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',
  'data:image/png;base64,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',
  'data:image/png;base64,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',
  'data:image/png;base64,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',
  'data:image/png;base64,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',
  'data:image/png;base64,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',
  'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFoAAABoCAYAAABxGuekAAAqsUlEQVR42u29649k93nn93me3+9cqrq6e2Z6pufGISmKFCXxJpmWJdmSlWizjtfeGItNDDh54TU2ibFGXuy7/AX7IsibAAFyQYAASXYRYGHEqwSRtbY36wiWFFkWRYnWjReNSA6HHM6tb9VVdS6/58mLc6qnuqdnOBSnaVvyIQ57qqq76tT3PL/vc39+8qPdl0c7afI5D0ldpUlmx90lqOqWYIG/wYc6CcCEAOCgi68LGMlG4iDdi40i1SDLnx/E/LWVbImIEFEEAbfufaF7fODNAGzx8xcexajZOCQdJ/eBuxgYIjLjZ+RwlUacJEjl5kUyW5m1zUfcvYiavZRrIJeMCAQRcEe8v213ANsP+ZwYCATTWXIfiRji2rhYBmIHbtBPzWHSSbb6HtgtSOUCjpSN20m3Fqmm00GWXyITIAL90lhE9V5XlxJRso3gOhFTW7yYg0vtp+0QkcpB3b0wQV2lQWVmCknIJk31iWlTX6g9kXAMxwRQATkEaL/zLdBRsUQu8U1vfVXRibiHqm0eV2X60wqwOqaOJXzgKg0ijbkPzX3oKi1Bxy5gUSe7TfXJjd2dZ8ftlAbDEFqcZC24g1l3ut/9M4NkRCnGShirayWEiapu8zN6eMcoakJwgaSExm1tmpqVidXMaGhxJARMHBe60x3c9yjgoFRrRsYgK4mSX8ZEVXU7hHA1ua38FHBxsAVaFTBZ0Dtzyb4T4AaZC9Sezkyb+uO71ezUpK7oqERIAqkHGnqwrQNbb+foQB5zCs1fdpfQPzlxT8uIKT/Dh3dA3gK7rZ/ZbapHJ20n2UnAVXCRjrcXwD5oekRxyKQgD3krzW6GeUEmVWptJUq4+TedBvbs5YP28z383Xw1mIqJQ2O25qkppJHK3S8t5SUZSibaGXtKB7J5xx16i0MiBlEziqxAG52Y2SlgKiIVf3vgKo06CZHKxUPT2pqk5nF3L1T1FQsRkUiGItDb2IfY0ThEgTzPCVW46s6jwFRVt35arOiDkj33GA/j9Pnvzf/GQV2lAqncKESlatzW6Ozs5CH/cchAQ+yhPtzA07lVkmkkSLyBSQgWx5F442ddmkVkJmDuXnRoSWUqqbez46StPz6x5lzliRanFUhBespYcBMdJCXHpaWWxE6zzeZs+9zEps+apoJorYvFvQ92be8WSzgqSfyJgXqPnu2dPl/A1ElqEJwm1/DmMCteGOUDcmJP7Ikc3bOvFXVEuhBJlEgkbETPbqhJf5GW/cxK9AFzcJ/pJwRTaPFRbencNDUfmKaaGS0NjmvAFkyP2EEsKEoIgRjjNFqz0aJruINocyeCPypJvmeJmy/pOy/96f0C/E4S7gLJbHXW1M+IeeaFv0QsUCImt5RjlJ5GFFBRQshQrTc0YUBKUPyt7XE4rSS8UCEl95Hjxaypn3YBEXlJA4goEqS3OhaOgJKHSKXhKkmbLiS4n5ff76X7Ts7fEcdE7kkHSdAtS7baig9J7SNSz6oU0muaD4AubBfdfU9BKoGoGVEzCxJvuKe1o1zaf9XUcg+3evJO7++q2+IklXDVk60mt9VZ23wkpbQeNfxFESKZRKJIRx4KBIRcInnIySVeTl4fV9eFJECnGG/d4blFctAa6f4mkYq/SiCPyumax7NFpJk7NeIYoltmXrj7yDyVO/V0q435S8Mc9JZiVKSTaXLJCKJb6joTU7sVp9bmb9n5kGife7kQz67m1si0qT8+S81DtSXEk4F0hkgSoyHReqKm5vLGm/8BuU1FZGakkeGlKhMT1Kw9iXYpr7lmVdeqk7JOwk2s+EmXtIhUuKYDf1cedCjqun4ypbQeQrgaQrg6l+IQwtU21Q/fSbJFZHaH5289l2wkIjMTwmKSYNE9n0cBD+oVdRLmRUTGuYQrcU7QIkJAcAIudJId48XWm5NuPkQkqDJzt8IhiMjM3yMnHgTu4HvUVfUREakOgqKq26q6JSKzGOOlGOOlEMJVdy+apnkspbQOEDO9LCLV4nvO38fdy/nn3ylHKgevq6eKewxIIQKN2clOGM075d2/awIMp6bhenWNcT3+RJvqhwgylcAkebtmQpDAxD2N5pQiDmKy50G63C7RB29E/2WLg6/Pfxax+N4eL5qtmNmquxc9+FVd10+4ezm/EYvSHEK4Wqf60YNSeifePvA7s7tx/V7s5B10wGKWPd5m0vS/oghlVjJtZtfrVD+pKlNczN1LB5UFjdw/R2D/BaqT9lL9+wEtDwP2Nomu6yfm4M6/2FzCAcqy/JqZrZrZysH3SCmtL3xOeRh4h63A/vlyEfT5zf0JgiWNB52IucbOF5c+ey57pp6gZFoQY7ykjW4d9j4JH/ZqdOEitHWT6GpBhHSvAB/2OMuyV1JK63MqmIPl7qWZrSw8X/VUUrl70bbthbZtL4Q8XFoEdRGsg3RyGJg9Jw9VZLL4+pyH72TnL9CHKlKZUsT+U/dldaUPOWUEili0dagvJup1d8+6ZXq4Ad9laDwIkvYei+8D+KDkLUrPwdcm1eSxuy7h/sub2WrTNI/O+bsHfnvxRiyshJU9wA5QyuLK2ScQYD9JrYuZrbrITMHi4WlzAVGEQBYzsix7xZo0Mm9XNeg2gtoeP7+DQU/HwweleJGf54DPKWDvxrS+kuf592KMr6eU1quqerZpmsdUdSvGeKlt2wt5nn83xnhpLskppfUe7FkirS4APTsI8OIqWKSkxRXYK30FghzwGIX9ce3D4tlGR6vxTto29nKdEygkG7deTx1GXaFJO0rennDpboqhnSJ0TV3C0xQzGreRCIjHibsnp1kV86z/EhHzDGkLfHrGzFa1jZ3Z6NMzANboSNr8eJWmj1+7fim8/sZLvH31MtWsWVfiYyvLJzl75oHHzp+/wPLKWpOH4YtJRN1llPAymM5EpDJ0hErlGsYuklAysKyzItKooz7J1EVFgon01CCHJwjeZTwbBKRLk99uzzhGa1NQZ2Y117c3Tu2mnc9bmaqUN3Fqs2eyYviN3Un9+UKWn6PytWPD0b/Yvvr2f5PRoJnc2G3TE0liixVj3KP47KRbvS4mYKJlzH5w8+brv3HlyrfIs8DujUiZK5s7P6QsImm8zIkTJ7ly42VafZu1s7tImLC2corNaxWbV42NGxXjsZGVZxid+ADDtbMMTywxGq0wCiOOjdYmjapWLmUxWv6TinS2xUeDQfFnyaoLKt5kIpsBmSg6UcI4ELbQuO3B95T5wmrYs3DMblUKHEZHIcbLTdM86i6hA/rQo8VshijMkrM52Wa73Xm2idValVXrjTZrLVKmxMpSWP3jNK2evnn54n/74x88R7VzCfMpxAIkIpQojugEpe0KCi1n89ouZ06v8pnPfBC8Zvtazbeff45f/uWnGQ6HbN1o+eIf/gmf+NTP8fgz57YmzSury6tKtZOINmIpnrxcTzm/ubXDlWvbvHm9ZmtaY1kiLzPKmFO3gZoh5fJZitWznDj3gZc1G7w4q6tns1wuRbwK6pPoMlHitpBtRcmuuIiR+cTEikUQ3w3Qs9nsF0ej0b9sk6/Fu4q+zrO7Ql6MyFyeq9P4F11kRWNxyZv6yTzI5YzURNk63k5/yANnrzJ8eIOMbQoLXR2mJlQdCTVIjYihNsCbk3zn+a8yu7bDiZMFjzyVXz2x7Ovf+NoX+Oy/8++zcqrmyU+sYNJQ7a4Mm+pxvvgnXyfTJYZFxaC8dv7hCyc4fXopHTvRhI8+VrBUKintcmP3LepyysQjs/Y0s7bk5R9vUQ7yx5aPPbwRLNumtqGJFaqeJRXMBSUbuwwMlVmwmbqm4iCA9+qYDYbDP3bQuq6fvAvQ2uduHZWMPItkqYEKSLYs0XdGg+EX1Uk2qZ5udnZ/fffGdT78gVXOnXGkdgZmBDdcFKTGtONzxzALpLrkQx/4+2/91//Vf3f2t3/nH3L95uvrg2U4fvwsr/74Jo8+dZ7106f55//L73PyxDey0coJnnnq03zxi3/Opz79d6hc+H++8V2u3fxWKLItzh4fcX79BI9dOMfpB05TZxsczws2dwbcHDvtZJN2ukOT7/yChuXLHW9rY5HWXUYC6lqvJ9GkwsQ9tXLIip/b1u8EdAjh6u7u7j/I8/L5uwLtnpN6MzuIEjMhtDXCeF3wUVvF8yEVG6HKbcipL8ru6i+0GzCTGtoSYwaecHIaIkZNQ4bhtLYMfpzdbc4+8bF/xD//l9/kP/unn6UoisvnP3zs/P/8P36BC9+c8vb1FyFNeOqZIZ/57Mep6zJ994cPhCkl5dJpzjz1AGcGP8+02mDr+hbPXd/iG6/XlO02tvk2gyywOXuV0akH0OEaKx8oiZJIPjue2rxB40ZyTRpMPdSrKs1ZjZsXkLCFl1fFsg0RKVRv9yXeyeSr6/oJV2lCkI34Di4koY+uKxC0JIbBi8HGH0mpWi+z/Otty4WgupFpuLK7tc0Lb7/IsHiVQXYDb8adgeMFrTit1CRxWleSL6O8Sduc4ft/WfHKj25w5l+9zoMPnT7/rW+9wI9fu4g0O3zs6bP84uc+yfrZkp3JJrE4tiGBk6+9cYWnLjzJTFrG05rWAqsnz3F6XZltbLJ75VVWRxknVgpqIlIeY9cyUjWjbnewYMMsC7iqKkpXa2cDVwNrC1OyaFap+nTB1NtnX98N6HlecXl5+X+d7Ix/M94teSEkVLq6YHOItkQhZ25U7n9hafeJxljDLWhokGzn+MlzLcNMWT+eMxqOyH0FcQXJu/KpUJFESRQkH6K6Qhkf58rrPyBr1viT338bia+wcvI6v/kPP8gnn17l1PESCYaNA16d4kt/9K2TK8ce5bW3b7Bx/SqzpiFfguPDgq03X+S1115guZjyoQ+WnDuzzeqxktHxj7A9zvn293bZ2LzO8bWTlPnypGp86KFddpFShB0IlXg2FgtXu4pSbwxbCSHMfpKgWUrNefd8JCLVXYFGWsSF4BEDMiDTkkyLi3UaP2vWnsyz8Kq39WhruvGfZsOSc+ce4cypVbx6qy/LjAh5V6Omfb0aBeYDxEvGmw3j7YtUs7c5t/5Bnv3E4/zyr3yO9fWKQTYmCmyPnX/1hf+bH758k1/99d8mDI7zja/+OT/+9iYhd6rmJk11g3PrIz77c4/wwQdPkhe7hOENNnZ3sFDSaMasNVozJGTs7OwMY14iorhJRuKEoDsQpi5Zo0LjmlTwuXNVvVvvsCiK5yaz6eejhq27mncw6/2cJQyoBaYyYbN9i5362n/c+OyRum4+WoSl5+qtzf/kzYvffTak6zyw7iwPEvXuDhhYm+EuGC1mRkoJSxmb1xtefvH7mF3m5z/xCGdOZ5w8OSJKYDxe4oevRL7/4qv86LWv89DD5/jks5/n7Tc2+c43/5Jf+3uf4eT6Fh6uonGHvByQZ+dwVpnOSiazguvbysXXb/Cj168wawMnzj3EmfOPsrR8EiMSYkEIgRACBEGjIIGJZnq18xrDuI8EXpt7kSIym7v5ix7lYXESEysl6FYwreI7+NBdDKT/EQQyhCJE6pi95NYMyaHMB1/2hpWaY89efv1tvvOXb7Gz+RZ53uIJUlOQWsFtRtvWWOt4o0Rb4XOf+yS/8GljOLpCPX2L3ek2Vy/P+Pbz17n45jLF6AS/9Y/+c5I1/L9//B1+9MPX+N3f+W0efqicLQ2bkpCTbMDuTLhydYc3rmxz6e2GmxtLIA+TDz7IuQtPkS+XaCFIFmncCJng3uLuuAtqnQ8tQVTcho6aIJW77oUQFjn6XqJ57l6IeQFUdzfvvLhV/Ju6ytQoAwZyAos8V01unmub6SMz59FYrHzlwiNP/f75Bz70qJK0qjefmfh1kjtpeoy2AbcxqZ3R1kAd+OZXn+fy2JmWKzTtjKtvCs//fy+wdX2bEFs+/yunePDRR3j98tv8wf/5LV57LWNWrXFdz7N7fadMNmCys8L1a8L1axU7VSIUxxmunWTp4bNIdYw8XyEbRiwYM6+hhVaNQluiZri3iAmigluERImESSA0HiQcFqe5U4j1NgR7S8VJgzsD7V26Fte9BiQ1iAFySlpdYZi1f9y2nEytr5k0Iy2yH0kM1wNhq82zjUG2stq6HU/10Lz1leSTk5YqvAJpA2cenvJHX/4Cx89+mDde/yaT67s89fgTfPqXPsAjj5z+vzbHL//G91/6Ln/4b77JE8/8GuWogHCSL/3pN2nSJpY2WV5e5tjyY4xW11nLh6QgVKFmqxHWhkOSGU1TdQGyMidkCjhV1aBF6GNojpuCOG4Rt4CrKIeEeA+L8t0p6B9UN5L7CHeNd7XtCB263uJmfbpLyXAKIjQyjK47SD3w0A6zgd9IKQVPvqqqV6xeMSwhsvW4aT0k9cZi2AULPPzYg4yGv8UfffFLfPDhB/nH/+STN+vpGyfK4Pzw4sXfeOUHU77wxb/k1/7DT/CxTzzIk0+v8eU/fYWVlQ/TNoFkM0Qz0BVaKRGEpA0xF0QS4+oGecgJWY6GDLOAt11FVtBOb4h10SNXQfYKmsWsq5ZLh8XM341SVAxHuCtHd6yhiBhI08esA8EjwXNWi7UNlfAHW9W1f1LNqmdNqrVuqUkQGV7JJVwxkUkiHndpHnYMxUiSSOIUZcH6mXP8+q//Dj9++at88Q+/duKjHz3GzsYGb766weWLiRMrqzx8YYWTx2revnyR1ZEzGW8yXH6QLC5TJadqIk3VIsnI3cnEiZlSlh1G5om6TrhAzAqKrJNs7cPBPbh7NOkqjbznkgXLzGQFPANp4l0MbmxeZKAR0YjQ9rmXSOYRbSKZuZVaf0VVtz1rtG6rj1RV84xbfSpKg3sMNEs3opWZ+M751ipIOZIMySuoE1GHnH/oo1x5a8pffOMa33vhBZ740Dn+6X/x7/G1r/4+q9kblD5kYBnTzW2WTjzE1HfZbSosRmSwRKYZuThZMuIUZAq1tliEmAeKQUE2zAlZBHMsJdACJYDHLnknAkpC2wzVIKrtYkhzMS95T8nnZKuqTFCp7kGiF2MfoZNwh+iwWgakHjKeRa2TPS7GxJESD00IetWtegghUwY3AxpF9AyEIBJJIVHNxpTDkvHGlKXVY1woniHILpff2OKjTzxEm17j5z9+jOtbV2jGU6JGmmYX9xYLqVcahtOQzGmTEV0JEoghp1XwTAhRcXeaWUXbtmRZRow5Il3Mfa//REDVG0FM1Ju7udvvDLg2IoaIjnFt9O6B64UYtQfwvCtOsg52b51BJpwYLX17GIZf91aLIEsvh2zw/Vnjj7gWNzzEbc+qUkOVdSmmHJXuLIpjjGctYRhoY4XnTu3wwCMfosUphrugY27cqMnLs4QyUvuEZBWanNgGQiVIZUiTcFeSKo3CTCpSTLgYJoaLoBqJEhEJuIGr92fCI6gKQpgEwpZYnPU281YI4eq8xGFuTy9kaG67AfMzkF0XC43YO3D0/lyAdsUKey90LrrQElGKmH+/Sel4ixVgVYz5xa7W1SA0K+4pU3TLLAxFOk2PBkJWoBhmjqngUUkExpNdJNRoaGnriFkJ1KTe9u0qNCPi4KKIKFEURLEAEgQJTgidxKp2v6MauiJlVURBg3S/23XEJhHpei2FMejksIKbd0Mf8yqv+9LeFmPOoFz6cZmVz2FeiHkWY/bqwTvcJ00nqt0XVVWyLCOEsPc4xhwMbt7cmIcaqeu6dyyclNJewY/IHEBZeCz7XrsF8v6fHdDduXA9W73kbs+9vzvx8r2C7Wrqaqp3N01ur9g58GGoQ4yRsijIs+xFda0w0b0shKCoVF3sVxqCjl1BgnZWQJ4hIaASu6UdckC5cX2jqwWMOdPpDEtdKaaZ9VzagUPoQQvamWhy+Kn7AT3snCy4092p3hzsIj5YW3LPwvie6odVMQQVIZOMPOQWRLfEgT4Je+sCPRGYgBQSmIlI6ZYIIWCtIDFAysiks3F3dqa4BUIomExme63WKXl3U2KOu6FzRYagMpdu+nM/wF3jpaJBunP/athLUYl6K6KV6P7U1bs19UysfEegFzsBbnty/kMF6VLhBAJFljHMB18xs9XG2nURnUiw6GgmaBTz0khlV0uc1oOFUiQgrRKDklIk4MSYU1cNZhAJ7Ow2fV+7YOY9xURaa1ERvG880x5IUVDldqntA0jzc1GaVXVbFgJHIlIh3Ca9i6+/m7Dpu5douX3wh/TF7JnmDIvhldTaX1g7+UwUy1rRbgiAqIokCyIbIsxcogVhxd1L1TjMgiJNQ3AjxgwzaBNEDUwndEEpB+s9VFXtBpWI4gRM+rJjFYKCiBNCQFRvARuVEPU2oCUyRr3RwFiVMapTF0kq3FGa7wXoxY62+N7U4Dz30kE/b+BvY/tC1VRPmziGZ66gprh6X85LUrGAhrElX5GgD2qMOxqzZWlbVCJCRmqFlAWqGppkJBeSCybala/1loSje/+hXXhGVJBwZ06WW4pxshj6nPNz99ibw7j4J/EW9Z1MuwVXdO+JzorqnABVJUog9l80l4xhPmBluPy/i2ubabychXB5Xj2kqtsx6pUsy1529yIvsu/F2F3GYDC4nnA0ZsyaFtWMyW7FdArugdQKTZMYDAa90xGJMRLCLS7eL61CCNrFd4PcBnKIMtNMrocQroUQrkoIG6hOF+LOWwcspq29iNxCVes7cXhKaf09SXTXnyh7A3C0f1RGSCQrmunLlVePuEmmhLEIJNo1dzvuncbM3L2QGG4qukmymGclWezCs5Y6yrAE1vOz950JhIC604p3gSFdsIRUEPE7WiDzE71lQYjIjAN1G4dPR3pX+FSd+RsvxXfLz7eHUr0rSehKZMjoFFGKQwZ59Wdtk1bNmvOqYSzKBDe11B5PKDHGS/MLUcNItpZl2U6McdkMmiS0rXcxFw+4dzy9J70Ewt5wEkUJBNmvCAl6u90c9n5na14Q2Sm/bsVpYNzTxnvqgUmtn8zz/LvvmaO9L/l1jK67qzOxoOstH5WjtrH6u16356ANIoL5/IuFWcj1Sp3sfCS8aU0643iZxXDNhOXuvZWmNawzcWiTYwkkxD5O0UmvybwlteNo6Tl6EeQDVsaic7I1/zc9X0uvBN+L3Tz3JpumeVREKn2nPoG7rZ49Z4DQZbutCzWKK9EDwzBgmJWvFLH4XnQdi2sTkEnUriI/xnhpHksA1/65192drMgRDbiFLgGnsR9fZHf0Cu/mpIhIJ8kBFsDdUtVtFzFUJ6LedDb0nS2NdwN0FvKLqbGznhi+Z46+xYsK1s2E61i7G8xX5gMstX82rdqi9fSwiVQhZJcRGxqmqkykt1fzPLsoqV2t24qiKFCNpD64JRq7QJDonmstfdpHTLvYCd51qwp3BfyAArvlCQrtXHLv1mpxr0dd10+WZfnVEMLVe4t1HJDs2wS9B3cvQ9FLtblRaslosGRFnr8gIrMguqVIJe7q7kUfGdsS9SbP44tt217Y2dkhmXXe3Hw6wEK0IGhG0OyukrxP6R0QClRmC4qwEvUWWZhaKdIs9KnMflKTrm3bC6q6HUTG75mjZbGQXRbvgGJtIM9yojqV7l6piTdMdBvSSmtpXUllCGwkZZDEhh51XDXp0fH2Lm3VgscOaAHVGaJd5Z4EIChYP4pE5pN1OmA7V3v/yvNbVPcTA/duj7Isv7a7u/sP8hgvxndlZRx8+lbDy36gvTPCSs27KKkqq4MlwL64ORn/R26M8lBeinmzsz3d+a0mi5N8qfja9qz+XCiKH1Tj2cdX8hHFYNSMJ+NssARFvonYLuYtkglJBZeuXF5T6oYGeOwcGDVcQUNAQ+iuUztX3VG7rdaZMBF0Mrc05uMj5jbzT3pT2lQ/vLyy9C9SnS7c/ylgC+PJAhAMogcKyRnkS5T50leiFq+ph4m0PsxUrseoVyw4rlpJ0C3B8JQYj2dZiBkhgJuBBc6cOg8SqFONy9w39fkQ18NnGul++nivlHCvR57n393e3v7dlNL60Y9bk85VzwiUsWRYDK5kml3CRD0xzEL5UqbZJRKFKFWM4c0QExqMwdKQGJbIFJrpMtNxwbBcRyVnMBh09YE6H6E675e0Hki9F2VeHQzq39ev3ivbkIdLerQAd9/drWuBDmQUcUiWDV4IEm9AnIjoxJMUbWPnwTLRRJCWGBVri3TzprM8OsPy8tnnYxxSVQ1VVVFVDUKGWoZIoAvYNiiJ+ZjiAxL8jhbEwcr+9wpB0zSPDofDf21mK0cq0UE7uxXvInhCpAglg2zIIBt+TZIiKSRvfUVFJkF0K9nsodZ2uoRqu3J1d2vIaPksLnEi2tLYLssrA/K8BBt1p2eIOGgFMu3bp/opz4d0nd218OU+Snbyds1Io7qtPnLk1KHSpaOU0M9OKCjzJZYGKxu5FBclBROLVably0EZN/XkWdWa9VOrXH7jrbObmxO2NxNXr45/yaXci6tsb28y76eU+Tw/Sag40puXh9n7h9HGUX33eYteURTPxaODuK8jE+vsakL3U4RCczQz2nL0p6m2AmvXVFMws5Gnulw7UfKxDz/I6XMFP34t8mdffpGVYy/RyBKzaUGdWk6dPsHWzrgD1Jueo7TL1vdzzN8pKHTQze6DN/eVo1WZqOr2kUp0attb39UFMe35UwgeWBqMyMPge5IUGhmktj2v1nDq5CrPPPWh/yFmzsmTxxkMC55++kn+7q/+nS999InHmEy3mEzGt6S5l9RbEyq7MazKoRz9vk2oNLMVEal2dnZ++0iAnntkIVPwNM97sWfSOl3qS3MGcXBpEId/roRxofHV6e4WmTbcuH7l9+pK2NjYJvk2a6cNLd5+JMlbDJcCqhHS0gJHd/V2XdFKt4LmDpWI7GXR52AvTko4WCl6P+nEjMERU0dvdu15i7rHpXOrIGhkkJUMkX9TT5sLyaarJ1aPNZduXMle+M4lzqyvcvXaJZoEL73yPJ6vPL6xeZXy9A5xuIaod/sb9O9vfX3H4ZVWf7VHPOoPcNnvRKgv3IjWyEJkNStprfnS9a0bv1mIbBxbHqyfPV2wtDrlk59+mGEe+dZzL7A1LXjgQz/HhbMP8fqNCd0SUaCnKCuAnM5H5zYFeLcSryNZ2f4+Ae17/w894osXYQRxpDViFlgerFwZ7+bfvXb52t87d+oUH/7QaCcbboZXL/5o+Olf+hgrqx9Ml9/28KMrFdeuXWc4OsVk1oIEXAzvK5a6UmPHtX3Xpt0R2FxtV0OnrR4lyIZ3YMv+gFMXsjc0ZqgI9awhDznrx0/9lxtXb1CEyBuvXlq+fmU8HO9MyWJNXV8Ju7PLZHmFiNDUCj4AK/q8Tv/eapg2XZnx3Pw7xLx7X2B2krpW6jo7cjva9lJe+6VZcWgqyiwnCznWOoXmtLOGYTngzTcu461RT2tm022Wl3OKvKtUwnNiGHYKb15AowEk9LmHvtJ0wbw7LM7xPkDdzCer6dFSh+wPAc4f9lu8pLoCUYqY4a2zszX+RBBlUJbkWaBNFUji5s2b1JWxtVGzvdlgKdDULUjbF8i3t0ofXPvn264Q884c/b5QyFzxHyFHa88Wvk8hitPN9/BAKIZYk8Args1oZxu/kmlid3dGVbdsbWzSti2zqqVpApPaMFfKImNCQxJBvesj0C7E1AOrC8njwyRA7bYwn5i+201s3o0xcGQSLb3LoH32em8hC4gE0BIYkloYZk6WNrn+xvf+2cPnjvHKjy+ydGydNimzqVO1BZVFJtWMSbtN8h3yUNMlRhQkYppjGrqmIDKCZ6iGLsbi89RtPznYvFC/tQ2KYgRkOh/qom4h4O95mGLr7XrIw6Xk7Ul9P5bNLbbuk2De0UpywTyQmpblQcnp48efn+yM2dpuOXv+Q4issrstjCeBt6/NmFTO0nCZlCrcGnTPK1TmO6DYXiy8t9t7U+9WdkXsziPZPN1X/WS2mlJa1yxePnJlKIvOy4GhWiFCnpfUlWOpYHn57D9LaZlZPWAwfPD5ZCeYTJcxO8F0WtK2I+o6Z3urwi3uB1G9K5pR65qbSD24i+k2DyI0Bzn6qPg6y/Mf1E3zuJmtvk/7rPQB+QP7nFWzXoWFAaJDTp/54B888eRn/v7jj30K8ZPPP3D+2bc2N0tee23K0tKDPPTg04x3YePGjEE5omvGU0S6JBV9caP0LRNdJf9ewrZZyKrMjjLgv6elVLf2pkoevdpNC7TRWRwuAQdi1imJvMxJTWB3UgHHXsTX+OZzb/xj0pgnnvpVYlkyGD5w+crNK+cH5WlWT55hVgmqGe6+N+JdgyPa9aaohANdADR7cYzgLbq/EqmnFUAaE9d+5Nx7mk9dVdWz84lmRwu02OGRSrE9i2Ayg6Kgq/q3JY6vPfjKs59Yktl0+2PHV4pvv/nmG//991764e+l0J7Py3WOHRuytnYGzwJbu2NcHPGEi6MqfanX/rKwg4Xmt6exOBKpdvciy7JXOn3lfnRAO0DCSJ1VLV2Zl7l21fwqVP1XbGunaaeEaMQIQZ2drRtogI2trd9tsZWZpwubO9u/N22r7ObOFsVSSVLDPfU2lHeVpQFUYjdGXyIhhBRCuCqR+bSCq31V61siUhF0fNiAqvfM4epJRCpLjI6eo/fZsrqPs5vWyTLIcwiZMBgOCbFgOmvZGs+QMKRNBaOV0/9TiKMXgg4u5vnwG3jg1IlTXZEjQtgrTZO9EOm9uttH7bjMa++OmDoA6TptvZfqeXprz2tzIRloMBpLGC2aRUJftou3pFSTZcUPPOrY8NLEysls99ksRtSNhBNDV+zYxU0VkYCErs1CAmMJjG91XDFVZeIqrcm8GOHWNII7jeZ8918/TIPKFUtp7eiV4VyS3fdKAeaAC20/QawDPoh1WzOK9+5793vJfdTZxjLJY/byUj78tyHIzZ3dnb9bE/f0gErfDcC+mrvZQnnu1kKt3fvigs/L3t6HMOlCesnnjrItpBUNFcd72zeI4drlGTU65kY0xo35SpRwVYRGlUmWwqvWtOdDCh+trO43JxRUu6HLdMpw1uXsOgkW8aTK1FVaV2n0QBPQwnUfumvcuz2C6kZq23NN0zz2Pkk0C8ElXYzrIf3OloKjAi7d1phJurYIM8OsBcKVbgnTCBaUvF1ZWvnfsnr6i6EJn6qlXU9iXTSvs6Enqoz75Oi+1uKDXbBHJd1VVT3bT2ovjxho62NqC6l/ly5TLdqbZbcqi+b9gaqKuOPJUISoGUowM5uq2bTrM1Adlfn/IRo3TFC3+qN4e6YlDUVk3mE16SXZRNxctbnbiIj5SP37tqJNYjEYfMPdi3h0tLHfC3QRdLGX3AW68dLMWzK7G+Dd3os4ySqga3NTdVwEkxYlXBOaqSiTNiuPG2mE6Yam6qNm6Wk652SmKlsdyPO+wf0F5gdNOuf+bklVFMVzTdM8JiKzI5ZoX6CJsP+pvQjQ/BK62MQ8n6tYP/OooxX3rpfFNRAwVOPYSAwiz2uUjeDxZW35PK1PGpozGmVDxE01bM07wlxpRDrbdnEyo9+akbGoxEqRu294cw9RpeFsUn2uHORfj0fJyLc6b7tIWj/dfr+W9EUb2zvLoX8xy7Keow1a74NF7PXKmCVizFsN8ZWM+AqNTEGbaM0FEwum7cC73e1mrtIcqPLfk+aDRef3N7AULpZl+bWj9Qz3qEPvLOyd+OzFK7rOq+7f1jZ79Rjz/hV3J3lHSy7QmmEkTA1zp27rtUk1++wkjT/TFPWw0eakQNIQbsyleL5T9OJE8w54y/aD/d72CfM2rQ2Hwy+1bXvhiKlD39kImWN+W9z6ViFOcuvDnd1LMq/j6BtKRXRv5nsM2Q2J8d+q6taYrc+mrgYBJeyoMLld4VnW5fXu/76N/RYmT5rZyvto3r3jRS1WEnU/5925cquXZd5yN18J7n2qrL8pXSdt2M7QP7W2NYxPJU/H1HVbYDzfG8ZJA3op7j+0mgvA/drxzgR1t+POEVod9xNwFcH2NQ/dAn2P+voBKDCvXhWaUH85JLk+a2bPGmlkBqpURjsCJrdcVcu6f9/fvcDmSvd9sKPvyUW9DeS9gFD/b2d/U5LOJd6dtHhTFuo3Ihmr5Qqx1u+paVPb7PHG2/XW/Lhq3yMKmHRzRUSk0fusrvremKlZGv21lOhb3H17XYaIHNjLVW5Z677YPyPkWiLBiXl4aZbia1ObfqwyezKJDR0a3xda9Pu+rauZrc6Vb/zrIs2H69K55O6X+LlEWz+Ybw52Z3PvRRqILgy1JMszcsuq0Mqf06asgoddEi2+srjN1H3/fgLJGUbR8V87iX4nKT9osewpwW6/qFsNoAAtRM3JohFRTFpqq18xt7J1HQRvMxMruuZque97NYYQrratnUkprR+xHX1/Jf7gY7tLRb84BA+4GYkE0Wi1ZcqM7WqbcTX+dxvaddSTBKau0szHfS6GON9LgsC5tR/j3yigDz53t/rnLrOlkLq4i4VECkZNxbSdMkkzZvXu0w1prfV23cUyCbo13wzy4BaA7xXovxHUcSfzT+9WwiW979OHXkFR6+Y+SQxksSR6eGHazk5N0+RTDZwUkRA03ADLzD1779U0nY0urk386w7qYZJ9r/lAw7vZSvSRQqSr+RMnw5FCCJpfA/2KpOnHkqehJ1tB/b5vg/3/A44pbYq0PVj3AAAAAElFTkSuQmCC',
  'data:image/png;base64,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',
  'data:image/png;base64,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',
  'data:image/png;base64,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',
  'data:image/png;base64,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',
  'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACsAAABQCAYAAACAuIzCAAAY60lEQVR42s2b2Y9l13Xef2vvfYY71L0198RqNrubzaY4KGSLFiXFtowoMmTESWDkIUACJEDyYCD/QJAggIMkL3lOXvIQBEiAGAaMJI6RybJkMTKjUBRFUk1xaLKn6qnmqlt3ONPeKw/n3qpb1UWKshDAB9g4p27fc8531/r22mt9a7eMqgyxQkbG9miL/WL/N70LVi1lpdWyw+7w5+QwThwWIcLSTFukSfP7Ru0whNDhz9lhnLEACIamNGjH7R2nbseUllijh/XXgjsc/58PNf7IeeoQVaXCowQqAgUlwypnMNhf6Jf739JG7iup5lQ1FTFDg+2L2L4EdapirbXrRx8ZIoAgIQEIaDJ+eTgJm4jtH7NfWT9jfFbfnPyLAzAYAuAwKNAQwIYtCN/eD8U3jNNKjH2ICiClqiYqAOJVx2AOTRMB6BikQH3bpxlyfL+oKVVAVBMVQVQT0Iipex9zq8UQWYemKar6KMv21ytCR9SOADwSgdbcMRq8hu6J/Arig2Br69R3Hlpu+vDR2MW5Kk6gmpwDOBGqI2BFwQgogiCABQdCYFQ1fphhL3rvl7yGrhjJVRQFwzGrChxxtVG8GjnGPamO/BX0wGCGGpiBaoyp0unn1bypba3oeKoZIgwxEa2ku9OQxjvGm0BJWyvaFrtX28p3g4R0MlRqvo4fXZ1ocQ1meojWxhIN7qRh9MAlR2lgJo5BEcBgaZs2WK08+iHkxmvVDkEizJhvRsOEcwEiA/7QwqZSDclk0k3IMA0AkVL0szmtYAGcqk5ceAy0GX8oNG0bjc0dUw56o5C96H2+ooQmMn6YUUQ1ETXl+Hl+8tyANhE1RwAc5SzmGH3q34BXsCp2eGBZVUVEDqmgWrtFavaijkQsGkHA71RF9bAK+UoQwTrpew1dghpVQNWoKqgpCRLUBBM0dIKE1EB5Ii2QzJ9IF0IQjIEDsEaMAZGxPU1thCAE7/FlwI0/S21CK26T2vgjqUi01DmD7WvlFwxmKGrKUFWnfVWdAzDG7KlqqqppCDRKr0tVoKNiM7HRuorNqkBnlGdfK6ryaa+hq1KHORUIUjs4hNCdDKmCZxIRJmdVBQloEKqq9om6gLrASIf0Rj16+e7fyEP+jInNo7zKnwdwLr6pQSJflk9qkMhF5j7GjFRCFELoeO+XQwhdNVLG1t3Gmr5zblXVt1U1CSF0CaExbWFnogcH1xP3y2H4GYM2BDEkieADVEGpCo+1joZLKIr0/bLIX3LW9UMImyoQ4dYxUNjQCBK6IpJrCI2g2hYxeRrHP3DOrQY08WW1UlbFxbwoL6pqEgQrIpkxpmeM2TPG9IxysOiISC5BFUUPLRoUVcUAXgURWwdQ9RShRFxArTKsBgxG++3Nva1/JpZhEI0Cvh0Ea5xdV4EQQseK6YXKL3uvcyrBiUiuAhNQGDNUfBORUkRyEcnH7u+oauKsfXRg2aqOPIjWIGUcb+vJrBRFiYsjRGoSlYVHxYMH603Zcq3vlSG7XIRyRaEpRr33fhmj3mD71aC4Fll7vxGlf6qGUJbl5aIsnzaW3CVmL8+L5xkvyfUPET8BPM4xumPLZlIccFYf424dgwIiQgiBqqoIoQIjqAmoCYyKETv727/VG+39bSLpaWT2Cl88XWp51gRTdePWH+T90TfKsrxsIvcgjuPrgdCsgl/yqjNRFN3AaPBoI6ApgFiz55xbNcbsVVotH9CgCH7s/oCqoj6Mw5cBAgGl9BUExVqLMYaqKsjznMJnc0kz2emN9q6t7a7/q34+eDVuJ9eTdvqd3f7uP9h8tG4/+fGH9DZ3GQwGtDstzpw7x7mVJ1g8tUy70/6Dsiwv28itirU7NXWqhUrDvIhkxtl1sYyCYGqwRUbQilB5Qlnhqwp8IIzB4yKyMusYJUTO9fPh6LnVO/eu3/jwYx48fMgT588hifBgY5XbD27Snp9h5eJ5NrY2+dEP36KpMTYYDIKqUuUFIQQa7RbduVkuPX2RZmeG7uIs7c4MURpjI4NzbpPYPSKJVtWqF7F919/b5Lvf+bY2nWPj0RqJtQiBdtIgqwKjSggCkfVYVapBTn9nxCcfrfLhBx/z0rWXmVvqcPPG27x34x0uXDyPfbRH5Q23XnuP0WiExbLUnaMaFMwkDWJjiTtdspkhd1b77OcDShNIZxucv7DC7NI8UeIWZ88sL85dWnk+7rb/Uz4qXnX//b/+ob7x+uvcufERPi+ZaTRoJTFWofRK6R1Yg5JhRVmcX2K+e5r+Tp8Htx6x/fC7/MZf+SadqMPe/R3eXdvmqdOXCLmwMrfC3JV5ut0Z5ruzUHry/QFrD++ztbHJjdsfoUZIWw12B/tkPufU6dMUvsDFEV/5xq/wYvQrnH36whfjKPrQrT3YYLiX8e6P3ifC4AK0koRiOMIZhy88zhlG1YChz1k6c45nn30JF80xf+YJNja2+PH1j3j+xYtcfe5LfPDRT1nfGdJozHPluZc5e3oeEwnpTMJTVy+xO9jl+gfv0u3v80xs6ff2yfsZo8GIvF/gS2XQH+FczO5eyXCYURTFRWPMnqsKJZIGT557mlaUMOr1SU3ESPqkSYwxYJzgbUmuntbsPJ25ZWbnzjG39CQ/fusd7q1vs7RzigsXrvLM1Rd5cP8hj27d4dkvfIHf+/e/xxd/6QVOX36CxUvnsIttnvu1V7GxZbjfI9sdsPtwk7KXk/cyRjs1YCEiajWYm5kjhMBoNHrJvfTCl3B5xLMXnqPpUsr9Ec24SZXlEAkhDgz9iFG2z2g0QmxClHbZ3s24efchf/Evf5Pr19+mnyv7vR5kGZJ53HrFf3njP7J0uourhCqrqMpAHDVJW65O+gY5Z5fneWr+SYqtEf2NHuV84OYnd9jY2GH+9GlCVcd/AFcWyief3KHsZwx7A8Io0IpTTICSEtO2VKZilA0YDIe0ZuY4d/4ihXfkVckP33yTVjMlzwsWO/NsbN/l3o3btG2D3/rWX2fuXId93SdTqDIhGglb2z0wkJoma2vbbNy6z/6jbfKdERtrW9y8dYcyKOdHW7SvzvDUqQbtdnvfjYqcfjbiow/eZ3djh1gSDILxoL7CUGATQ26UQZkTzXTYKQJzc4vYyLDQmUPLgod37/LRxruEquDatZd54vwK1ilvf/gezU4DN9PijT9+k6TbwbgYrQL97R5Ntbz75lv0t7fBB0ZlRmeuw/mnLzB/bp5hNqIoCrz3My5qRDx15SK9Xo8Lly6yNLdEqCrKvEJ8xf1bt4iSiJm5WZqzXUya4tIG1kaUZcm9W3dYe/iI0X4PMZ4vfeUaM7MzPNi9T+kLfNNSRIY4brDx4BF7N+6zu7VLNayo8oowymk1UtozCzQ6MecvnWfx3CI+VqLZmGa3hfee4XCIvPPmT/7d9777J39n7cEaaZwwGIwwCAuzcwBkWUbsEvq7eyzPLfLTd95jfn6ejc01fvDmG5gkYvncKeI0whiwRnAmMOz1KEJg7uwTxDMdQq785K132F7bIxbH0sIy2TCn02lz6twypy+cobvcpjHfoL3UYm5plngmQRqgTnHO4a6+cPXv2tTeHA2yb8RxfD3P82tOzE6apq/nVflMUJIyDxe7Sfv37318+5/ff/SQ4D33H9zmuasXOX/pAmvb6zQaDXZ7Ozx6cJ/e/g4rZ5YxcUSvzDjdPM3sQodX0wa9jT0aUUwIgb3+Pleev0p3eZbu2TnS2RhNFJsImhgKVyFBscEQQkAGoyFZluGpc4SiKJJJipZl2df6g/xb83NL/3B7c+93GnHj9f/xh//td3/y5pucPz1Pf3OdRIRfevkar/3x93jtT1+j0Wlx7csvkbQjLr/4Anc2M2bnz1DlGdVgQH+vx7lzp0mbCZIKpQPTstBwhEgJ1mOtwTmHMQY3zkecc8jO3jbiLN57smJEqHy79NVKURTPVVV1Pk2a//vu3QdvtJqzvx+Z9EaZ51989803vvX2G9/nlRe+wGv/83/x+p98n1ajxVMXLnH+0pPs9DcpZcQn9x/yG3/tb3H2/EW6MzNEVqjKEUkjYlgOGIWMKoLclpSieKMYJ0SJI4lirLVYiQ/AutglqAS8L7HiiKOorzpaD8YuNxvJD4ejwbeePHPq18uhPpPvZ78qZTV37dkv3L18duH8//0/rxHPzfDKN79OI+0w253HWctip8nqvY/pbexgshGuyEhMm1E2IE4dmc8hMViNCVrVKyeANVhnUBUoKiqpMGk0pfJUnnJUUuYVlFoH4YK5kPuVIs9fCmXxJL5Y3t/b++08z6/NdDv/RpzdCkZ5+Wuv8sqvfI3nrr1MrpZ2d5kbH97m7PIFXBUx3B6w+slN9rbXUJ9ThRLvLHmASmN8iIlMi1hbRCEhKh3kihaBEAA1ddo6Hvaf/pPfqRUY44iMw6hgVLbF2wzVRpTwYJiN/lJzZvY/BGuztd7uv7Ct+F3TsPMmdo1Tp87iSElCg1s/vcnNdz8hqYROnLL+4AFRy3Hq/FlmFufIxZIZh7oG0CSJZklNm1gbOI0xYgFDsII0YpJWsy6xROpcuixLvPcIlhACZVFfJ0nykTFmryz9k0ma/qCfjX5dYnc/bkVvVBLaFZKWKgzzgqWlJdrNFrsbe4Qc8l7BaGeA9cru9jZVKAlAo9UkeLAmIhuVlKOKkIF4S+pazCSzNKI2RmNCLhRZhcFgzGREBhMZvAmoBZNY1EEl3hjnHrkofV+xZSNuvG5C1Ww5ez3G57FEq82odT+OY6pQQqR1qV4GShWMVcRBuzNL8AanFs1zZiKLH/TopkLsCozLsc5jrMcaaMVNFtI55qVLo0yxWgPFKA4jdQGuoS4SjYIqGA2oetQOjZEtKyaomA4mLGhgqOI2Pd4YY1CjVOIZFiMqr3ivdOY6GFvXcN4rooKtpUecCQhVXYSKIKZWgIyxWLE4ExMbT2xiMjMEAgZb6waTYUxN6MNr07OMlW1raxEZs2CtTTRMdFY7F0XRorWWJEnqGs17ut15QqjLo6IoakHZGmTCP2OYKJiT9xlj6nDlLGIjYhcwAsFUBOUo2MlNE80LbP9AZvdm3lq7rthFAA2mqktmO5emads5l549e5Y719fGv80ePKcoCsaSUg3IOcSaiX41xckarDg3dJG5T0Q/dlFUaPFkFcoZdxzkgQJuLSJKQLdEJMeO9VZxd2sUtu+9X1a161FidlT1a2fOnEH1LUSEvChwUa03VFV1AESNENkIGf8Yw9iatgY7xrJnrV0XZ9aTKN5oSPJGpdWyO8mqh5Y1WCwi0seO3S62XctMtllb1s2J0ch7T5TEFFWJGqkToDjGOUcI4QCsF8E6h8qYEtgDsNZYjDGZFekbY3pWzE4k0W3n7H1x0jsCduKqabCRCEEC4kwuIqsSnBORbAJWJGpq5ReiKDri7qIoyMuCbhwRhDEgi1JzNlC/00r9eewsYu2e2Nqq1tp1Z9yDCLceSXTHWnvXTZP8UMg9yuNpDiJ2Y8zZ+ckEU8WnjQZFURBFEWINhS8YDAYH901czIH2e+jN8Q/ZFGt3jDE9Y+36hAqxiW8aNX0bXP9Q+Z4CO3mwquC9n5C4/p5xfRHJELvlvV8WE0Vi7KOdnR2aM22SZoO1tTW6rfq6LMtxnKzdH4KOATq898cjQ26tXbfOrRpr1i12z2J7TuxDo7amwSRcHdPyj/J4vE6Pz5VR01PVJHjwaKMK/kDFcS6q2z9AWZaEELDW1vz14chzx4YpjTE9Z8ymMWbPSs1XK2P5U9yOtSZ3x0FOW1dVx1FBEDUI4MctMK17Ehsa7HrwfkFVCbWPidP04L6yqghaWzOKIrx4xE6FKzFlzVGzbq3dmKaANTV3rZWRtVOLwsSS01nOhCJj9GOLm2mwCNHHE2l+Qqdms4lzh9Y8EKzHCwLmcAEaC8d7xpg9EclEJB9Hgp4xDLHkMv5hbvolj3dMzGN0mIA1E1qI7Y9fdHBfmqYoQwJKu90mjmOCjFtWIsjBnFAmAvIE5DRojOQY9WoUNcoRGjzO3cNwVrdOzGNgNQhj1ZpxOUQURYQQ8N4zMzNDkiSHdOIgymTGmHQa7ATk1HWGkQpTtxvNUUvKY9dTq8qR87HPehMOTng+yQvSNCVNU+I4Joqi9eMzf8qS2ZSF9w5Ba51cGT0K9sQu1UG8VcQylXTUNDYIVtymtRFGHEjARPVCEiQg4+JvvJqtGmOGE/dba9cxRyx7MA4/t4dtxOMTanpSiQjqgSCoVDBO6zAWI4oQMKK008ZGlSs7Wz36ox4SK/v5PkGUXq+H93Xl7L1fCiE0VZUqhIVJ72C6h3DM0znjRb8ej3/hMeuO29d1b0ymGR0wCr2d3V9L45S7d+8SRRHOGcTWzfUoTRARnHOb4yYeaZp+6Jxb9d4vHdlWAdFUMySrO4z2sd4yn81dcxS8Hs1F2+32dwmBjUdrGAXvPc1mE+/rhaIsywkF9kIIOOfuTreRDhock0n1KYeb7tmeCFhPDmvH08mHDx9y4cIFzi6coZEkFDYZZ1V1iigiuREJ467Pee91KXbulvDp4I5jORJnjwM+6QYZd8omR1EU7G7s/eM4jvnqV79KyzW5d/cDHq6tc+rUqbqYbLepqmpFrRmOU8ZOCNoVkQz9dK4ef787CdBngZ52vwJLS0tsPdpebrfb/NEffZuGSWgknsXFJl/58pdJZmaYm5ujLMtzqM2SJPlQpdaSq6paiWx881PATSLDp++ROW5lEfg07CLCvdXVV7Jh/stV4bn+7k/Q3PPC8xfxvuDBxh1OXXiahXPnxgtISJ1IVvlqxbp4NVTVmalnZcd5zMlT/fNx5oQ9WCwuLP+w1Wr95zt37tBsNul25jh35gliG3Pn9ipvvfVWra3W8TkLIXTzPJ+fAPx5tnz9zE1lQce93FCX7HUsBlVBVMmLHGvt+rPPPkvI4NYHtyYTiheef57cxZRlSRRF94MRX3m/HMfx0BjTq6rqzGTFMsb0jlt1Kg5/HrCfHgUmvV3nHHmeX1tbW+P+6j0uXrhAIwFnZ+gsNtFmmytXrpAkyY+yqnxWhCxo6FZVtWKM2ftZE+vnsizjKH2wGAQztTUHilHGztb2399a3yBNU27dukUae4aD2+Q64Ou/+Vc5deoUVVWteO+XRexQkFxVkyiO3xeV8lOsmR+P94Zf8GiMa68QAmdPnWV+do7lhUWstezt7XHnzp3JwnBZVRMRyZ1zq5/m8hOuf74J9lnHzs7Os48erYMaNjY2OHv2LFmW0Wm1eemll7h37x6j0Yg4jt9zzq1O31tV1crncf9BBviLghWx/Rs3bpCNRkRRxHCQMRiMqCpPmqYUWc729vaBxeoFIXQm1cExUNln54C/4LG1tfUv3377bTY3Nwkh0Ov1mJ2dxRjDrVu3abVarK+vUxTFcxMaqGoy0QZOoEP2C3O23ixhpuccqOH9jz78m3Ecc+2Vv0BWjWh1YgbZgLg5w6nTT9BdWKQ/HOJDmLE2uh9F0ceqmoqqVa13bowzLjd5rhnnC0Y/g7OP57S1/KmE+qtBDhNyLGosj9a2ePrqVTTy7GfbjOhDojzx1NMMfcTpladY291lVJS4KPkoy4pXujOz/7oqysuh8ssi6lVCNNnPdWDVeiPbn2EF05NXMwV++Ve//m8vP3OFnf1dbt//hM3ddaJmTIXQG4zY6vUIKoyygqIongPw3i9bazcmqeJ0GTNZHKZp8Lkn2LSEVJ8D01sHn75y+e9duXplc2FpkVNnz7CwvMDSmSV2ejvcunWTKIpYXKxDmaqm46R72Tl311q7MVWK96ZAZ5Oabvrd7vPP+mMppISDFHFlZeWFL3/11YfLS4t0Gm00eN55623ml5d45plnOH/5At1udz2O4+uTnXHW1prZxJLTQCdWPa63fQ6wYezw8ZB66x9G0aBUoWRuce7R8y8+l166/NQ3jReKbPRqd3b2Hz119RJPfeEyS2dO/+703vBxVMhCCN1j5Xd+QgVxOKatdWIeO95BFziceHWfoC5ZQlWX3qPBECeGsijqumx377er4JczLS+mzcZ3iqJ4vl5uD0OXqiZRFH18IBdZu2GtXXfOrTrnDhSdidL4My0r44aIhMB4vyyi4cje0Swb1h0bYymq/IqI5DZ1H6NmvaHudjlOWlQ1mfB2Siqa8LU3xd/H+PpzLQoH+2lPqL/EGpIkIUpixNodsXbHpck7KhJs5FZDCF3n3Gocx+9NLDe+d/0EJSY/LqIcvP/TShid2u53RFeQWmnxGiZawJGhPuC9b481gm5VhdPjEjyZ/m8CE2B2SjU0xvSstfnE7RPlcQLc/dnygVqzOtqG0qnEXPsTYNaKHUeAzmTFOhDexpuCp2iQT7eZpqWqz5/PTpZXkbFmUG9hNQeVrhDGLwl1PYGge1IXhtV0TnBMI8ineJtPxLuTwP5ccfaxkvxAsqxbUFYMKnpgZaASkS2Fvqomk23VJxWIE6DHwR0fPxusqRfto9vz9cCqCqjYcedFCFqBGETGjrCSq2o+pslxzj7WYTyuVE6P/wcXWd2XhKropgAAAABJRU5ErkJggg==',
  'data:image/png;base64,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',
  'data:image/png;base64,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',
  'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFEAAABjCAYAAADjPeyQAAA19klEQVR42tW9W5Ak53Ue+J1z/j8zq7q6qy/TPTMA544hZggQIAgSwoJL0aJEc6lb2BIVG+HYDYVX++I3x+phHeFXh0MP++oXR6x3I7zrvUVsKFbWxaJM8QJBICgsSNyGuA0HaMxMT/f09FR1dVVl5v+fsw9/VnV1T88AFLFhuxjJ6q4u1GR+de7nOydpZDUAQ6++izvD7acrrk7AaR0RF8CmUGIAYHMDNA8FPEjFACZA8R/oYQADgBKYiEo2KMw8qTkyQAyhYHe15bJX53yOgj0cCAxAFADR0R888/KDLo6bZ2cAIhTBFAo4Iipt/+/pzQYla06c8B/dg4hKAY0AcxStJYbAoLEn3p7PWq/m4lCwhweDAZDZAz7saAD5Af++U0TUCIgWoIjzRuqU1KvFeQb32P7DSdpHggeoAZzO0RxH82wIzmhYsLuai7vadhk8MRwI1ABoZgARHiQP+hEqMHsSDo0kRlNEWAuEGv+pPcw81FoUTRx4pyX+Sttl6y2fIScBGyAzV09EUGpes5/dhhz+3UUYFIpaw8L+OVluZjlgDJD+x4+h5aTmhfh2xu5a22Xrcz5Hzg5iAM1eOBMUmMjlQZmjnwFA239/MsymM8D9p/UgQNkQGTTOxL3f9vnb7SxHRgKnDVh2EAACwQAo7Ejg9ONI48xnOsBgpDCLHUD99FDLiUmVwGxcPtihqAM4GKkjmzwnJ7QvBRyO9HCGOP0UarRuxvMeBuzwf0vRcgaCB+8U7K4WzsOTAwPQqGBmwBJY1ly4UgKQAPAERbo/gHw/50MzjmVv3HdVHD3OYiOz2GZCzd6/q6oLgIw0fYwHuE4gTz5DGUx1UnuLCu0wMFbSgoGoBCGz5v12wNaScS2gIdTyKeCUgDSAjWU0UdUDoNn0wgIHy6mqH25n/uW5In++8Bk8GIgRxgxx0rieBBcIsMahcIOBWTygquk1m/X8SXOJmj8eBNBgCURFnFcyT9BDoHNt6cuKCcCpzPifNz4kovIoo24AK0FgloOoVrM2Ew3T+82ZWcFATcoqZmEuK/6y8O7Nlnh4EkgjW0SN7aODSkrGMLImWtT7ndsBIJsvcx/Iw47FYNNvu4kR2/sS8NFBIRlgRgyQMPGYjAMDY0r6WGN6MlwfPClykTRnQjRK0q0Eaf5J35ygh2nLQCxGYEM0BUOtK4TbDBq3ixQHenFgapSzCWMag39A/9M56zTwpft/yUc5sCNfdxFxCuLE7plZAaJhesbwwZ6RBKAA45gugCPMcjOOIBUiHsx60XusKWmxLyuWq2Gi/gwApOaZEGDWsWg5KcGBBpmTjdy5q14cJCVVKQZUa4wfQYmSTZ4EGIqpkSaLUALM+GMB+CAg3cQzf2w1bM5v4izYeNxcswJgU/JEXMI4ApCJyirgAIrTLwnmAWMj8xM7G2HtfaGxcXqvtqEoTM1RNO/IbXhx24WTd1rebwkEbATSJH1m1pgunfgTwCbAKGAzWZcBBjngOo5S5cOgTf4+ed2pKoLp0kSd1dAxs5zwYAk8+KmsAGBKjRpynD6Tyj5wByXSYF5hOchk9oskNa9ATpZ+hpqnaM4Rb2ckG22XvZyL3/IkSepsEnEouLkwMwKRQbWxhXTIxjXSMMlb7id9s6DeD0ynqgcu8OCF0kEJvCc0Ua+EwszcxMAwEO79nJkgntQbJq+pmMEbCGbwyb5azqAaqgtkUERiUogzHuTi19sueyUXv5FxykQ4GswOAkGU1NpmTtxMD0TMk/cmMG2qprPqehRoR9pEbT7UHpxjP8BGxA6ocRoTCTzC/plZDlLZl8LYbiTIp5iX65R5AACEI0AGZjUR5dKBexn7azln7+eSgTU5DdMkgQAhOU9KwGgKX5gnSddsdjJJN/aj5lkAjwL0QQ+uqqrFTjaZuZ/iQoCZe0RUMnPviMCzJjVnZnmEtYPGtaKdfz9o/XC0cMzYECysmVkuIpshhFMhhFPQ0J18viG2zSxX1YV23v72oDf4Xa11LefsXVZSZ9IT5TIz2aaAnCOh2+n+y/Gw/HK3s4gwqlHulTmZgBSoRmXLkUMoa4xGY4Yx6qCIBtRRUdURMRhEPFSBsqxckl6GWQIrxghVRaOZ02Py2uT1w39vMpZZO/GzS6JqWBnX46djjKut3L9gBnHkNqPGtWpUP8UkQzMrDLElzH0SDJXcKGpc1RiXdjbv/vPjyyf+Gw1x9c7tO//MsbtZZNmP4ri6rMQ7pOZd5tetRvfEyon/4dbNzf88Y7e+s739zzc3N/8BkwMz48SJE/+k1c6/45xbL8vqRlVVZ5xz6yKsgKDUOq+qACKLWdYKTA5lWUK8O6CuzPxA1T3K4dDbu1eXxlyeiVavGeoFQL2xpZjRiAEOSU2TyjJSipiyDPUqBvayEcr60blW5/8Z742/ypABQwaxCmfa7faf1mX1eFlXj8cYV5XME1GpiB2LaDv4zbKsn9jZvvPr/bt3Udc1uvMLmC862N66jRsffoiHj5/E55544r9FHY/98Acv/cELf/VX0DpiPB7Di2B3dxc+z7C8vIhTZ8/g/PnzOHnyJNbWjv1jZu63Wq1v54V/30JkVe2KyA5MOYTqfN4q3gUURHTfYwLYUT8zM+it/nsnJiCCQm5s2E/tuP4oECNil4R7VoeTpG588/rGvwhlRCtvg41RjsaoxiVGZYW6LkHCyHOPvN1C7nJYBGIV8eILL+C1115Du93GwycfQu5ybG/dxs0bN9DKcnz63AXkWYZbt27h+e99H8wOsarBZPBeMDffQbvdgs8L+Myh0+lg5dgxLC0uotVq4eTJ4zh+/DiWFrpXvffvZF6urqws/VOIRmYMmTkcBeBEMu8HLjPD/W0qN2SzFRQuWbnU6MabNzf/xZVX3sDVd9/HXNYGg7GyuIIQAkajEqPRHqoY4JxDq9VCURQY7g4h7LG3O8KH793Aa6+9hl/+pa/iuV94Fne3eviLP/k2TqyuIY4MF86fx7f+/Dt4772raLUKLC8u4syphzEaDnDlzbfQ391DVngsLM7j+PHjOLa2ivFwhF6vh8XFRZw5cwarK8fOAzi/1O3iC1946h999olLT4mznohsMafEYAIeM0NVD6j1UR7bNSWw4nBeexS4bFCaJk/pkUv+JgDUVi9dv3Ydb/z4Cr71J9+CBUMsDSdWj8OioqoqjKsSZVkixuQ1RQTHjx/HY5/5LE4cP46CcsTdGi/91UuwUcSFCxewsriKa1fXsXbsJJ568gt46nNfxCMXLmF5eRntdoHjx5awsNDG7dt3cH3jOu7s9PDh9Q/w3tUP8Dd/cwXzCzl2+yVgwPz8j+Cdg6ri0sVPo9Pp4NLlC48YsGVmhYhsTvN6YHBYAiegzkpnk/ZZW3EvYEYpQObmw45qE5ByDHW4aBHtelw/sbWxhWqvwsb6LWipQA1svb95wGMRqKmqpBDkxk9v4O3X3sbXvvY1PLR6EifWTmBzcxM/fe8aHrv8OH75l34Ff/InfwJmh3feeQ/tuXm02h0sLCzg+NoxxHKIz3/+C8iyAlffv4r3P/gQd+58Guw8wIyNjQ3s7OwAquj1eujt3MXe3h7E51Aw6jpcMFh3WtwlKolo3EQX2xPAmPmA45kAKyJwgAmgPn0AZooFxulvR4ALDmTqjABh7sWo7cz7t9pZG4+cewSXH7mEnHPEWuFMUJcBdR3SSTiGElCHgLqusbS4ACLC8uIK5ufn8cu/1MZLL72ED9c/xNat22i15vDbf/+bGI5G2Lh5C3f7PRw7toxvf/s7uHD+NC5fuoC6rrG8euxbly5devzipz+9VNd1MSrH2N7exnh8GXcbh9XbuQsAqOsaGhQrKyuIMa4SU2S2JQA1YG0ijbMSSURTCZwNbabBtpE6Y0Qzg4EBUzFDm4hLAgaTAFpJU+XbJhJKNQDEGM4WefFyGFVPfOrUQ3j1b36MZ774NHLOMd4tMdfqoBzXAAjsBCQC8oIyVNjr72K+00a7XYBIsHX7Nuo64pu/81/i5s2bKMsS73/wAQCgaGXYHfTwo1deRlWNsbCwiLw4h7wQDMY9LIfukyDLibTIcxq32vObi925bp63Xrx58+bXqzLgw/V1XLt2Db1eD0XehoggRlvKMn8lBlspx+PPZVn2us/kpzHacoxhWUQ2mbknQv0JmEkyASJGCAFuv5o9zYObrIMiHtwN8wzUWZG/PN4bfoWNdHe4h9NnzuDdN9+Fswglxe7uLphSLDYeDlBphM8zDMsxtrZuYbS3i5WlZfzar/0Grl+/jusf3kSMEdvb2+h2u1haWgIR4aUfvoibN28ixhpnz57FM888g0cvXcDGzWu4desmut3uWpZlyVs6Vwz6u6f39vZw/fr1r1+9eg3D4RDXr1/Hm2/+BOvr6zh27BjUKjxy/tR/TWTqvX/XDD6EcBoAWDAQka1J26TxH2E/l55kNIeC7b/No6rGn4uw9vz8wr/cuXv3Dz68eR3/+n/9N0CV8kgLAEGmRllh8LmDESGUJbLcoxrXUFW0Wi0sryxib7iLLMsAAJubm/jBD36AqDVOnz6NL3/5S/j85z+PV1/9EV5//XWcPnUCt7d2sNjdgnMpgB6Px3j77Xdx48YNbG5u4ic/eRv9fh9lWSHUgAjQKuYgIhgMBj7L+blJdhZjXDWzXIy2myyumxwtClUd7NvHiRP+OUFUwIuTzfG4eqYK9SNziwuYW1zA6qeOoR4GWKU4efwkdu/uIlQ1RASjcoyqGqMoCrSPryDPMpw7ewGtVgvHj5/E3t4ebt++g17/Lr73ve+hrEocO7aMX/zFr+PSpUtYX38ff/zHfwzvBXUoQfB4+eUf4+WXf4zd3V3s7e3BzHDjxg2UZYnd3QFCABYWWjhz5jTOnkmBeLvdxvLycpN1aTfGuJZSXRqYWalqC5MIRVUXiCg2Diek9G/fyTiQSipXHXIiRHJEuUFmC6YAQM5ts5PNYVU+u7SyiAoBn/uFp5GzhzNBu5jD3a0dVOMSQoThcICyLNFqtTA/18HCwiLm5xfQ6XRw9b1rePPNN3H9+k0MBgOsrh7HxYtPYWEhOZ9XXnkZ/X4fzIyVlSW0WosoywrvvP0ebt26hX5/gBiTpMUIdLttnD93AWtrazhx4gS63S5OPnQcn/rUpzA/P49Op408z0FEZQjhFBGV3rurKa83iTGuTSSUmVP6ajaYqPM0Tvx51bksy6dd7t5l4/Hy2rEfZ3P5k5cev4xW1kpdNyXY+QAxQEMNixG5z5DnGVQNr/y/r8E5wRtvvI4/+7N/D+8JS4sr+NVf/VX0ej1kWYHRaITt7S28++67OHHiBBYXF9Hr9fDss8/i2//+W3jvvauo66RfnU6OdruNoijw0EMP4dKlS3j4Uydx+vRprKykCCA5BUKWOfgsdRtDCKeJaCzC2wkdlRDCKe99CaDfAJhbKhaH+xYg/pakIqlDOEMkg8XVlX/ym7/1m/99d677PyJqZ9jf+x2rbYmjeQcrKWqLgnYyL1fJgOFw/HfOnTuH/+lf/WssLy/jM5+5iLNnz+HChQsY7A7R7c7jJz95G7dv38aHH36IkydP4vz5s9jd3cXi4gI2NjbwzW9+E889959hc3MTZoaiKCCO0Ol0cPz4cZw7dw7eJwXKcwfmVIURcRDHUA2iSgszseCEuCD3q63eU0/8eQFk5h45uU1KuNvf+e9aRfHiYLj7O2RA0PpUkfm3yr3Rr8Bo0M78y+JETeMCorUzxzdXj62cfOTiefR6PfzWb/097O2NcOvWJrrdLq799AO89tqPMR5X+OpXv4rV1VWoBiwuLuL48eNotXP0enextNxFe65Aq9XC4uIiRAhzc3OYn59HWY7gfZbaBVBErZIdNENZ1sgcQ4S6zNyblADNrCBCPZu5PSg9/rklUVW7aqnBXxTFC4jaZqaBxrjiHG+U5eiZLHNvtcRfccCQgs5H1RUzazNjlGUOX/07X8HGxgb++q9/gCeffBLf/9538Nqrb8AMuHz5MVy+fBk7OzsYDQf44IMP0O/38Xu/93tYWOjAnVgFke33UBqJYgHG5R5ECGU1hAiByCFqyt2JAWIGs4Oq+okUxhhXRWRLRDZVdUFENg9LYlJlfILq3PSHJ4UJVe2ahiVE65CZ5N6/mbHcEPAOG2pwLJoKEJuiRWQ4f+HM98fl6Mu/+qv/BX74wx/iueeexcrKCs6dvQAixp07d6cp1wTEDz74AGfOnEJ3sQ1ixQGOl0WQCcwizASGCJCDIaTfLex3cnFPf7m4X3vjfs0rlzytutR9O/C2I4LtKZthUirT2Z4ymQnUclJzAiuZEOfy/HkHGogiaozHDLSgqb8NIipZgLt373z5kUfO37lz587yhQsX8P776zh//jw+XL+OU6dO49FHL2Jubg7r6+u4c+cOnHPo9Xrw/lxiMJhOveUkGDabKf4bwUxnXjekvs6R7dLxxyAeHCxA/HxkImWAazYo1HKo5RzNM/G297LhwTtzPn+R1LyRdlRNImiFmXtgbquhUxT56/1+//G88Mt57vH4Zx/DuXPnEKPhO9/5Hpxk+IM/+ANcvHgR3/jGN7C0tIStrS289957OH36YZw5e3KqyunZQDTpq/CB7OJA462h/cxUacomV54Ceei1yXNTd/yEQJz0Y6BWwIxZEZnlesa8XYh/KxN3zStKgy6oUgxmXWPbZkbbhIRIx0xULi52UZYVVBXj8QA+y4BKp84FMFRVha2tLRAZRAi93g5ardY9YS1NmQ0yvVAibg4BkYAnzywgYjDz7qSnxMz9I37uE9G4AfWeIu3PDWKinlhByVXfzZhvt9lfaYm/kovbCePqIUsJeQHiO8Ti4CgCFIl0ePfu9m+LCDqduXd2du5eXF5erLe3d3yr1UG3O4/VtRXUdTLi8/PzcM6hrhXee2xvb2Pt+OKBnkjqNzcqrACLAxEw6cWIODA7MCcQRWSXmftNoaGfig2yyUz9iceeAMrMg8OV7U9EEimxDGoCcSay3gD4Zg4OYgQit2GgmkkVBA8hjaZemDxQY3l5+d8wUPfu7v7uwlynLsvSt7IcDKDTamP92vvwApTDEepxiXOnz+DO1m2QGtpF0VyQHOp/WAMUwOwgTOl3YjA5CHsIOwgLJsBNjgmYIrw5+3vz93sA/MS8M03I5yKbzvt3HLlA0aBRQUQKopIINTP3zADH2lezJaTUarWsqkdZgCLPXwTwbFVV3vsWDBFlqBMrzgkky+HyAjFG5HmOqhrDMSc+7z0gcgMiT1S2OVxTpXZgTraQmQazzzOqW05Um4jCwSZVMhNAMy2QirLamTGm4xkPXD/Ic7GTXqzDadW4NDZcFuK+d/xyUh2GaQA56jMznGJgwZiZdgW8TSQQoR3HvG1mL5ej8Ze8o5vzc+3TIRp8nmOu00G708GoirjT66O7uIwqKpxzqarsHGiGEU1EYCEwEcQRmAzCgGPAC8EJwTuGE4oitCPCt1PZi2+Lo20R2naOb4jIpohsOufWE5Ay80XwtPjAoE9EEgswjdnJpiqkCvUjQ0Nt4t/MWYJ4B4sKwEpAcxYMHPENDVoQSSSikoEaGjvR8U2B9MlFEOGY89IGGHOdBZR1RBUURVHAe596xsSNNM0QklK7Fyw4dNE4/DxkpkFTcN0WR9sz6jt9vp8zmf7+SYDYeOg+w9hiXCtj/SiidsQhsqc3xPvEUIWVAEaOaF1V+0RUxhhXVbUbgFPEtJN7f4UhA4BrMHZy558kAzqdDkJ/AFWFc3njXGqwE4hI8sg0IS7xtPcxaYYliZWp5IpI3TT2t1N2QrcnUjeRQBHaYaZeKlZMKtnWeH9tvrgUNv2cIHINwDNoDCaQWN+idoLp0lDry7G2Nph+6IjAmYNEG1hUIISpeQghwLHkZChUZJMhAxfRgaEWkSfNDM455N5DRFJ/pMleiAjOuZTuzRj7ifRNQJv9uXluwOLtBrDb++ClIwHIYdaZ7B82jUuZHwgi1x8DQAilepuZ5STcQ+Zg0VwFPRZDtaywvOWyVwuf9ZkTk9UiKRGNHcvYJIVHDIJFXWDIwBx5EAaOZcp/mYCw27uLGCO89/sMBDZgnzN/QBKZARGaVe3dRl23RLgBj7YPSiBGk2b+RBIPSCNb850Z7JNoDxzgGxJF8e4DFe3GENdCjCsaLDemWlR+ABY0xOQBEw3IADCVStxjKKBWMGRgRkyEnnMuxX8pJ4fWAXujYSIVccpSnHMHqlSTHPvwMaPeWwfiP8FgJg7sN/HhYL+BP0MXIZra3Fm76I6WMDpCCmdHKPYnARioI5BPHEyAdYzgjSnC86CKtoBYfwYA5iT7UU5SOu9A0QBViFGfQSVDoSGuMWQgYotqJo7TLF5RFNjp9aelf2ZGWZYwThK3z0G0GUlMqjaxiQ2At5lpV4S3G6fS348PaScdMtiXQJva2In0HY4T6RPzzo19U7NiShkWCsyyA9J2HXWFQ/2ogEYuk1c9C5gMGgBTBZhKM3JgKoEUo02qK2aGVquFUNXY29uD8wJ2grIs97kyxPeAyEyYtWfNz+WhtG5CIZyAOSOBh/k3ODLQBmjCxeGaiGYJ6sV+THjvEM8kGT9q1o2IxpNROiNEZndTrT47rurLFrVLBlBWvJo36VcYl6kfrQh5q/VyLMMJce5G27srN27caKrQMgUixoiqqpr4sAGnsZ0TVsXsBU+kkAixCabHs8F0ciIYTkKZ/YOnBY1JLs7T1/YfMeonFOIAoRnzHWOGvG6ABNNlZh7CA1HBpYYzrq52FLaeswPnHqSGaBECgJgHJOiRUWlmCCFgPB5DRFAUBVhmLyCCOfUt95mtfICQNPNzbwLeVPIEAyJTIp5kJ0cG1BOJSyW1gxIpkj/QO4ePILvHgx3ABzgdpiGTDFBrp4rhrKp2W2QvmcPbeZalr0CbgUXBAIYBYhpREBGEEJBlGfI8h/MJmDzPp1I2iRGTMB4EMak1xX3HMVXdfhPG9IgsEllMlfGDJTLn/IHO3uG64riqPhlJnC1GCNFQCTPc7Kb4SjQwB8Q6HlPoCmL9mQhrG9OPPDHYMZgEUSNIMQAYJAySdFHee4QQAGIwUg9lH0SeKdvbUVzCciYnHs/mx406jyaSeJBqDJRl1ZTVJvnyQbtYZHP3884fRwIP5tNsVijgmkmqCNAwTcayJjtJkYT7ICqhlpema3VdnjBr4kgnIxMGBYOx1gSKExuIGYkMdaLltVqtKS/msHTsO4J7+YRTe04qACUKDaFkYSU2MOGAGYjBml7MfvHCzGCaPndchk9OEoloLACiWWd21YEQ98wsN1gOopIc70C1rTEWMerKuK6ebApKV4S4D8bEW7PxPoOfnSDPc+wN+siyDFmWzczb0T2zJYfPbSJ5h6rUTTePpvSQVB4jMHsQBC6XaYVcI6AaEYI2RHnD7t7eYx8fxEMS+CAnM+0EGhxTiiOncyxmuRGgTJEc90OwTlXXjyKGJQf68wxOmRmmpLN0thgjsixDL4SpdHmWe0A8ghp8UHPYapAykcxIJDPNOKc0LRAAU4QwhioaANFMD4ATQ4612115wyWrzAHTseMJQ2zyjz/AwZCKpuF8mYJMFGc7ZAr4yTeuSCwCGGBMtZC7aYjLddClGOJJx7JFjl92LDAGoipIgBArjIcjwBLZvaoqhBBgTE3Kd3DU8V57yKPJAWMlyLA5egS+TaAdWAZTgRnvgwhGVYZWCgFTHp1nbWRZpllWjCBJSp2Qu00almAEFh2DeaQWFwzUXLw6GOtkXJcsgcxQKNQZgZU0n+yOYIPuz/6l0bNJVwuE8SSuZAWiaVdjOJVn2evlqHqOQ/lFI65d5HHO+dtSZBiNRrh79y5EchRFKsgGrbFXDuEyQbAAIZ3Sg/bz3EnuLDtEKZUMQU+kiQgdM/GGsL9myLeqyhZGo7gWY7lmZjmz2/bevyPiR0V7fiQiEPbTYkbTf0DD1cQEoJnYWfMkjawHqRMzDoe0aeYmzvGsBGszXcWGZmp//3l20n4SkHPmrykbAqwzDvVlU/LeZMccQ2GoQo3NzU2cO3MeVVUhxjpVdfIcd/u9dGGIjbppQ1RnmAUwO4xGew/nWQvtdvs7RV68kIqsCdSyDI+P+uU/EPYbzrl17/N3ssy/m+e55nkxDehnMp4pgPsTyATXDGBHO2A6uD5QFrmf/UtRAPOBDSY6HfNL0+2sbNNdDTMbAtQbzDNzzwAm4X4d6hMUzKvykCPHEALa7TaiKvKigKpieXkZRdNbeejkpxCDpVF3IlgjJWYMI4aRYG6+fY3ZbSuxDsvqWR2Nvw4jpFjRbefZ3F85568VRfFCnuf9PM/hvYf3HsSMo6f1rMEyDZ87ggynbt9Yp4sSPm62MgHyCMlrXo+6v2ahGeFWP5HyKoazRFSSox6TqxEIavDjsnymrGvML3bx9a9/HY49mBlZlmE4GKGuAuZaHQAutSCatQQTCVFtbFuszgLV2WnFxWW7rVbrL+fm5v4wz1sv5lnrinMeWZZN1ZWIUmgVDSKHM2VJV9KEUTM9lon0NVtJYIUBTA8YGFeCJMnimpu1KUnyVGYlr/mdZ0IQBinMSJTS6FHUuJoJb0HNg0kNlpehvBw0oru0iOee+RKuvvtTDIdj3L6d4dy5c/js449jOBzDuwxqKYZM6h6nEpI8O8F7j6Io0Gq1vpPnrRdbrdZfFkXxgnf5IDWxXNO35mZitSlzgafx4IzXAvERhCYiKkmbMdkUkhQfZ8eDElj0noHy6daQ2efpFGsz/5xsqXnn86vj8fg5BXk1XdKI3IFCFeqLMUa89957+PM//Qs8/bkvon+3hzzP8bWvfQ1VGZrQh1DXEWVZTUFMNjNL4OXtXe/9u1mWve69f9c5t25Kvq70jMZqsyjaW5OwZtb2TfrU+8E63Zcax0kSKRJkCHCdVJoAo3tmnD8m3Y6POo6iKs8EvAV4PxiO0ZaGw/HZwXAPz7/wAl7/8Rv4oz/6I4SgWFlaxmuvvoqF+XlYNAz3xijLGmYEEY8i76BVzKNVzKHI27siboOIh2bwMepKjLoCUHQuu5plxdZswTaZBAHNuoNp6oP94zC1jpDWpDSrYgCYZ0KtkxUuRv5BqeBRk6lHeeUDQXsKcGvA2FQ7ptoRctsm8CQ2iFY9MRqW2O0PsLu7B19kOHP6HIbDIW7c2MB3v/t9VFWFb37ztxBChHMezrsDNo1IdgEqU4wnAxF/fSKJzLJtSj7GOJpN8Q4Ph5sZLNo0jbyfMHKraI8ArjXaQnL9KVBOjfaPnvtT0vzgAQZTaSxDkIwgbkeJ1ViGEeSrqA8rGM5lVzVinqPUom6QUX41DOPlelw/xuBhu93B0tIKvvCFL+DixYsNwVOxsLCAxe4i7t69CyJCd2lxPNdZGGZ5K4IEUQE1goGV2O2AZGRgVSM/OUAyNOLaGptnSoDxtNAwm2+HkMKqo5ytqcKaGiAENFKgng4+NtSQCOR0cCnKLHzuvjPSKb3zRFSOy/IZAMhc/qaw34BwdMTbZFQ687et1iWOHFHr0lze+ksS5BRJ0JFOu5j79cuXP4P33QfIsxxrx44DAH7/938fNzeuY21tbbp/Yj8ssyPDkn3ONXHaoLJfNptI3dQpTbIdNmR5AZDCNEKjHujhkBBgEY4hIJLdSUk+2UaVdHI2BfUosIzUT1dTTXPryUhvclSd9vz/WVXV4wLpQwEL1q01rIm4DTHXcy77KdeV6kjPQGN3PBj/SrVXPndna6e48sZP8K0//Qs8fPI0tja28Y1vfBZ//cLzuLW1gd/4jV/D8ZMnZsfoPlJrkmal4adUjD2474GZIa6phosAUGisp0xccYzD8TAowjEzGMmgszVSx/u/Kz5e4WE2bmzO2MM4hjJcDFW4CMZNL27dwW8yQR1nV5llUI3KL3JtrXJUfolhUUt9mKIVo90RNm/ewnPPfgl/9md/jsufvoznn38e77z9E6yuruDKlSv47BOPfWTp7ijqy0yF+yCFGBEhADHWU2nM8my6P8JMEZqZxLouEWMNg8L5JImDRvJqwALMIjFKVV04vE+xkUgmTGJDm/lmuIaZTzu9uGyi3o5TGmfsNjzlV9V0LdT1+Wo8/ko9rh+3Ckte5LqO4nkzdZ5kp8g6/64eVl8f7Y3xyOlHcfH8RSwuLmFz8xb6u7sgAYbjEYajEebn8o+k/iXQLKbiq0Ui02SONNR1w+txidM926QCDKPRADEm0EIIUIsLU9YHA84DjuEgoCE1ZRwiGoOgBDtCApsKDynPLCiLk9jGLM6zud1EELCcjcvc569EjacRiWNdf0breIIhQ1IMQ1V3UKNFER0JBFVqM8sgxHj+xvp1DHcHqKoKo9EIu7u76Ha7yPMWnn76ady8eRP9fh/zc4sfi0M5W82ezHir6iDz+bQRluxijRAmqqq4c+f2E8wYiuNN57ifuazvfcOsEMAxwVEqeYfZNuXP3KhKKhxhqaBCZkJGNRvqcjD+KpREID0h2Wll7W8vdLo3yIA9v/eHmxu3/2cLWMrM3ySxD0Rkq7fX+9LGjVvIfYHu/CLICPNzHXQ6c1BV5HmOD29uHWDKNrZu1ot6gLxqWGHGcOpsSMUQ21Fxwsx2iqy1raoIZUCMEXVdroZQn1ULS2axs7Ky9H+LYyTgOO3cQXJCMUZAazhGoqFNcl1AvZGpkvkIazPpCMZxUgLbrzGqA7hmhZJxnThFVKafTUil5kigaIN23vruXDG3kbscmeTw4jHc28OwN/yd3OVv1GX1WNpKR6iq6rHNzU1cfe89DAYDXL+xjtFoiLm51ET0jnHjxg0IEW7evIXlxVUc9s5NSBdT7GseFtsEYYIKFC1jaqtiCWx8a/PD/4qZ+865def5uvdyrT1X/DDPc/jMTXk3IIVamgwjUniWpkRDcKYRbclR8fj6KA6fRk47kWOn1vCwy9y6xdAicM1RwqQqzcw9Ezci41pMhlrFU8KyCdW21bZUjcuntKwfOra0/E+XVpY2Ct+CGCAkSflrILcMGdzGuC6/7DL/7nA4+M08z1/Os+LFqz/96ZeqUOLTn34EdT3CcHQX49Eu2u02Ou0Wjq+sQkRw9/ZdEHyPmfsxhIfIQuFEbpPF3GKcZ5YNYQyEMCQL7VjHR0MVn05rvdQT0bg73/5fnKN1X/Ar3ktI9hFgrqEW4LC/9QnTpZoNsJaqhc6DkZGHkNsm4mEk5QhrG6k3ix1S8p55g8X1SQkR1jIjRIVAySNQW0t9uFI7ZVV4GGYeNboZshstaW948/DGoElL1NJmzbTpUAYx2pJRhPdpl8Tdu/1/3OvtwkmGxaUFXL9+HT5L5ctefwef/exnMRwOMddqYTQqEUI47Zz7AGxKlAjsBvJJq9UbKC/L8tnBoDymFuC9x9xc+9/Oz8//q1Yrfx4UchHelgzBOQJzbHrMzVhH0+g+uFb64C5aJ+wgJBCRnbQayoqEONdsPGbwkE2GHAkWdMkMHYOxwdoWkaOOXkf1ZVKChrhGBgikL457mXgIOYAE0Qwyqc8RoBxBzINW3v5uiPEEk/UAlVbe+YuLFz799WpYodXO8cLzf43eTh97gxHa7TZWVlbw5ptvYmEhZS3BSjClHQ5R6/mgNl/XZZqcinw2VDWy3KHTbm225xb+tJ0X3/de3mfmXojVmVYr+4E4gkvjaQf2jaUfm4jtwEaSmTgx1RObigUJCDKCWQvGkciGZKRkXCNQW0PoxlpPEHyPhftR47E4rj9NNSsqLDnmDQKvE1PJRrWAB2TceD6BUWiYXE2o5Bjksw+q3uAxBgIBGFXlL2RZ9sajFy9d1RDPf/DBB7h7d59Kd/rsGVy5cgXbO3fw5FOfx6geYW+8hxpVt1mlgGCKqhojao08eiwsdFBk+Z28VXw3K/yr7HiTBbte3DUR2jFTZ7Y/NbpfyaaPtSesWbiWRrqmy3KAGkQDM6mJeGCVnjKNbYlumFH2euZbPyIng73h+Cu74+orFNHzAZplsslNKKGGFhuXZAyeMgqkqTons2ji4DK/pSGcdM6/UxTFCzGGE7Gqz+fOv3Xs2LHzo9EIX/jiFxFCwKVLl9BZmMf3/+p7qEKJpdVl+Nxhd7yLDJJWP2v6opQV7AjIBVQ4UMY34KkXLayUdexAed2xbIr4rQjNAQrNhsoZti03YU9sagSHNqpgdm2+UTMY41Llw7TbzHAplDnWcS2X7Gonb3+3lbW0yDtJksqdl4Zx8A9z+HWluCLqBmaxYyCGWcHEm26ivrbfRFdq7DEDLs/Q6XT+9/Fw9NUY41qe5y/Xdf1IsLA2313AheI8Vk+uIm+nGea33nkbFy49glu3t7C4uoS1k8fAmQJeEK1GIAUJpyW/AiADtnZvo9uZfzwv/CuuVbyekWyQmo+xfnhchvl2u3iVBDg8XvFxdoVpA6SbcuwSPaOcqLDGuKTR2rnLX5/PO3+5kHfRcgUcPKJG5OpHProeiwxg1iHI0GA5lAQGTnVJbqrMie9nTfneTCFNqd8X2av9fu8fjavxFyWTdRIM1UIb3tAu2uPVT639H8Vc+9/VsTp/q7/1z37xa1/BTq+HtVOrWFldBqgG+cRI4AiYS2O4CgNxBBWCCgH98eC3zUK3kxXfnfP5i5nzV5xzO4dHzGYhOooIYDMSm3qeUxCnJfIBELtm1kJErkE77dbC/9Up5jDHbQgEFgErDVYbUyRRYq9gQHhA5msi8zHGtWa134GZOkqBOZIJ4WTMPW+0Fop/G2Ncq2N1PpJ2FMrmDFGiv7N353cxvvO74t2d7toi5o8tpG0mwyFIDFVdgcEIUNRicI7BTRPJJOWpNSLGsWpn6s60kZi7BrBqyMFUsu7XFCfATWyi3edmD7OTgkwQKCK8OLSy/N2UrlHw4t+3YN1Y6wnHPi1ebqhrXjI4E3XkNg0EyfK3yipcroM+rMRaq60E06Uy1OkkZnpfTAbHgMYAoYiFYwsb2Xz2/DAOnx3q+Kmaw3J00UtbriGn7WKx/Z1sPn/ZMgxcR8BzjIpKcItgmUFyDwjAjiCeoRQRWQFP02fKGOaAyupTw3r03KgePRtZc858aUyA8PSYqrSmY1oWm/5PmukVaTbHp+sBG0+JjftTUokxFUI4FWN8H4J9koQBPs3H7dSwjqotRbJ2eksTY1LqGzOnNj+iIVpoeDUELwQShwiA5/zrvnQvQ21TvFuHWO05K9nRzrAc/hLMhlAtwajB8CZI+YhxY2QJk/6SHbFhziixKWoLyyOjpxyncQsjvJTn+Q21RH0GABKBIwJPsGhiQrK0KG2f12qNNHLD4mKCA09XLU8q2+Tcel2FU3UM+11oTV7BOQEzDdRsCU130JhCYkNQbYBUocyjhTJNNzVESRhqjYh1jWEs0S8Hq7vV3q9HbyrirojIZtDybK3xvNbajhzbqtqNrLnBopl6m27iJbg8SyRRpEMp6dfEUXhxcMQQUC1GPSPpBWZUhiWyeCpjumFGjYHh5p4Vk65fM68yXcxiR3CPeJ8VxqBJNaM0szSi5uR2GFWPhBAQM4MTmvIg2TuIyCZiPGVmrTRUSDtNy6BgoFWWo2dHYfxdh0S2rDV15IblsFWW5dPjunoCbXk/cmy5dvaK83wdbGq1liGoRwQT4JhJVeEZGDrnYDEWxMmZxKqe3qSBpsVgmu7UNm5khgjKpBFWjDWcR12GyuKJomj/IGOCc2ls1wAEVQhRMmE6Q0ig/duQzPBnG0k0QChJoiPeiYoVI2MmKJFpGUoXLARHeZJIMohnSCbrMqLLtcYTLDIS0DDGuEZmHCysDcv4S4rw3cqAUNcYjvdae+PRr8QY10i4h7a8T95tkCVnFEL9mRQmac5ONl3m3ynL8mkzyx24JuNaDR0SWbCoXQgpO/GkaTeNzlj6SXkJYDjmXS9unZn7TLRroLIScgZbGpbl08jzlx0JSBxosuzcKFW3o6al5zOtU5pZLQ1EOJrpFztquM2JL10oEMW79XFVPj2qRj/Ic9/0lQXsGXkre3VUjp/TqGBFbqRLGsOJlNyjDBpPvnftvf9NcrkGQTmO1WfqGE6BLbJzGxxl0+qk+obYUtWualgx0/a0bKXkYObT33RBo83vL8clEUijfgZu4lG1Zgo/UfOikNtmdtsitNPcGgCR4JngB+PR300mjV9OCyWb4UpMWaIpYaB9LiQd6EMz3OQeG9zod1LR5Fw0aqfl/dVqUD4zHA1+0PYtiBGYAPGMubk5VHvlD0d1XIJRTWpsUbvi+I7L/Rs14oqQeincu5zJ9Vzm/lDFoKR5NO0GjWvlsHpWRDbFudvJ5IZjMca1WIdTIdanoPCU6pRMCiGlVMxIa6VRVRFmYXrThpTn2jT/FRFRxdkYbYkZw7TUOI1g1OA+EV9lNY51ONXK8xdzdhuOBUqMUAXILNlrsvdxn9gFZjSVHkteiCFw5kcMGajGjpnlyKg3juVjgzB8rmPjF4QcHAGeMriWh7TlLYv4BdX6mBK4tnrBF/4DN+dfUcOpvNX6YSDtVFqfVcSOEUoS2lVTjhqW5haKPwS4thhWgsY1Bg2Y3SCtm8pzjXHFzApES5Ia0VHV7qSdW+X6MIwjY9LGUL9PjVGvBGbmPkkzPkfp7+zd9Yxko67qhzSUz4xD9XgZq0dbWf5SIf4tMdRpnwWNJky2yYyOmrUmmuKcW6fUoFHUUNSoMdIRdvZ2TgyqwTdcIe8YIHVdP4Kg3SJrvbhYLL0wny3AIYNawJ29HewM7vzD8Xj8nHNuPW/lL7JgYESRBCNDbCmZTwCqTyeifrI9lNSV08ksS2tgZu9SNAGsCd67qrrQlPbTzu5mVf/hHjkRlSCVmXHbMTP3wTyc3e+Qe/9mrMNpCtrJWK53suK7nby1MecyZBBoXacW8iyleeYGOBZj2vie/JCCwfDI4CG3HWQneWgMQDYwhoy1vLw93Ons7g3XXfS9aHEpZMHXXj07/6rL3FvmaLOK9cPR4hIjzYqkb1ELQF0ifarH5GY3FABwrUAOmBhhlsGfG++z+ZOXRWlqBQhls4Z/En+EQ7dESa8LSoOBmEojA7PVxBZAyiDicSifBAHiUNfQziiWT3CNIUH7yg6Z82mDwGyFhwgx5a+JTWa6z3ISECRxU0IaM9MihvoEsUU46iGQr+rqkVjH82J+h4hKDRHMGIq4a977d6aU4uZi9J59O4dY/DOMsWa1XnHk5NY+K6M4MJR56PfD/+2MJM6uJRjPDBStOufWhXmbtKH6qXlWe8FctuPyDJBmKUeDDxGl4FtTBcxNcluBpE4TErVWRLaixRNq2gWhZKYePJfMvMFOaq9+k5l7FZWnADqWhsDrh6Np10zbxDQWkc1a61P7zmzCDZ/tFR8kqt2nTzzt0JnZZHHu5MvqP2CL0mR/Q3mwfbr/5TBzX5h3SOQ2RfMw46C6NIz1Ywq85bJ6yyOtYuCmQUwzc9UwSyHOfuDIEBC8c5CKezA6IU42I2ue7IB6pF3U44jYDhaWyNMOFN2oYWWy8ii1XalUC0v3LiSS4cGLNp69qGbD8PgwgM1zObPSuv9Ry9BmJfCwhE6evcjmhJlmhGhMSoS6gh7TWBVUjr7dcpm2XdEojSKoNpMiPMNPPJTQePYQ8ddFq4cjUQ4gr7U+RZARyDwYO6qaq+kCKzqG2AaIiS0wuR2QcjTthqCnSJJtve+A5SEe5Axo45lhzfKj3vMg9sPsf3+/WZY03QAI0zCYFVDtBLU11OVQCS+JSEBzw0SeBcwsEZqmLoeSwAoLhHjEoHGtuqqk3RSIKRvIKTRnx6UYbUWEJUAdORkA5q0hwlMaud2/F6BR4zFxiBQQ/f1AngA1Mw5c3uc95f1s4lGvHfgcNT/lGRHVEfAGeBKqjYASumahegrAKx2noSUe3KSH1vy/21ejpjxAADe9uKbEH4StB0ah0Ha02E10ZN8TpgGZRSIeAgZVy1Xr7oRUzsz9OsaHfpZtT7PqOStxh4E84j3l/WzpfYAcT1mpzRorNWtHWLshv9bCvKMKVBofpqr0bHjRiaiDpMa2KoQJFIJCmrA8msLIEBGxG3dxd7SzOqLh4zXXK4FiV6FtIiqF5A6leptIM4WvNPGyh4aHDk1i2YGF6Ophsf2glQiH7eX9htZ/RkJTOcPeiBNm2+R2d5NzTHUFHrOauIiYk9xou+yVOZ+PWj7FkaYKPjCKb8kDCRiOHBz7LUTkbFzOMl4nuW1Drftb3VHoQWp3eGPcR7335/33Zu9iefgLN6YA5qEKhUDWHsf60VFV5sNQoUQEmOGm7Rab9FNTQUnIIRMPVPBQEmKuhWnHTNuWYkElonFzW0t+0OjawXHeiWROyFH3qujPOpiJ/78fTCUR1bGKK+MYHooc1yLj+waM2BUzjuUg+x9CjMzlEEhfTZcE0oOFjhnVESl3bO7q+LNd+ATUmTupPciGfZTd/CQkvqkVSlMcZ8XBBKAZP8sjWZtgHYOuUJrXvsbM2/8fK7WVe7Rhy4EAAAAASUVORK5CYII=',
  'data:image/png;base64,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',
  'data:image/png;base64,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',
];

// ── CONSTANTS ──
const DIAS_SEMANA=['Dom','Seg','Ter','Qua','Qui','Sex','Sáb'];
const MESES=['Janeiro','Fevereiro','Março','Abril','Maio','Junho','Julho','Agosto','Setembro','Outubro','Novembro','Dezembro'];
const MOD_CORES={'Capoeira Regional':{bg:'rgba(249,212,65,.1)',tx:'#c89a00'},'Capoeira Angola':{bg:'rgba(7,157,40,.12)',tx:'#4ebe6a'},'Maculelê':{bg:'rgba(184,96,16,.12)',tx:'#d07830'},'Musicalidade':{bg:'rgba(7,62,142,.13)',tx:'#4a7acc'},'Acrobacia':{bg:'rgba(122,56,184,.12)',tx:'#a064d8'},'Infantil':{bg:'rgba(16,140,140,.12)',tx:'#30b8b0'},'Juvenil':{bg:'rgba(16,140,140,.12)',tx:'#30b8b0'},'Roda':{bg:'rgba(184,53,48,.12)',tx:'#d06058'},'Treino Livre':{bg:'rgba(100,130,110,.1)',tx:'#7a9080'}};
const PLANOS={basico:{nome:'Básico',cor:'#4ebe6a'},intermediario:{nome:'Intermediário',cor:'#f9d441'},completo:{nome:'Completo',cor:'#4a7acc'},bolsista:{nome:'Bolsista',cor:'#a064d8'}};

// ── UTILS ──
// dateToStr: formata um objeto Date usando os componentes LOCAIS (ano/mês/dia),
// evitando o bug de toISOString() que converte para UTC e pode "pular" o dia
// perto da meia-noite em fusos como o do Brasil (UTC-3).
function dateToStr(d){const y=d.getFullYear();const m=String(d.getMonth()+1).padStart(2,'0');const day=String(d.getDate()).padStart(2,'0');return`${y}-${m}-${day}`;}
function today(){return dateToStr(new Date());}
function parseD(s){return new Date(s+'T12:00:00');}
function diffMonths(a,b){const da=parseD(a),db=parseD(b);return(db.getFullYear()-da.getFullYear())*12+(db.getMonth()-da.getMonth());}
function fmtBR(s){if(!s)return'';const[y,m,d]=s.split('-');return`${d}/${m}/${y}`;}
function fmtMes(s){if(!s)return'';const[y,m]=s.split('-');return`${MESES[parseInt(m)-1]} ${y}`;}
function fmtMoeda(v){return'R$ '+parseFloat(v||0).toFixed(2).replace('.',',');}
function uid(){return Date.now()+Math.random().toString(36).slice(2,6);}
function durMin(a,b){const[ha,ma]=a.split(':').map(Number);const[hb,mb]=b.split(':').map(Number);return(hb*60+mb)-(ha*60+ma);}
function durStr(m){if(m<=0)return'?';const h=Math.floor(m/60),mm=m%60;return h?`${h}h${mm?mm+'min':''}`:mm+'min';}
function fmtRange(a,b){return`${a} – ${b}`;}
function isLightHex(h){const c=h.replace('#','');if(c.length<6)return false;const r=parseInt(c.slice(0,2),16),g=parseInt(c.slice(2,4),16),b=parseInt(c.slice(4,6),16);return(r*299+g*587+b*114)/1000>148;}
function darkenHex(h,f){const c=h.replace('#','');const r=parseInt(c.slice(0,2),16),g=parseInt(c.slice(2,4),16),b=parseInt(c.slice(4,6),16);return`#${Math.round(r*f).toString(16).padStart(2,'0')}${Math.round(g*f).toString(16).padStart(2,'0')}${Math.round(b*f).toString(16).padStart(2,'0')}`;}
function cordGrad(c,deg=135){if(!c.c2||c.c1===c.c2)return`linear-gradient(${deg}deg,${c.c1},${darkenHex(c.c1,.68)})`;return`linear-gradient(${deg}deg,${c.c1},${c.c2})`;}

// ── ÍCONE DE CORDA NA NAV (cor dinâmica conforme corda do usuário) ──
function svgCorda(c1,c2){
  // Faixa de capoeira enrolada com nó, em duas cores (faixa de transição ou sólida)
  return`<svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
    <path d="M3 8c0-2 2-4 5-4h8c3 0 5 2 5 4s-2 4-5 4H8c-3 0-5-2-5-4z" fill="${c1}"/>
    <path d="M3 8c0-2 2-4 5-4h4v8H8c-3 0-5-2-5-4z" fill="${c1}"/>
    <path d="M12 4h4c3 0 5 2 5 4s-2 4-5 4h-4z" fill="${c2}"/>
    <path d="M9 12l-3 7 3 1 2-6z" fill="${c1}"/>
    <path d="M15 12l3 7-3 1-2-6z" fill="${c2}"/>
    <circle cx="12" cy="8" r="2.4" fill="none" stroke="rgba(0,0,0,.18)" stroke-width="1"/>
  </svg>`;
}
function updateCordaNavIcon(){
  const el=document.getElementById('corda-nav-icon');
  if(!el)return;
  const a=alunoLogado();
  const c=a?CORDAS[a.cordaIdx]:CORDAS[0];
  el.innerHTML=svgCorda(c.c1,c.c2||c.c1);
  el.title=a?`Sua corda: ${c.nome}`:'Cordas';
}

// ── STATE ──
let S=loadState();
function loadState(){try{const s=localStorage.getItem('fiu4');if(s){const d=JSON.parse(s);if(!d.notificacoes)d.notificacoes=[];if(!d.videos)d.videos={};if(!d.tags)d.tags={};if(!d.chats)d.chats={};if(!d.config)d.config={basico:89,intermediario:149,completo:219,tolerancia:5};return d;}}catch(e){}return{alunos:[],presencas:{},grade:[],pagamentos:[],tags:{},videos:{},chats:{},config:{basico:89,intermediario:149,completo:219,tolerancia:5},notificacoes:[]};}
function save(){localStorage.setItem('fiu4',JSON.stringify(S));}

let selectedAluno=null,calY,calM,calDia=null,addAulaDiaDate=null,pagTabAtivo='todos';

// ── HELPERS ──
function getAluno(id){return S.alunos.find(a=>a.id===id);}
function getAulasDia(aId,d){return(S.presencas[aId]||{})[d]||[];}
function setAulasDia(aId,d,aulas){if(!S.presencas[aId])S.presencas[aId]={};if(!aulas.length)delete S.presencas[aId][d];else S.presencas[aId][d]=aulas;}
function statsAluno(aId){const p=S.presencas[aId]||{};let pr=0,fa=0,tot=0;Object.values(p).forEach(aulas=>aulas.forEach(a=>{if(a.status==='P'){pr++;tot++;}else if(a.status==='A'){fa++;tot++;}}));return{present:pr,falta:fa,total:tot,pct:tot?Math.round(pr/tot*100):0};}
function statsMes(aId,y,m){const p=S.presencas[aId]||{};let pr=0,fa=0,tot=0;Object.entries(p).forEach(([date,aulas])=>{const d=parseD(date);if(d.getFullYear()===y&&d.getMonth()===m){aulas.forEach(a=>{if(a.status==='P'){pr++;tot++;}else if(a.status==='A'){fa++;tot++;}});}});return{present:pr,falta:fa,total:tot,pct:tot?Math.round(pr/tot*100):0};}
function cordaProg(a){const c=CORDAS[a.cordaIdx];const ul=a.historicoCordas[a.historicoCordas.length-1];const m=diffMonths(ul.data,today());const p=Math.min(100,Math.round(m/c.min*100));return{meses:m,min:c.min,max:c.max,pct:p,pronto:m>=c.min};}
function statusPagAluno(a){if(a.plano==='bolsista')return'isento';const now=new Date();const mes=`${now.getFullYear()}-${String(now.getMonth()+1).padStart(2,'0')}`;const paid=S.pagamentos.find(p=>p.alunoId===a.id&&p.mes===mes&&p.status==='pago');if(paid)return'em_dia';const vd=new Date(now.getFullYear(),now.getMonth(),a.vencimento||5);const diff=Math.floor((now-vd)/(86400000));if(diff<=0||diff<=S.config.tolerancia)return'pendente';return'atrasado';}
function statusPagLabel(st){const m={em_dia:{cls:'p-ok',label:'✓ Em Dia'},pendente:{cls:'p-warn',label:'⏳ Pendente'},atrasado:{cls:'p-err',label:'⚠ Atrasado'},isento:{cls:'p-info',label:'★ Bolsista'}};return m[st]||{cls:'p-mute',label:'—'};}
function tagsAuto(a){const st=statusPagAluno(a);const sl=statusPagLabel(st);const c=CORDAS[a.cordaIdx];const pl=PLANOS[a.plano]||{nome:a.plano};return[{cls:sl.cls,label:sl.label},{cls:'p-mute',label:'🤸 '+c.nome},{cls:'p-info',label:'📋 '+pl.nome}];}
function permsAluno(a){const st=statusPagAluno(a);const c=CORDAS[a.cordaIdx];const perms=[];if(st==='em_dia'||st==='isento'){perms.push({ok:true,txt:'Acesso a todas as aulas do plano'});perms.push({ok:true,txt:'Participação em rodas e eventos'});if(a.plano!=='basico')perms.push({ok:true,txt:'Aulas extras e musicalidade'});if(a.plano==='completo'||a.plano==='bolsista')perms.push({ok:true,txt:'Consultoria nutricional'});}else if(st==='pendente'){perms.push({ok:true,txt:'Acesso básico à musculação'});perms.push({ok:false,txt:'Aulas coletivas (restrito)'});perms.push({ok:false,txt:'Rodas e eventos bloqueados'});}else{perms.push({ok:false,txt:'Acesso bloqueado'});perms.push({ok:false,txt:'Todas as aulas suspensas'});perms.push({ok:false,txt:'Rodas e eventos bloqueados'});}if(['avancado','instrutor','professor','contramestre','mestre','grandmestre'].includes(c.nivel))perms.push({ok:st==='em_dia'||st==='isento',txt:'Treinos avançados — '+c.nivel});return perms;}

// ── ALUNOS CRUD ──
function addAluno(){if(isAluno()){toast('Sem permissão','warn');return;}const nome=document.getElementById('add-nome').value.trim();const inicio=document.getElementById('add-inicio').value;const cidx=parseInt(document.getElementById('add-corda').value);const plano=document.getElementById('add-plano').value;const venc=parseInt(document.getElementById('add-venc').value);if(!nome){toast('Digite o nome','warn');return;}if(!inicio){toast('Selecione a data','warn');return;}const a={id:Date.now(),nome,inicio,cordaIdx:cidx,historicoCordas:[{cordaIdx:cidx,data:inicio}],plano,vencimento:venc};S.alunos.push(a);save();closeModal('modal-add-aluno');renderAlunoList();renderAlunosGrid();toast('Aluno '+nome+' adicionado!');}
function removeAluno(id){if(isAluno()){toast('Sem permissão','warn');return;}if(!confirm('Remover este aluno?'))return;S.alunos=S.alunos.filter(a=>a.id!==id);delete S.presencas[id];delete S.tags[id];S.pagamentos=S.pagamentos.filter(p=>p.alunoId!==id);if(selectedAluno&&selectedAluno.id===id){selectedAluno=null;document.getElementById('attend-panel').innerHTML='<div class="empty-st"><div class="empty-icon">🤸</div><p>Selecione um aluno.</p></div>';}save();renderAlunoList();renderAlunosGrid();toast('Aluno removido.');}
function abrirPromover(id){const a=getAluno(id);if(!a)return;const prog=cordaProg(a);document.getElementById('promover-info').textContent=`${a.nome} — ${prog.meses} meses na corda "${CORDAS[a.cordaIdx].nome}".`+(prog.pronto?' ✓ Tempo mínimo atingido!':` Faltam ${prog.min-prog.meses} meses.`);populateSel('promover-corda',Math.min(a.cordaIdx+1,CORDAS.length-1));document.getElementById('promover-data').value=today();selectedAluno=a;openModal('modal-promover');}
function promoverAluno(){if(isAluno()){toast('Sem permissão','warn');return;}const a=selectedAluno;if(!a)return;const ni=parseInt(document.getElementById('promover-corda').value);const data=document.getElementById('promover-data').value;if(!data){toast('Selecione a data','warn');return;}a.cordaIdx=ni;a.historicoCordas.push({cordaIdx:ni,data});save();closeModal('modal-promover');renderAlunoList();renderAlunosGrid();if(selectedAluno&&selectedAluno.id===a.id)renderAttendPanel();aplicarCorCordaNav();addNotif('promocao','Aluno promovido',`${a.nome} agora é faixa ${CORDAS[ni].nome}.`,'🎽','var(--wn-bg)','var(--wn-tx)');toast('🎽 '+a.nome+' promovido para '+CORDAS[ni].nome+'!');}

// ── PRESENÇA ──
function renderAlunoList(){
  const q=(document.getElementById('search-aluno')||{value:''}).value.toLowerCase();
  const list=document.getElementById('aluno-list');
  const f=S.alunos.filter(a=>a.nome.toLowerCase().includes(q));
  if(!f.length){list.innerHTML='<div class="empty-st" style="padding:14px"><p>Nenhum aluno.</p></div>';return;}
  list.innerHTML=f.map(a=>{
    const c=CORDAS[a.cordaIdx];const st=statusPagAluno(a);const sl=statusPagLabel(st);
    const stats=statsAluno(a.id);const ini=a.nome.split(' ').slice(0,2).map(w=>w[0]).join('');
    const grad=cordGrad(c);
    return`<div class="aitem${selectedAluno&&selectedAluno.id===a.id?' sel':''}" onclick="selectAluno(${a.id})">
      <div class="av" style="background:${grad}">${ini}</div>
      <div style="flex:1;min-width:0"><div class="a-name">${a.nome}</div><div class="a-cord" style="color:${c.c1}">${c.nome}</div></div>
      <div style="display:flex;flex-direction:column;align-items:flex-end;gap:2px">
        <span class="pill ${sl.cls}" style="font-size:.54rem;padding:2px 6px">${sl.label}</span>
        <span style="font-size:.6rem;color:var(--mute)">${stats.pct}%</span>
      </div>
    </div>`;
  }).join('');
}

function selectAluno(id){selectedAluno=getAluno(id);const n=new Date();calY=n.getFullYear();calM=n.getMonth();calDia=today();renderAlunoList();renderAttendPanel();}

function renderAttendPanel(){
  const a=selectedAluno;if(!a)return;
  const c=CORDAS[a.cordaIdx];const st=statsAluno(a.id);const sm=statsMes(a.id,calY,calM);
  const prog=cordaProg(a);const pagSt=statusPagAluno(a);const pagSl=statusPagLabel(pagSt);
  const grad=cordGrad(c);const todayS=today();

  const fd=new Date(calY,calM,1).getDay();const dim=new Date(calY,calM+1,0).getDate();
  let cc=DIAS_SEMANA.map(d=>`<div class="cal-dow">${d}</div>`).join('');
  for(let i=0;i<fd;i++)cc+='<div class="cday emp"></div>';
  for(let d=1;d<=dim;d++){
    const ds=`${calY}-${String(calM+1).padStart(2,'0')}-${String(d).padStart(2,'0')}`;
    const isT=ds===todayS,isFut=ds>todayS;
    const aulas=getAulasDia(a.id,ds);
    const np=aulas.filter(x=>x.status==='P').length,na=aulas.filter(x=>x.status==='A').length;
    let cls='cday';
    if(isFut)cls+=' fut';else if(np>0&&na===0)cls+=' has-p';else if(na>0&&np===0)cls+=' has-a';else if(np>0&&na>0)cls+=' has-m';
    if(isT)cls+=' tod';
    const dots=aulas.slice(0,5).map(au=>{const mc=MOD_CORES[au.mod]||{tx:'#888'};return`<div class="cdot" style="background:${au.status==='P'?mc.tx:au.status==='A'?'#c06060':'#555'}"></div>`;}).join('');
    cc+=`<div class="${cls}"${isFut?'':` onclick="selectDia('${ds}')"`}><span class="cdn">${d}</span>${aulas.length?`<div class="cdots">${dots}</div>`:''}</div>`;
  }

  const allLog=[];Object.entries(S.presencas[a.id]||{}).forEach(([date,aulas])=>aulas.forEach(au=>allLog.push({date,...au})));
  allLog.sort((a,b)=>b.date!==a.date?b.date.localeCompare(a.date):(b.inicio||'').localeCompare(a.inicio||''));
  const logHtml=allLog.slice(0,20).map(au=>{const mc=MOD_CORES[au.mod]||{tx:'#888'};return`<div class="lrow"><div class="ldot" style="background:${au.status==='P'?mc.tx:au.status==='A'?'#c06060':'#555'}"></div><div class="ldate">${fmtBR(au.date)}</div><div class="ltime">${au.inicio||''}${au.fim?' – '+au.fim:''}</div><div class="lmod">${au.mod||''}</div><div class="lst" style="color:${au.status==='P'?'var(--ok-tx)':'var(--er-tx)'}">${au.status==='P'?'✓':au.status==='A'?'✗':'—'}</div></div>`;}).join('')||'<div style="font-size:.76rem;color:var(--mute);padding:8px 0">Nenhum registro ainda.</div>';

  const tagsA=tagsAuto(a);const tagsC=S.tags[a.id]||[];
  const tagsHtml=[...tagsA.map(t=>`<span class="pill ${t.cls}">${t.label}</span>`),...tagsC.map(t=>`<span class="pill ${t.cor}">${t.nome} <button onclick="removeTag(${a.id},'${t.id}')" style="background:none;border:none;color:inherit;cursor:pointer;margin-left:2px">×</button></span>`)].join('');

  document.getElementById('attend-panel').innerHTML=`
  ${pagSt==='atrasado'?`<div class="inadim" style="margin-bottom:10px"><span style="font-size:1rem">🚫</span><span style="font-size:.8rem;color:var(--er-tx)"><strong>${a.nome}</strong> — pagamento em atraso. Acesso bloqueado.</span></div>`:''}
  <div class="att-cols">
    <div>
      <div class="cal-wrap">
        <div class="cal-head">
          <button class="cal-btn" onclick="chgMes(-1)">◀</button>
          <div style="text-align:center"><div class="cal-lbl">${MESES[calM]} ${calY}</div><div style="font-size:.62rem;color:var(--mute)">${sm.present}✓ ${sm.falta}✗ · ${sm.pct}%</div></div>
          <button class="cal-btn" onclick="chgMes(1)">▶</button>
        </div>
        <div class="cal-body"><div class="cal-grid">${cc}</div></div>
      </div>
      <div class="dia-panel" id="dia-panel">${renderDiaHtml(a.id,calDia)}</div>
      <div class="card" style="margin-top:10px"><div class="card-tit">Últimas 20 aulas</div><div class="log-list">${logHtml}</div></div>
    </div>
    <div class="right-col">
      <div class="card">
        <div class="card-tit">${a.nome}</div>
        <div style="display:flex;align-items:center;gap:9px;margin-bottom:11px">
          <div class="av" style="background:${grad};width:40px;height:40px;font-size:.88rem;flex-shrink:0">${a.nome.split(' ').slice(0,2).map(w=>w[0]).join('')}</div>
          <div><div style="font-family:'Cinzel',serif;font-size:.88rem;font-weight:700">${a.nome}</div><div style="font-size:.65rem;color:var(--mute)">Desde ${fmtBR(a.inicio)}</div></div>
        </div>
        <div style="display:flex;flex-wrap:wrap;gap:3px;margin-bottom:11px">${tagsHtml}</div>
        <div class="stat-grid">
          <div class="sbox"><div class="snum" style="color:var(--ok-tx)">${st.present}</div><div class="slbl">Presenças</div></div>
          <div class="sbox"><div class="snum" style="color:var(--er-tx)">${st.falta}</div><div class="slbl">Faltas</div></div>
          <div class="sbox"><div class="snum">${st.total}</div><div class="slbl">Aulas</div></div>
          <div class="sbox"><div class="snum" style="color:${st.pct>=75?'var(--ok-tx)':st.pct>=50?'var(--wn-tx)':'var(--er-tx)'}">${st.pct}%</div><div class="slbl">Freq.</div></div>
        </div>
      </div>
      <div style="background:var(--surf2);border:1px solid var(--bord);border-radius:8px;padding:13px">
        <div style="display:flex;align-items:center;gap:9px;margin-bottom:9px">
          <div style="width:30px;height:30px;border-radius:50%;background:${grad};flex-shrink:0;border:2px solid rgba(255,255,255,.12);box-shadow:0 2px 8px rgba(0,0,0,.25)"></div>
          <div>
            <div style="font-family:'Cinzel',serif;font-size:.86rem;font-weight:700;color:${c.c1}">${c.nome}</div>
            <div style="font-size:.66rem;color:var(--acc);font-style:italic">"${c.sim}"</div>
          </div>
          ${prog.pronto?`<span class="pill p-ok" style="margin-left:auto">✓</span>`:''}
        </div>
        <div class="pbar-wrap">
          <div class="pbar-row"><span>${prog.meses}m</span><span>Mín: ${prog.min}m</span></div>
          <div class="pbar"><div class="pbar-fill" style="width:${prog.pct}%;background:${grad}"></div></div>
        </div>
        <div style="font-size:.65rem;color:var(--mute);margin-bottom:9px">${prog.pronto?'✓ Tempo mínimo atingido.':`Faltam ${prog.min-prog.meses} meses.`}</div>
        <div class="divider"></div>
        <div style="display:flex;gap:5px">
          <button class="btn btn-y btn-sm" style="flex:1" onclick="abrirPromover(${a.id})">🎽 Promover</button>
          <button class="btn btn-ghost btn-sm" onclick="abrirPagRapido(${a.id})">💰</button>
        </div>
      </div>
      <div class="card">
        <div class="card-tit">Histórico de Cordas</div>
        ${a.historicoCordas.slice().reverse().map(h=>{const hc=CORDAS[h.cordaIdx];return`<div style="display:flex;align-items:center;gap:7px;padding:5px 0;border-bottom:1px solid var(--bord)"><div style="width:11px;height:11px;border-radius:50%;background:${cordGrad(hc)};flex-shrink:0"></div><div style="font-size:.78rem;flex:1">${hc.nome}</div><div style="font-size:.63rem;color:var(--mute)">${fmtBR(h.data)}</div></div>`;}).join('')}
      </div>
      <button class="btn btn-red btn-sm" style="width:100%" onclick="removeAluno(${a.id})">🗑 Remover</button>
    </div>
  </div>`;
}

function renderDiaHtml(aId,dateStr){
  const aulas=getAulasDia(aId,dateStr)||[];
  const sorted=[...aulas].sort((a,b)=>(a.inicio||'').localeCompare(b.inicio||''));
  const d=parseD(dateStr);const dLabel=`${DIAS_SEMANA[d.getDay()]}, ${fmtBR(dateStr)}`;
  const isFut=dateStr>today();const np=aulas.filter(x=>x.status==='P').length,na=aulas.filter(x=>x.status==='A').length;
  const rows=sorted.map(au=>{
    const mc=MOD_CORES[au.mod]||{bg:'rgba(128,128,128,.1)',tx:'#888'};
    const dur=au.inicio&&au.fim?durStr(durMin(au.inicio,au.fim)):'';
    const sc=au.status==='P'?'sp-p':au.status==='A'?'sp-a':'sp-n';
    const sl=au.status==='P'?'✓ Presente':au.status==='A'?'✗ Falta':'— Marcar';
    return`<div class="aula-row"><div class="aula-hora">${fmtRange(au.inicio||'?',au.fim||'?')}</div><div class="mod-badge" style="background:${mc.bg};color:${mc.tx};flex:1">${au.mod||'Aula'}</div>${dur?`<span style="font-size:.63rem;color:var(--mute);white-space:nowrap">${dur}</span>`:''}<span class="sp ${sc}" onclick="cycleStatus('${aId}','${dateStr}','${au.id}')">${sl}</span><button class="adel" onclick="delAula('${aId}','${dateStr}','${au.id}')">×</button></div>`;
  }).join('');
  return`<div class="dia-head"><div class="dia-ttl">📅 <span>${dLabel}</span>${np||na?`<span style="font-size:.67rem;font-family:'Barlow',sans-serif;color:var(--mute);margin-left:7px">${np}✓ ${na}✗</span>`:''}</div>${!isFut?`<div style="display:flex;gap:4px;flex-wrap:wrap"><button class="btn btn-g btn-xs" onclick="marcarTodos('${aId}','${dateStr}','P')">✓ Todos</button><button class="btn btn-red btn-xs" onclick="marcarTodos('${aId}','${dateStr}','A')">✗ Todos</button><button class="btn btn-ghost btn-xs" onclick="openAddAulaDia('${aId}','${dateStr}')">+ Aula</button></div>`:'<span style="font-size:.65rem;color:var(--mute)">Futuro</span>'}</div>${aulas.length?`<div class="aulas-list">${rows}</div>`:`<div class="empty-st" style="padding:18px">${!isFut?`<button class="btn btn-ghost btn-sm" onclick="openAddAulaDia('${aId}','${dateStr}')">+ Adicionar Aula</button>`:''}</div>`}`;
}

function selectDia(ds){calDia=ds;if(selectedAluno)renderAttendPanel();}
function chgMes(d){calM+=d;if(calM<0){calM=11;calY--;}if(calM>11){calM=0;calY++;}if(selectedAluno)renderAttendPanel();}
function cycleStatus(aId,ds,auId){const aulas=getAulasDia(aId,ds);const au=aulas.find(x=>x.id===auId);if(!au)return;au.status=au.status==='P'?'A':au.status==='A'?'':'P';setAulasDia(aId,ds,aulas);save();renderAttendPanel();renderAlunoList();}
function delAula(aId,ds,auId){setAulasDia(aId,ds,getAulasDia(aId,ds).filter(x=>x.id!==auId));save();renderAttendPanel();}
function marcarTodos(aId,ds,status){let aulas=getAulasDia(aId,ds);if(!aulas.length){const g=aulasGradeNoDia(ds);aulas=g.length?g.map(gr=>({id:uid(),inicio:gr.inicio,fim:gr.fim,mod:gr.mod,status})):[{id:uid(),inicio:'08:00',fim:'09:00',mod:'Treino Livre',status}];}else aulas=aulas.map(au=>({...au,status}));setAulasDia(aId,ds,aulas);save();renderAttendPanel();renderAlunoList();toast(status==='P'?'✓ Todos presentes.':'✗ Todos com falta.');}
function openAddAulaDia(aId,ds){addAulaDiaDate={alunoId:parseInt(aId)||aId,dateStr:ds};document.getElementById('add-aula-dia-info').textContent=`Aula em ${fmtBR(ds)}`;const g=aulasGradeNoDia(ds)[0];if(g){document.getElementById('ad-inicio').value=g.inicio;document.getElementById('ad-fim').value=g.fim;document.getElementById('ad-mod').value=g.mod;}openModal('modal-add-aula-dia');}
function addAulaDia(){if(!addAulaDiaDate)return;const{alunoId,dateStr}=addAulaDiaDate;const ini=document.getElementById('ad-inicio').value;const fim=document.getElementById('ad-fim').value;const mod=document.getElementById('ad-mod').value;const st=document.getElementById('ad-status').value;if(!ini||!fim){toast('Informe o horário','warn');return;}const aulas=getAulasDia(alunoId,dateStr);aulas.push({id:uid(),inicio:ini,fim,mod,status:st});aulas.sort((a,b)=>(a.inicio||'').localeCompare(b.inicio||''));setAulasDia(alunoId,dateStr,aulas);save();closeModal('modal-add-aula-dia');renderAttendPanel();renderAlunoList();toast('Aula adicionada!');}

// ── ALUNOS GRID ──
function renderAlunosGrid(){
  const grid=document.getElementById('alunos-grid');
  if(!S.alunos.length){grid.innerHTML='<div class="empty-st" style="grid-column:1/-1"><div class="empty-icon">👥</div><p>Nenhum aluno cadastrado.</p></div>';return;}
  grid.innerHTML=S.alunos.map(a=>{
    const c=CORDAS[a.cordaIdx];const st=statsAluno(a.id);const prog=cordaProg(a);
    const pagSt=statusPagAluno(a);const pagSl=statusPagLabel(pagSt);
    const ini=a.nome.split(' ').slice(0,2).map(w=>w[0]).join('');
    const pl=PLANOS[a.plano]||{nome:a.plano};const grad=cordGrad(c);
    return`<div class="acard" style="--card-grad:${grad}">
      <div class="acard-top">
        <div class="acard-av" style="background:${grad}">${ini}</div>
        <div><div class="acard-name">${a.nome}</div><div class="acard-meta">Desde ${fmtBR(a.inicio)} · ${diffMonths(a.inicio,today())}m</div></div>
      </div>
      <div class="acard-pills">
        <span class="pill ${pagSl.cls}">${pagSl.label}</span>
        <span class="pill p-info">📋 ${pl.nome}</span>
        <span class="pill p-mute" style="border-color:${c.c1}40;color:${c.c1}">🤸 ${c.nome}</span>
      </div>
      <div class="pbar-wrap"><div class="pbar-row"><span style="font-size:.62rem">Corda: ${prog.meses}/${prog.min}m</span><span style="font-size:.62rem">${prog.pct}%</span></div><div class="pbar"><div class="pbar-fill" style="width:${prog.pct}%;background:${grad}"></div></div></div>
      <div class="pbar-wrap"><div class="pbar-row"><span style="font-size:.62rem">Freq: ${st.pct}%</span><span style="font-size:.62rem">${st.present}/${st.total}</span></div><div class="pbar"><div class="pbar-fill" style="width:${st.pct}%;background:${st.pct>=75?'var(--g1)':st.pct>=50?'var(--y1)':'var(--r1)'}"></div></div></div>
      <div class="acard-acts">
        <button class="btn btn-ghost btn-xs" onclick="goPresenca(${a.id})">📋</button>
        <button class="btn btn-y btn-xs" onclick="abrirPromover(${a.id})">🎽 Promover</button>
        <button class="btn btn-b btn-xs" onclick="abrirPagRapido(${a.id})">💰</button>
        <button class="btn btn-red btn-xs" onclick="removeAluno(${a.id})">🗑</button>
      </div>
    </div>`;
  }).join('');
}
function goPresenca(id){document.querySelectorAll('.ntab').forEach(t=>t.classList.remove('active'));document.querySelectorAll('.ntab')[0].classList.add('active');showPage('presenca',null);selectAluno(id);}

// ── PAGAMENTOS ──
function regPag(){
  if(!canEdit()){toast('Sem permissão','warn');return;}
  const alunoId=parseInt(document.getElementById('pag-aluno-sel').value);
  const valor=parseFloat(document.getElementById('pag-valor').value);
  const data=document.getElementById('pag-data').value;
  const mes=document.getElementById('pag-mes').value;
  const forma=document.getElementById('pag-forma').value;
  const status=document.getElementById('pag-status-sel').value;
  const obs=document.getElementById('pag-obs').value.trim();
  if(!alunoId||!data||!mes){toast('Preencha os campos','warn');return;}
  const novoPag={id:uid(),alunoId,valor:valor||0,data,mes,forma,status,obs};
  S.pagamentos.push(novoPag);
  save();closeModal('modal-reg-pag');renderPagamentos();renderAlunoList();
  if(status==='pago'){
    const a=getAluno(alunoId);
    if(a){
      addNotif('pagamento_confirmado','Pagamento confirmado',`${a.nome} · ${fmtMoeda(valor||0)} · ${fmtMes(mes)}`,'💰','var(--ok-bg)','var(--ok-tx)');
      enviarComprovanteChat(alunoId,novoPag);
      atualizarChatNavBadge();
    }
  }
  toast('💰 Pagamento registrado!');
}
function removePag(id){S.pagamentos=S.pagamentos.filter(p=>p.id!==id);save();renderPagamentos();renderAlunoList();}
function marcarPago(id){
  const p=S.pagamentos.find(x=>x.id===id);
  if(!p)return;
  p.status='pago';
  save();renderPagamentos();renderAlunoList();
  const a=getAluno(p.alunoId);
  if(a){
    addNotif('pagamento_confirmado','Pagamento confirmado',`${a.nome} · ${fmtMoeda(p.valor)} · ${fmtMes(p.mes)}`,'💰','var(--ok-bg)','var(--ok-tx)');
    enviarComprovanteChat(p.alunoId,p);
    atualizarChatNavBadge();
  }
  toast('✓ Pagamento confirmado!');
}
function salvarConfig(){S.config.basico=parseFloat(document.getElementById('cfg-basico').value)||89;S.config.intermediario=parseFloat(document.getElementById('cfg-intermediario').value)||149;S.config.completo=parseFloat(document.getElementById('cfg-completo').value)||219;S.config.tolerancia=parseInt(document.getElementById('cfg-tolerancia').value)||5;save();closeModal('modal-config-pag');renderPagamentos();toast('Configurações salvas!');}
function setPagTab(tab,btn){pagTabAtivo=tab;document.querySelectorAll('.ptab').forEach(t=>t.classList.remove('active'));if(btn)btn.classList.add('active');renderPagamentos();}
function abrirPagRapido(aId){populateAlunoSel('pag-aluno-sel');document.getElementById('pag-aluno-sel').value=aId;const a=getAluno(aId);if(a&&S.config[a.plano])document.getElementById('pag-valor').value=S.config[a.plano];document.getElementById('pag-data').value=today();const n=new Date();document.getElementById('pag-mes').value=`${n.getFullYear()}-${String(n.getMonth()+1).padStart(2,'0')}`;openModal('modal-reg-pag');}
function renderPagamentos(){
  const now=new Date();const mesAtual=`${now.getFullYear()}-${String(now.getMonth()+1).padStart(2,'0')}`;
  let emDia=0,pendente=0,atrasado=0,receita=0;
  S.alunos.forEach(a=>{const st=statusPagAluno(a);if(st==='em_dia'||st==='isento')emDia++;else if(st==='pendente')pendente++;else if(st==='atrasado')atrasado++;});
  S.pagamentos.filter(p=>p.mes===mesAtual&&p.status==='pago').forEach(p=>receita+=p.valor||0);
  document.getElementById('pr-emdia').textContent=emDia;
  document.getElementById('pr-pendente').textContent=pendente;
  document.getElementById('pr-atrasado').textContent=atrasado;
  document.getElementById('pr-receita').textContent=fmtMoeda(receita);
  const inadim=S.alunos.filter(a=>statusPagAluno(a)==='atrasado');
  const banner=document.getElementById('inadim-banner');
  banner.innerHTML=inadim.length?`<div class="inadim"><span style="font-size:1rem">⚠️</span><span style="font-size:.8rem;color:var(--er-tx)"><strong>${inadim.length} inadimplente(s):</strong> ${inadim.map(a=>a.nome).join(', ')}</span></div>`:'';
  const plRes=document.getElementById('pag-planos-resumo');
  const contP={};S.alunos.forEach(a=>{contP[a.plano]=(contP[a.plano]||0)+1;});
  plRes.innerHTML=Object.entries(contP).map(([pl,n])=>{const info=PLANOS[pl]||{nome:pl,cor:'#888'};const val=S.config[pl]||0;return`<div style="display:flex;align-items:center;justify-content:space-between;padding:6px 0;border-bottom:1px solid var(--bord);font-size:.8rem"><span style="color:${info.cor}">● ${info.nome}</span><span style="color:var(--txt2)">${n} aluno${n>1?'s':''}</span><span style="color:var(--acc)">${val?fmtMoeda(val):'isento'}</span></div>`;}).join('')||'<div style="font-size:.78rem;color:var(--mute)">Nenhum aluno.</div>';
  const hist=document.getElementById('pag-historico');
  const recent=[...S.pagamentos].sort((a,b)=>b.data.localeCompare(a.data)).slice(0,15);
  hist.innerHTML=recent.map(p=>{const a=getAluno(p.alunoId);return`<div style="display:flex;align-items:center;gap:6px;padding:6px 0;border-bottom:1px solid var(--bord);font-size:.76rem"><span class="pill ${p.status==='pago'?'p-ok':'p-warn'}" style="font-size:.56rem">${p.status==='pago'?'✓':'⏳'}</span><span style="flex:1;color:var(--txt2)">${a?a.nome:'—'}</span><span style="color:var(--acc)">${fmtMoeda(p.valor)}</span><span style="color:var(--mute)">${fmtBR(p.data)}</span>${p.status!=='pago'?`<button class="btn btn-g btn-xs" onclick="marcarPago('${p.id}')">Confirmar</button>`:`<button class="btn btn-ghost btn-xs" onclick="enviarComprovante('${p.id}')" title="Enviar comprovante pelo chat">📄</button>`}<button class="btn btn-red btn-xs" onclick="removePag('${p.id}')">×</button></div>`;}).join('')||'<div style="font-size:.76rem;color:var(--mute);padding:8px 0">Nenhum pagamento.</div>';
  let lista=S.alunos;if(pagTabAtivo!=='todos')lista=lista.filter(a=>{const st=statusPagAluno(a);return pagTabAtivo==='em_dia'?(st==='em_dia'||st==='isento'):st===pagTabAtivo;});
  const tbody=document.getElementById('pag-tbody');
  if(!lista.length){tbody.innerHTML=`<tr><td colspan="7" style="text-align:center;padding:22px;color:var(--mute)">Nenhum resultado.</td></tr>`;return;}
  tbody.innerHTML=lista.map(a=>{
    const c=CORDAS[a.cordaIdx];const st=statusPagAluno(a);const sl=statusPagLabel(st);
    const pl=PLANOS[a.plano]||{nome:a.plano};
    const pags=[...S.pagamentos.filter(p=>p.alunoId===a.id&&p.status==='pago')].sort((a,b)=>b.data.localeCompare(a.data));
    const ult=pags[0];const rc=st==='atrasado'?'per':st==='em_dia'||st==='isento'?'pok':'pwn';
    return`<tr class="${rc}"><td style="font-weight:600;color:var(--txt)">${a.nome}</td><td style="font-size:.74rem;color:${c.c1}">● ${c.nome}</td><td style="font-size:.76rem;color:${pl.cor}">${pl.nome}</td><td style="font-size:.76rem">Dia ${a.vencimento||5}</td><td style="font-size:.76rem;color:var(--txt2)">${ult?fmtBR(ult.data)+' · '+fmtMoeda(ult.valor):'—'}</td><td><span class="pill ${sl.cls}">${sl.label}</span></td><td><div style="display:flex;gap:3px">${st!=='em_dia'&&st!=='isento'?`<button class="btn btn-g btn-xs" onclick="abrirPagRapido(${a.id})">💰</button>`:''}${canEdit()?`<button class="btn btn-xs" style="${st==='atrasado'?'background:var(--er-bg);border:1px solid var(--er-bd);color:var(--er-tx)':'background:var(--surf2);border:1px solid var(--bord);color:var(--txt2)'}" onclick="abrirChatComAluno(${a.id})" title="Conversar">💬</button>`:''}</div></td></tr>`;
  }).join('');
}

// ── PERMISSÕES ──
function addTag(){const aId=parseInt(document.getElementById('tag-aluno-sel').value);const nome=document.getElementById('tag-nome').value.trim();const cor=document.getElementById('tag-cor').value;const perm=document.getElementById('tag-perm').value.trim();if(!nome){toast('Digite o nome','warn');return;}if(!S.tags[aId])S.tags[aId]=[];S.tags[aId].push({id:uid(),nome,cor,perm});save();closeModal('modal-add-tag');renderPermissoes();renderAlunoList();if(selectedAluno&&selectedAluno.id===aId)renderAttendPanel();toast('🏷 Tag criada!');}
function removeTag(aId,tagId){if(!S.tags[aId])return;S.tags[aId]=S.tags[aId].filter(t=>t.id!==tagId);save();renderPermissoes();renderAlunoList();if(selectedAluno&&selectedAluno.id===aId)renderAttendPanel();}
function renderPermissoes(){
  const grid=document.getElementById('perm-grid');
  if(!S.alunos.length){grid.innerHTML='<div class="empty-st" style="grid-column:1/-1"><div class="empty-icon">🔑</div><p>Nenhum aluno.</p></div>';return;}
  grid.innerHTML=S.alunos.map(a=>{
    const c=CORDAS[a.cordaIdx];const grad=cordGrad(c);const ini=a.nome.split(' ').slice(0,2).map(w=>w[0]).join('');
    const tagsA=tagsAuto(a);const tagsC=S.tags[a.id]||[];const perms=permsAluno(a);
    return`<div class="perm-card">
      <div class="perm-top"><div class="av" style="background:${grad};width:36px;height:36px;font-size:.76rem">${ini}</div><div><div style="font-family:'Cinzel',serif;font-size:.86rem;font-weight:700">${a.nome}</div><div style="font-size:.64rem;color:var(--mute)">${c.nome}</div></div></div>
      <div style="display:flex;flex-wrap:wrap;gap:3px;margin-bottom:9px">${tagsA.map(t=>`<span class="pill ${t.cls}">${t.label}</span>`).join('')}${tagsC.map(t=>`<span class="pill ${t.cor}">${t.nome} <button onclick="removeTag(${a.id},'${t.id}')" style="background:none;border:none;color:inherit;cursor:pointer">×</button></span>`).join('')}<button class="btn btn-ghost btn-xs" onclick="openAddTagFor(${a.id})">+ tag</button></div>
      ${perms.map(p=>`<div class="perm-row"><span style="font-size:.76rem;color:var(--txt2)">${p.txt}</span><span class="pill ${p.ok?'p-ok':'p-err'}">${p.ok?'✓':'✗'}</span></div>`).join('')}
      ${tagsC.filter(t=>t.perm).map(t=>`<div class="perm-row"><span style="font-size:.76rem;color:var(--txt2)">🏷 ${t.perm}</span><span class="pill p-info">custom</span></div>`).join('')}
    </div>`;
  }).join('');
}
function openAddTagFor(aId){populateAlunoSel('tag-aluno-sel');document.getElementById('tag-aluno-sel').value=aId;document.getElementById('tag-nome').value='';document.getElementById('tag-perm').value='';openModal('modal-add-tag');}

// ── GRADE (editor visual + chamada) ──
let gradeViewMode = 'visual'; // 'visual' | 'chamada'

function toggleGradeView(){
  gradeViewMode = gradeViewMode==='visual'?'chamada':'visual';
  document.getElementById('grade-visual-section').style.display = gradeViewMode==='visual'?'':'none';
  document.getElementById('grade-chamada-section').style.display = gradeViewMode==='chamada'?'':'none';
  document.getElementById('btn-grade-view').textContent = gradeViewMode==='visual'?'📋 Chamada':'📅 Grade';
  if(gradeViewMode==='chamada') initChamada();
}

function renderDiasCheck(){
  document.getElementById('dias-check').innerHTML = DIAS_SEMANA.map((d,i)=>
    `<label style="display:flex;align-items:center;gap:3px;cursor:pointer;font-size:.76rem;padding:4px 9px;background:var(--bg2);border:1px solid var(--bord);border-radius:5px">
      <input type="checkbox" value="${i}" ${[1,3,5].includes(i)?'checked':''}> ${d}
    </label>`).join('');
}

function addAulaGrade(){
  const dias = [...document.querySelectorAll('#dias-check input:checked')].map(c=>parseInt(c.value));
  const ini  = document.getElementById('ag-inicio').value;
  const fim  = document.getElementById('ag-fim').value;
  const mod  = document.getElementById('ag-mod').value;
  const turma= document.getElementById('ag-turma').value.trim();
  if(!dias.length){toast('Selecione ao menos um dia','warn');return;}
  if(!ini||!fim){toast('Informe o horário','warn');return;}
  S.grade.push({id:uid(),dias,inicio:ini,fim,mod,turma});
  save();closeModal('modal-add-aula-grade');renderGrade();
  renderPresenca(); // update presença view
  const diasTxt=dias.map(d=>DIAS_SEMANA[d]).join(', ');
  addNotif('aula_nova','Nova aula na grade',`${mod}${turma?' — '+turma:''} · ${diasTxt} · ${ini}–${fim}`,'🕐','var(--in-bg)','var(--in-tx)');
  toast('✓ Aula adicionada à grade!');
}

function removeAulaGrade(id){
  S.grade = S.grade.filter(g=>g.id!==id);
  save(); renderGrade(); renderPresenca();
  toast('Aula removida.');
}

function aulasGradeNoDia(ds){
  const dow = parseD(ds).getDay();
  return S.grade.filter(g=>g.dias.includes(dow));
}

// ── GRADE VISUAL: weekly grid ──
const GRADE_DIAS = ['Dom','Seg','Ter','Qua','Qui','Sex','Sáb']; // Dom–Sáb, consistente com DIAS_SEMANA
const GRADE_DIAS_IDX = [0,1,2,3,4,5,6];

function renderGrade(){
  renderGradeGrid();
  renderGradeTable();
}

function renderGradeGrid(){
  const grid = document.getElementById('gv-week');
  if(!grid) return;

  const agora = new Date();
  const todayDow = agora.getDay(); // 0=sun

  // Sort all grade entries by start time
  const sorted = [...S.grade].sort((a,b)=>(a.inicio||'').localeCompare(b.inicio||''));

  // Collect unique time slots (start times)
  const timeSlots = [...new Set(sorted.map(g=>g.inicio))].sort();
  if(!timeSlots.length) timeSlots.push('08:00','10:00','18:00','19:00','20:00');

  let html = '';

  // Header row
  html += `<div class="gv-col-head" style="background:var(--surf2);padding:10px 4px;text-align:center;font-size:.6rem;color:var(--mute);border-right:1px solid var(--bord)">Hora</div>`;
  GRADE_DIAS.forEach((d,i)=>{
    const dow = GRADE_DIAS_IDX[i];
    const isToday = dow===todayDow;
    html += `<div class="gv-col-head${isToday?' today-col':''}">${d}${isToday?'<br><span style="font-size:.55rem;opacity:.7">Hoje</span>':''}</div>`;
  });

  // Time slot rows
  timeSlots.forEach(time=>{
    // Time label
    html += `<div class="gv-time-col"><span>${time}</span></div>`;
    // Cells for each day
    GRADE_DIAS_IDX.forEach(dow=>{
      const isToday = dow===todayDow;
      const aulas = S.grade.filter(g=>g.dias.includes(dow)&&g.inicio===time);
      const mc = aulas[0] ? (MOD_CORES[aulas[0].mod]||{bg:'rgba(7,157,40,.12)',tx:'var(--ok-tx)'}) : null;

      let cellContent = '';
      aulas.forEach(g=>{
        const mc2 = MOD_CORES[g.mod]||{bg:'rgba(7,157,40,.12)',tx:'var(--ok-tx)'};
        const canE = canEdit();
        cellContent += `<div class="gv-aula" style="background:${mc2.bg};color:${mc2.tx};border-color:${mc2.tx}22"
          onclick="event.stopPropagation()">
          <div class="gv-aula-time">${g.inicio}${g.fim?' – '+g.fim:''}</div>
          <div class="gv-aula-mod">${g.mod}</div>
          ${g.turma?`<div class="gv-aula-turma">${g.turma}</div>`:''}
          ${canE?`<button class="gv-aula-del" onclick="event.stopPropagation();removeAulaGrade('${g.id}')" title="Remover">×</button>`:''}
        </div>`;
      });

      const canE = canEdit();
      html += `<div class="gv-cell${isToday?' today-col':''}"
        onclick="${canE?`quickAddCell(${dow},'${time}')`:''}">
        ${cellContent}
        ${canE?`<div class="gv-add-hint">＋</div>`:''}
      </div>`;
    });
  });

  // Extra empty row for adding new slots
  const canE = canEdit();
  if(canE){
    html += `<div class="gv-time-col" style="font-size:.58rem;color:var(--bord2)">+</div>`;
    GRADE_DIAS_IDX.forEach(dow=>{
      html += `<div class="gv-cell" onclick="openAddForDay(${dow})" style="border-style:dashed"><div class="gv-add-hint" style="opacity:.35">＋</div></div>`;
    });
  }

  grid.style.gridTemplateColumns = `60px repeat(7,1fr)`;
  grid.innerHTML = html;
}

function quickAddCell(dow, time){
  // Open modal pre-filled
  renderDiasCheck();
  // Uncheck all, check this dow
  document.querySelectorAll('#dias-check input').forEach(cb=>{
    cb.checked = parseInt(cb.value)===dow;
  });
  document.getElementById('ag-inicio').value = time;
  // Auto-set fim = +1h
  const [h,m] = time.split(':').map(Number);
  const endH = String(h+1).padStart(2,'0');
  document.getElementById('ag-fim').value = `${endH}:${String(m).padStart(2,'0')}`;
  openModal('modal-add-aula-grade');
}

function openAddForDay(dow){
  renderDiasCheck();
  document.querySelectorAll('#dias-check input').forEach(cb=>{
    cb.checked = parseInt(cb.value)===dow;
  });
  openModal('modal-add-aula-grade');
}

function renderGradeTable(){
  const tbody = document.getElementById('grade-tbody');
  if(!tbody) return;
  if(!S.grade.length){
    tbody.innerHTML=`<tr><td colspan="6" style="text-align:center;padding:20px;color:var(--mute)">Nenhuma aula. Clique nas células da grade ou em "+ Nova Aula".</td></tr>`;
    return;
  }
  const sorted = [...S.grade].sort((a,b)=>{
    const da=Math.min(...a.dias),db=Math.min(...b.dias);
    return da!==db?da-db:(a.inicio||'').localeCompare(b.inicio||'');
  });
  tbody.innerHTML = sorted.map(g=>{
    const mc = MOD_CORES[g.mod]||{bg:'rgba(128,128,128,.1)',tx:'#888'};
    return `<tr>
      <td><div style="display:flex;flex-wrap:wrap;gap:2px">${g.dias.sort().map(d=>`<span class="dchip">${DIAS_SEMANA[d]}</span>`).join('')}</div></td>
      <td style="font-family:'Barlow Condensed',sans-serif;font-size:.9rem;font-weight:900;color:var(--txt)">${fmtRange(g.inicio,g.fim)}</td>
      <td style="color:var(--mute)">${durStr(durMin(g.inicio,g.fim))}</td>
      <td><span class="mod-badge" style="background:${mc.bg};color:${mc.tx}">${g.mod}</span></td>
      <td style="color:var(--txt2)">${g.turma||'—'}</td>
      <td>${canEdit()?`<button class="btn btn-red btn-xs" onclick="removeAulaGrade('${g.id}')">×</button>`:''}</td>
    </tr>`;
  }).join('');
}

// ── CHAMADA EM MASSA ──
function initChamada(){
  const dataEl = document.getElementById('chamada-data');
  if(!dataEl.value) dataEl.value = today();
  populateChamadaAulas();
}

function populateChamadaAulas(){
  const ds  = document.getElementById('chamada-data').value || today();
  const aulas = aulasGradeNoDia(ds);
  const sel = document.getElementById('chamada-aula-sel');
  sel.innerHTML = aulas.length
    ? aulas.map((g,i)=>`<option value="${i}">${fmtRange(g.inicio,g.fim)} — ${g.mod}${g.turma?' ('+g.turma+')':''}</option>`).join('')
    : `<option value="-1">Nenhuma aula neste dia</option>`;
}

document.addEventListener('change', e=>{
  if(e.target.id==='chamada-data') populateChamadaAulas();
});

function renderChamada(){
  const ds    = document.getElementById('chamada-data').value || today();
  const idx   = parseInt(document.getElementById('chamada-aula-sel').value);
  const aulas = aulasGradeNoDia(ds);
  const aula  = aulas[idx];
  const cont  = document.getElementById('chamada-container');

  if(!aula || idx<0){
    cont.innerHTML = `<div class="empty-st"><div class="empty-icon">📋</div><p>Selecione uma aula para lançar a chamada.</p></div>`;
    return;
  }
  if(!S.alunos.length){
    cont.innerHTML = `<div class="empty-st"><div class="empty-icon">👥</div><p>Nenhum aluno cadastrado.</p></div>`;
    return;
  }

  const mc = MOD_CORES[aula.mod]||{bg:'rgba(7,157,40,.12)',tx:'var(--ok-tx)'};

  cont.innerHTML = `
    <div class="chamada-card">
      <div class="chamada-card-head">
        <div>
          <div class="chamada-card-title">${aula.mod}${aula.turma?' — '+aula.turma:''}</div>
          <div style="font-size:.72rem;color:var(--mute)">${fmtBR(ds)} · ${fmtRange(aula.inicio,aula.fim)}</div>
        </div>
        <div style="display:flex;gap:6px">
          <button class="btn btn-g btn-sm" onclick="marcarChamadaTodos('${ds}','${aula.inicio}','${aula.fim}','${aula.mod}','P')">✓ Todos Presentes</button>
          <button class="btn btn-red btn-sm" onclick="marcarChamadaTodos('${ds}','${aula.inicio}','${aula.fim}','${aula.mod}','A')">✗ Todos Faltaram</button>
        </div>
      </div>
      <div id="chamada-rows">
        ${S.alunos.map(a=>{
          const existingAulas = getAulasDia(a.id, ds);
          const thisAula = existingAulas.find(au=>au.inicio===aula.inicio&&au.mod===aula.mod);
          const status = thisAula ? thisAula.status : '';
          const aulaId = thisAula ? thisAula.id : null;
          const c = CORDAS[a.cordaIdx]; const grad = cordGrad(c);
          const ini = a.nome.split(' ').slice(0,2).map(w=>w[0]).join('');
          return `<div class="aluno-chamada-row" id="chamada-row-${a.id}">
            <div class="av" style="background:${grad};width:30px;height:30px;font-size:.7rem;flex-shrink:0">${ini}</div>
            <div class="aluno-chamada-name">${a.nome}</div>
            <div style="font-size:.65rem;color:${c.c1};min-width:80px">${c.nome}</div>
            <div class="chamada-btns">
              <button class="cbtn cbtn-p${status==='P'?' active':''}"
                onclick="setChamadaStatus(${a.id},'${ds}','${aula.inicio}','${aula.fim}','${aula.mod}','P','${aulaId||''}')">✓ P</button>
              <button class="cbtn cbtn-a${status==='A'?' active':''}"
                onclick="setChamadaStatus(${a.id},'${ds}','${aula.inicio}','${aula.fim}','${aula.mod}','A','${aulaId||''}')">✗ F</button>
            </div>
          </div>`;
        }).join('')}
      </div>
    </div>`;
}

function setChamadaStatus(alunoId, ds, ini, fim, mod, status, existingId){
  const aulas = getAulasDia(alunoId, ds);
  const existing = aulas.find(a=>a.inicio===ini&&a.mod===mod);
  if(existing){
    existing.status = existing.status===status ? '' : status;
  } else {
    aulas.push({id:uid(),inicio:ini,fim,mod,status});
  }
  setAulasDia(alunoId, ds, aulas);
  save();
  // Re-render just the row buttons
  renderChamada();
  renderPresenca();
}

function marcarChamadaTodos(ds, ini, fim, mod, status){
  S.alunos.forEach(a=>{
    const aulas = getAulasDia(a.id, ds);
    const existing = aulas.find(au=>au.inicio===ini&&au.mod===mod);
    if(existing) existing.status=status;
    else aulas.push({id:uid(),inicio:ini,fim,mod,status});
    setAulasDia(a.id, ds, aulas);
  });
  save(); renderChamada(); renderPresenca();
  toast(status==='P'?'✓ Todos marcados como presentes!':'✗ Todos marcados como faltaram.');
}

// ── CORDAS — lista compacta com expand/collapse ──
function toggleCorda(idx){
  const row=document.getElementById('cr-row-'+idx);
  if(row)row.classList.toggle('open');
}
function renderCordas(){
  const NLBL={iniciante:'Iniciante',basico:'Básico',intermediario:'Intermediário',avancado:'Avançado',instrutor:'Instrutor',professor:'Professor',contramestre:'Contra Mestre',mestre:'Mestre',grandmestre:'Grão-Mestre'};
  let lastNivel=null,out='';
  CORDAS.forEach((c,i)=>{
    const nc=NIVEL_COR[c.nivel];
    const alunosNaCorda=S.alunos.filter(a=>a.cordaIdx===i);
    const tempo=c.max===999?`Mín. ${c.min}m`:`${c.min}–${c.max}m`;
    const grad=cordGrad(c);
    const isTrans=c.nome.includes(' e ');
    const circleStyle=isTrans?`background:conic-gradient(from 90deg,${c.c1} 0deg 180deg,${c.c2||c.c1} 180deg 360deg)`:`background:${grad}`;

    if(c.nivel!==lastNivel){
      lastNivel=c.nivel;
      out+=`<div class="nivel-hdr" style="background:${nc.bg};border:1px solid ${nc.bd};margin-top:${out?'22px':'0'}">
        <div style="width:8px;height:8px;border-radius:50%;background:${nc.tx};box-shadow:0 0 8px ${nc.tx};flex-shrink:0"></div>
        <span style="font-family:'Cinzel',serif;font-size:.78rem;font-weight:900;letter-spacing:.12em;text-transform:uppercase;color:${nc.tx}">Nível ${NLBL[c.nivel]}</span>
        <span style="margin-left:auto;font-size:.6rem;color:${nc.tx};opacity:.7">⏱ ${tempo}</span>
      </div>`;
    }

    const chips=alunosNaCorda.length?`<div class="cr-chips">${alunosNaCorda.map(a=>`<span class="pill p-mute" style="font-size:.58rem">👤 ${a.nome}</span>`).join('')}</div>`:'';
    const countBadge=alunosNaCorda.length?`<span class="pill p-ok" style="font-size:.62rem">${alunosNaCorda.length}</span>`:'';

    out+=`<div class="corda-row" id="cr-row-${i}" onclick="toggleCorda(${i})">
      <div class="cr-circle" style="${circleStyle}"></div>
      <div class="cr-info">
        <div class="cr-name">${c.nome}</div>
        <div class="cr-meta"><span>${NLBL[c.nivel]}</span> · <span class="cr-sim">${c.sim}</span></div>
      </div>
      <div class="cr-right">
        ${countBadge}
        <span class="cr-chevron">▶</span>
      </div>
    </div>
    <div class="cr-detail">
      ${c.desc}
      ${chips}
    </div>`;
  });
  document.getElementById('cordas-list').innerHTML=out;
}

// ── SESSÃO DE USUÁRIO (compatível com FIU_Entrada.html) ──
function loadSess(){try{return JSON.parse(sessionStorage.getItem('fiu_session')||'null');}catch(e){return null;}}
let currentUser=loadSess(); // {username, nome, role} ou null se acessado direto sem login
function canEdit(){return !currentUser||currentUser.role==='professor'||currentUser.role==='contramestre'||currentUser.role==='mestre';}
function isMestre(){return !currentUser||currentUser.role==='mestre';}
function isAluno(){return currentUser&&currentUser.role==='aluno';}
// Retorna o registro do aluno (em S.alunos) vinculado ao usuário logado, se houver.
function alunoLogado(){
  if(!currentUser||currentUser.role!=='aluno')return null;
  return S.alunos.find(a=>a.username===currentUser.username)||null;
}

// ── NOTIFICAÇÕES ──
function addNotif(tipo,titulo,sub,icon,iconBg,iconColor,alunoId){
  S.notificacoes.unshift({
    id:uid(),tipo,titulo,sub,icon,iconBg,iconColor,alunoId,
    data:new Date().toISOString(),lida:false
  });
  if(S.notificacoes.length>80)S.notificacoes=S.notificacoes.slice(0,80);
  save();
  renderNotifBadge();
}
function notifTempoRel(iso){
  const diffMs=Date.now()-new Date(iso).getTime();
  const min=Math.floor(diffMs/60000),h=Math.floor(min/60),d=Math.floor(h/24);
  if(min<1)return'Agora mesmo';
  if(min<60)return`Há ${min} min`;
  if(h<24)return`Há ${h}h`;
  if(d===1)return'Há 1 dia';
  if(d<30)return`Há ${d} dias`;
  return fmtBR(iso.slice(0,10));
}
const NOTIF_ICONS={
  pagamento_atraso:{icon:'⚠',bg:'var(--er-bg)',color:'var(--er-tx)'},
  pagamento_confirmado:{icon:'💰',bg:'var(--ok-bg)',color:'var(--ok-tx)'},
  aula_nova:{icon:'🕐',bg:'var(--in-bg)',color:'var(--in-tx)'},
  promocao:{icon:'🎽',bg:'var(--wn-bg)',color:'var(--wn-tx)'},
  mensagem:{icon:'✉',bg:'rgba(122,56,184,.12)',color:'#a064d8'}
};
function renderNotifBadge(){
  const n=S.notificacoes.filter(x=>!x.lida).length;
  const badge=document.getElementById('notif-badge');
  if(!badge)return;
  badge.textContent=n>9?'9+':n;
  badge.classList.toggle('hidden',n===0);
}
function toggleNotifPanel(force){
  const panel=document.getElementById('notif-panel');
  const willOpen=force!==undefined?force:!panel.classList.contains('open');
  panel.classList.toggle('open',willOpen);
  if(willOpen)renderNotifPanel();
}
document.addEventListener('click',e=>{
  const wrap=document.querySelector('.notif-wrap');
  if(wrap&&!wrap.contains(e.target))document.getElementById('notif-panel').classList.remove('open');
});
function renderNotifPanel(){
  const list=document.getElementById('notif-list');
  const sub=document.getElementById('notif-head-sub');
  const naoLidas=S.notificacoes.filter(x=>!x.lida).length;
  sub.textContent=naoLidas?`${naoLidas} não lida${naoLidas>1?'s':''}`:'Tudo em dia';
  if(!S.notificacoes.length){
    list.innerHTML=`<div class="notif-empty"><div class="ne-icon"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M6 8a6 6 0 0 1 12 0c0 7 3 9 3 9H3s3-2 3-9"/><path d="M10.3 21a1.94 1.94 0 0 0 3.4 0"/></svg></div><p>Nenhuma notificação ainda.</p></div>`;
    return;
  }
  list.innerHTML=S.notificacoes.map(n=>{
    const meta=NOTIF_ICONS[n.tipo]||{icon:'🔔',bg:'var(--surf2)',color:'var(--mute)'};
    return`<div class="notif-item${n.lida?'':' unread'}" onclick="marcarNotifLida('${n.id}')">
      <div class="notif-ic" style="background:${n.iconBg||meta.bg};color:${n.iconColor||meta.color}">${n.icon||meta.icon}</div>
      <div class="notif-body">
        <div class="notif-title">${n.titulo}</div>
        ${n.sub?`<div class="notif-sub">${n.sub}</div>`:''}
        <div class="notif-time">${notifTempoRel(n.data)}</div>
      </div>
      <button class="notif-del" onclick="event.stopPropagation();delNotif('${n.id}')">×</button>
    </div>`;
  }).join('');
}
function marcarNotifLida(id){
  const n=S.notificacoes.find(x=>x.id===id);
  if(n)n.lida=true;
  save();renderNotifBadge();renderNotifPanel();
  if(n&&n.alunoId){
    toggleNotifPanel(false);
    abrirChatComAluno(n.alunoId);
  }
}
function marcarTodasLidas(){S.notificacoes.forEach(n=>n.lida=true);save();renderNotifBadge();renderNotifPanel();toast('✓ Todas marcadas como lidas.');}
function delNotif(id){S.notificacoes=S.notificacoes.filter(x=>x.id!==id);save();renderNotifBadge();renderNotifPanel();}
function limparNotificacoes(){if(!S.notificacoes.length)return;if(!confirm('Limpar todas as notificações?'))return;S.notificacoes=[];save();renderNotifBadge();renderNotifPanel();toast('Notificações limpas.');}

// ── Mensagens manuais entre usuários ──
function enviarMensagem(){
  const destino=document.getElementById('msg-destino').value;
  const assunto=document.getElementById('msg-assunto').value.trim();
  const texto=document.getElementById('msg-texto').value.trim();
  if(!assunto||!texto){toast('Preencha assunto e mensagem','warn');return;}
  const destLabel=destino==='todos'?'Mural geral':'Professores e Mestres';
  addNotif('mensagem',assunto,`Para: ${destLabel} · ${texto}`,'✉','rgba(122,56,184,.12)','#a064d8');
  document.getElementById('msg-assunto').value='';
  document.getElementById('msg-texto').value='';
  closeModal('modal-nova-msg');
  toast('✉ Mensagem enviada!');
}

// ── Geração automática de notificações ──
function checarNotificacoesAutomaticas(){
  const vistos=S.notificacoes.filter(n=>n.tipo==='pagamento_atraso').map(n=>n.refId);
  S.alunos.forEach(a=>{
    if(statusPagAluno(a)==='atrasado'&&!vistos.includes('atraso-'+a.id+'-'+today().slice(0,7))){
      const n={id:uid(),tipo:'pagamento_atraso',titulo:'Pagamento em atraso',sub:`${a.nome} está com a mensalidade atrasada.`,icon:'⚠',iconBg:'var(--er-bg)',iconColor:'var(--er-tx)',data:new Date().toISOString(),lida:false,refId:'atraso-'+a.id+'-'+today().slice(0,7)};
      S.notificacoes.unshift(n);
    }
  });
  save();
  renderNotifBadge();
}
// ── BADGE DE USUÁRIO LOGADO (nav) ──
const ROLE_META={
  aluno:{label:'Aluno',icon:'🤸',dot:'#079d28'},
  professor:{label:'Professor',icon:'👨‍🏫',dot:'#073e8e'},
  contramestre:{label:'Contra Mestre',icon:'🛡️',dot:'#d4704a'},
  mestre:{label:'Mestre',icon:'⭐',dot:'#886e12'}
};
function aplicarUserBadge(){
  const badge=document.getElementById('user-badge');
  if(!badge)return;
  if(!currentUser){badge.style.display='none';return;}
  const meta=ROLE_META[currentUser.role]||{label:currentUser.role,icon:'👤',dot:'#888'};
  badge.style.display='flex';
  badge.querySelector('.rdot').style.background=meta.dot;
  document.getElementById('user-badge-name').textContent=`${meta.icon} ${currentUser.nome}`;
  badge.title='Logado como '+meta.label+' · Clique para sair';
}
function doLogout(){
  if(!confirm('Deseja sair da sua conta?'))return;
  sessionStorage.removeItem('fiu_session');
  window.location.href='FIU_Entrada.html';
}

checarNotificacoesAutomaticas();

// ── CHAT (Mensagens entre staff e alunos) ──
function escapeHtml(s){
  const div=document.createElement('div');
  div.textContent=s==null?'':String(s);
  return div.innerHTML;
}
let chatSelecionadoId=null;

function getChatAluno(alunoId){return S.chats[alunoId]||[];}

function enviarChatMsg(alunoId,texto,remetente,autorNome){
  if(!texto||!texto.trim())return;
  if(!S.chats[alunoId])S.chats[alunoId]=[];
  S.chats[alunoId].push({id:uid(),remetente,autorNome,texto:texto.trim(),data:new Date().toISOString(),lida:false});
  save();
  if(remetente==='aluno'){
    const aluno=getAluno(alunoId);
    addNotif('mensagem','Nova mensagem de '+(aluno?aluno.nome:'aluno'),texto.trim(),'✉','rgba(122,56,184,.12)','#a064d8',alunoId);
  }
}

// Monta e insere no chat do aluno um "cartão" de comprovante referente a um pagamento já pago.
function enviarComprovanteChat(alunoId,pagamento){
  const aluno=getAluno(alunoId);
  if(!aluno)return false;
  if(!S.chats[alunoId])S.chats[alunoId]=[];
  S.chats[alunoId].push({
    id:uid(),remetente:'staff',autorNome:currentUser?currentUser.nome:'Equipe',
    tipo:'comprovante',
    texto:'Comprovante de pagamento — '+fmtMoeda(pagamento.valor)+' ('+fmtMes(pagamento.mes)+')',
    comprovante:{valor:pagamento.valor,mes:pagamento.mes,forma:pagamento.forma,data:pagamento.data,alunoNome:aluno.nome},
    data:new Date().toISOString(),lida:false
  });
  save();
  return true;
}

// Envia (ou reenvia) o comprovante de um pagamento específico já confirmado, pelo seu id.
function enviarComprovante(pagamentoId){
  const p=S.pagamentos.find(x=>x.id===pagamentoId);
  if(!p){toast('Pagamento não encontrado','warn');return;}
  if(p.status!=='pago'){toast('Só é possível enviar comprovante de pagamentos já confirmados','warn');return;}
  const ok=enviarComprovanteChat(p.alunoId,p);
  if(!ok){toast('Aluno não encontrado','warn');return;}
  if(chatSelecionadoId===p.alunoId){
    renderChatThread(p.alunoId,'chat-thread-wrap','staff');
  }
  renderChatLista();
  atualizarChatNavBadge();
  toast('📄 Comprovante enviado pelo chat!');
}

function countChatNaoLidas(alunoId,meuLado){
  const outroLado=meuLado==='staff'?'aluno':'staff';
  return getChatAluno(alunoId).filter(m=>m.remetente===outroLado&&!m.lida).length;
}

function marcarChatLido(alunoId,meuLado){
  const outroLado=meuLado==='staff'?'aluno':'staff';
  let changed=false;
  getChatAluno(alunoId).forEach(m=>{if(m.remetente===outroLado&&!m.lida){m.lida=true;changed=true;}});
  if(changed)save();
}

function totalChatNaoLidasStaff(){
  let total=0;
  Object.keys(S.chats).forEach(aId=>{total+=countChatNaoLidas(aId,'staff');});
  return total;
}

function atualizarChatNavBadge(){
  const badge=document.getElementById('chat-nav-badge');
  if(!badge)return;
  let n;
  if(isAluno()){
    const aluno=alunoLogado();
    n=aluno?countChatNaoLidas(aluno.id,'aluno'):0;
  }else{
    n=totalChatNaoLidasStaff();
  }
  badge.textContent=n>9?'9+':n;
  badge.classList.toggle('hidden',n===0);
}

function renderMensagens(){
  if(isAluno()){
    document.getElementById('chat-staff-view').style.display='none';
    document.getElementById('chat-aluno-view').style.display='';
    const aluno=alunoLogado();
    if(!aluno){
      document.getElementById('chat-thread-aluno-wrap').innerHTML='<div class="empty-st"><div class="empty-icon">💬</div><p>Não foi possível localizar seu cadastro de aluno.</p></div>';
      return;
    }
    renderChatThread(aluno.id,'chat-thread-aluno-wrap','aluno');
    marcarChatLido(aluno.id,'aluno');
  }else{
    document.getElementById('chat-staff-view').style.display='';
    document.getElementById('chat-aluno-view').style.display='none';
    renderChatLista();
    if(chatSelecionadoId){
      renderChatThread(chatSelecionadoId,'chat-thread-wrap','staff');
      marcarChatLido(chatSelecionadoId,'staff');
      renderChatLista();
    }
  }
  atualizarChatNavBadge();
}

function renderChatLista(){
  const q=(document.getElementById('chat-search')||{value:''}).value.toLowerCase();
  const lista=document.getElementById('chat-lista');
  if(!lista)return;
  let alunos=S.alunos.filter(a=>a.nome.toLowerCase().includes(q));
  alunos=[...alunos].sort((a,b)=>{
    const aInad=statusPagAluno(a)==='atrasado',bInad=statusPagAluno(b)==='atrasado';
    if(aInad!==bInad)return aInad?-1:1;
    const aUn=countChatNaoLidas(a.id,'staff'),bUn=countChatNaoLidas(b.id,'staff');
    if((aUn>0)!==(bUn>0))return aUn>0?-1:1;
    return a.nome.localeCompare(b.nome);
  });
  if(!alunos.length){lista.innerHTML='<div class="empty-st" style="padding:20px"><p>Nenhum aluno.</p></div>';return;}
  lista.innerHTML=alunos.map(a=>{
    const msgs=getChatAluno(a.id);
    const ultima=msgs[msgs.length-1];
    const unread=countChatNaoLidas(a.id,'staff');
    const inad=statusPagAluno(a)==='atrasado';
    const c=CORDAS[a.cordaIdx];const grad=cordGrad(c);
    const ini=a.nome.split(' ').slice(0,2).map(w=>w[0]).join('');
    const previewTxt=ultima?(ultima.tipo==='comprovante'?'📄 Comprovante de pagamento':ultima.texto):null;
    const preview=previewTxt?escapeHtml((ultima.remetente==='staff'?'Você: ':'')+previewTxt):(inad?'⚠ Sem conversa ainda':'Sem conversa ainda');
    return`<div class="chat-item${chatSelecionadoId===a.id?' sel':''}${inad?' inadimplente':''}" onclick="selectChatAluno(${a.id})">
      <div class="av" style="background:${grad};width:34px;height:34px;font-size:.72rem;flex-shrink:0">${ini}</div>
      <div class="chat-item-info">
        <div class="chat-item-name">${a.nome}${inad?' <span style="color:var(--er-tx);font-size:.62rem">⚠</span>':''}</div>
        <div class="chat-item-preview">${preview}</div>
      </div>
      ${unread>0?`<div class="chat-item-unread">${unread>9?'9+':unread}</div>`:''}
    </div>`;
  }).join('');
}

function selectChatAluno(id){
  chatSelecionadoId=id;
  renderChatLista();
  renderChatThread(id,'chat-thread-wrap','staff');
  marcarChatLido(id,'staff');
  renderChatLista();
  atualizarChatNavBadge();
}

function montarBolhaHtml(m,meuLado){
  const mine=m.remetente===meuLado;
  const hora=new Date(m.data);
  const horaStr=`${String(hora.getHours()).padStart(2,'0')}:${String(hora.getMinutes()).padStart(2,'0')}`;
  const metaHtml=`<div class="chat-bubble-meta">${m.autorNome?escapeHtml(m.autorNome)+' · ':''}${horaStr}</div>`;
  if(m.tipo==='comprovante'&&m.comprovante){
    const r=m.comprovante;
    return`<div class="chat-bubble-row ${mine?'mine':'theirs'}">
      <div class="chat-receipt">
        <div class="chat-receipt-head"><span class="cr-ic">✅</span><span class="cr-lbl">Comprovante de Pagamento</span></div>
        <div class="chat-receipt-value"><div class="cr-num">${fmtMoeda(r.valor)}</div><div class="cr-sub">Pago</div></div>
        <div class="chat-receipt-body">
          <div class="chat-receipt-row"><span>Aluno</span><span>${escapeHtml(r.alunoNome)}</span></div>
          <div class="chat-receipt-row"><span>Referente a</span><span>${escapeHtml(fmtMes(r.mes))}</span></div>
          <div class="chat-receipt-row"><span>Forma</span><span>${escapeHtml(r.forma)}</span></div>
          <div class="chat-receipt-row"><span>Data</span><span>${fmtBR(r.data)}</span></div>
        </div>
      </div>
      ${metaHtml}
    </div>`;
  }
  return`<div class="chat-bubble-row ${mine?'mine':'theirs'}">
    <div class="chat-bubble">${escapeHtml(m.texto)}</div>
    ${metaHtml}
  </div>`;
}

function renderChatThread(alunoId,wrapId,meuLado){
  const wrap=document.getElementById(wrapId);
  if(!wrap)return;
  const aluno=getAluno(alunoId);
  if(!aluno){wrap.innerHTML='<div class="empty-st"><div class="empty-icon">💬</div><p>Aluno não encontrado.</p></div>';return;}
  const msgs=getChatAluno(alunoId);
  const st=statusPagAluno(aluno);
  const sl=statusPagLabel(st);
  const c=CORDAS[aluno.cordaIdx];

  const bubbles=msgs.length?msgs.map(m=>montarBolhaHtml(m,meuLado)).join(''):`<div class="empty-st" style="padding:30px"><div class="empty-icon">💬</div><p>Nenhuma mensagem ainda. Envie a primeira!</p></div>`;

  wrap.innerHTML=`
    <div class="chat-thread-header">
      <div class="av" style="background:${cordGrad(c)};width:36px;height:36px;font-size:.76rem;flex-shrink:0">${aluno.nome.split(' ').slice(0,2).map(w=>w[0]).join('')}</div>
      <div style="flex:1">
        <div class="chat-thread-title">${aluno.nome}</div>
        <div class="chat-thread-sub">${meuLado==='staff'?`<span class="pill ${sl.cls}" style="font-size:.56rem">${sl.label}</span>`:'Fale com a academia'}</div>
      </div>
      ${meuLado==='staff'&&st==='atrasado'?`<button class="chat-quick-btn" onclick="enviarLembretePagamento(${aluno.id})">⚠ Cobrar</button>`:''}
    </div>
    <div class="chat-messages" id="chat-messages-${wrapId}">${bubbles}</div>
    <div class="chat-input-row">
      <input class="inp" id="chat-input-${wrapId}" placeholder="Escreva uma mensagem..." onkeydown="if(event.key==='Enter')enviarMsgChatForm(${alunoId},'${wrapId}','${meuLado}')"/>
      <button class="btn btn-g btn-sm" onclick="enviarMsgChatForm(${alunoId},'${wrapId}','${meuLado}')">Enviar</button>
    </div>`;
  const msgsEl=document.getElementById('chat-messages-'+wrapId);
  if(msgsEl)msgsEl.scrollTop=msgsEl.scrollHeight;
}

function enviarMsgChatForm(alunoId,wrapId,meuLado){
  const input=document.getElementById('chat-input-'+wrapId);
  const texto=input.value.trim();
  if(!texto)return;
  const autorNome=currentUser?currentUser.nome:(meuLado==='aluno'?'Aluno':'Equipe');
  enviarChatMsg(alunoId,texto,meuLado,autorNome);
  input.value='';
  renderChatThread(alunoId,wrapId,meuLado);
  if(meuLado==='staff')renderChatLista();
  atualizarChatNavBadge();
}

function enviarLembretePagamento(alunoId){
  const aluno=getAluno(alunoId);
  if(!aluno)return;
  const texto=`Olá, ${aluno.nome}! Notamos que sua mensalidade está em atraso. Poderia regularizar assim que possível? Qualquer dúvida, estamos à disposição. 🙏`;
  enviarChatMsg(alunoId,texto,'staff',currentUser?currentUser.nome:'Equipe');
  renderChatThread(alunoId,'chat-thread-wrap','staff');
  renderChatLista();
  atualizarChatNavBadge();
  toast('Lembrete de pagamento enviado!');
}

function abrirChatComAluno(id){
  document.querySelectorAll('.ntab').forEach(t=>t.classList.remove('active'));
  const tab=document.getElementById('ntab-mensagens');
  if(tab)tab.classList.add('active');
  showPage('mensagens',null);
  selectChatAluno(id);
}

// ── Cor do ícone de Cordas conforme o usuário logado ──
function aplicarCorCordaNav(){
  const el=document.getElementById('corda-nav-icon');
  if(!el)return;
  const aluno=alunoLogado();
  if(aluno&&CORDAS[aluno.cordaIdx]){
    const c=CORDAS[aluno.cordaIdx];
    el.style.setProperty('--corda-c1',c.c1);
    el.style.setProperty('--corda-c2',c.c2||c.c1);
    el.title='Sua corda: '+c.nome;
  }else{
    el.style.removeProperty('--corda-c1');
    el.style.removeProperty('--corda-c2');
    el.title='Cordas';
  }
}
// ── PRESENÇA ──────────────────────────────────────────────────────
function renderPresenca(){
  const td=today();
  const tdDate=parseD(td);
  const diaSem=tdDate.getDay(); // 0=Dom … 6=Sáb

  // ── Hero: data + nome + mini-stats ──
  const meses=['Janeiro','Fevereiro','Março','Abril','Maio','Junho','Julho','Agosto','Setembro','Outubro','Novembro','Dezembro'];
  const el_date=document.getElementById('ph-date');
  if(el_date) el_date.textContent=`${DIAS_SEMANA[diaSem]}, ${tdDate.getDate()} de ${meses[tdDate.getMonth()]} de ${tdDate.getFullYear()}`;

  const el_user=document.getElementById('ph-username');
  if(el_user) el_user.textContent=currentUser?currentUser.nome:'FIU Capoeira';

  // mini-stats
  const el_stats=document.getElementById('ph-stats-mini');
  if(el_stats){
    const total=S.alunos.length;
    const presHoje=S.alunos.filter(a=>{
      const aulas=getAulasDia(a.id,td);
      return aulas.some(au=>au.status==='P');
    }).length;
    const aulasHoje=S.grade.filter(g=>g.dias.includes(diaSem)).length;
    el_stats.innerHTML=[
      {v:total,l:'Alunos'},
      {v:aulasHoje,l:'Aulas hoje'},
      {v:presHoje,l:'Presenças'}
    ].map(s=>`<div style="text-align:center">
      <div style="font-family:'Cinzel',serif;font-size:1.4rem;font-weight:900;color:#fff;line-height:1">${s.v}</div>
      <div style="font-size:.6rem;color:rgba(255,255,255,.7);letter-spacing:.1em;text-transform:uppercase">${s.l}</div>
    </div>`).join('<div style="width:1px;background:rgba(255,255,255,.18);height:28px;align-self:center"></div>');
  }

  // ── Aulas de hoje ──
  const el_sub=document.getElementById('hoje-subtitle');
  const el_grid=document.getElementById('hoje-grid');
  const aulasGrade=S.grade.filter(g=>g.dias.includes(diaSem));

  if(el_sub) el_sub.textContent=aulasGrade.length
    ?`${aulasGrade.length} aula${aulasGrade.length>1?'s':''} programada${aulasGrade.length>1?'s':''} para hoje`
    :'Nenhuma aula programada para hoje';

  // Botões de ações professor
  const profAct=document.getElementById('pres-prof-actions');
  if(profAct) profAct.style.display=canEdit()?'':'none';

  if(!el_grid) return;

  if(!aulasGrade.length){
    el_grid.innerHTML=`<div class="empty-hoje"><div class="empty-icon">📅</div><p>Não há aulas na grade para hoje.<br><span style="font-size:.8em">Adicione aulas na aba Grade.</span></p></div>`;
  } else {
    el_grid.innerHTML=aulasGrade.map(g=>{
      // contar presença geral desta aula hoje (por slot exato da grade: modalidade + horário,
      // evitando somar presenças de outra turma que tenha a mesma modalidade em outro horário)
      const alunosPresentes=S.alunos.filter(a=>{
        const aulas=getAulasDia(a.id,td);
        return aulas.some(au=>au.mod===g.mod&&au.inicio===g.inicio&&au.status==='P');
      }).length;
      const alunosFalta=S.alunos.filter(a=>{
        const aulas=getAulasDia(a.id,td);
        return aulas.some(au=>au.mod===g.mod&&au.inicio===g.inicio&&au.status==='A');
      }).length;
      const cor=alunosPresentes>0?'var(--ok-bd)':alunosFalta>0?'var(--er-bd)':'var(--bord2)';
      const turmaLabel=g.turma?` — ${g.turma}`:'';
      return `<div class="aula-card-hoje" style="border-left:4px solid ${cor}">
        <div class="ach-time">⏱ ${g.inicio} – ${g.fim}</div>
        <div class="ach-mod">${g.mod}</div>
        <div class="ach-turma">${DIAS_SEMANA[diaSem]}${turmaLabel}</div>
        <div class="ach-status">
          <div style="display:flex;gap:8px;font-size:.72rem">
            <span style="color:var(--ok-tx)">✓ ${alunosPresentes}</span>
            <span style="color:var(--er-tx)">✗ ${alunosFalta}</span>
            <span style="color:var(--mute)">/ ${S.alunos.length}</span>
          </div>
          ${canEdit()?`<button class="ach-mark-btn ach-n" onclick="showPage('presenca',null);document.getElementById('pres-prof-view').style.display=''">Ver Chamada</button>`:''}
        </div>
      </div>`;
    }).join('');
  }

  // ── Strip semanal (7 dias da semana atual) ──
  const el_week=document.getElementById('week-grid');
  const el_range=document.getElementById('week-range');
  if(el_week){
    // início da semana (segunda)
    const inicio=new Date(tdDate);
    inicio.setDate(tdDate.getDate()-((diaSem+6)%7));
    const dias=[];
    for(let i=0;i<7;i++){
      const d=new Date(inicio);d.setDate(inicio.getDate()+i);
      dias.push(d);
    }
    if(el_range){
      const fmt=d=>`${d.getDate()}/${d.getMonth()+1}`;
      el_range.textContent=`${fmt(dias[0])} – ${fmt(dias[6])}`;
    }
    el_week.innerHTML=dias.map(d=>{
      const ds=dateToStr(d);
      const isTd=ds===td;
      const temAula=S.grade.some(g=>g.dias.includes(d.getDay()));
      // checar presença de qualquer aluno neste dia
      let hasP=false,hasA=false,hasMixed=false;
      S.alunos.forEach(a=>{
        const aulas=getAulasDia(a.id,ds);
        aulas.forEach(au=>{
          if(au.status==='P')hasP=true;
          if(au.status==='A')hasA=true;
        });
      });
      if(hasP&&hasA)hasMixed=true;
      let cls='wday-num';
      if(isTd)cls+=' today';
      else if(hasMixed)cls+=' has-m';
      else if(hasP)cls+=' has-p';
      else if(hasA)cls+=' has-a';
      else if(!temAula)cls+=' no-class';
      return `<div class="wday">
        <div class="wday-label">${DIAS_SEMANA[d.getDay()]}</div>
        <div class="${cls}" onclick="goToDate('${ds}')">${d.getDate()}</div>
        <div class="wday-dots">${temAula?`<div class="wdot" style="background:${hasP?'var(--ok-tx)':hasA?'var(--er-tx)':'var(--bord2)'}"></div>`:''}</div>
      </div>`;
    }).join('');
  }

  // ── Visibilidade dos painéis prof/aluno ──
  const profView=document.getElementById('pres-prof-view');
  if(profView) profView.style.display=canEdit()?'':'none';
}

aplicarCorCordaNav();
aplicarUserBadge();

renderAlunoList();
renderDiasCheck();
renderNotifBadge();
renderPresenca();
atualizarChatNavBadge();

function goToDate(ds){
  if(selectedAluno)renderAttendPanel();
}
</script>
</body>
</html>
