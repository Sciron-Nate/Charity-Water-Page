# Charity-Water-Page
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Charity: Water Landing Page - Responsive</title>
<style>
@font-face {
  font-family: 'Proxima Nova';
  src: local('Proxima Nova'), local('ProximaNova'), url('https://fonts.cdnfonts.com/s/17852/ProximaNova-Regular.woff') format('woff');
}

body {
  margin: 0;
  font-family: 'Proxima Nova', Arial, Helvetica, sans-serif;
  line-height: 1.6;
  color: #1A1A1A;
  background-color: #f9fafb;
}

h1, h2, h3 { font-family: 'Georgia', serif; margin: 0 0 20px 0; line-height: 1.3; }

p, a { font-family: 'Proxima Nova'; color: #1A1A1A; line-height: 1.6; }

a { text-decoration: none; transition: color 0.3s ease, transform 0.3s ease; }

.navbar {
  display: flex; justify-content: space-between; align-items: center;
  padding: 20px 50px; background: #FFC907; color: #1A1A1A;
  position: sticky; top: 0; z-index: 1000; border-radius: 0 0 10px 10px;
}
.navbar .logo { font-size: 1.8rem; font-weight: bold; }
.navbar ul { list-style: none; display: flex; gap: 30px; margin: 0; padding: 0; }
.navbar ul li a:hover { color: #BF6C46; transform: scale(1.1); }

.hero {
  background: url("https://via.placeholder.com/1400x600") no-repeat center center/cover;
  text-align: center; padding: 160px 20px; position: relative;
  transition: all 0.5s ease;
}
.hero:hover { transform: scale(1.02); }
.hero-overlay { position: absolute; top: 0; left: 0; right: 0; bottom: 0; background: rgba(26,26,26,0.5); border-radius: 15px; }
.hero-content { position: relative; z-index: 1; max-width: 900px; margin: 0 auto; }
.hero h1 { color: #FFEB3B; font-size: 4rem; margin-bottom: 25px; text-shadow: 2px 2px 5px rgba(0,0,0,0.3); }
.hero p { color: #FFFFFF; font-size: 1.4rem; margin-bottom: 40px; text-shadow: 1px 1px 3px rgba(0,0,0,0.2); }

.btn-primary {
  background: #BF6C46; color: #FFFFFF; padding: 22px 45px; border-radius: 12px;
  font-size: 1.4rem; font-weight: bold; transition: all 0.3s ease, transform 0.3s ease;
  box-shadow: 0 6px 10px rgba(0,0,0,0.15);
}
.btn-primary:hover { background: #77A8BB; transform: scale(1.1); }

.section { padding: 100px 20px; max-width: 1000px; margin: 50px auto; border-radius: 15px; }
.about { background-color: #77A8BB; text-align: center; }
.about h2 { font-size: 2.5rem; margin-bottom: 25px; }
.about p { font-size: 1.3rem; line-height: 1.8; }
.story { background-color: #fff; text-align: left; box-shadow: 0 6px 15px rgba(0,0,0,0.1); padding: 60px; border-radius: 15px; }
.story h2 { font-size: 2.3rem; margin-bottom: 25px; }
.story p { font-size: 1.25rem; line-height: 1.8; margin-bottom: 25px; }
.story .highlight { font-weight: bold; color: #77A8BB; }
.cta { background: #FFC907; text-align: center; padding: 100px 20px; }
.cta h2 { color: #1A1A1A; margin-bottom: 40px; font-size: 2.5rem; }
.cta a { background: #BF6C46; color: #FFFFFF; padding: 22px 45px; border-radius: 12px;
  font-size: 1.4rem; font-weight: bold; transition: all 0.3s ease, transform 0.3s ease; box-shadow: 0 6px 10px rgba(0,0,0,0.15);
}
.cta a:hover { background: #77A8BB; transform: scale(1.1); }

.story-cta { text-align: center; margin-top: 30px; }

@media (max-width: 1024px) { .hero h1 { font-size: 3.5rem; } }
@media (max-width: 768px) {
  .hero h1 { font-size: 3rem; }
  .hero p { font-size: 1.2rem; }
  .btn-primary { font-size: 1.2rem; padding: 18px 36px; }
  .about h2, .cta h2 { font-size: 2rem; }
  .about p, .story p { font-size: 1.15rem; }
}
@media (max-width: 480px) {
  .navbar { flex-direction: column; gap: 15px; }
  .hero { padding: 120px 15px; }
  .hero h1 { font-size: 2.5rem; }
  .btn-primary { font-size: 1rem; padding: 15px 30px; }
}
</style>
</head>
<body>

<nav class="navbar">
  <div class="logo">Charity: Water</div>
  <ul>
    <li><a href="#about">About</a></li>
    <li><a href="#story">Story</a></li>
    <li><a href="#donate">Donate</a></li>
  </ul>
</nav>

<section class="hero">
  <div class="hero-overlay"></div>
  <div class="hero-content">
    <h1>Be the Change. Join the Movement for Clean Water.</h1>
    <p>Every donation powers life-changing solutions in communities lacking safe drinking water.</p>
    <a href="#donate" class="btn-primary">Donate Now</a>
  </div>
</section>

<section id="about" class="section about">
  <h2>Why Clean Water?</h2>
  <p>Every person deserves access to clean, safe drinking water. Your support makes it possible to provide sustainable water solutions to communities in need, improving health, education, and opportunity for generations to come.</p>
</section>

<section id="story" class="section story">
  <h2>Our Story</h2>
  <p>In a small village in Uganda, access to clean water was once a daily struggle. Children walked hours to collect water from contaminated sources, resulting in illness and missed school days. Through sustainable water systems, they now enjoy <span class="highlight">safe, clean water every day</span>.</p>
  <p>Families focus on education and community development, children attend school consistently, and health outcomes have improved. Your donation directly expands these projects and brings <span class="highlight">hope to more communities worldwide</span>.</p>
  <div class="story-cta">
    <a href="#donate" class="btn-primary">Donate Now</a>
  </div>
</section>

<section id="donate" class="section cta">
  <h2>Ready to Make a Difference?</h2>
  <a href="#">Donate Today</a>
</section>

</body>
</html>
