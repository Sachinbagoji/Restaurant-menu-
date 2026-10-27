<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Bagoji’s Dum House | Hyderabadi Biryani &amp; More</title>
<meta name="description" content="Hyderabadi dum biryani, kebabs, curries and sweets. Order online from Bagoji’s Dum House, Hyderabad.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Anton&family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<style>
:root{--red:#E3112B;--black:#0b0b0b;--white:#fff;--grey:#f4f4f4;--mid:#6b6b6b;--line:#e4e4e4;--d:"Anton","Impact",sans-serif;--b:"Inter",system-ui,sans-serif}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{font-family:var(--b);color:var(--black);background:var(--white);font-size:15px;line-height:1.5}
button,input,select{font:inherit;color:inherit}
button{cursor:pointer}
:focus-visible{outline:3px solid var(--red);outline-offset:2px}
.wrap{max-width:1360px;margin:0 auto;padding:0 28px}
.up{text-transform:uppercase}
h1,h2,h3{font-family:var(--d);font-weight:400;text-transform:uppercase;line-height:.95}

/* announcement + header */
.ann{background:var(--black);color:#fff;text-align:center;font-size:12px;font-weight:600;letter-spacing:.04em;padding:9px 12px;text-transform:uppercase}
header{position:sticky;top:0;z-index:30;background:#fff;border-bottom:1px solid var(--line)}
.bar{display:flex;align-items:center;gap:30px;height:68px}
.logo{font-family:var(--d);font-size:30px;text-transform:uppercase;text-decoration:none;letter-spacing:.01em;font-style:italic;white-space:nowrap}
.logo span{color:var(--red)}
nav{display:flex;gap:26px;flex:1}
nav a{font-weight:700;font-size:13px;text-transform:uppercase;text-decoration:none;padding:6px 0;border-bottom:3px solid transparent}
nav a:hover{border-color:var(--red)}
.icons{display:flex;gap:14px;align-items:center}
.cartbtn{background:var(--black);color:#fff;border:0;padding:11px 18px;font-weight:700;font-size:13px;text-transform:uppercase;display:flex;gap:10px;align-items:center}
.cartbtn:hover{background:var(--red)}
.cartbtn b{background:#fff;color:var(--black);min-width:22px;height:22px;border-radius:11px;display:grid;place-items:center;font-size:12px}
@media(max-width:800px){nav{display:none}.bar{justify-content:space-between}}

/* hero */
.hero{background:var(--black);color:#fff;position:relative;overflow:hidden}
.hero .wrap{display:grid;grid-template-columns:1.15fr 1fr;align-items:center;min-height:78vh;gap:20px;padding-top:50px;padding-bottom:50px}
.tag{display:inline-block;background:var(--red);font-weight:800;font-size:12px;padding:6px 12px;text-transform:uppercase;letter-spacing:.05em;margin-bottom:22px}
.hero h1{font-size:clamp(4.2rem,12.5vw,11.5rem);letter-spacing:-.005em}
.hero h1 em{font-style:normal;color:var(--red)}
.hero p{max-width:42ch;margin:24px 0 32px;color:#cfcfcf;font-size:17px}
.btns{display:flex;gap:12px;flex-wrap:wrap}
.btn{display:inline-block;padding:16px 34px;font-weight:800;font-size:13px;text-transform:uppercase;letter-spacing:.04em;text-decoration:none;border:2px solid #fff;background:#fff;color:#000;transition:.15s}
.btn:hover{background:var(--red);border-color:var(--red);color:#fff}
.btn.out{background:transparent;color:#fff}
.btn.out:hover{background:#fff;color:#000;border-color:#fff}
.btn.dark{background:#000;color:#fff;border-color:#000}
.btn.dark:hover{background:var(--red);border-color:var(--red)}
.art{display:grid;place-items:center;position:relative}
.art svg{width:min(100%,520px);height:auto}
.steam path{fill:none;stroke:#fff;stroke-width:5;stroke-linecap:round;opacity:.55;animation:rise 3.2s ease-in-out infinite}
.steam path:nth-child(2){animation-delay:.9s}.steam path:nth-child(3){animation-delay:1.8s}
@keyframes rise{0%{transform:translateY(14px);opacity:0}40%{opacity:.6}100%{transform:translateY(-22px);opacity:0}}
@media(max-width:900px){.hero .wrap{grid-template-columns:1fr;min-height:0}.art{order:-1;max-width:340px;margin:0 auto}}
@media(prefers-reduced-motion:reduce){*{animation:none!important;scroll-behavior:auto!important}}

/* ticker */
.ticker{background:var(--red);color:#fff;overflow:hidden;white-space:nowrap;padding:13px 0}
.ticker div{display:inline-block;font-family:var(--d);font-size:22px;text-transform:uppercase;animation:tick 28s linear infinite}
.ticker span{margin:0 26px}
@keyframes tick{to{transform:translateX(-50%)}}

section{padding:70px 0}
.head{display:flex;justify-content:space-between;align-items:flex-end;gap:20px;flex-wrap:wrap;margin-bottom:28px}
.head h2{font-size:clamp(2.4rem,6vw,4.6rem)}
.head p{color:var(--mid);max-width:44ch}

/* category tiles */
.tiles{display:grid;grid-template-columns:repeat(4,1fr);gap:12px}
.tile{background:var(--grey);border:0;text-align:left;padding:22px;min-height:300px;display:flex;flex-direction:column;justify-content:space-between;position:relative;overflow:hidden;transition:.2s}
.tile .em{font-size:96px;line-height:1;transition:.3s}
.tile h3{font-size:2.2rem}
.tile small{font-weight:700;text-transform:uppercase;font-size:11px;color:var(--mid);letter-spacing:.05em}
.tile:hover{background:var(--black);color:#fff}
.tile:hover small{color:#bbb}
.tile:hover .em{transform:scale(1.12) rotate(-6deg)}
@media(max-width:900px){.tiles{grid-template-columns:repeat(2,1fr)}.tile{min-height:220px}.tile .em{font-size:70px}}

/* toolbar */
.tools{display:flex;gap:12px;flex-wrap:wrap;align-items:center;margin-bottom:24px;padding-bottom:20px;border-bottom:1px solid var(--line)}
.chips{display:flex;gap:8px;flex-wrap:wrap;flex:1}
.chip{border:2px solid var(--black);background:#fff;padding:9px 16px;font-weight:700;font-size:12px;text-transform:uppercase}
.chip[aria-pressed="true"]{background:var(--black);color:#fff}
.tools input[type=search],.tools select{border:2px solid var(--line);padding:10px 14px;background:#fff;min-width:170px}
.tools input:focus,.tools select:focus{border-color:var(--black);outline:none}
.sw{display:flex;gap:8px;align-items:center;font-weight:700;font-size:12px;text-transform:uppercase;cursor:pointer}
.sw input{accent-color:#1b8a3a;width:18px;height:18px}

/* product grid */
.grid{display:grid;grid-template-columns:repeat(4,1fr);gap:26px 12px}
@media(max-width:1100px){.grid{grid-template-columns:repeat(3,1fr)}}
@media(max-width:780px){.grid{grid-template-columns:repeat(2,1fr)}.wrap{padding:0 16px}}
@media(max-width:460px){.grid{grid-template-columns:1fr}}
.card{display:flex;flex-direction:column}
.pic{background:var(--grey);aspect-ratio:1/1;display:grid;place-items:center;font-size:104px;position:relative;overflow:hidden}
.pic .e{transition:transform .35s}
.card:hover .e{transform:scale(1.1) rotate(-5deg)}
.badge{position:absolute;left:0;top:14px;background:var(--red);color:#fff;font-size:11px;font-weight:800;padding:5px 10px;text-transform:uppercase;letter-spacing:.04em;font-family:var(--b)}
.dot{position:absolute;right:12px;top:12px;width:16px;height:16px;border:2px solid;background:#fff}
.dot::after{content:"";position:absolute;inset:2px;border-radius:50%;background:currentColor}
.dot.v{color:#1b8a3a}.dot.n{color:#b3261e}
.quick{position:absolute;left:0;right:0;bottom:0;background:var(--black);color:#fff;border:0;padding:15px;font-weight:800;font-size:13px;text-transform:uppercase;transform:translateY(101%);transition:.22s}
.card:hover .quick,.quick:focus-visible{transform:none}
.quick:hover{background:var(--red)}
@media(hover:none){.quick{transform:none}}
.info{padding-top:12px}
.info h3{font-family:var(--b);font-weight:800;font-size:14px;line-height:1.3}
.info p{color:var(--mid);font-size:13px;margin:4px 0 8px}
.row{display:flex;justify-content:space-between;align-items:center;gap:10px}
.price{font-weight:800;font-size:16px}
.spice{border:1px solid var(--line);padding:5px 8px;font-size:12px;background:#fff}
.empty{grid-column:1/-1;padding:60px 0;text-align:center;color:var(--mid)}

/* story */
.story{background:var(--grey)}
.story .wrap{display:grid;grid-template-columns:1fr 1fr;gap:60px;align-items:center}
.story h2{font-size:clamp(2.6rem,6vw,5rem);margin-bottom:22px}
.story p{max-width:52ch;color:#333;margin-bottom:14px}
.stats{display:grid;grid-template-columns:1fr 1fr;gap:12px}
.stat{background:#000;color:#fff;padding:28px 22px}
.stat b{display:block;font-family:var(--d);font-size:3.4rem;font-weight:400;color:#fff;line-height:1}
.stat:nth-child(2){background:var(--red)}
.stat span{font-size:12px;text-transform:uppercase;font-weight:700;letter-spacing:.05em;color:#ddd}
@media(max-width:800px){.story .wrap{grid-template-columns:1fr}}

/* reviews */
.revs{display:grid;grid-template-columns:repeat(3,1fr);gap:12px}
.rev{border:2px solid var(--black);padding:26px}
.rev .st{color:var(--red);letter-spacing:3px;font-size:18px}
.rev p{margin:12px 0 16px;font-weight:600;font-size:16px}
.rev small{font-weight:700;text-transform:uppercase;font-size:12px;color:var(--mid)}
@media(max-width:800px){.revs{grid-template-columns:1fr}}

/* visit */
.visit .wrap{display:grid;grid-template-columns:1fr 1fr;gap:60px}
@media(max-width:800px){.visit .wrap{grid-template-columns:1fr}}
.visit h2{font-size:clamp(2.4rem,5vw,4rem);margin-bottom:20px}
.visit dt{font-weight:800;text-transform:uppercase;font-size:12px;margin-top:18px;letter-spacing:.05em}
form{display:grid;gap:12px}
form label{display:grid;gap:5px;font-weight:700;font-size:12px;text-transform:uppercase}
form input,form select{border:2px solid var(--line);padding:13px;background:#fff;font-weight:500;text-transform:none}
form input:focus,form select:focus{border-color:var(--black);outline:none}
.two{display:grid;grid-template-columns:1fr 1fr;gap:12px}
form .btn{width:100%;cursor:pointer}

footer{background:var(--black);color:#fff;padding:50px 0 30px}
footer .wrap{display:flex;justify-content:space-between;gap:30px;flex-wrap:wrap}
footer .logo{font-size:44px}
footer p{color:#aaa;max-width:34ch;margin-top:10px}
footer ul{list-style:none}footer li{margin:7px 0}footer a{color:#ddd;text-decoration:none}footer a:hover{color:var(--red)}
.copy{border-top:1px solid #2a2a2a;margin-top:34px;padding-top:18px;color:#888;font-size:12px}

/* cart drawer */
.shade{position:fixed;inset:0;background:rgba(0,0,0,.55);opacity:0;pointer-events:none;transition:.25s;z-index:40}
.shade.on{opacity:1;pointer-events:auto}
aside{position:fixed;right:0;top:0;bottom:0;width:min(440px,100%);background:#fff;z-index:50;transform:translateX(100%);transition:.3s;display:flex;flex-direction:column}
aside.on{transform:none}
.ch{display:flex;justify-content:space-between;align-items:center;padding:20px 24px;border-bottom:1px solid var(--line)}
.ch h2{font-size:2rem}
.x{background:none;border:0;font-size:30px;line-height:1}
.lines{flex:1;overflow:auto;padding:6px 24px}
.ln{display:grid;grid-template-columns:1fr auto;gap:4px 12px;padding:16px 0;border-bottom:1px solid var(--line)}
.ln b{font-size:14px}.ln small{color:var(--mid);grid-column:1}
.qty{display:flex;align-items:center;border:2px solid var(--black);width:max-content;margin-top:8px}
.qty button{width:32px;height:32px;border:0;background:#fff;font-size:18px;font-weight:700}
.qty button:hover{background:var(--black);color:#fff}
.qty span{min-width:30px;text-align:center;font-weight:700}
.ln .lp{font-weight:800;grid-row:1;grid-column:2}
.cf{padding:18px 24px;border-top:1px solid var(--line);display:grid;gap:12px;background:#fff}
.mode{display:grid;grid-template-columns:1fr 1fr}
.mode button{padding:11px;border:2px solid var(--black);background:#fff;font-weight:800;font-size:12px;text-transform:uppercase}
.mode button[aria-pressed="true"]{background:var(--black);color:#fff}
.cf input{border:2px solid var(--line);padding:12px}
.cf input:focus{border-color:var(--black);outline:none}
.tot{display:flex;justify-content:space-between;font-size:14px}
.tot.big{font-weight:800;font-size:18px}
.cf .btn{text-align:center;width:100%}
.ce{padding:50px 0;text-align:center;color:var(--mid)}

.heroimg{display:none;width:100%;max-width:560px;aspect-ratio:4/5;object-fit:cover}
.pic img{position:absolute;inset:0;width:100%;height:100%;object-fit:cover;transition:transform .45s}
.card:hover .pic img{transform:scale(1.06)}
.pic .badge,.pic .dot,.pic .quick{z-index:2}
</style>
</head>
<body>

<div class="ann">Free delivery on orders above ₹499 &nbsp;|&nbsp; Open daily 11 am to 11 pm &nbsp;|&nbsp; Call 70953 68952</div>

<header>
  <div class="wrap bar">
    <a class="logo" href="#top">Bagoji’s<span>.</span></a>
    <nav aria-label="Main">
      <a href="#menu">Menu</a><a href="#categories">Categories</a><a href="#story">Our story</a><a href="#reviews">Reviews</a><a href="#visit">Visit</a>
    </nav>
    <div class="icons"><button class="cartbtn" id="openCart" aria-label="Open order">Order <b id="count">0</b></button></div>
  </div>
</header>

<main id="top">
<div class="hero">
  <div class="wrap">
    <div>
      <span class="tag">Hyderabad’s dum house</span>
      <h1>Sealed.<br>Slow.<br><em>Biryani.</em></h1>
      <p>Every handi is layered by hand, sealed with dough and cooked on low heat. Order biryani, kebabs, curries and sweets from Sachin Bagoji’s kitchen.</p>
      <div class="btns"><a class="btn" href="#menu">Order now</a><a class="btn out" href="tel:+917095368952">Call 70953 68952</a><a class="btn out" href="#visit">Book a table</a></div>
    </div>
    <div class="art">
      <img class="heroimg" src="images/hero.jpg" alt="Hyderabadi dum biryani in a handi" onload="this.nextElementSibling.style.display='none';this.style.display='block'" onerror="this.remove()">
      <svg aria-hidden="true" viewBox="0 0 400 400">
        <g class="steam"><path d="M150 110 q-18-26 0-50 t0-40"/><path d="M200 100 q-18-26 0-50 t0-40"/><path d="M250 110 q-18-26 0-50 t0-40"/></g>
        <ellipse cx="200" cy="360" rx="130" ry="16" fill="#1a1a1a"/>
        <path d="M70 200 Q70 350 200 350 Q330 350 330 200 Z" fill="#E3112B"/>
        <path d="M70 200 Q70 230 90 260 Q200 290 310 260 Q330 230 330 200 Z" fill="#b30d22"/>
        <rect x="62" y="186" width="276" height="22" rx="11" fill="#fff"/>
        <path d="M95 186 Q95 120 200 120 Q305 120 305 186 Z" fill="#f2f2f2"/>
        <circle cx="200" cy="112" r="12" fill="#fff"/>
        <path d="M120 186 Q125 150 160 140" stroke="#ccc" stroke-width="6" fill="none" stroke-linecap="round"/>
      </svg>
    </div>
  </div>
</div>

<div class="ticker" aria-hidden="true"><div id="tick"></div></div>

<section id="categories">
  <div class="wrap">
    <div class="head"><h2>Shop by craving</h2><p>Pick a category and jump straight to the menu.</p></div>
    <div class="tiles" id="tiles"></div>
  </div>
</section>

<section id="menu" style="padding-top:0">
  <div class="wrap">
    <div class="head"><h2>The menu</h2><p>Add dishes to your order, then send it to us on WhatsApp.</p></div>
    <div class="tools">
      <div class="chips" id="chips"></div>
      <label class="sw"><input type="checkbox" id="veg"> Veg only</label>
      <input type="search" id="q" placeholder="Search dishes" aria-label="Search dishes">
      <select id="sort" aria-label="Sort"><option value="pop">Popular</option><option value="lo">Price: low to high</option><option value="hi">Price: high to low</option></select>
    </div>
    <div class="grid" id="grid"></div>
  </div>
</section>

<section class="story" id="story">
  <div class="wrap">
    <div>
      <h2>Not rushed.<br>Never.</h2>
      <p>Bagoji’s Dum House is run by Sachin Bagoji in Hyderabad. The kitchen is built around one rule: a proper dum biryani cannot be hurried.</p>
      <p>Rice and meat steam together in a sealed handi, so every grain takes on the masala. Around the biryani, the menu covers starters, curries, breads and sweets for the whole table.</p>
      <div class="btns" style="margin-top:22px"><a class="btn dark" href="#menu">Start your order</a></div>
    </div>
    <div class="stats">
      <div class="stat"><b>1 pot</b><span>One sealed handi per order</span></div>
      <div class="stat"><b>30+</b><span>Dishes on the menu</span></div>
      <div class="stat"><b>11–11</b><span>Open every day</span></div>
      <div class="stat"><b>₹499</b><span>Free delivery above</span></div>
    </div>
  </div>
</section>

<section id="reviews">
  <div class="wrap">
    <div class="head"><h2>What guests say</h2></div>
    <div class="revs">
      <div class="rev"><div class="st">★★★★★</div><p>Sample review: the mutton biryani was soft and full of flavour. Replace with a real guest review.</p><small>Guest name</small></div>
      <div class="rev"><div class="st">★★★★★</div><p>Sample review: fast delivery and the rice was still hot. Replace with a real guest review.</p><small>Guest name</small></div>
      <div class="rev"><div class="st">★★★★★</div><p>Sample review: the double ka meetha was the best part. Replace with a real guest review.</p><small>Guest name</small></div>
    </div>
  </div>
</section>

<section class="visit" id="visit" style="padding-top:0">
  <div class="wrap">
    <div>
      <h2>Visit us</h2>
      <dl>
        <dt>Address</dt><dd>Add your street address, Hyderabad, Telangana</dd>
        <dt>Hours</dt><dd>Every day, 11:00 am to 11:00 pm</dd>
        <dt>Phone</dt><dd><a href="tel:+917095368952">+91 70953 68952</a></dd>
        <dt>Owner</dt><dd>Sachin Bagoji</dd>
      </dl>
    </div>
    <div>
      <h2>Book a table</h2>
      <form id="book">
        <label>Name<input name="name" required autocomplete="name"></label>
        <div class="two"><label>Date<input type="date" name="date" required></label><label>Time<input type="time" name="time" value="20:00" required></label></div>
        <label>Guests<select name="guests"><option>1</option><option>2</option><option selected>4</option><option>6</option><option>8</option><option>10+</option></select></label>
        <button class="btn dark" type="submit">Send booking on WhatsApp</button>
      </form>
    </div>
  </div>
</section>
</main>

<footer>
  <div class="wrap">
    <div><a class="logo" href="#top">Bagoji’s<span>.</span></a><p>Hyderabadi dum biryani and more. Owned by Sachin Bagoji.</p></div>
    <ul><li><a href="#menu">Menu</a></li><li><a href="#story">Our story</a></li><li><a href="#visit">Visit</a></li></ul>
  </div>
  <div class="wrap copy">© <span id="yr"></span> Bagoji’s Dum House, Hyderabad. All rights reserved.</div>
</footer>

<div class="shade" id="shade"></div>
<aside id="drawer" aria-label="Your order" aria-hidden="true">
  <div class="ch"><h2>Your order</h2><button class="x" id="closeCart" aria-label="Close order">×</button></div>
  <div class="lines" id="lines"></div>
  <div class="cf" id="cf">
    <div class="mode"><button data-m="Delivery" aria-pressed="true">Delivery</button><button data-m="Pickup" aria-pressed="false">Pickup</button></div>
    <input id="cname" placeholder="Your name" autocomplete="name">
    <input id="caddr" placeholder="Delivery address" autocomplete="street-address">
    <div class="tot"><span>Subtotal</span><span id="sub">₹0</span></div>
    <div class="tot"><span>Delivery</span><span id="fee">₹0</span></div>
    <div class="tot big"><span>Total</span><span id="total">₹0</span></div>
    <a class="btn out" style="color:#000;border-color:#000" href="tel:+917095368952">Or call 70953 68952</a>
    <a class="btn dark" id="send" href="#" target="_blank" rel="noopener">Send order on WhatsApp</a>
  </div>
</aside>

<script>
// Change to your real WhatsApp number (country code first, no + or spaces)
const WA = "917095368952";
const FREE_ABOVE = 499, FEE = 40;

const ITEMS = [
 {n:"Hyderabadi Chicken Dum Biryani",d:"Basmati, marinated chicken, saffron, fried onions",p:280,c:"Biryani",v:0,e:"🍛",b:"Bestseller",s:1},
 {n:"Mutton Dum Biryani",d:"Slow-cooked mutton on the bone, sealed handi",p:380,c:"Biryani",v:0,e:"🍖",b:"Bestseller",s:1},
 {n:"Vegetable Dum Biryani",d:"Seasonal vegetables, mint, whole spices",p:220,c:"Biryani",v:1,e:"🥘",s:1},
 {n:"Paneer Biryani",d:"Paneer cubes in rich masala, layered with rice",p:250,c:"Biryani",v:1,e:"🧀",b:"New",s:1},
 {n:"Egg Biryani",d:"Boiled eggs and masala over fragrant rice",p:200,c:"Biryani",v:0,e:"🥚",s:1},
 {n:"Family Handi (serves 4)",d:"Chicken or mutton, with raita and salan",p:950,c:"Biryani",v:0,e:"🍲",b:"Value",s:1},
 {n:"Chicken 65",d:"Crisp, spicy, curry-leaf tempered",p:240,c:"Starters",v:0,e:"🍗",b:"Bestseller"},
 {n:"Chicken Tikka",d:"Charcoal-grilled, yogurt marinade",p:260,c:"Starters",v:0,e:"🍢"},
 {n:"Paneer Tikka",d:"Smoky paneer with peppers and onion",p:230,c:"Starters",v:1,e:"🧆"},
 {n:"Fish Fry",d:"Marinated fish, shallow fried",p:290,c:"Starters",v:0,e:"🐟"},
 {n:"Gobi Manchurian",d:"Crisp cauliflower in a tangy sauce",p:180,c:"Starters",v:1,e:"🥦"},
 {n:"Mirchi ka Salan",d:"Peanut, sesame and tamarind gravy with green chillies",p:140,c:"Curries & breads",v:1,e:"🌶️"},
 {n:"Bagara Baingan",d:"Baby aubergines in a nutty gravy",p:160,c:"Curries & breads",v:1,e:"🍆"},
 {n:"Butter Chicken",d:"Creamy tomato gravy, mild",p:290,c:"Curries & breads",v:0,e:"🥣"},
 {n:"Dal Tadka",d:"Yellow lentils with garlic and cumin",p:150,c:"Curries & breads",v:1,e:"🍛"},
 {n:"Rumali Roti",d:"Thin, soft, hand-tossed",p:30,c:"Curries & breads",v:1,e:"🫓"},
 {n:"Butter Naan",d:"Tandoor-baked",p:45,c:"Curries & breads",v:1,e:"🫓"},
 {n:"Double ka Meetha",d:"Fried bread pudding with milk and nuts",p:120,c:"Sweets & drinks",v:1,e:"🍮",b:"Bestseller"},
 {n:"Qubani ka Meetha",d:"Stewed apricots with cream",p:140,c:"Sweets & drinks",v:1,e:"🍑"},
 {n:"Irani Chai",d:"Strong, milky, sweet",p:40,c:"Sweets & drinks",v:1,e:"☕"},
 {n:"Sweet Lassi",d:"Thick yogurt drink",p:70,c:"Sweets & drinks",v:1,e:"🥛"},
 {n:"Masala Soda",d:"Fizzy lime with spices",p:60,c:"Sweets & drinks",v:1,e:"🥤"}
];
const CATS = ["All","Biryani","Starters","Curries & breads","Sweets & drinks"];
const $ = s => document.querySelector(s);
const slug = n => n.toLowerCase().replace(/[^a-z0-9]+/g,"-").replace(/^-|-$/g,"");
const st = {cat:"All", q:"", veg:false, sort:"pop", mode:"Delivery"};
let cart = {};
try{ cart = JSON.parse(localStorage.getItem("bdh-cart")||"{}"); }catch(e){}

/* ticker */
const words = ["Dum biryani","Chicken 65","Double ka meetha","Irani chai","Mirchi ka salan","Seekh & tikka"];
$("#tick").innerHTML = (words.map(w=>`<span>${w}</span><span>★</span>`).join("")).repeat(4);

/* tiles */
$("#tiles").innerHTML = CATS.slice(1).map(c=>{
  const n = ITEMS.filter(i=>i.c===c).length;
  const em = ITEMS.find(i=>i.c===c).e;
  return `<button class="tile" data-c="${c}"><span class="em">${em}</span><span><h3>${c}</h3><small>${n} dishes</small></span></button>`;
}).join("");
$("#tiles").onclick = e=>{
  const t = e.target.closest(".tile"); if(!t) return;
  st.cat = t.dataset.c; renderChips(); renderGrid();
  $("#menu").scrollIntoView({behavior:"smooth"});
};

/* chips + filters */
function renderChips(){
  $("#chips").innerHTML = CATS.map(c=>`<button class="chip" aria-pressed="${st.cat===c}" data-c="${c}">${c}</button>`).join("");
}
$("#chips").onclick = e=>{ const b=e.target.closest(".chip"); if(!b) return; st.cat=b.dataset.c; renderChips(); renderGrid(); };
$("#veg").onchange = e=>{ st.veg=e.target.checked; renderGrid(); };
$("#q").oninput = e=>{ st.q=e.target.value.toLowerCase(); renderGrid(); };
$("#sort").onchange = e=>{ st.sort=e.target.value; renderGrid(); };

function renderGrid(){
  let list = ITEMS.filter(i=>(st.cat==="All"||i.c===st.cat)&&(!st.veg||i.v)&&(i.n+" "+i.d).toLowerCase().includes(st.q));
  if(st.sort==="lo") list.sort((a,b)=>a.p-b.p);
  if(st.sort==="hi") list.sort((a,b)=>b.p-a.p);
  $("#grid").innerHTML = list.length ? list.map(i=>{
    const idx = ITEMS.indexOf(i);
    return `<article class="card" data-i="${idx}">
      <div class="pic">${i.b?`<span class="badge">${i.b}</span>`:""}<span class="dot ${i.v?"v":"n"}" title="${i.v?"Vegetarian":"Non-vegetarian"}"></span><span class="e">${i.e}</span><img src="images/${slug(i.n)}.jpg" alt="${i.n}" loading="lazy" onerror="this.remove()">
      <button class="quick" aria-label="Add ${i.n}">Quick add</button></div>
      <div class="info"><h3>${i.n}</h3><p>${i.d}</p>
      <div class="row"><span class="price">₹${i.p}</span>
      ${i.s?`<select class="spice" aria-label="Spice level"><option>Medium</option><option>Mild</option><option>Hot</option></select>`:""}</div></div></article>`;
  }).join("") : `<div class="empty">No dishes match. Try clearing the search or filters.</div>`;
}
$("#grid").onclick = e=>{
  const b = e.target.closest(".quick"); if(!b) return;
  const card = b.closest(".card"), it = ITEMS[card.dataset.i];
  const sp = card.querySelector(".spice");
  add(it, sp ? sp.value : "");
  b.textContent = "Added ✓"; setTimeout(()=>b.textContent="Quick add",900);
};

/* cart */
function save(){ try{ localStorage.setItem("bdh-cart",JSON.stringify(cart)); }catch(e){} }
function add(it, spice){
  const k = it.n+"|"+spice;
  cart[k] = cart[k] || {n:it.n,p:it.p,s:spice,q:0};
  cart[k].q++; save(); renderCart();
}
function renderCart(){
  const ents = Object.entries(cart);
  const cnt = ents.reduce((a,[,v])=>a+v.q,0);
  const sub = ents.reduce((a,[,v])=>a+v.q*v.p,0);
  const fee = st.mode==="Delivery" && sub>0 && sub<FREE_ABOVE ? FEE : 0;
  $("#count").textContent = cnt;
  $("#lines").innerHTML = ents.length ? ents.map(([k,v])=>`<div class="ln"><b>${v.n}</b><span class="lp">₹${v.p*v.q}</span>
    <small>${v.s?v.s+" spice · ":""}₹${v.p} each</small>
    <div class="qty"><button data-k="${k}" data-d="-1" aria-label="Less">−</button><span>${v.q}</span><button data-k="${k}" data-d="1" aria-label="More">+</button></div></div>`).join("")
    : `<div class="ce">Your order is empty.<br>Add something from the menu.</div>`;
  $("#cf").style.display = ents.length ? "grid" : "none";
  $("#caddr").style.display = st.mode==="Delivery" ? "block" : "none";
  $("#sub").textContent = "₹"+sub;
  $("#fee").textContent = fee ? "₹"+fee : (sub?"Free":"₹0");
  $("#total").textContent = "₹"+(sub+fee);
  const lines = ents.map(([,v])=>`${v.q} x ${v.n}${v.s?" ("+v.s+")":""}`).join("\n");
  const msg = `Hello Bagoji’s Dum House, I’d like to order for ${st.mode}:\n${lines}\nTotal: ₹${sub+fee}\nName: ${$("#cname").value||"-"}`+(st.mode==="Delivery"?`\nAddress: ${$("#caddr").value||"-"}`:"");
  $("#send").href = `https://wa.me/${WA}?text=${encodeURIComponent(msg)}`;
}
$("#lines").onclick = e=>{
  const b = e.target.closest("button[data-k]"); if(!b) return;
  const k = b.dataset.k; cart[k].q += +b.dataset.d;
  if(cart[k].q<=0) delete cart[k];
  save(); renderCart();
};
document.querySelectorAll(".mode button").forEach(b=>b.onclick=()=>{
  st.mode=b.dataset.m;
  document.querySelectorAll(".mode button").forEach(x=>x.setAttribute("aria-pressed",x===b));
  renderCart();
});
$("#cname").oninput = $("#caddr").oninput = renderCart;

function drawer(open){
  $("#drawer").classList.toggle("on",open); $("#shade").classList.toggle("on",open);
  $("#drawer").setAttribute("aria-hidden",!open);
  if(open) $("#closeCart").focus(); else $("#openCart").focus();
}
$("#openCart").onclick = ()=>drawer(true);
$("#closeCart").onclick = $("#shade").onclick = ()=>drawer(false);
document.addEventListener("keydown",e=>{ if(e.key==="Escape") drawer(false); });

/* booking */
$("#book").onsubmit = e=>{
  e.preventDefault();
  const f = new FormData(e.target);
  const msg = `Hello Bagoji’s Dum House, I’d like to book a table.\nName: ${f.get("name")}\nDate: ${f.get("date")}\nTime: ${f.get("time")}\nGuests: ${f.get("guests")}`;
  window.open(`https://wa.me/${WA}?text=${encodeURIComponent(msg)}`,"_blank","noopener");
};

$("#yr").textContent = new Date().getFullYear();
renderChips(); renderGrid(); renderCart();
</script>
</body>
</html>
