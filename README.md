# Rojak-Mee-Siam.<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Rojak & Mee Siam | Geylang Serai</title>

<style>
:root{
  --green:#0b5d1e;
  --gold:#c9a227;
  --bg:#f5f6f4;
}

*{
  box-sizing:border-box;
  margin:0;
  padding:0;
  font-family: "Segoe UI", Arial, sans-serif;
}

body{
  background:var(--bg);
  color:#222;
  line-height:1.7;
}

p{
  text-align:justify;
}

h1,h2,h3{
  color:var(--green);
}

header{
  position:sticky;
  top:0;
  background:#fff;
  box-shadow:0 6px 20px rgba(0,0,0,.08);
  z-index:1000;
}

.nav{
  max-width:1200px;
  margin:auto;
  padding:18px 22px;
  display:flex;
  justify-content:space-between;
  align-items:center;
}

.logo{
  font-weight:800;
  font-size:1.2rem;
}

.menu-btn{
  font-size:1.6rem;
  display:none;
  cursor:pointer;
}

nav a{
  margin-left:26px;
  text-decoration:none;
  color:#222;
  font-weight:600;
}

nav a:hover{
  color:var(--green);
}

@media(max-width:768px){
  .menu-btn{display:block;}
  nav{
    position:absolute;
    top:70px;
    left:0;
    right:0;
    background:white;
    display:none;
    flex-direction:column;
    padding:20px;
  }
  nav a{
    margin:12px 0;
  }
  nav.show{
    display:flex;
  }
}

section{
  max-width:1100px;
  margin:auto;
  padding:90px 22px;
}

.section-title{
  text-align:center;
  font-size:2.1rem;
  margin-bottom:12px;
}

.section-sub{
  text-align:center;
  color:#666;
  margin-bottom:55px;
}

/* HERO */
.hero{
  text-align:center;
  padding-top:110px;
}

.hero h1{
  font-size:2.6rem;
}

.hero span{
  color:var(--gold);
}

.hero p{
  max-width:720px;
  margin:22px auto;
  color:#555;
}

/* MENU */
.menu-grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
  gap:22px;
}

.card{
  background:#fff;
  padding:22px;
  border-radius:16px;
  box-shadow:0 14px 40px rgba(0,0,0,.08);
  transition:.3s ease;
}

.card:hover{
  transform:translateY(-6px);
}

.price{
  margin-top:6px;
  font-weight:700;
  color:var(--green);
}

.badge{
  display:inline-block;
  background:var(--green);
  color:#fff;
  padding:6px 12px;
  border-radius:20px;
  font-size:.75rem;
  margin-bottom:8px;
}

/* INFO / REVIEW */
.box{
  background:#fff;
  padding:45px;
  border-radius:20px;
  box-shadow:0 18px 45px rgba(0,0,0,.08);
}

.box p{
  margin-bottom:16px;
}

.stars{
  color:var(--gold);
  font-size:1.3rem;
  margin-bottom:12px;
}

/* FOOTER */
footer{
  background:var(--green);
  color:white;
  text-align:center;
  padding:26px;
  margin-top:80px;
}
</style>
</head>

<body>

<header>
  <div class="nav">
    <div class="logo">Rojak & Mee Siam</div>
    <div class="menu-btn" onclick="toggleMenu()">☰</div>
    <nav id="nav">
      <a href="#menu">Menu</a>
      <a href="#info">Info</a>
      <a href="#reviews">Reviews</a>
      <a href="#location">Location</a>
    </nav>
  </div>
</header>

<section class="hero">
  <h1>Authentic <span>Indian Rojak</span> & Mee Siam</h1>
  <p>
    A legacy hawker from the old Geylang Serai Market, serving timeless flavours
    prepared the traditional way.
  </p>
</section>

<section id="menu">
  <h2 class="section-title">Menu</h2>
  <p class="section-sub">Freshly prepared • Authentic taste</p>

  <div class="menu-grid">

    <div class="card">
      <div class="badge">Morning Only • Limited</div>
      <h3>Mee Siam</h3>
      <div class="price">$4.00</div>
    </div>

    <div class="card"><h3>Tepung Kosong</h3><div class="price">$1.00</div></div>
    <div class="card"><h3>Tepung Kelapa</h3><div class="price">$1.20</div></div>
    <div class="card"><h3>Tepung Sayur</h3><div class="price">$1.20</div></div>
    <div class="card"><h3>Tepung Telur</h3><div class="price">$1.60</div></div>

    <div class="card"><h3>Fish Ball</h3><div class="price">$1.00</div></div>
    <div class="card"><h3>Fish Cake</h3><div class="price">$1.60</div></div>
    <div class="card"><h3>Fish Fillet</h3><div class="price">$2.00</div></div>

    <div class="card"><h3>Sotong Kering</h3><div class="price">$2.00</div></div>
    <div class="card"><h3>Udang Tepung</h3><div class="price">$2.00</div></div>
    <div class="card"><h3>Udang Cake</h3><div class="price">$1.60</div></div>

    <div class="card"><h3>Paru Lembu</h3><div class="price">$2.00</div></div>
    <div class="card"><h3>Limpa Lembu</h3><div class="price">$2.00</div></div>
    <div class="card"><h3>Hati Lembu</h3><div class="price">$1.20</div></div>

    <div class="card"><h3>Ayam Cake</h3><div class="price">$1.60</div></div>
    <div class="card"><h3>Hot Dog</h3><div class="price">$0.80</div></div>
    <div class="card"><h3>Tempeh</h3><div class="price">$2.00</div></div>
    <div class="card"><h3>Tahu</h3><div class="price">$1.20</div></div>
    <div class="card"><h3>Ubi Kentang</h3><div class="price">$0.80 – $1.00</div></div>
    <div class="card"><h3>Wadeh Dal</h3><div class="price">$1.00</div></div>

  </div>
</section>

<section id="info">
  <h2 class="section-title">Information</h2>
  <div class="box">
    <p>🕌 Closed every Friday from <b>12:30 PM – 2:00 PM</b> for prayer.</p>
    <p>🍠 Sweet potato–based rojak gravy with <b>unlimited refills</b>.</p>
    <p>🏨 Featured at The Fullerton Hotel.</p>
    <p>🇸🇬 Former Prime Minister Halimah Yacob’s husband has dined here.</p>
    <p>📞 Contact: Yet to come.</p>
  </div>
</section>

<section id="reviews">
  <h2 class="section-title">Customer Review</h2>
  <div class="box">
    <div class="stars">★★★★★</div>
    <p>
      A legacy Indian Rojak and Mee Siam stall that has existed for over 50 years.
      The sweet potato–based rojak gravy is authentic and nostalgic, while the
      Mamak-style Mee Siam is increasingly rare to find today. Long queues are a
      testament to its popularity.
    </p>
    <b>— Anonymous Customer</b>
  </div>
</section>

<section id="location">
  <h2 class="section-title">Location</h2>
  <p class="section-sub">Visit us</p>
  <p style="text-align:center;font-weight:600">
    Geylang Serai Market & Food Centre<br>
    Level 2, #02-126
  </p>
</section>

<footer>
  © Rojak & Mee Siam • Legacy Hawker
</footer>

<script>
function toggleMenu(){
  document.getElementById("nav").classList.toggle("show");
}
</script>

</body>
</html>
