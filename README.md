# PARSA_Plus
PARSA PLUS Official Website

<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>PARSA PLUS</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Vazirmatn:wght@400;500;600;700;800;900&display=swap');

:root{
 --bg:#080b16;--panel:#11182a;--blue:#2787ff;
 --purple:#853cff;--gold:#efbd51;--text:#f4f6ff;
 --muted:#9ba8c0;--border:#293650;
}
*{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--text);font-family:Vazirmatn,Tahoma,sans-serif}
header{position:sticky;top:0;z-index:20;background:#090e1bf2;backdrop-filter:blur(15px);border-bottom:1px solid var(--border);padding:13px 4%;display:flex;align-items:center;justify-content:space-between;gap:12px;flex-wrap:wrap}
.logo{font-size:24px;font-weight:900;color:#61aaff}
.logo span{color:#a477ff}
nav{display:flex;gap:6px;flex-wrap:wrap}
button,.btn{font-family:inherit;cursor:pointer;border:0;border-radius:10px;padding:10px 14px;color:white;background:#263653;font-weight:700}
button:hover{filter:brightness(1.2)}
button:disabled{opacity:.55;cursor:not-allowed}
.primary{background:linear-gradient(110deg,var(--blue),var(--purple))}
.gold{background:linear-gradient(110deg,#a87817,#e8bd50);color:#17120a}
.danger{background:#922d49}
.container{width:min(1120px,93%);margin:auto}
.tab{display:none}.tab.active{display:block}
.hero{margin:30px auto;padding:65px 20px;text-align:center;border:1px solid #34446a;border-radius:24px;background:radial-gradient(ellipse at top,#193c70,#171b3b 50%,#101426)}
.hero h1{font-size:clamp(36px,7vw,65px);margin:5px}
.hero h1 span{color:#63aaff}
.hero p{line-height:2;color:#c3cce0}
.section{margin:35px auto}
h2{font-size:25px}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:16px}
.card{background:var(--panel);border:1px solid var(--border);border-radius:16px;padding:18px;overflow:hidden}
.card h3{margin:8px 0}
.thumb{height:145px;border-radius:12px;background:linear-gradient(135deg,#183c76,#512c87);display:grid;place-items:center;font-size:45px;margin-bottom:12px}
.muted{color:var(--muted);font-size:13px;line-height:1.9}
.badge{display:inline-block;padding:4px 10px;border-radius:20px;background:#263d67;color:#b8d7ff;font-size:12px}
.coin{color:var(--gold);font-weight:900}
.wallet{background:linear-gradient(135deg,#152f54,#34235b);border:1px solid #5365a1}
.wallet-number{font-size:36px;font-weight:900;color:var(--gold);direction:ltr;text-align:right}
input,textarea,select{width:100%;padding:12px;margin:7px 0 14px;border-radius:10px;border:1px solid var(--border);background:#0b1120;color:white;font-family:inherit;outline:none}
input:focus,textarea:focus{border-color:var(--blue)}
textarea{min-height:95px;resize:vertical}
label{font-size:14px;color:#cbd5e8}
.form{max-width:550px}
.hidden{display:none!important}
.actions{display:flex;gap:8px;flex-wrap:wrap;margin-top:12px}
.notice{background:#172b48;border:1px solid #315b8a;padding:13px;border-radius:12px;line-height:1.9;margin:15px 0;font-size:13px}
.row{display:flex;justify-content:space-between;align-items:center;gap:10px}
.rank{border-color:#59429b}
.price{font-size:25px;color:#b49aff;font-weight:900}
.leader{display:flex;align-items:center;justify-content:space-between;padding:13px;border-bottom:1px solid var(--border);gap:10px}
.leader:last-child{border:0}
.leader-left{display:flex;align-items:center;gap:12px}
.medal{font-size:23px}
.lucky-box{
 background:radial-gradient(ellipse at top,#49318c,#172348 55%,#101426);
 border:1px solid #8161d2;border-radius:24px;
 padding:30px 18px;text-align:center;
 box-shadow:0 0 35px #713cff22;
}
.gift{
 font-size:100px;display:block;
 filter:drop-shadow(0 0 20px #c69aff);
 animation:float 2s ease-in-out infinite;
}
@keyframes float{0%,100%{transform:translateY(0) rotate(-3deg)}50%{transform:translateY(-12px) rotate(3deg)}}
.lucky-title{font-size:30px;color:#e0c6ff;font-weight:900}
.prize-result{
 display:none;margin:20px auto;padding:20px;
 border:1px solid #9272d8;background:#171a37;
 border-radius:17px;max-width:420px;
}
.prize-result.show{display:block;animation:appear .4s ease}
@keyframes appear{from{opacity:0;transform:scale(.8)}to{opacity:1;transform:scale(1)}}
.prize-emoji{font-size:65px}
.probability{display:grid;grid-template-columns:repeat(3,1fr);gap:10px;margin-top:20px}
.probability .card{text-align:center;padding:12px}
footer{margin-top:60px;padding:30px;text-align:center;border-top:1px solid var(--border);color:var(--muted)}
a{color:#8ebeff}
@media(max-width:650px){
 header{justify-content:center}
 nav{justify-content:center}
 .hero{padding:40px 12px}
 .probability{grid-template-columns:1fr}
}
</style>
</head>
<body>

<header>
 <div class="logo">PARSA <span>PLUS</span></div>
 <nav>
  <button onclick="showTab('home')">خانه</button>
  <button onclick="showTab('videos')">ویدیوها</button>
  <button onclick="showTab('wallet')">کیف پول 💎</button>
  <button onclick="showTab('missions')">مأموریت‌ها</button>
  <button onclick="showTab('lucky')">جعبه شانس 🎁</button>
  <button onclick="showTab('leaderboard')">برترین‌ها</button>
  <button onclick="showTab('ranks')">فروشگاه</button>
  <button onclick="showTab('support')">پشتیبانی</button>
  <button onclick="showTab('account')">حساب من</button>
 </nav>
</header>

<main class="container">

<!-- HOME -->
<section id="home" class="tab active">
 <div class="hero">
  <span class="badge">WELCOME TO PARSA PLUS</span>
  <h1>دنیای <span>پارسا پلاس</span></h1>
  <p>ویدیوها، چالش‌ها، مأموریت‌ها و رقابت برای کسب PLUS COIN</p>
  <button class="primary" onclick="showTab('lucky')">بازکردن جعبه شانس 🎁</button>
  <button class="gold" onclick="showTab('wallet')">کیف پول من 💎</button>
 </div>

 <div class="section grid">
  <div class="card wallet">
   <div class="muted">موجودی کیف پول من</div>
   <div class="wallet-number" id="homeCoins">0 PC</div>
   <button class="gold" onclick="showTab('wallet')">مشاهده کیف پول</button>
  </div>
  <div class="card">
   <div class="muted">مأموریت‌های انجام‌شده</div>
   <h2 id="homeMissions">0</h2>
   <button onclick="showTab('missions')">مأموریت‌ها</button>
  </div>
  <div class="card">
   <div class="muted">رنک من</div>
   <h2 id="homeRank">کاربر عادی</h2>
   <button onclick="showTab('account')">پروفایل</button>
  </div>
 </div>

 <div class="section">
  <h2>✨ امکانات پارسا پلاس</h2>
  <div class="grid">
   <div class="card"><div class="thumb">🎬</div><h3>ویدیوها</h3><p class="muted">تماشای ویدیوهای کانال</p><button onclick="showTab('videos')">مشاهده</button></div>
   <div class="card"><div class="thumb">💎</div><h3>PLUS COIN</h3><p class="muted">کیف پول و تراکنش‌ها</p><button onclick="showTab('wallet')">ورود</button></div>
   <div class="card"><div class="thumb">🎁</div><h3>جعبه شانس</h3><p class="muted">هر روز یک جایزه شانسی</p><button onclick="showTab('lucky')">باز کردن</button></div>
  </div>
 </div>
</section>

<!-- LUCKY BOX -->
<section id="lucky" class="tab section">
 <h2>🎁 PLUS LUCKY BOX</h2>
 <p class="muted">هر روز یک جعبه شانس رایگان برای هر کاربر!</p>

 <div class="lucky-box">
  <div class="lucky-title">PLUS LUCKY BOX</div>
  <span class="gift" id="giftEmoji">🎁</span>
  <h3>شانس امروزت رو امتحان کن!</h3>
  <p class="muted">شاید برنده یک جایزه فوق‌العاده بشی...</p>
  <button class="gold" id="openBoxBtn" onclick="openLuckyBox()">باز کردن جعبه شانس</button>
  <p id="boxStatus" class="muted">برای باز کردن جعبه وارد حساب کاربری شو.</p>

  <div id="prizeResult" class="prize-result">
   <div class="prize-emoji" id="prizeEmoji">🎉</div>
   <h2 id="prizeTitle">جایزه تو!</h2>
   <p id="prizeDescription"></p>
  </div>
 </div>

 <div class="section">
  <h2>🎯 جوایز احتمالی</h2>
  <div class="probability">
   <div class="card">
    <div class="prize-emoji">💎</div>
    <h3 class="coin">۱ تا ۶۰ کوین</h3>
    <p class="muted">احتمال ۹۴٪</p>
   </div>
   <div class="card">
    <div class="prize-emoji">🍌</div>
    <h3>موز کلکسیونی</h3>
    <p class="muted">احتمال ۵٪</p>
   </div>
   <div class="card">
    <div class="prize-emoji">👑</div>
    <h3>بهترین رنک سایت</h3>
    <p class="muted">۵ روز رایگان • احتمال ۱٪</p>
   </div>
  </div>
 </div>

 <div class="card section">
  <h3>📜 تاریخچه جعبه‌های من</h3>
  <div id="luckyHistory" class="muted">برای مشاهده وارد حساب شو.</div>
 </div>
</section>

<!-- VIDEOS -->
<section id="videos" class="tab section">
 <h2>🎬 ویدیوهای پارسا پلاس</h2>
 <input id="videoSearch" placeholder="جست‌وجوی ویدیو..." oninput="renderVideos()">
 <div id="videoList" class="grid"></div>
 <div class="card section">
  <h3>➕ افزودن ویدیو</h3>
  <label>عنوان</label><input id="vTitle" placeholder="عنوان ویدیو">
  <label>توضیحات</label><textarea id="vDesc"></textarea>
  <label>لینک آپارات یا ویدیو</label><input id="vUrl" placeholder="https://...">
  <label>تصویر بندانگشتی</label><input id="vImage" placeholder="https://...">
  <label>یا انتخاب فایل ویدیو (حداکثر ۲ مگابایت)</label>
  <input id="vFile" type="file" accept="video/*">
  <button class="primary" onclick="addVideo()">ثبت ویدیو</button>
 </div>
</section>

<!-- WALLET -->
<section id="wallet" class="tab section">
 <h2>💎 کیف پول PLUS COIN</h2>
 <div class="card wallet">
  <div class="muted">موجودی فعلی شما</div>
  <div class="wallet-number" id="walletBalance">0 PC</div>
 </div>
 <div class="grid section">
  <div class="card"><div class="muted">کل کوین دریافتی</div><h2 class="coin" id="totalEarned">0 PC</h2></div>
  <div class="card"><div class="muted">کل کوین خرج‌شده</div><h2 id="totalSpent">0 PC</h2></div>
  <div class="card"><div class="muted">رتبه ثروت</div><h2 id="walletRank">-</h2></div>
 </div>
 <div class="card section">
  <h3>📜 تاریخچه تراکنش‌ها</h3>
  <div id="transactions"></div>
 </div>
</section>

<!-- MISSIONS -->
<section id="missions" class="tab section">
 <h2>🎯 مأموریت‌ها و چالش‌ها</h2>
 <p class="muted">مأموریت انجام بده و PLUS COIN دریافت کن!</p>
 <div id="missionList" class="grid"></div>
</section>

<!-- LEADERBOARD -->
<section id="leaderboard" class="tab section">
 <h2>🏆 جدول ثروتمندان</h2>
 <div class="card"><div id="leaderList"></div></div>
</section>

<!-- RANKS -->
<section id="ranks" class="tab section">
 <h2>🎖️ فروشگاه رنک</h2>
 <div class="grid">
  <div class="card rank"><span class="badge">BRONZE</span><h3>رنک برنزی</h3><div class="price">500 PC</div><button class="primary" onclick="buyRank('برنزی',500)">خرید</button></div>
  <div class="card rank"><span class="badge">SILVER</span><h3>رنک نقره‌ای</h3><div class="price">1200 PC</div><button class="primary" onclick="buyRank('نقره‌ای',1200)">خرید</button></div>
  <div class="card rank"><span class="badge">GOLD</span><h3>رنک طلایی</h3><div class="price">2500 PC</div><button class="gold" onclick="buyRank('طلایی',2500)">خرید</button></div>
 </div>
 <div class="card section"><h3>سفارش‌های من</h3><div id="myOrders"></div></div>
</section>

<!-- SUPPORT -->
<section id="support" class="tab section">
 <h2>🎫 پشتیبانی</h2>
 <div class="card form">
  <label>موضوع</label><input id="tSubject" placeholder="موضوع تیکت">
  <label>دسته‌بندی</label>
  <select id="tCategory">
   <option>حساب کاربری</option><option>خرید رنک</option>
   <option>PLUS COIN</option><option>جعبه شانس</option><option>مشکل سایت</option><option>سایر</option>
  </select>
  <label>پیام</label><textarea id="tMessage" placeholder="پیام خود را بنویس..."></textarea>
  <button class="primary" onclick="sendTicket()">ارسال تیکت</button>
 </div>
 <div class="section"><h3>تیکت‌های من</h3><div id="myTickets" class="grid"></div></div>
</section>

<!-- ACCOUNT -->
<section id="account" class="tab section">
 <h2>👤 حساب کاربری</h2>
 <div id="loggedOut" class="grid">
  <div class="card form">
   <h3>ورود</h3>
   <input id="loginEmail" type="email" placeholder="ایمیل">
   <input id="loginPass" type="password" placeholder="رمز عبور">
   <button class="primary" onclick="login()">ورود</button>
  </div>
  <div class="card form">
   <h3>ثبت‌نام</h3>
   <input id="regName" placeholder="نام نمایشی">
   <input id="regEmail" type="email" placeholder="ایمیل">
   <input id="regPass" type="password" placeholder="رمز عبور">
   <button class="primary" onclick="register()">ساخت حساب و کیف پول</button>
  </div>
 </div>
 <div id="loggedIn" class="card hidden">
  <h3>خوش آمدی، <span id="userName"></span>! 👋</h3>
  <p id="userEmail" class="muted"></p>
  <p>موجودی: <strong class="coin" id="accountCoins">0 PC</strong></p>
  <p>موزهای کلکسیونی: <strong id="accountBananas">0 🍌</strong></p>
  <p>وضعیت رنک ویژه: <strong id="accountRank">کاربر عادی</strong></p>
  <div class="actions">
   <button onclick="showTab('wallet')">کیف پول</button>
   <button onclick="showTab('missions')">مأموریت‌ها</button>
   <button onclick="showTab('lucky')">جعبه شانس</button>
   <button onclick="showTab('support')">تیکت‌ها</button>
   <button class="danger" onclick="logout()">خروج</button>
  </div>
 </div>
 <div class="notice">این نسخه آزمایشی است و اطلاعات فقط در مرورگر ذخیره می‌شود. برای استفاده واقعی به سرور نیاز است.</div>
</section>

</main>

<footer>
 <div class="logo">PARSA <span>PLUS</span></div>
 <p>PLUS COIN • LUCKY BOX • VIDEO • COMMUNITY</p>
 <p>© 2026 PARSA PLUS</p>
</footer>

<script>
const get=k=>JSON.parse(localStorage.getItem(k)||"[]");
const save=(k,v)=>localStorage.setItem(k,JSON.stringify(v));
let currentUser=localStorage.getItem("pp_session")||null;

const missions=[
 {id:"m1",title:"اولین ورود",desc:"حساب کاربری خود را بساز و وارد شو.",reward:100,icon:"👤"},
 {id:"m2",title:"تماشاگر پارسا پلاس",desc:"یکی از ویدیوهای کانال را تماشا کن.",reward:150,icon:"🎬"},
 {id:"m3",title:"کاوشگر سایت",desc:"از بخش‌های مختلف سایت بازدید کن.",reward:100,icon:"🧭"},
 {id:"m4",title:"ارسال پیشنهاد",desc:"یک پیشنهاد مفید در بخش پشتیبانی ارسال کن.",reward:200,icon:"💡"},
 {id:"m5",title:"طرفدار واقعی",desc:"چهار مأموریت دیگر را انجام بده.",reward:500,icon:"🏆"}
];

function allUsers(){return get("pp_users")}
function user(){return allUsers().find(u=>u.email===currentUser)}
function balance(){return user()?.coins||0}
function safe(v){const d=document.createElement("div");d.textContent=String(v??"");return d.innerHTML}
function today(){return new Date().toLocaleDateString("en-CA")}
function requireLogin(){
 if(!user()){alert("ابتدا وارد حساب کاربری شو.");showTab("account");return false}
 return true;
}

function updateUser(email,fn){
 const users=allUsers(),u=users.find(x=>x.email===email);
 if(!u)return;
 fn(u);save("pp_users",users);
}
function addTransaction(email,amount,reason){
 updateUser(email,u=>{
  u.coins=(u.coins||0)+amount;
  u.transactions=u.transactions||[];
  u.earned=u.earned||0;u.spent=u.spent||0;
  if(amount>0)u.earned+=amount;else u.spent+=Math.abs(amount);
  u.transactions.unshift({amount,reason,date:new Date().toLocaleDateString("fa-IR")});
 });
}
function rankPosition(){
 return allUsers().sort((a,b)=>(b.coins||0)-(a.coins||0))
 .findIndex(u=>u.email===currentUser)+1;
}
function rankActive(){
 return !!user()&&user().bestRankUntil>Date.now();
}
function rankRemaining(){
 if(!rankActive())return 0;
 return Math.ceil((user().bestRankUntil-Date.now())/86400000);
}

function showTab(id){
 document.querySelectorAll(".tab").forEach(x=>x.classList.remove("active"));
 document.getElementById(id).classList.add("active");
 if(id==="account")renderAccount();
 if(id==="wallet")renderWallet();
 if(id==="missions")renderMissions();
 if(id==="leaderboard")renderLeaderboard();
 if(id==="videos")renderVideos();
 if(id==="support")renderTickets();
 if(id==="ranks")renderOrders();
 if(id==="lucky")renderLucky();
 window.scrollTo({top:0,behavior:"smooth"});
}

function register(){
 const name=document.getElementById("regName").value.trim();
 const email=document.getElementById("regEmail").value.trim().toLowerCase();
 const pass=document.getElementById("regPass").value;
 if(!name||!email||!pass)return alert("تمام فیلدها را پر کن.");
 if(pass.length<6)return alert("رمز باید حداقل ۶ کاراکتر باشد.");
 if(!email.includes("@"))return alert("ایمیل معتبر وارد کن.");
 const users=allUsers();
 if(users.some(u=>u.email===email))return alert("این ایمیل قبلاً ثبت شده.");
 users.push({
  name,email,pass,coins:0,claimed:[],transactions:[],
  earned:0,spent:0,bananas:0,luckyHistory:[],
  lastLuckyDate:null,bestRankUntil:0
 });
 save("pp_users",users);
 currentUser=email;localStorage.setItem("pp_session",email);
 alert("حساب و کیف پول PLUS COIN ساخته شد! 💎");
 refresh();
}
function login(){
 const email=document.getElementById("loginEmail").value.trim().toLowerCase();
 const pass=document.getElementById("loginPass").value;
 const u=allUsers().find(x=>x.email===email&&x.pass===pass);
 if(!u)return alert("ایمیل یا رمز اشتباه است.");
 currentUser=email;localStorage.setItem("pp_session",email);
 alert("خوش آمدی!");refresh();
}
function logout(){
 currentUser=null;localStorage.removeItem("pp_session");refresh();
}
function renderAccount(){
 const logged=!!user();
 document.getElementById("loggedOut").classList.toggle("hidden",logged);
 document.getElementById("loggedIn").classList.toggle("hidden",!logged);
 if(!logged)return;
 document.getElementById("userName").textContent=user().name;
 document.getElementById("userEmail").textContent=user().email;
 document.getElementById("accountCoins").textContent=balance()+" PC";
 document.getElementById("accountBananas").textContent=(user().bananas||0)+" 🍌";
 document.getElementById("accountRank").textContent=rankActive()?"👑 بهترین رنک • "+rankRemaining()+" روز باقی‌مانده":"کاربر عادی";
}
function updateHome(){
 document.getElementById("homeCoins").textContent=balance()+" PC";
 document.getElementById("homeMissions").textContent=user()?.claimed?.length||0;
 document.getElementById("homeRank").textContent=rankActive()?"👑 بهترین رنک":"کاربر عادی";
}
function refresh(){
 renderAccount();renderWallet();renderMissions();
 renderLeaderboard();renderVideos();renderTickets();
 renderOrders();renderLucky();updateHome();
}

function renderWallet(){
 const box=document.getElementById("transactions");
 if(!user()){
  document.getElementById("walletBalance").textContent="0 PC";
  document.getElementById("totalEarned").textContent="0 PC";
  document.getElementById("totalSpent").textContent="0 PC";
  document.getElementById("walletRank").textContent="-";
  box.textContent="برای مشاهده کیف پول وارد حساب شو.";return;
 }
 const u=user();
 document.getElementById("walletBalance").textContent=balance()+" PC";
 document.getElementById("totalEarned").textContent=(u.earned||0)+" PC";
 document.getElementById("totalSpent").textContent=(u.spent||0)+" PC";
 document.getElementById("walletRank").textContent="#"+rankPosition();
 box.innerHTML="";
 if(!u.transactions?.length){box.textContent="هنوز تراکنشی نداری.";return}
 u.transactions.forEach(t=>{
  const el=document.createElement("div");el.className="leader";
  const left=document.createElement("span");left.textContent=t.reason+" • "+t.date;
  const right=document.createElement("strong");
  right.style.color=t.amount>0?"#efbd51":"#ff8c9b";
  right.textContent=(t.amount>0?"+":"")+t.amount+" PC";
  el.append(left,right);box.append(el);
 });
}

function renderMissions(){
 const box=document.getElementById("missionList");box.innerHTML="";
 missions.forEach(m=>{
  const claimed=user()?.claimed?.includes(m.id);
  const el=document.createElement("div");el.className="card";
  const icon=document.createElement("div");icon.className="thumb";icon.textContent=m.icon;
  const h=document.createElement("h3");h.textContent=m.title;
  const p=document.createElement("p");p.className="muted";p.textContent=m.desc;
  const reward=document.createElement("p");reward.className="coin";reward.textContent="پاداش: "+m.reward+" PC";
  const btn=document.createElement("button");
  btn.textContent=claimed?"✓ دریافت شده":"ثبت انجام مأموریت";
  if(claimed)btn.disabled=true;
  else{btn.className="primary";btn.onclick=()=>claimMission(m.id)}
  el.append(icon,h,p,reward,btn);box.append(el);
 });
}
function claimMission(id){
 if(!requireLogin())return;
 const m=missions.find(x=>x.id===id);
 if(user().claimed?.includes(id))return alert("قبلاً دریافت شده.");
 if(id==="m5"&&(user().claimed||[]).length<4)return alert("ابتدا چهار مأموریت دیگر را انجام بده.");
 if(!confirm("آیا مأموریت را انجام داده‌ای؟"))return;
 updateUser(currentUser,u=>{u.claimed=u.claimed||[];u.claimed.push(id)});
 addTransaction(currentUser,m.reward,"پاداش مأموریت: "+m.title);
 alert(m.reward+" PLUS COIN دریافت کردی!");
 refresh();
}

function renderLeaderboard(){
 const box=document.getElementById("leaderList");box.innerHTML="";
 const users=allUsers().sort((a,b)=>(b.coins||0)-(a.coins||0));
 if(!users.length){box.textContent="هنوز کاربری ثبت‌نام نکرده است.";return}
 users.forEach((u,i)=>{
  const el=document.createElement("div");el.className="leader";
  const left=document.createElement("div");left.className="leader-left";
  const medal=document.createElement("span");medal.className="medal";
  medal.textContent=["🥇","🥈","🥉"][i]||"🏅";
  const name=document.createElement("strong");
  name.textContent=u.name+(u.email===currentUser?" (من)":"");
  left.append(medal,name);
  const amount=document.createElement("strong");amount.className="coin";
  amount.textContent=(u.coins||0)+" PC";
  el.append(left,amount);box.append(el);
 });
}

function openLuckyBox(){
 if(!requireLogin())return;
 const u=user(),date=today();
 if(u.lastLuckyDate===date)return alert("جعبه شانس امروزت را قبلاً باز کرده‌ای! فردا دوباره بیا.");
 if(!confirm("آماده‌ای جعبه شانس امروزت را باز کنی؟"))return;

 const roll=Math.random()*100;
 let prize={type:"coin",emoji:"💎",title:"جایزه کوین!",description:"",amount:0};
 if(roll<94){
  prize.amount=Math.floor(Math.random()*60)+1;
  prize.description="تبریک! "+prize.amount+" PLUS COIN برنده شدی!";
 }else if(roll<99){
  prize={type:"banana",emoji:"🍌",title:"موز کلکسیونی!",description:"یک موز ویژه به کلکسیونت اضافه شد!"};
 }else{
  prize={type:"rank",emoji:"👑",title:"جایزه فوق‌العاده!",description:"بهترین رنک سایت برای ۵ روز به تو تعلق گرفت!"};
 }

 updateUser(currentUser,x=>{
  x.lastLuckyDate=date;
  x.luckyHistory=x.luckyHistory||[];
  x.luckyHistory.unshift({
   title:prize.title,emoji:prize.emoji,
   description:prize.description,date:new Date().toLocaleDateString("fa-IR")
  });
  if(prize.type==="banana")x.bananas=(x.bananas||0)+1;
  if(prize.type==="rank"){
   const start=Math.max(Date.now(),x.bestRankUntil||0);
   x.bestRankUntil=start+5*24*60*60*1000;
  }
 });

 if(prize.type==="coin")addTransaction(currentUser,prize.amount,"جایزه جعبه شانس");
 showPrize(prize);
 renderLucky();refresh();
}

function showPrize(prize){
 document.getElementById("prizeEmoji").textContent=prize.emoji;
 document.getElementById("prizeTitle").textContent=prize.title;
 document.getElementById("prizeDescription").textContent=prize.description;
 document.getElementById("prizeResult").classList.add("show");
 document.getElementById("giftEmoji").textContent="✨";
}
function renderLucky(){
 const btn=document.getElementById("openBoxBtn");
 const status=document.getElementById("boxStatus");
 const history=document.getElementById("luckyHistory");
 const result=document.getElementById("prizeResult");
 if(!user()){
  btn.disabled=true;status.textContent="برای باز کردن جعبه وارد حساب کاربری شو.";
  history.textContent="برای مشاهده وارد حساب شو.";return;
 }
 const already=user().lastLuckyDate===today();
 btn.disabled=already;
 btn.textContent=already?"جعبه امروز باز شده":"باز کردن جعبه شانس";
 status.textContent=already?"جعبه امروزت را باز کرده‌ای؛ فردا برگرد!":"امروز یک شانس رایگان داری!";
 history.innerHTML="";
 result.classList.remove("show");
 const list=user().luckyHistory||[];
 if(!list.length){history.textContent="هنوز جعبه‌ای باز نکرده‌ای.";return}
 list.forEach(item=>{
  const el=document.createElement("div");el.className="leader";
  const a=document.createElement("span");
  a.textContent=item.emoji+" "+item.title+" • "+item.date;
  el.append(a);history.append(el);
 });
}

function buyRank(rank,cost){
 if(!requireLogin())return;
 if(balance()<cost)return alert("موجودی کافی نیست! مأموریت انجام بده یا جعبه شانس باز کن.");
 if(!confirm("خرید رنک "+rank+" با "+cost+" PC؟"))return;
 addTransaction(currentUser,-cost,"خرید رنک "+rank);
 const orders=get("pp_orders");
 orders.unshift({email:currentUser,rank,cost,status:"در انتظار بررسی مدیر",date:new Date().toLocaleDateString("fa-IR")});
 save("pp_orders",orders);
 alert("درخواست خرید ثبت شد!");
 refresh();
}
function renderOrders(){
 const box=document.getElementById("myOrders");box.innerHTML="";
 if(!user()){box.textContent="ابتدا وارد حساب شو.";return}
 const orders=get("pp_orders").filter(o=>o.email===currentUser);
 if(!orders.length){box.textContent="هنوز سفارشی نداری.";return}
 orders.forEach(o=>{
  const el=document.createElement("div");el.className="card";
  el.innerHTML="<h3>رنک "+safe(o.rank)+"</h3><p class='muted'>هزینه: "+o.cost+" PC | "+safe(o.date)+"</p><span class='badge'>"+safe(o.status)+"</span>";
  box.append(el);
 });
}

function renderVideos(){
 const box=document.getElementById("videoList");
 const search=(document.getElementById("videoSearch")?.value||"").toLowerCase();
 const videos=get("pp_videos").filter(v=>(v.title+" "+v.desc).toLowerCase().includes(search));
 box.innerHTML="";
 if(!videos.length){box.textContent="هنوز ویدیویی اضافه نشده است.";return}
 videos.forEach(v=>{
  const el=document.createElement("div");el.className="card";
  if(v.image){
   const img=document.createElement("img");img.src=v.image;
   img.style.width="100%";img.style.borderRadius="12px";el.append(img);
  }
  const h=document.createElement("h3");h.textContent=v.title;
  const p=document.createElement("p");p.className="muted";p.textContent=v.desc||"";
  el.append(h,p);
  if(v.url){
   const a=document.createElement("a");a.href=v.url;a.target="_blank";a.rel="noopener";
   a.className="btn primary";a.textContent="تماشای ویدیو";el.append(a);
  }
  if(v.file){
   const a=document.createElement("a");a.href=v.file;a.download=v.fileName||"video";
   a.className="btn";a.textContent="دریافت ویدیو";el.append(a);
  }
  box.append(el);
 });
}
function addVideo(){
 if(!requireLogin())return;
 const title=document.getElementById("vTitle").value.trim();
 const desc=document.getElementById("vDesc").value.trim();
 const url=document.getElementById("vUrl").value.trim();
 const image=document.getElementById("vImage").value.trim();
 const file=document.getElementById("vFile").files[0];
 if(!title)return alert("عنوان را وارد کن.");
 if(!url&&!file)return alert("لینک یا فایل ویدیو لازم است.");
 if(url&&!/^https?:\/\//i.test(url))return alert("لینک معتبر نیست.");
 if(image&&!/^https?:\/\//i.test(image))return alert("لینک تصویر معتبر نیست.");
 if(file&&file.size>2*1024*1024)return alert("فایل باید حداکثر ۲ مگابایت باشد.");
 const saveVideo=data=>{
  const videos=get("pp_videos");
  videos.unshift({title,desc,url,image,...data});
  save("pp_videos",videos);
  alert("ویدیو اضافه شد!");
  ["vTitle","vDesc","vUrl","vImage","vFile"].forEach(id=>document.getElementById(id).value="");
  renderVideos();
 };
 if(file){
  const reader=new FileReader();
  reader.onload=()=>saveVideo({file:reader.result,fileName:file.name});
  reader.readAsDataURL(file);
 }else saveVideo({});
}

function sendTicket(){
 if(!requireLogin())return;
 const subject=document.getElementById("tSubject").value.trim();
 const message=document.getElementById("tMessage").value.trim();
 const category=document.getElementById("tCategory").value;
 if(!subject||!message)return alert("موضوع و پیام را وارد کن.");
 const tickets=get("pp_tickets");
 tickets.unshift({id:Date.now(),email:currentUser,subject,message,category,status:"در انتظار پاسخ",date:new Date().toLocaleDateString("fa-IR")});
 save("pp_tickets",tickets);
 alert("تیکت ثبت شد.");
 document.getElementById("tSubject").value="";
 document.getElementById("tMessage").value="";
 renderTickets();
}
function renderTickets(){
 const box=document.getElementById("myTickets");
 if(!box)return;
 box.innerHTML="";
 if(!user()){box.textContent="برای مشاهده تیکت‌ها وارد شو.";return}
 const tickets=get("pp_tickets").filter(t=>t.email===currentUser);
 if(!tickets.length){box.textContent="هنوز تیکتی نداری.";return}
 tickets.forEach(t=>{
  const el=document.createElement("div");el.className="card";
  const h=document.createElement("h3");h.textContent=t.subject;
  const p=document.createElement("p");p.className="muted";p.textContent=t.category+" • "+t.date;
  const msg=document.createElement("p");msg.textContent=t.message;
  const b=document.createElement("span");b.className="badge";b.textContent=t.status;
  el.append(h,p,msg,b);box.append(el);
 });
}

renderAccount();
refresh();
</script>
</body>
</html>

