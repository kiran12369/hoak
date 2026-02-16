<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>HoaK — Smart E-commerce for India</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;900&display=swap" rel="stylesheet">

<style>
:root {
  --bg: #0a0c10;
  --panel: #11141c;
  --text: #ffffff;
  --muted: #9aa3b2;
  --accent: #d4b36a;
  --line: rgba(255,255,255,0.08);
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: 'Inter', sans-serif;
  background: radial-gradient(900px 500px at 50% -20%, #1a1f2e, var(--bg));
  color: var(--text);
  overflow-x: hidden;
}

/* NAV */
nav {
  position: fixed;
  top: 0;
  width: 100%;
  padding: 22px 40px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: rgba(10,12,16,0.7);
  backdrop-filter: blur(14px);
  border-bottom: 1px solid var(--line);
  z-index: 1000;
}

.logo {
  font-size: 22px;
  font-weight: 800;
}

.logo span {
  color: var(--accent);
}

.menu-btn {
  font-size: 26px;
  cursor: pointer;
}

/* MENU */
.menu {
  position: fixed;
  inset: 0;
  background: rgba(10,12,16,0.92);
  backdrop-filter: blur(24px);
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 32px;
  opacity: 0;
  pointer-events: none;
  transition: 0.4s ease;
  z-index: 2000;
}

.menu.active {
  opacity: 1;
  pointer-events: auto;
}

.menu a {
  font-size: 32px;
  font-weight: 600;
  text-decoration: none;
  color: var(--text);
}

.menu a:hover {
  color: var(--accent);
}

/* HERO */
.hero {
  padding: 200px 24px 140px;
  text-align: center;
}

.hero h1 {
  font-size: clamp(64px, 10vw, 120px);
  font-weight: 900;
  letter-spacing: -0.04em;
}

.hero h1 span {
  color: var(--accent);
}

.hero p {
  max-width: 620px;
  margin: 32px auto 56px;
  font-size: 20px;
  color: var(--muted);
  line-height: 1.6;
}

.buttons {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 16px;
}

.buttons a {
  padding: 16px 28px;
  border-radius: 14px;
  font-weight: 600;
  text-decoration: none;
  border: 1px solid var(--line);
  background: var(--panel);
  color: var(--text);
  transition: 0.3s ease;
}

.buttons a.primary {
  border-color: var(--accent);
}

.buttons a:hover {
  transform: translateY(-4px);
  border-color: var(--accent);
}

/* SECTIONS */
section {
  max-width: 1100px;
  margin: 120px auto;
  padding: 0 24px;
}

.block {
  border-top: 1px solid var(--line);
  padding-top: 60px;
}

.block h2 {
  font-size: 42px;
  margin-bottom: 24px;
}

.block p {
  max-width: 720px;
  font-size: 18px;
  line-height: 1.7;
  color: var(--muted);
}

/* FOOTER */
footer {
  border-top: 1px solid var(--line);
  padding: 60px 24px;
  text-align: center;
  color: var(--muted);
  font-size: 14px;
}
</style>
</head>

<body>

<nav>
  <div class="logo">Hoa<span>K</span></div>
  <div class="menu-btn" onclick="toggleMenu()">☰</div>
</nav>

<div class="menu" id="menu">
  <a href="#about" onclick="toggleMenu()">About HoaK</a>
  <a href="#founder" onclick="toggleMenu()">Founder</a>
  <a href="mailto:thehoak@outlook.com">Help</a>
  <a href="#join" onclick="toggleMenu()">Join as Shopper</a>
</div>

<section class="hero">
  <h1>Hoa<span>K</span></h1>
  <p>
    A smart, personalised e-commerce platform built in India,
    designed for how Indians actually shop.
  </p>

  <div class="buttons">
    <a class="primary" href="#">Google Play</a>
    <a href="#">App Store</a>
    <a href="#">Download APK</a>
  </div>
</section>

<section id="about">
  <div class="block">
    <h2>About HoaK</h2>
    <p>
      HoaK is a next-generation e-commerce platform focused on intelligent discovery,
      personalization, and trust. Instead of endless scrolling, HoaK helps users find
      what truly fits them — faster, simpler, and smarter.
    </p>
  </div>
</section>

<section id="founder">
  <div class="block">
    <h2>Founder</h2>
    <p>
      <strong>Ravikiran</strong> is the Founder & CEO of HoaK. With a focus on building
      meaningful consumer technology, he is driven to create platforms that combine
      simplicity, intelligence, and real impact for everyday users.
    </p>
  </div>
</section>

<footer>
  © 2026 HoaK. Made in India 🇮🇳
</footer>

<script>
function toggleMenu() {
  document.getElementById('menu').classList.toggle('active');
}
</script>

</body>
</html>
