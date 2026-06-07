<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<title>Blushbooth By Gift 🎀</title>
<style>
:root{--pk:#f9a8c9;--pkd:#e87dab;--pkl:#fde8f1;--pkp:#fff0f7;--br:#8b5c6e;--tx:#6b3a52}
*{box-sizing:border-box;margin:0;padding:0;-webkit-tap-highlight-color:transparent}
body{font-family:-apple-system,'Helvetica Neue',sans-serif;background:var(--pkp);min-height:100vh;overflow-x:hidden}
body::before{content:'';position:fixed;inset:0;background-image:radial-gradient(circle,#f9a8c940 1.5px,transparent 1.5px);background-size:28px 28px;pointer-events:none;z-index:0}
.scr{display:none;position:relative;z-index:1;min-height:100vh}
.scr.on{display:flex;flex-direction:column}
/* flash */
.flash{position:fixed;inset:0;background:#fff;opacity:0;pointer-events:none;z-index:999;transition:opacity .08s}
.flash.go{opacity:1}
/* WELCOME */
#sw{align-items:center;justify-content:center;gap:18px;padding:32px 18px;text-align:center}
.bow{font-size:48px;animation:bounce 2s infinite}
@keyframes bounce{0%,100%{transform:translateY(0)}50%{transform:translateY(-8px)}}
.logo-t{font-family:Georgia,serif;font-style:italic;font-size:54px;color:var(--pkd);text-shadow:2px 3px 0 #fff,4px 5px 0 #f9a8c940;line-height:1}
.logo-s{font-size:11px;color:var(--br);letter-spacing:5px;text-transform:uppercase;opacity:.8;margin-top:3px}
.card{background:#fff;border-radius:24px;padding:20px 18px;width:100%;max-width:480px;box-shadow:0 6px 32px #f9a8c940;border:2px solid var(--pkl)}
.card h2{font-family:Georgia,serif;font-style:italic;font-size:26px;color:var(--tx);margin-bottom:6px}
.card p{color:#b07090;font-size:13px;line-height:1.7}
.name-wrap{display:flex;flex-direction:column;gap:6px;align-items:center;width:100%;max-width:300px}
.name-wrap label{font-size:11px;font-weight:700;color:var(--br);letter-spacing:1px;text-transform:uppercase}
.name-in{width:100%;border:2.5px solid var(--pkl);border-radius:50px;padding:10px 20px;font-size:22px;font-family:Georgia,serif;font-style:italic;color:var(--pkd);text-align:center;outline:none;background:#fff;transition:border-color .2s}
.name-in:focus{border-color:var(--pkd)}
.name-in::placeholder{color:#e8b0cc}
.mode-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:12px;width:100%;max-width:480px}
.mode-card{background:#fff;border-radius:20px;padding:18px 8px;text-align:center;cursor:pointer;border:2.5px solid var(--pkl);box-shadow:0 4px 20px #f9a8c830;transition:all .2s}
.mode-card:active{transform:scale(.96)}
.mode-card .mi{font-size:34px;display:block;margin-bottom:7px}
.mode-card .mn{font-weight:700;font-size:13px;color:var(--tx)}
.mode-card .md{font-size:11px;color:#c090a8;margin-top:3px;line-height:1.4}
.pearls{display:flex;gap:6px;align-items:center;justify-content:center}
.pearl{width:9px;height:9px;border-radius:50%;background:radial-gradient(circle at 35% 35%,#fff,#e8ddd8);box-shadow:0 1px 3px #0002}
/* CAMERA */
#sc{background:linear-gradient(160deg,#fff0f7,#fde8f1);padding:14px;gap:12px;align-items:center}
.cam-hdr{display:flex;align-items:center;justify-content:space-between;width:100%;max-width:640px}
.cam-title{font-family:Georgia,serif;font-style:italic;font-size:24px;color:var(--pkd)}
.back-btn{background:#fff;border:2px solid var(--pkl);border-radius:50px;padding:8px 16px;font-weight:700;font-size:13px;color:var(--br);cursor:pointer}
.back-btn:active{background:var(--pkl)}
.err-box{background:#fff0f7;border:2px solid var(--pkd);border-radius:16px;padding:14px 16px;max-width:640px;width:100%}
.err-box h4{color:var(--pkd);font-size:13px;font-weight:700;margin-bottom:6px}
.err-box p{font-size:12px;color:var(--tx);line-height:1.7}
.strip-wrap{background:#fff;border-radius:20px;padding:14px;box-shadow:0 8px 40px #f9a8c940;border:2px solid var(--pkl);display:flex;gap:12px;max-width:640px;width:100%}
.strip-thumbs{display:flex;flex-direction:column;gap:7px;width:90px;flex-shrink:0}
.thumb{aspect-ratio:4/3;background:var(--pkp);border-radius:10px;overflow:hidden;border:2px solid var(--pkl);display:flex;align-items:center;justify-content:center;font-size:10px;color:#d4a0b8;font-weight:700;position:relative}
.thumb img{width:100%;height:100%;object-fit:cover}
.thumb .ck{position:absolute;top:3px;right:4px;font-size:12px}
.strip-live{flex:1;display:flex;flex-direction:column;align-items:center;gap:10px}
.vid-wrap{width:100%;border-radius:14px;overflow:hidden;border:2px solid var(--pkl);aspect-ratio:4/3;background:var(--pkl);position:relative}
.vid-wrap video{width:100%;height:100%;object-fit:cover;transform:scaleX(-1)}
.single-wrap{width:100%;max-width:360px;aspect-ratio:3/4;border-radius:20px;overflow:hidden;border:3px solid var(--pkl);background:var(--pkl);position:relative}
.single-wrap video{width:100%;height:100%;object-fit:cover;transform:scaleX(-1)}
.gif-badge{position:absolute;top:8px;right:8px;background:var(--pkd);color:#fff;font-size:10px;font-weight:700;padding:3px 9px;border-radius:20px}
.cdown{font-family:Georgia,serif;font-style:italic;font-size:88px;color:var(--pkd);text-align:center;text-shadow:2px 2px 0 #fff;animation:pulse 1s infinite}
@keyframes pulse{0%,100%{transform:scale(1)}50%{transform:scale(1.1)}}
.hint{font-size:13px;color:#c090a8;font-weight:600;text-align:center}
.shutter{width:72px;height:72px;border-radius:50%;background:linear-gradient(135deg,var(--pkd),#f472b6);border:5px solid #fff;box-shadow:0 0 0 3px var(--pk),0 8px 24px #f9a8c960;cursor:pointer;font-size:26px;display:flex;align-items:center;justify-content:center;transition:transform .1s}
.shutter:active{transform:scale(.93)}
.gif-grid{display:grid;grid-template-columns:1fr 1fr;gap:6px;width:100%;max-width:300px}
.gif-thumb{aspect-ratio:3/4;background:var(--pkl);border-radius:10px;overflow:hidden;border:2px solid var(--pkl)}
.gif-thumb img{width:100%;height:100%;object-fit:cover}
.controls{display:flex;flex-direction:column;align-items:center;gap:10px;max-width:640px;width:100%}
.filter-label{font-size:11px;font-weight:700;color:var(--br);letter-spacing:1px;text-transform:uppercase;align-self:flex-start}
.filter-row{display:flex;gap:7px;overflow-x:auto;width:100%;padding-bottom:4px;scrollbar-width:none}
.filter-row::-webkit-scrollbar{display:none}
.fpill{flex-shrink:0;background:#fff;border:2px solid var(--pkl);border-radius:50px;padding:7px 13px;font-size:12px;font-weight:700;color:var(--tx);cursor:pointer;white-space:nowrap;transition:all .15s}
.fpill.on{background:var(--pkd);color:#fff;border-color:var(--pkd)}
/* RESULT */
#sr{align-items:center;padding:24px 18px;gap:18px;background:linear-gradient(160deg,#fff0f7,#fde8f1)}
.res-title{font-family:Georgia,serif;font-style:italic;font-size:44px;color:var(--pkd);text-align:center}
#res-img{border-radius:18px;box-shadow:0 12px 48px #f9a8c960;max-width:320px;width:100%}
.res-note{font-size:12px;color:#b07090;text-align:center;max-width:280px;line-height:1.6}
.res-btns{display:flex;gap:10px;flex-wrap:wrap;justify-content:center}
.btn-p{background:linear-gradient(135deg,var(--pkd),#f472b6);color:#fff;border:none;border-radius:50px;padding:13px 24px;font-weight:700;font-size:14px;cursor:pointer;box-shadow:0 4px 20px #f9a8c970}
.btn-s{background:#fff;color:var(--tx);border:2.5px solid var(--pkl);border-radius:50px;padding:13px 24px;font-weight:700;font-size:14px;cursor:pointer}
.btn-s:active{background:var(--pkl)}
</style>
</head>
<body>
<div class="flash" id="fl"></div>

<!-- WELCOME -->
<div class="scr on" id="sw">
  <span class="bow">🎀</span>
  <div><div class="logo-t">Blushbooth</div><div class="logo-s">By Gift</div></div>
  <div class="card">
    <h2>Welcome, Darling ✨</h2>
    <p>Your personal pink photo booth. Enter your name then choose a mode — camera opens automatically! 💕</p>
  </div>
  <div class="name-wrap">
    <label>✦ Your Name on Photos ✦</label>
    <input class="name-in" id="uname" type="text" placeholder="Gift" maxlength="20" value="Gift">
  </div>
  <div class="mode-grid">
    <div class="mode-card" onclick="startMode('strip')"><span class="mi">🎞️</span><div class="mn">Photo Strip</div><div class="md">4 shots stacked</div></div>
    <div class="mode-card" onclick="startMode('single')"><span class="mi">📸</span><div class="mn">Single Photo</div><div class="md">One framed shot</div></div>
    <div class="mode-card" onclick="startMode('gif')"><span class="mi">✨</span><div class="mn">GIF Grid</div><div class="md">4 rapid shots 2×2</div></div>
  </div>
  <div class="pearls"><div class="pearl"></div><div class="pearl"></div><div class="pearl"></div><span style="color:#d8c6f0;font-size:13px;padding:0 4px">♡</span><div class="pearl"></div><div class="pearl"></div><div class="pearl"></div></div>
</div>

<!-- CAMERA -->
<div class="scr" id="sc">
  <div class="cam-hdr">
    <button class="back-btn" onclick="goBack()">← Back</button>
    <div class="cam-title" id="ctitle">Photo Strip 🎞️</div>
    <div style="width:60px"></div>
  </div>
  <div class="err-box" id="errbox" style="display:none">
    <h4>📷 Camera access needed</h4>
    <p id="errmsg"></p>
    <button class="btn-p" style="margin-top:10px;font-size:13px" onclick="startCam()">🔄 Try Again</button>
  </div>
  <!-- Strip -->
  <div id="lay-strip" class="strip-wrap" style="display:none">
    <div class="strip-thumbs" id="strip-thumbs">
      <div class="thumb" id="t0">Shot 1</div>
      <div class="thumb" id="t1">Shot 2</div>
      <div class="thumb" id="t2">Shot 3</div>
      <div class="thumb" id="t3">Shot 4</div>
    </div>
    <div class="strip-live">
      <div class="vid-wrap"><video id="v-strip" autoplay playsinline muted></video></div>
      <div class="cdown" id="cd-strip" style="display:none">3</div>
      <div class="hint" id="hint-strip">Tap 📸 to take shot 1 of 4</div>
      <button class="shutter" id="shr-strip" onclick="doStrip()">📸</button>
    </div>
  </div>
  <!-- Single -->
  <div id="lay-single" style="display:none;flex-direction:column;align-items:center;gap:14px;width:100%;max-width:640px">
    <div class="single-wrap"><video id="v-single" autoplay playsinline muted></video></div>
  </div>
  <!-- GIF -->
  <div id="lay-gif" style="display:none;flex-direction:column;align-items:center;gap:14px;width:100%;max-width:640px">
    <div class="gif-grid" id="gif-thumbs">
      <div class="gif-thumb" id="g0"></div><div class="gif-thumb" id="g1"></div>
      <div class="gif-thumb" id="g2"></div><div class="gif-thumb" id="g3"></div>
    </div>
    <div class="single-wrap" style="max-width:200px"><video id="v-gif" autoplay playsinline muted></video><div class="gif-badge">GIF GRID</div></div>
    <div class="hint" id="hint-gif">Tap 📸 to start 4-shot sequence</div>
  </div>
  <div class="cdown" id="cd-main" style="display:none">3</div>
  <div class="controls">
    <div id="shr-wrap"><button class="shutter" id="shr-main" onclick="doMain()">📸</button></div>
    <div class="filter-label">Choose a Filter</div>
    <div class="filter-row" id="frow">
      <div class="fpill on" onclick="setF(this,'none')">✨ Original</div>
      <div class="fpill" onclick="setF(this,'pink')">🩷 Pinky</div>
      <div class="fpill" onclick="setF(this,'bw')">🤍 B&W</div>
      <div class="fpill" onclick="setF(this,'warm')">🧡 Warm</div>
      <div class="fpill" onclick="setF(this,'cool')">💙 Cool</div>
      <div class="fpill" onclick="setF(this,'soft')">🌸 Soft</div>
      <div class="fpill" onclick="setF(this,'vintage')">📷 Vintage</div>
    </div>
  </div>
</div>

<!-- RESULT -->
<div class="scr" id="sr">
  <div class="res-title">So Cute! 🎀</div>
  <div class="pearls"><div class="pearl"></div><div class="pearl"></div><div class="pearl"></div><span style="color:var(--pk);font-size:13px;padding:0 4px">✦</span><div class="pearl"></div><div class="pearl"></div><div class="pearl"></div></div>
  <img id="res-img" src="" alt="result">
  <p class="res-note">Tap <strong>Save Photo</strong> to download. Tap <strong>Retake</strong> to shoot again.</p>
  <div class="res-btns">
    <button class="btn-p" onclick="savePhoto()">💾 Save Photo</button>
    <button class="btn-s" onclick="retake()">🔄 Retake</button>
    <button class="btn-s" onclick="goHome()">🏠 Home</button>
  </div>
</div>

<script>
var mode='strip', flt='none', stream=null, caps=[], busy=false;
var fmap={none:'none',pink:'sepia(30%) saturate(150%) hue-rotate(300deg) brightness(1.05)',bw:'grayscale(100%) contrast(110%)',warm:'sepia(40%) saturate(120%) brightness(1.05)',cool:'hue-rotate(180deg) saturate(80%) brightness(1.05)',soft:'brightness(1.08) contrast(90%) saturate(90%)',vintage:'sepia(60%) contrast(90%) brightness(.95) saturate(80%)'};

function show(id){['sw','sc','sr'].forEach(function(s){var el=document.getElementById(s);el.classList.remove('on');el.style.display='none';});var t=document.getElementById(id);t.classList.add('on');t.style.display='flex';}
function name(){return document.getElementById('uname').value.trim()||'Gift';}
function sleep(ms){return new Promise(function(r){setTimeout(r,ms);});}

function doFlash(){var f=document.getElementById('fl');f.classList.add('go');setTimeout(function(){f.classList.remove('go');},180);}

async function startCam(){
  document.getElementById('errbox').style.display='none';
  var vid=document.getElementById('v-'+mode);
  if(stream){stream.getTracks().forEach(function(t){t.stop();});stream=null;}
  try{
    stream=await navigator.mediaDevices.getUserMedia({video:{facingMode:'user',width:{ideal:1280},height:{ideal:960}},audio:false});
    vid.srcObject=stream;
    await vid.play();
  }catch(e){
    var msg='Camera permission denied.';
    if(e.name==='NotFoundError')msg='No camera found on this device.';
    else if(e.name==='NotAllowedError')msg='Permission denied.\n\nTo fix: Settings → Privacy & Security → Camera → turn ON Safari (or Chrome).';
    document.getElementById('errmsg').textContent=msg;
    document.getElementById('errbox').style.display='block';
  }
}

function stopCam(){if(stream){stream.getTracks().forEach(function(t){t.stop();});stream=null;}}

function startMode(m){
  mode=m; caps=[];
  ['lay-strip','lay-single','lay-gif'].forEach(function(id){document.getElementById(id).style.display='none';});
  document.getElementById('shr-wrap').style.display='flex';
  document.getElementById('cd-main').style.display='none';
  document.getElementById('errbox').style.display='none';
  var titles={strip:'Photo Strip 🎞️',single:'Single Photo 📸',gif:'GIF Grid ✨'};
  document.getElementById('ctitle').textContent=titles[m];
  if(m==='strip'){
    document.getElementById('lay-strip').style.display='flex';
    document.getElementById('shr-wrap').style.display='none';
    resetThumbs();
    document.getElementById('hint-strip').textContent='Tap 📸 to take shot 1 of 4';
  }else if(m==='single'){
    var sl=document.getElementById('lay-single');sl.style.display='flex';sl.style.flexDirection='column';sl.style.alignItems='center';
  }else{
    var gl=document.getElementById('lay-gif');gl.style.display='flex';gl.style.flexDirection='column';
    [0,1,2,3].forEach(function(i){var g=document.getElementById('g'+i);g.innerHTML='';g.style.background='var(--pkl)';});
    document.getElementById('hint-gif').textContent='Tap 📸 to start 4-shot sequence';
  }
  show('sc');
  startCam();
}

function resetThumbs(){[0,1,2,3].forEach(function(i){var t=document.getElementById('t'+i);t.innerHTML='Shot '+(i+1);t.style.border='2px solid var(--pkl)';});}

function setF(el,f){flt=f;document.querySelectorAll('.fpill').forEach(function(p){p.classList.remove('on');});el.classList.add('on');}

function capFrame(w,h){
  var vid=document.getElementById('v-'+mode);
  var c=document.createElement('canvas');c.width=w;c.height=h;
  var ctx=c.getContext('2d');
  ctx.translate(w,0);ctx.scale(-1,1);
  ctx.filter=fmap[flt]||'none';
  ctx.drawImage(vid,0,0,w,h);
  return c;
}

function drawName(ctx,nm,x,y,sz){
  ctx.save();ctx.font='italic bold '+sz+'px Georgia,serif';ctx.fillStyle='rgba(255,255,255,.9)';ctx.textAlign='center';ctx.shadowColor='rgba(0,0,0,.35)';ctx.shadowBlur=10;ctx.fillText(nm,x,y);ctx.restore();
}
function drawLabel(ctx,nm,cx,w,ly){
  var lb=ctx.createLinearGradient(0,ly,0,ly+68);lb.addColorStop(0,'#e87dab');lb.addColorStop(1,'#f472b6');
  ctx.fillStyle=lb;ctx.fillRect(0,ly,w,68);
  ctx.save();ctx.font='italic bold 22px Georgia,serif';ctx.fillStyle='#fff';ctx.textAlign='center';ctx.shadowColor='rgba(0,0,0,.2)';ctx.shadowBlur=6;ctx.fillText('Blushbooth',cx,ly+24);
  ctx.font='12px sans-serif';ctx.fillStyle='rgba(255,255,255,.85)';ctx.shadowBlur=0;ctx.fillText('By '+nm+'  ✦  🎀',cx,ly+48);ctx.restore();
}
function rr(ctx,x,y,w,h,r){ctx.beginPath();ctx.moveTo(x+r,y);ctx.lineTo(x+w-r,y);ctx.quadraticCurveTo(x+w,y,x+w,y+r);ctx.lineTo(x+w,y+h-r);ctx.quadraticCurveTo(x+w,y+h,x+w-r,y+h);ctx.lineTo(x+r,y+h);ctx.quadraticCurveTo(x,y+h,x,y+h-r);ctx.lineTo(x,y+r);ctx.quadraticCurveTo(x,y,x+r,y);ctx.closePath();}

async function countdownThen(elId,from,cb){
  var el=document.getElementById(elId);el.style.display='block';
  for(var i=from;i>=1;i--){el.textContent=i;await sleep(1000);}
  el.style.display='none';doFlash();await sleep(80);cb();
}

// Strip
async function doStrip(){
  if(busy)return;var next=caps.length;if(next>=4)return;
  busy=true;
  document.getElementById('shr-strip').style.display='none';
  await countdownThen('cd-strip',3,function(){
    var c=capFrame(480,360);caps.push(c);
    var t=document.getElementById('t'+next);t.innerHTML='';
    var img=document.createElement('img');img.src=c.toDataURL('image/jpeg',.9);t.appendChild(img);
    var ck=document.createElement('span');ck.className='ck';ck.textContent='✅';t.appendChild(ck);
    t.style.border='2px solid var(--pkd)';
  });
  busy=false;
  var rem=4-caps.length;
  if(rem>0){
    document.getElementById('hint-strip').textContent=rem+' shot'+(rem>1?'s':'')+' remaining — tap to continue';
    document.getElementById('shr-strip').style.display='flex';
  }else{
    document.getElementById('hint-strip').textContent='Building your strip... ✨';
    await sleep(300);buildStrip();
  }
}

function buildStrip(){
  var nm=name(),fw=320,fh=240,pad=18,gap=9,lh=70;
  var tw=fw+pad*2,th=pad+4*fh+3*gap+pad+lh;
  var rc=document.createElement('canvas');rc.width=tw;rc.height=th;
  var ctx=rc.getContext('2d');
  var bg=ctx.createLinearGradient(0,0,0,th);bg.addColorStop(0,'#fff0f7');bg.addColorStop(1,'#fde8f1');
  ctx.fillStyle=bg;rr(ctx,0,0,tw,th,20);ctx.fill();
  ctx.strokeStyle='#f9a8c9';ctx.lineWidth=3;rr(ctx,2,2,tw-4,th-4,18);ctx.stroke();
  ctx.fillStyle='#f9a8c918';for(var x=10;x<tw;x+=22)for(var y=10;y<th;y+=22){ctx.beginPath();ctx.arc(x,y,1.5,0,Math.PI*2);ctx.fill();}
  caps.forEach(function(c,i){var y=pad+i*(fh+gap);ctx.save();rr(ctx,pad,y,fw,fh,10);ctx.clip();ctx.drawImage(c,pad,y,fw,fh);ctx.restore();ctx.strokeStyle='#e8c0d8';ctx.lineWidth=2;rr(ctx,pad,y,fw,fh,10);ctx.stroke();drawName(ctx,nm,pad+fw-55,y+fh-14,18);});
  drawLabel(ctx,nm,tw/2,tw,th-lh);
  showResult(rc.toDataURL('image/jpeg',.95));
}

// Single
async function doSingle(){
  if(busy)return;busy=true;
  document.getElementById('shr-main').style.display='none';
  await countdownThen('cd-main',3,function(){caps=[capFrame(600,800)];});
  busy=false;buildSingle();
}
function buildSingle(){
  var nm=name(),src=caps[0],pad=20,lh=68;
  var w=src.width+pad*2,h=src.height+pad*2+lh;
  var rc=document.createElement('canvas');rc.width=w;rc.height=h;
  var ctx=rc.getContext('2d');
  var bg=ctx.createLinearGradient(0,0,0,h);bg.addColorStop(0,'#fff0f7');bg.addColorStop(1,'#fde8f1');
  ctx.fillStyle=bg;rr(ctx,0,0,w,h,24);ctx.fill();
  ctx.strokeStyle='#f9a8c9';ctx.lineWidth=3;rr(ctx,2,2,w-4,h-4,22);ctx.stroke();
  ctx.save();rr(ctx,pad,pad,src.width,src.height,14);ctx.clip();ctx.drawImage(src,pad,pad);ctx.restore();
  ctx.strokeStyle='#e8c0d8';ctx.lineWidth=2;rr(ctx,pad,pad,src.width,src.height,14);ctx.stroke();
  drawName(ctx,nm,w/2,pad+src.height-22,28);
  ctx.font='20px serif';ctx.fillText('🎀',pad-2,pad+6);ctx.fillText('🎀',w-pad-18,pad+6);
  drawLabel(ctx,nm,w/2,w,h-lh);
  showResult(rc.toDataURL('image/jpeg',.95));
}

// GIF Grid
async function doGif(){
  if(busy)return;busy=true;caps=[];
  document.getElementById('shr-main').style.display='none';
  for(var i=0;i<4;i++){
    await countdownThen('cd-main',2,function(){
      var c=capFrame(400,533);caps.push(c);
      var g=document.getElementById('g'+(caps.length-1));
      g.innerHTML='';var img=document.createElement('img');img.src=c.toDataURL('image/jpeg',.9);g.appendChild(img);
    });
    document.getElementById('hint-gif').textContent='Shot '+caps.length+' of 4 captured!';
    await sleep(200);
  }
  busy=false;document.getElementById('hint-gif').textContent='Building grid... ✨';await sleep(300);buildGif();
}
function buildGif(){
  var nm=name(),fw=200,fh=266,pad=14,gap=8,lh=60;
  var w=pad+2*(fw+gap)-gap+pad,h=pad+2*(fh+gap)-gap+pad+lh;
  var rc=document.createElement('canvas');rc.width=w;rc.height=h;
  var ctx=rc.getContext('2d');
  var bg=ctx.createLinearGradient(0,0,0,h);bg.addColorStop(0,'#d8c6f0');bg.addColorStop(1,'#fde8f1');
  ctx.fillStyle=bg;rr(ctx,0,0,w,h,20);ctx.fill();
  ctx.strokeStyle='#c6eae0';ctx.lineWidth=3;rr(ctx,2,2,w-4,h-4,18);ctx.stroke();
  caps.slice(0,4).forEach(function(c,i){var col=i%2,row=Math.floor(i/2),x=pad+col*(fw+gap),y=pad+row*(fh+gap);ctx.save();rr(ctx,x,y,fw,fh,10);ctx.clip();ctx.drawImage(c,x,y,fw,fh);ctx.restore();ctx.strokeStyle='#d8c6f0';ctx.lineWidth=2;rr(ctx,x,y,fw,fh,10);ctx.stroke();drawName(ctx,nm,x+fw/2,y+fh-10,16);});
  drawLabel(ctx,nm,w/2,w,h-lh);
  showResult(rc.toDataURL('image/jpeg',.95));
}

function doMain(){if(mode==='single')doSingle();else if(mode==='gif')doGif();}

function showResult(url){
  stopCam();
  document.getElementById('res-img').src=url;
  show('sr');
}
function savePhoto(){
  var url=document.getElementById('res-img').src;
  var a=document.createElement('a');a.download='blushbooth-'+name().toLowerCase()+'-'+mode+'-'+Date.now()+'.jpg';a.href=url;a.click();
}
function goBack(){stopCam();show('sw');}
function goHome(){stopCam();caps=[];show('sw');}
function retake(){caps=[];startMode(mode);}
</script>
</body>
</html>
