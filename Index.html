<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Ledgerline – Profit & Loss Tracker</title>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/4.4.1/chart.umd.min.js"></script>
<style>
:root{--bg:#0b0f19;--card:#121826;--card2:#171e2e;--line:rgba(255,255,255,.06);--tx:#e6e9f0;--mu:#8b94a7;--ok:#10b981;--bad:#ef4444;--pri:#6366f1;--r:16px}
*{box-sizing:border-box;margin:0}
html{scroll-behavior:smooth}
body{background:radial-gradient(900px 500px at 80% -10%,rgba(99,102,241,.12),transparent),var(--bg);color:var(--tx);font:15px/1.5 Inter,system-ui,sans-serif;min-height:100vh;padding-bottom:48px}
:focus-visible{outline:2px solid var(--pri);outline-offset:2px}
header{position:sticky;top:0;z-index:20;display:flex;justify-content:space-between;align-items:center;gap:12px;padding:14px 20px;background:rgba(11,15,25,.7);backdrop-filter:blur(14px);-webkit-backdrop-filter:blur(14px);border-bottom:1px solid var(--line)}
.brand{font-weight:700;font-size:18px;letter-spacing:-.02em}
.brand span{color:var(--mu);font-weight:500;font-size:13px;margin-left:8px}
main{max-width:1520px;margin:0 auto;padding:22px 16px;display:grid;gap:18px;animation:in .6s ease both}
@keyframes in{from{opacity:0}to{opacity:1}}
.card{background:var(--card);border:1px solid var(--line);border-radius:var(--r);padding:18px;box-shadow:0 8px 30px rgba(0,0,0,.25)}
.card h2{font-size:15px;font-weight:600;margin-bottom:14px}
.kpis{display:grid;grid-template-columns:repeat(auto-fit,minmax(210px,1fr));gap:14px}
.kpi{transition:transform .25s ease,border-color .25s ease}
.kpi:hover{transform:translateY(-3px);border-color:rgba(255,255,255,.14)}
.kpi small{color:var(--mu);font-size:13px}
.kpi b{display:block;font-size:28px;font-weight:700;letter-spacing:-.03em;margin:4px 0;font-variant-numeric:tabular-nums}
.kpi i{font-style:normal;font-size:12px;color:var(--mu)}
.pos{color:var(--ok)}.neg{color:var(--bad)}
.cols{display:grid;grid-template-columns:340px 1fr;gap:18px}
.charts{display:grid;grid-template-columns:1fr 1fr;gap:18px}
.charts .wide{grid-column:1/-1}
.ch{position:relative;height:230px}
@media(max-width:900px){.cols,.charts{grid-template-columns:1fr}}
label{display:block;font-size:13px;color:var(--mu);margin:12px 0 5px}
input,select,button,textarea{font:inherit;color:var(--tx)}
input,select{width:100%;background:var(--card2);border:1px solid var(--line);border-radius:10px;padding:10px 12px;transition:border-color .2s}
input:focus,select:focus{border-color:var(--pri);outline:none}
.err{color:var(--bad);font-size:12px;min-height:16px;margin-top:3px}
.seg{display:grid;grid-template-columns:1fr 1fr;background:var(--card2);border-radius:10px;padding:4px;gap:4px}
.seg button{border:0;background:none;padding:9px;border-radius:8px;cursor:pointer;color:var(--mu);transition:all .2s}
.seg button.on.inc{background:rgba(16,185,129,.18);color:var(--ok)}
.seg button.on.exp{background:rgba(239,68,68,.18);color:var(--bad)}
.btn{border:0;border-radius:10px;padding:10px 16px;cursor:pointer;font-weight:600;background:var(--pri);transition:filter .2s,transform .2s}
.btn:hover{filter:brightness(1.12)}.btn:active{transform:scale(.98)}
.btn.ghost{background:var(--card2);border:1px solid var(--line);font-weight:500}
.btn.danger{background:var(--bad)}
.row{display:flex;gap:10px;flex-wrap:wrap;align-items:center}
.filters{display:grid;grid-template-columns:2fr 1fr 1fr 1fr 1fr;gap:10px;margin-bottom:14px}
@media(max-width:900px){.filters{grid-template-columns:1fr 1fr}.filters input:first-child{grid-column:1/-1}}
.tw{overflow-x:auto}
table{width:100%;border-collapse:collapse;min-width:560px}
th{text-align:left;font-size:12px;color:var(--mu);font-weight:500;padding:8px 10px;border-bottom:1px solid var(--line)}
td{padding:11px 10px;border-bottom:1px solid var(--line);font-size:14px}
tr:hover td{background:rgba(255,255,255,.02)}
td.amt{font-variant-numeric:tabular-nums;font-weight:600;text-align:right}
.tag{display:inline-block;font-size:12px;padding:2px 9px;border-radius:99px;background:var(--card2)}
.ic{background:none;border:0;cursor:pointer;color:var(--mu);padding:4px 8px;border-radius:6px}
.ic:hover{color:var(--tx);background:var(--card2)}
.empty{text-align:center;color:var(--mu);padding:34px 10px}
.empty b{display:block;color:var(--tx);margin-bottom:4px}
.months{display:grid;grid-template-columns:repeat(auto-fit,minmax(150px,1fr));gap:10px}
.mo{background:var(--card2);border-radius:12px;padding:12px}
.mo small{color:var(--mu)}.mo b{display:block;font-size:17px;font-variant-numeric:tabular-nums}
#toasts{position:fixed;bottom:18px;left:50%;transform:translateX(-50%);display:grid;gap:8px;z-index:50;width:max-content;max-width:92vw}
.toast{background:#1d2538;border:1px solid var(--line);padding:11px 16px;border-radius:12px;box-shadow:0 10px 30px rgba(0,0,0,.4);animation:up .3s ease both}
@keyframes up{from{opacity:0;transform:translateY(10px)}to{opacity:1;transform:none}}
dialog{background:var(--card);color:var(--tx);border:1px solid var(--line);border-radius:var(--r);padding:22px;max-width:360px;margin:auto}
dialog::backdrop{background:rgba(0,0,0,.6)}
dialog p{color:var(--mu);margin:8px 0 18px}
@media(min-width:1100px){body{font-size:16px}header{padding:16px 40px}.brand{font-size:21px}main{padding:30px 40px;gap:24px}.card{padding:26px}.card h2{font-size:17px;margin-bottom:18px}.kpis{grid-template-columns:repeat(4,1fr);gap:22px}.kpi b{font-size:40px}.kpi small{font-size:14px}.cols{grid-template-columns:420px 1fr;gap:24px}.charts{gap:24px}.ch{height:310px}td{padding:15px 12px;font-size:15px}th{font-size:13px;padding:10px 12px}.months{grid-template-columns:repeat(6,1fr);gap:14px}.mo b{font-size:20px}table{min-width:0}input,select{padding:12px 14px}}
@media(prefers-reduced-motion:reduce){*{animation:none!important;transition:none!important;scroll-behavior:auto!important}}
</style>
</head>
<body>
<header>
  <div class="brand">Ledgerline<span>Profit &amp; Loss</span></div>
  <div class="row">
    <label for="cur" style="margin:0" class="sr">Currency</label>
    <select id="cur" aria-label="Currency" style="width:auto">
      <option value="৳">BDT ৳</option><option value="$">USD $</option><option value="₹">INR ₹</option>
    </select>
  </div>
</header>

<main>
  <section class="kpis" aria-label="Summary">
    <div class="card kpi"><small>Total income</small><b id="kInc">0</b><i>All time</i></div>
    <div class="card kpi"><small>Total expense</small><b id="kExp">0</b><i>All time</i></div>
    <div class="card kpi"><small>Net profit / loss</small><b id="kNet">0</b><i id="kMom">–</i></div>
    <div class="card kpi"><small>Profit margin</small><b id="kMar">0%</b><i>Net ÷ income</i></div>
  </section>

  <section class="cols">
    <form class="card" id="form" novalidate>
      <h2 id="formTitle">Add transaction</h2>
      <div class="seg" role="group" aria-label="Type">
        <button type="button" class="inc on" data-t="income">Income</button>
        <button type="button" class="exp" data-t="expense">Expense</button>
      </div>
      <label for="amount">Amount</label>
      <input id="amount" type="number" step="0.01" min="0" inputmode="decimal" placeholder="0.00">
      <div class="err" id="eAmount"></div>
      <label for="category">Category</label>
      <input id="category" list="cats" placeholder="e.g. Sales, Rent, Stock">
      <datalist id="cats"></datalist>
      <div class="err" id="eCat"></div>
      <label for="date">Date</label>
      <input id="date" type="date">
      <div class="err" id="eDate"></div>
      <label for="note">Note (optional)</label>
      <input id="note" maxlength="80" placeholder="Short description">
      <div class="row" style="margin-top:16px">
        <button class="btn" type="submit" id="saveBtn">Add transaction</button>
        <button class="btn ghost" type="button" id="cancelEdit" hidden>Cancel</button>
      </div>
    </form>

    <div class="charts">
      <div class="card"><h2>Income vs expense</h2><div class="ch"><canvas id="c1" role="img" aria-label="Monthly income versus expense bar chart"></canvas></div></div>
      <div class="card"><h2>Expense by category</h2><div class="ch"><canvas id="c3" role="img" aria-label="Expense by category chart"></canvas></div></div>
      <div class="card wide"><h2>Profit trend</h2><div class="ch"><canvas id="c2" role="img" aria-label="Monthly profit trend line chart"></canvas></div></div>
    </div>
  </section>

  <section class="card">
    <h2>Monthly summary</h2>
    <div class="months" id="months"></div>
  </section>

  <section class="card">
    <h2>Transactions</h2>
    <div class="filters">
      <input id="q" type="search" placeholder="Search note or category" aria-label="Search">
      <select id="fType" aria-label="Type"><option value="">All types</option><option value="income">Income</option><option value="expense">Expense</option></select>
      <select id="fCat" aria-label="Category"><option value="">All categories</option></select>
      <input id="fFrom" type="date" aria-label="From date">
      <input id="fTo" type="date" aria-label="To date">
    </div>
    <div class="tw"><table>
      <thead><tr><th>Date</th><th>Category</th><th>Note</th><th style="text-align:right">Amount</th><th></th></tr></thead>
      <tbody id="rows"></tbody>
    </table></div>
    <div class="row" style="margin-top:16px">
      <button class="btn ghost" id="exp">Export CSV</button>
      <button class="btn ghost" id="impBtn">Import CSV</button>
      <input type="file" id="imp" accept=".csv,text/csv" hidden>
      <button class="btn ghost" id="demo" hidden>Clear demo data</button>
      <button class="btn danger" id="reset" style="margin-left:auto">Reset all data</button>
    </div>
  </section>
</main>

<dialog id="dlg">
  <h2>Reset all data?</h2>
  <p>This deletes every transaction on this device. Export a CSV first if you want a backup.</p>
  <div class="row" style="justify-content:flex-end">
    <button class="btn ghost" id="no">Keep data</button>
    <button class="btn danger" id="yes">Delete everything</button>
  </div>
</dialog>
<div id="toasts" aria-live="polite"></div>

<script>
(function(){
"use strict";
var KEY="ledgerline.v1", S={tx:[],cur:"৳",demo:false}, type="income", editId=null, charts={};
var $=function(i){return document.getElementById(i)};

/* ---------- storage ---------- */
function load(){
  try{var r=localStorage.getItem(KEY); if(r){S=Object.assign(S,JSON.parse(r));return}}catch(e){}
  seed();
}
function save(){try{localStorage.setItem(KEY,JSON.stringify(S))}catch(e){}}
function seed(){
  var d=new Date(),out=[],id=1;
  for(var m=5;m>=0;m--){
    var y=new Date(d.getFullYear(),d.getMonth()-m,1),ym=y.toISOString().slice(0,7);
    var k=1+(5-m)*0.08;
    out.push({id:id++,type:"income",amount:Math.round(82000*k),category:"Sales",date:ym+"-05",note:"Product sales"});
    out.push({id:id++,type:"income",amount:Math.round(18000*k),category:"Services",date:ym+"-18",note:"Client work"});
    out.push({id:id++,type:"expense",amount:25000,category:"Rent",date:ym+"-02",note:"Shop rent"});
    out.push({id:id++,type:"expense",amount:Math.round(38000*(0.9+m%3*0.08)),category:"Stock",date:ym+"-10",note:"Inventory"});
    out.push({id:id++,type:"expense",amount:Math.round(16000+m*900),category:"Salary",date:ym+"-28",note:"Staff"});
    out.push({id:id++,type:"expense",amount:4200+m*150,category:"Utilities",date:ym+"-22",note:"Power & internet"});
  }
  S.tx=out;S.demo=true;save();
}

/* ---------- helpers ---------- */
function esc(s){return String(s).replace(/[&<>"']/g,function(c){return{"&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;","'":"&#39;"}[c]})}
function money(n){
  var neg=n<0,a=Math.abs(n),big=a>=1e7?{maximumFractionDigits:0}:{maximumFractionDigits:a%1?2:0};
  return (neg?"−":"")+S.cur+a.toLocaleString("en-US",big);
}
function sum(list,t){return list.filter(function(x){return x.type===t}).reduce(function(a,x){return a+x.amount},0)}
function toast(m){var t=document.createElement("div");t.className="toast";t.textContent=m;$("toasts").appendChild(t);setTimeout(function(){t.remove()},2600)}
var reduce=window.matchMedia("(prefers-reduced-motion: reduce)").matches;
function count(el,to,fmt){
  var from=parseFloat(el.dataset.v||0);el.dataset.v=to;
  if(reduce){el.textContent=fmt(to);return}
  var t0=performance.now();
  (function f(t){var p=Math.min(1,(t-t0)/600),e=1-Math.pow(1-p,3);el.textContent=fmt(from+(to-from)*e);if(p<1)requestAnimationFrame(f)})(t0);
}
function monthsOf(list){
  var m={};list.forEach(function(x){var k=x.date.slice(0,7);m[k]=m[k]||{i:0,e:0};x.type==="income"?m[k].i+=x.amount:m[k].e+=x.amount});
  return Object.keys(m).sort().map(function(k){return{k:k,i:m[k].i,e:m[k].e,n:m[k].i-m[k].e}});
}
function monthName(k){var p=k.split("-");return new Date(p[0],p[1]-1,1).toLocaleString("en-US",{month:"short",year:"2-digit"})}

/* ---------- render ---------- */
function filtered(){
  var q=$("q").value.trim().toLowerCase(),t=$("fType").value,c=$("fCat").value,f=$("fFrom").value,to=$("fTo").value;
  return S.tx.filter(function(x){
    return (!t||x.type===t)&&(!c||x.category===c)&&(!f||x.date>=f)&&(!to||x.date<=to)&&
      (!q||(x.note+" "+x.category).toLowerCase().indexOf(q)>-1);
  }).sort(function(a,b){return b.date.localeCompare(a.date)||b.id-a.id});
}
function renderKpis(){
  var i=sum(S.tx,"income"),e=sum(S.tx,"expense"),n=i-e,mg=i?n/i*100:0;
  count($("kInc"),i,money);count($("kExp"),e,money);count($("kNet"),n,money);
  count($("kMar"),mg,function(v){return v.toFixed(1)+"%"});
  var net=$("kNet");net.className=n>=0?"pos":"neg";
  var ms=monthsOf(S.tx),mom=$("kMom");
  if(ms.length>1){
    var a=ms[ms.length-1],b=ms[ms.length-2],d=a.n-b.n;
    mom.innerHTML=(n>=0?"▲ ":"▼ ")+monthName(a.k)+" vs "+monthName(b.k)+": <span class='"+(d>=0?"pos":"neg")+"'>"+(d>=0?"+":"")+money(d)+"</span>";
  }else mom.textContent=n>=0?"▲ In profit":"▼ At a loss";
}
function renderTable(){
  var l=filtered(),tb=$("rows");
  if(!l.length){tb.innerHTML="<tr><td colspan='5'><div class='empty'><b>No transactions yet</b>Add your first income or expense using the form.</div></td></tr>";return}
  tb.innerHTML=l.map(function(x){
    return "<tr><td>"+esc(x.date)+"</td><td><span class='tag'>"+esc(x.category)+"</span></td><td>"+esc(x.note||"–")+"</td>"+
    "<td class='amt "+(x.type==="income"?"pos":"neg")+"'>"+(x.type==="income"?"+":"−")+money(x.amount).replace("−","")+"</td>"+
    "<td style='white-space:nowrap;text-align:right'><button class='ic' data-e='"+x.id+"' aria-label='Edit'>Edit</button><button class='ic' data-d='"+x.id+"' aria-label='Delete'>Delete</button></td></tr>";
  }).join("");
}
function renderMonths(){
  var ms=monthsOf(S.tx).slice(-6).reverse();
  $("months").innerHTML=ms.length?ms.map(function(m,ix){
    var p=ms[ix+1],d=p?m.n-p.n:null;
    return "<div class='mo'><small>"+monthName(m.k)+"</small><b class='"+(m.n>=0?"pos":"neg")+"'>"+money(m.n)+"</b><small>"+(d===null?"First month":(d>=0?"▲ ":"▼ ")+money(Math.abs(d))+" vs prior")+"</small></div>";
  }).join(""):"<div class='empty' style='grid-column:1/-1'>Monthly results appear once you add transactions.</div>";
}
function renderCats(){
  var cs=[];S.tx.forEach(function(x){if(cs.indexOf(x.category)<0)cs.push(x.category)});cs.sort();
  $("cats").innerHTML=cs.map(function(c){return "<option value='"+esc(c)+"'>"}).join("");
  var cur=$("fCat").value;
  $("fCat").innerHTML="<option value=''>All categories</option>"+cs.map(function(c){return "<option"+(c===cur?" selected":"")+" value='"+esc(c)+"'>"+esc(c)+"</option>"}).join("");
}
function renderCharts(){
  if(typeof Chart==="undefined")return;
  Chart.defaults.color="#8b94a7";Chart.defaults.font.family="Inter, system-ui, sans-serif";
  Chart.defaults.borderColor="rgba(255,255,255,.06)";
  var ms=monthsOf(S.tx).slice(-6),lab=ms.map(function(m){return monthName(m.k)});
  var cats={};S.tx.filter(function(x){return x.type==="expense"}).forEach(function(x){cats[x.category]=(cats[x.category]||0)+x.amount});
  var ck=Object.keys(cats),pal=["#6366f1","#10b981","#f59e0b","#ef4444","#06b6d4","#a855f7","#ec4899","#84cc16"];
  var cfg={
    c1:{type:"bar",data:{labels:lab,datasets:[{label:"Income",data:ms.map(function(m){return m.i}),backgroundColor:"#10b981",borderRadius:6},{label:"Expense",data:ms.map(function(m){return m.e}),backgroundColor:"#ef4444",borderRadius:6}]}},
    c2:{type:"line",data:{labels:lab,datasets:[{label:"Net profit",data:ms.map(function(m){return m.n}),borderColor:"#6366f1",backgroundColor:"rgba(99,102,241,.15)",fill:true,tension:.35,pointRadius:4}]}},
    c3:{type:"doughnut",data:{labels:ck,datasets:[{data:ck.map(function(k){return cats[k]}),backgroundColor:pal,borderWidth:0}]},options:{cutout:"68%",plugins:{legend:{position:"right"}}}}
  };
  ["c1","c2","c3"].forEach(function(id){
    if(charts[id])charts[id].destroy();
    var c=cfg[id];c.options=Object.assign({responsive:true,maintainAspectRatio:false,animation:reduce?false:{duration:600}},c.options||{});
    if(id!=="c3")c.options.plugins={legend:{display:id==="c1",labels:{boxWidth:10}},tooltip:{callbacks:{label:function(x){return x.dataset.label+": "+money(x.parsed.y)}}}};
    else c.options.plugins.tooltip={callbacks:{label:function(x){return x.label+": "+money(x.parsed)}}};
    charts[id]=new Chart($(id),c);
  });
}
function render(){
  $("cur").value=S.cur;$("demo").hidden=!S.demo;
  renderCats();renderKpis();renderTable();renderMonths();renderCharts();
}

/* ---------- form ---------- */
function setType(t){
  type=t;document.querySelectorAll(".seg button").forEach(function(b){b.classList.toggle("on",b.dataset.t===t)});
}
function resetForm(){
  editId=null;$("form").reset();setType("income");$("date").value=new Date().toISOString().slice(0,10);
  $("formTitle").textContent="Add transaction";$("saveBtn").textContent="Add transaction";$("cancelEdit").hidden=true;
  ["eAmount","eCat","eDate"].forEach(function(i){$(i).textContent=""});
}
function submit(e){
  e.preventDefault();
  var a=parseFloat($("amount").value),c=$("category").value.trim(),d=$("date").value,ok=true;
  $("eAmount").textContent=$("eCat").textContent=$("eDate").textContent="";
  if(!(a>0)||!isFinite(a)||a>1e12){$("eAmount").textContent="Enter an amount greater than 0.";ok=false}
  if(!c){$("eCat").textContent="Add a category, like Sales or Rent.";ok=false}
  if(!d){$("eDate").textContent="Pick a date.";ok=false}
  if(!ok)return;
  var rec={type:type,amount:Math.round(a*100)/100,category:c,date:d,note:$("note").value.trim()};
  if(editId){S.tx=S.tx.map(function(x){return x.id===editId?Object.assign({id:editId},rec):x});toast("Transaction updated")}
  else{rec.id=Date.now()+Math.floor(Math.random()*1000);S.tx.push(rec);toast("Transaction added")}
  save();resetForm();render();
}

/* ---------- csv ---------- */
function exportCsv(){
  if(!S.tx.length){toast("Nothing to export yet");return}
  var q=function(v){return '"'+String(v).replace(/"/g,'""')+'"'};
  var csv="type,amount,category,date,note\n"+S.tx.map(function(x){return [x.type,x.amount,q(x.category),x.date,q(x.note||"")].join(",")}).join("\n");
  var a=document.createElement("a");a.href=URL.createObjectURL(new Blob([csv],{type:"text/csv"}));a.download="ledgerline-export.csv";a.click();
  toast("CSV exported");
}
function parseLine(l){
  var out=[],cur="",inq=false;
  for(var i=0;i<l.length;i++){var ch=l[i];
    if(inq){if(ch==='"'&&l[i+1]==='"'){cur+='"';i++}else if(ch==='"')inq=false;else cur+=ch}
    else if(ch==='"')inq=true;else if(ch===","){out.push(cur);cur=""}else cur+=ch}
  out.push(cur);return out;
}
function importCsv(file){
  var r=new FileReader();
  r.onload=function(){
    var lines=String(r.result).split(/\r?\n/).filter(Boolean).slice(1),n=0;
    lines.forEach(function(l){
      var p=parseLine(l),a=parseFloat(p[1]);
      if((p[0]==="income"||p[0]==="expense")&&a>0&&p[2]&&/^\d{4}-\d{2}-\d{2}$/.t
