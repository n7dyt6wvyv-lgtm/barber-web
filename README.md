# barber-web.build

<!DOCTYPE html>
<html lang="cs">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>BARBER CLUB | Premium Barbershop</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700;800&display=swap" rel="stylesheet">

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  background: #0b0b0b;
  color: white;
  font-family: 'Montserrat', sans-serif;
}

header {
  height: 85px;
  padding: 0 8%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: #101010;
  border-bottom: 1px solid #292929;
}

.logo {
  color: #d6ad65;
  font-size: 25px;
  font-weight: 800;
  letter-spacing: 3px;
}

nav a {
  color: white;
  text-decoration: none;
  margin-left: 28px;
  font-size: 13px;
  transition: .3s;
}

nav a:hover {
  color: #d6ad65;
}

.hero {
  min-height: 650px;
  display: flex;
  align-items: center;
  padding: 80px 10%;
  background:
    linear-gradient(90deg, #080808 15%, #080808bb 60%, #08080855),
    url('https://images.unsplash.com/photo-1503951914875-452162b0f3f1?auto=format&fit=crop&w=1800&q=85') center/cover;
}

.hero-content {
  max-width: 650px;
}

.small-title {
  color: #d6ad65;
  letter-spacing: 5px;
  font-size: 13px;
  margin-bottom: 25px;
}

h1 {
  font-size: clamp(45px, 7vw, 85px);
  line-height: 1.05;
  font-weight: 800;
  margin-bottom: 25px;
}

h1 span {
  color: #d6ad65;
}

.hero-description {
  color: #ccc;
  line-height: 1.8;
  font-size: 15px;
  margin-bottom: 35px;
}

.btn {
  display: inline-block;
  background: #d6ad65;
  color: #111;
  padding: 17px 32px;
  text-decoration: none;
  font-weight: 700;
  font-size: 13px;
  transition: .3s;
}

.btn:hover {
  background: white;
  transform: translateY(-3px);
}

section {
  padding: 100px 10%;
}

.section-heading {
  text-align: center;
  font-size: 38px;
  margin-bottom: 15px;
}

.gold {
  color: #d6ad65;
}

.subtitle {
  color: #999;
  text-align: center;
  margin-bottom: 55px;
}

.services {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 25px;
}

.service {
  background: #171717;
  border: 1px solid #333;
  padding: 45px 25px;
  text-align: center;
  transition: .3s;
}

.service:hover {
  border-color: #d6ad65;
  transform: translateY(-6px);
}

.service h3 {
  color: #d6ad65;
  font-size: 21px;
  margin-bottom: 20px;
}

.service p {
  color: #aaa;
  font-size: 14px;
  line-height: 1.8;
}

.price {
  font-size: 27px;
  font-weight: 700;
  margin-top: 25px;
}

.about {
  background: #171717;
  text-align: center;
}

.about p {
  max-width: 750px;
  margin: auto;
  color: #bbb;
  line-height: 2;
}

.contact {
  text-align: center;
}

.contact p {
  color: #bbb;
  line-height: 2.3;
}

.contact .btn {
  margin-top: 25px;
}

footer {
  background: #050505;
  padding: 35px;
  text-align: center;
  color: #777;
  font-size: 12px;
  border-top: 1px solid #292929;
}

@media(max-width: 750px) {
  header {
    height: auto;
    padding: 25px 5%;
    flex-direction: column;
    gap: 22px;
  }

  nav {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 15px;
  }

  nav a {
    margin: 0;
    font-size: 11px;
  }

  .hero {
    min-height: 570px;
    padding: 60px 7%;
  }

  section {
    padding: 70px 7%;
  }

  .services {
    grid-template-columns: 1fr;
  }
}
</style>
</head>

<body>

<header>
  <div class="logo">BARBER CLUB</div>

  <nav>
    <a href="#home">DOMŮ</a>
    <a href="#services">SLUŽBY</a>
    <a href="#about">O NÁS</a>
    <a href="#contact">KONTAKT</a>
  </nav>
</header>

<main>

<div class="hero" id="home">
  <div class="hero-content">
    <p class="small-title">PREMIUM BARBER EXPERIENCE</p>

    <h1>VÍC NEŽ JEN <span>STŘIH.</span></h1>

    <p class="hero-description">
      Styl, preciznost a profesionální péče.
      Objev místo, kde se z obyčejného střihu
      stává zážitek.
    </p>

    <a href="#contact" class="btn">OBJEDNAT SE</a>
  </div>
</div>

<section id="services">
  <h2 class="section-heading">NAŠE <span class="gold">SLUŽBY</span></h2>
  <p class="subtitle">Profesionální péče pro každého muže.</p>

  <div class="services">

    <div class="service">
      <h3>PÁNSKÝ STŘIH</h3>
      <p>Klasické i moderní účesy podle tvého stylu.</p>
      <div class="price">450 Kč</div>
    </div>

    <div class="service">
      <h3>ÚPRAVA VOUSŮ</h3>
      <p>Precizní tvarování a profesionální péče.</p>
      <div class="price">250 Kč</div>
    </div>

    <div class="service">
      <h3>FULL SERVICE</h3>
      <p>Kompletní péče o vlasy i vousy.</p>
      <div class="price">650 Kč</div>
    </div>

  </div>
</section>

<section class="about" id="about">
  <h2 class="section-heading">O <span class="gold">NÁS</span></h2>

  <p>
    Barber Club je místem, kde se potkává styl,
    kvalita a profesionální přístup.
    Naším cílem je nabídnout každému zákazníkovi
    skvělý střih a příjemný zážitek.
  </p>
</section>

<section class="contact" id="contact">
  <h2 class="section-heading">KONTAKTUJ <span class="gold">NÁS</span></h2>

  <p>Telefon: +420 123 456 789</p>
  <p>E-mail: info@barberclub.cz</p>
  <p>Adresa: Praha, Česká republika</p>

  <a href="tel:+420123456789" class="btn">
    ZAVOLAT A OBJEDNAT SE
  </a>
</section>

</main>

<footer>
  © 2026 BARBER CLUB | Všechna práva vyhrazena
</footer>

</body>
</html>
