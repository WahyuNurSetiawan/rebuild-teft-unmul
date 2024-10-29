```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Teknik Elektro Universitas Mulawarwan</title>

    <!-- Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap"
      rel="stylesheet"
    />

    <!-- Feeather Icon -->
    <script src="https://unpkg.com/feather-icons"></script>

    <!-- My Style -->
    <link rel="stylesheet" href="css/style.css" />
  </head>

  <body>
    <!-- Navbar Start -->
    <nav class="navbar">
      <a href="#" class="navbar-logo">Teknik <span>Elektro</span> UNMUL</a>

      <div class="navbar-nav">
        <a href="#home">Home</a>
        <a href="#about">Tentang Saya</a>
        <a href="#menu">Menu</a>
        <a href="#contact">Kontak</a>
      </div>

      <div class="navbar-extra">
        <a href="#" id="search"><i data-feather="search"></i></a>
        <a href="#" id="shopping-cart"><i data-feather="youtube"></i></a>
        <a href="#" id="hamburger-menu"><i data-feather="menu"></i></a>
      </div>
    </nav>
    <!-- Navbar End -->

    <!-- Hero Section Start -->
    <section class="hero" id="home">
      <main class="content">
        <h1>Teknik <span>Elektro</span></h1>
        <h2>Universitas Mulawarwan</h2>
        <p>
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ipsam,
          reprehenderit.
        </p>
        <a href="#" class="cta">Beli Sekarang</a>
      </main>
    </section>
    <!-- Hero Section End -->

    <!-- About Section Start -->
    <section id="about" class="about">
      <h2><span>Tentang</span> Kami</h2>

      <div class="row">
        <div class="about-img">
          <img src="img/tentang-kami.jpg" alt="Tentang Kami" />
        </div>
        <div class="content">
          <h3>Kenapa memilih kopi kami?</h3>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestias,
            adipisci repudiandae reiciendis dolor ipsum veniam.
          </p>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem ipsa
            voluptates eveniet alias consequatur laudantium, beatae reiciendis
            sed blanditiis quibusdam?
          </p>
        </div>
      </div>
    </section>
    <!-- About Section End -->

    <!-- Menu Section Start -->
    <section id="menu" class="menu">
      <h2><span>Menu</span> Kami</h2>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse culpa
        commodi neque reiciendis at rem!
      </p>

      <div class="row">
        <div class="menu-card">
          <img src="img/menu/1.jpg" alt="Espresso" class="menu-card-img" />
          <h3 class="menu-card-title">- Espresso -</h3>
          <pc class="menu-card-price">IDR 15K</pc>
        </div>
        <div class="menu-card">
          <img src="img/menu/1.jpg" alt="Espresso" class="menu-card-img" />
          <h3 class="menu-card-title">- Espresso -</h3>
          <pc class="menu-card-price">IDR 15K</pc>
        </div>
        <div class="menu-card">
          <img src="img/menu/1.jpg" alt="Espresso" class="menu-card-img" />
          <h3 class="menu-card-title">- Espresso -</h3>
          <pc class="menu-card-price">IDR 15K</pc>
        </div>
        <div class="menu-card">
          <img src="img/menu/1.jpg" alt="Espresso" class="menu-card-img" />
          <h3 class="menu-card-title">- Espresso -</h3>
          <pc class="menu-card-price">IDR 15K</pc>
        </div>
      </div>
    </section>
    <!-- Menu Section End -->

    <!-- Feather Icon -->
    <script>
      feather.replace();
    </script>

    <!-- My Javascript -->
    <script src="js/script.js"></script>
  </body>
</html>
```

```css
:root {
  --primary: #b6895b;
  --bg: #010101;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  outline: none;
  border: none;
  text-decoration: none;
}

body {
  font-family: "Poppins", sans-serif;
  background-color: var(--bg);
  color: #fff;
  min-height: 3000px;
}

/* Navbar */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1.4rem 7%;
  background-color: rgba(1, 1, 1, 0.8);
  border-bottom: 1px solid #513c28;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 99999;
}

.navbar .navbar-logo {
  font-size: 2rem;
  font-weight: 700;
  color: #fff;
  font-style: italic;
}

.navbar .navbar-logo span {
  color: var(--primary);
}

.navbar .navbar-nav a {
  color: #fff;
  display: inline-block;
  font-size: 1.4rem;
  margin: 0 1rem;
}

.navbar .navbar-nav a:hover {
  color: var(--primary);
}

.navbar .navbar-nav a::after {
  content: "";
  display: block;
  padding-bottom: 0.5rem;
  border-bottom: 0.1rem solid var(--primary);
  transform: scaleX(0);
  transition: 0.2s linear;
}

.navbar .navbar-nav a:hover::after {
  transform: scaleX(0.5);
}

.navbar .navbar-extra a {
  color: #fff;
  margin: 0 0.5rem;
}

.navbar .navbar-extra a::hover {
  color: var(--primary);
}

#hamburger-menu {
  display: none;
}

/* Hero Section */
.hero {
  min-height: 100vh;
  display: flex;
  align-items: center;
  background-image: url("../img/header-bg.jpeg");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}

/* Versi Asli */
/* .hero::after {
  content: "";
  display: block;
  position: absolute;
  width: 100%;
  height: 30%;
  bottom: 0;
  background: linear-gradient(
    0deg,
    rgba(1, 1, 3, 1) 10%,
    rgba(255, 255, 255, 0) 50%
  );
} */

/* Versi Editan */
.hero {
  position: relative; /* Tambahkan posisi relatif untuk referensi overlay */
}

.hero::after {
  content: "";
  display: block;
  position: absolute;
  width: 250%; /* Sesuaikan lebar overlay agar tidak terlalu lebar */
  height: 100%; /* Membuat overlay setinggi elemen .hero */
  left: 0; /* Menempatkan overlay di bagian kiri */
  background: linear-gradient(
    90deg,
    rgba(1, 1, 3, 1) 10%, /* Warna gelap solid di sisi kiri overlay */
    rgba(255, 255, 255, 0) 50% /* Warna transparan di sisi kanan overlay */
  );
  z-index: 1; /* Pastikan overlay berada di bawah konten */
}

.hero .content {
  position: relative; /* Pastikan konten memiliki posisi relatif */
  z-index: 2; /* Letakkan konten di atas overlay */
  padding: 1.4rem 7%;
  max-width: 60rem;
}

.hero .content h1 {
  font-size: 5em;
  color: #fff;
  text-shadow: 1px 1px 3px rgba(1, 1, 3, 0.5);
  line-height: 1.2;
}

.hero .content h1 span {
  color: var(--primary);
}

.hero .content h2 {
  font-size: 3em;
  color: #fff;
  text-shadow: 1px 1px 3px rgba(1, 1, 3, 0.5);
  line-height: 1.2;
}

.hero .content h2 span {
  color: var(--primary);
}

.hero .content p {
  font-size: 1.6rem;
  margin-top: 0.5rem;
  line-height: 1.4;
  font-weight: 100;
  text-shadow: 1px 1px 3px rgba(1, 1, 3, 0.5);
}

.hero .content .cta {
  margin-top: 1rem;
  display: inline-block;
  padding: 1rem 3rem;
  font-size: 1.4rem;
  color: #fff;
  background-color: var(--primary);
  border-radius: 0.5rem;
  box-shadow: 1px 1px 3px rgba(1, 1, 3, 0.5);
}

/* Akhir Editan */

/* .hero .content {
  padding: 1.4rem 7%;
  max-width: 60rem;
}

.hero .content h1 {
  font-size: 5em;
  color: #fff;
  text-shadow: 1px 1px 3px rgba(1, 1, 3, 0.5);
  line-height: 1.2;
  /* mix-blend-mode: difference; */
}

.hero .content h1 span {
  color: var(--primary);
}

.hero .content p {
  font-size: 1.6rem;
  margin-top: 0.5rem;
  line-height: 1.4;
  font-weight: 100;
  text-shadow: 1px 1px 3px rgba(1, 1, 3, 0.5);
  line-height: 1.2;
  mix-blend-mode: difference;
}

.hero .content .cta {
  margin-top: 1rem;
  display: inline-block;
  padding: 1rem 3rem;
  font-size: 1.4rem;
  color: #fff;
  background-color: var(--primary);
  border-radius: 0.5rem;
  box-shadow: 1px 1px 3px rgba(1, 1, 3, 0.5em);
} */

/* About Section */
.about,
.menu {
  padding: 8rem 7% 1.4rem;
}

.about h2,
.menu h2 {
  text-align: center;
  font-size: 2.6rem;
  margin-bottom: 3rem;
}

.about h2 span,
.menu h2 span {
  color: var(--primary);
}

.about .row {
  display: flex;
}

.about .row .about-img {
  flex: 1 1 45rem;
}

.about .row .about-img img {
  width: 100%;
}

.about .row .content {
  flex: 1 1 35rem;
  padding: 0 1rem;
}

.about .row .content h3 {
  font-size: 1.8rem;
  margin-bottom: 1rem;
}

.about .row .content p {
  margin-bottom: 0.8rem;
  font-size: 1.4rem;
  font-weight: 100;
  line-height: 1.6;
}

/* Menu Section */
.menu h2 {
  margin-bottom: 1rem;
}
.menu p {
  text-align: center;
  max-width: 30rem;
  margin: auto;
  font-weight: 100;
  line-height: 1.6;
}

.menu .row {
  display: flex;
  flex-wrap: wrap;
  margin-top: 5rem;
  justify-content: center;
}

.menu .row .menu-card {
  text-align: center;
  padding-bottom: 2rem;
}

.menu .row .menu-card img {
  border-radius: 50%;
  width: 40%;
}

.menu .row .menu-card .menu-card-title {
  margin: 1.5rem auto 1rem;
}

/* Media Quaries */

/* Laptop */
@media (max-width: 1366px) {
  html {
    font-size: 75%;
  }
}

/* Tablet */
@media (max-width: 768px) {
  html {
    font-size: 62.5%;
  }

  #hamburger-menu {
    display: inline-block;
  }

  .navbar .navbar-nav {
    position: absolute;
    top: 100%;
    right: -100%;
    background-color: #fff;
    width: 30rem;
    height: 100vh;
    transition: 0.3s;
  }

  .navbar .navbar-nav.active {
    right: 0;
  }

  .navbar .navbar-nav a {
    color: var(--bg);
    display: block;
    margin: 1.5em;
    padding: 0.5rem;
    font-size: 2rem;
  }

  .navbar .navbar-nav a::after {
    transform-origin: 0 0;
  }

  .navbar .navbar-nav a:hover::after {
    transform: scaleX(0.2);
  }

  .about .row {
    flex-wrap: wrap;
  }

  .about .row .about-img img {
    height: 24rem;
    object-fit: cover;
    object-position: center;
  }

  .about .row .content {
    padding: 0;
  }

  .about .row .content p {
    font-size: 1.6rem;
  }
}

/* Mobile Phone */
@media (max-width: 450px) {
  html {
    font-size: 55%;
  }
}

```

```js
// Toggle class active
const navbarNav = document.querySelector(".navbar-nav");
// ketika hamburger menu di klik
document.querySelector("#hamburger-menu").onclick = () => {
  navbarNav.classList.toggle("active");
};

// Klik di luar sidebar untuk menghilangkan nav
const hamburger = document.querySelector("#hamburger-menu");

document.addEventListener("click", function (e) {
  if (!hamburger.contains(e.target) && !navbarNav.contains(e.target)) {
    navbarNav.classList.remove("active");
  }
});

```

mengapa tampilan hamburger menu tidak muncul