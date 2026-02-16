<div class="hero">
  <span class="badge">MADE IN INDIA 🇮🇳</span>

  <h1 class="title">HoaK</h1>

  <p class="tagline">A smart, personalised shopping experience built for India</p>

  <h2 class="coming-soon">Coming Soon</h2>

  <div class="store-badges">
    <a href="#" aria-label="Google Play – coming soon">
      <img src="https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg" alt="Get it on Google Play">
    </a>
    <a href="#" aria-label="Apple App Store – coming soon">
      <img src="https://developer.apple.com/assets/elements/badges/download-on-the-app-store.svg" alt="Download on the App Store">
    </a>
  </div>
</div>
<style>
:root {
  --primary: #7b2ff7;
  --secondary: #00c6ff;
  --bg: #0b0d12;
  --text: #ffffff;
  --muted: #a0a4b8;
}

body {
  background: radial-gradient(1200px 600px at 50% -10%, #1a1d2e, #0b0d12);
}

.hero {
  text-align: center;
  margin: 120px auto;
  padding: 60px 24px;
  max-width: 900px;
  color: var(--text);
  animation: fadeUp 1.1s ease forwards;
}

.badge {
  display: inline-block;
  padding: 6px 14px;
  font-size: 12px;
  letter-spacing: 0.12em;
  border-radius: 999px;
  background: rgba(255,255,255,0.08);
  backdrop-filter: blur(10px);
  margin-bottom: 24px;
  color: var(--muted);
}

.title {
  font-size: clamp(56px, 8vw, 88px);
  font-weight: 900;
  margin: 0;
  letter-spacing: -0.03em;
}

.tagline {
  font-size: 18px;
  max-width: 520px;
  margin: 20px auto 48px;
  color: var(--muted);
}

.coming-soon {
  font-size: clamp(42px, 6vw, 72px);
  font-weight: 900;
  background: linear-gradient(90deg,var(--primary),var(--secondary));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  margin-bottom: 40px;
  position: relative;
}

.coming-soon::after {
  content: "";
  position: absolute;
  inset: -12px;
  background: linear-gradient(90deg,var(--primary),var(--secondary));
  filter: blur(40px);
  opacity: 0.25;
  z-index: -1;
}

.store-badges img {
  height: 56px;
  margin: 0 12px;
  transition: transform 0.25s ease, filter 0.25s ease;
  filter: grayscale(1) brightness(0.9);
}

.store-badges a:hover img {
  transform: translateY(-4px) scale(1.03);
  filter: grayscale(0) brightness(1);
}

@keyframes fadeUp {
  from {
    opacity: 0;
    transform: translateY(24px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>
