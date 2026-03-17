[ahh-bot.html](https://github.com/user-attachments/files/26067544/ahh-bot.html)
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ahh Bot</title>

<!-- Fonts & Libraries -->
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/aos/2.3.4/aos.css">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@9/swiper-bundle.min.css"/>

<style>
  /* RESET */
  * {margin:0;padding:0;box-sizing:border-box;font-family: 'Roboto', sans-serif;}
  body {background:#0d0d0d;color:#fff;overflow-x:hidden;}
  a {text-decoration:none;color:inherit;}
  img {display:block;max-width:100%;}

  /* HERO SECTION */
  .hero {
    position:relative;height:100vh;display:flex;justify-content:center;align-items:center;text-align:center;
    background:linear-gradient(135deg, #0d0d0d, #111);
    overflow:hidden;
  }
  #particles-js {position:absolute;width:100%;height:100%;top:0;left:0;z-index:0;}
  .hero-content {position:relative;z-index:1;color:#fff;}
  .hero-content h1 {font-size:4rem;letter-spacing:3px;margin-bottom:20px;text-shadow:0 0 10px #7289da;}
  .hero-content p {font-size:1.3rem;margin-bottom:40px;color:#aaa;}
  .hero-content .buttons {display:flex;gap:20px;justify-content:center;}
  .hero-content .buttons a {
    padding:15px 35px;background:linear-gradient(45deg,#7289da,#99a9f5);
    border-radius:8px;font-weight:700;color:#fff;transition:0.3s;box-shadow:0 0 20px rgba(114,137,218,0.5);
  }
  .hero-content .buttons a:hover {transform:scale(1.1);box-shadow:0 0 40px #7289da;}

  /* FEATURES */
  .features {padding:100px 20px;background:#111;}
  .features h2 {text-align:center;font-size:2.8rem;margin-bottom:60px;letter-spacing:2px;color:#7289da;}
  .cards {display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:30px;}
  .card {background:#1a1a1a;padding:30px;border-radius:15px;text-align:center;transition:0.3s;box-shadow:0 0 20px rgba(0,0,0,0.5);}
  .card:hover {transform:translateY(-10px);box-shadow:0 0 50px #7289da;}
  .card h3 {margin-bottom:15px;color:#fff;}
  .card p {color:#bbb;}

  /* COMMANDS */
  .commands {padding:100px 20px;background:#0d0d0d;}
  .commands h2 {text-align:center;font-size:2.8rem;margin-bottom:50px;letter-spacing:2px;color:#7289da;}
  .accordion {max-width:900px;margin:0 auto;}
  .accordion-item {background:#1a1a1a;margin-bottom:10px;border-radius:10px;overflow:hidden;box-shadow:0 0 15px rgba(0,0,0,0.4);}
  .accordion-item button {
    width:100%;padding:20px;text-align:left;font-size:1.2rem;background:#2a2a2a;border:none;color:#fff;cursor:pointer;
  }
  .accordion-item button:hover {background:#3b3b3b;}
  .panel {padding:0 20px;max-height:0;overflow:hidden;background:#111;transition:max-height 0.3s ease;}
  .panel p {padding:20px 0;color:#ccc;}

  /* ADMINS */
  .admins {padding:100px 20px;background:#111;}
  .admins h2 {text-align:center;font-size:2.8rem;margin-bottom:50px;color:#7289da;}
  .admin-cards {display:flex;flex-wrap:wrap;justify-content:center;gap:30px;}
  .admin-card {background:#1a1a1a;padding:20px;border-radius:15px;text-align:center;transition:0.3s;width:200px;box-shadow:0 0 15px rgba(0,0,0,0.5);}
  .admin-card:hover {transform:scale(1.05);box-shadow:0 0 50px #7289da;}
  .admin-card img {border-radius:50%;width:100px;height:100px;margin-bottom:15px;object-fit:cover;}
  .admin-card h3 {color:#fff;margin-bottom:5px;}
  .admin-card p {color:#aaa;font-size:0.9rem;}

  /* GALLERY */
  .gallery {padding:100px 20px;background:#0d0d0d;}
  .gallery h2 {text-align:center;font-size:2.8rem;margin-bottom:50px;color:#7289da;}
  .swiper {width:90%;max-width:1000px;margin:0 auto;}
  .swiper-slide {background:#1a1a1a;border-radius:15px;display:flex;justify-content:center;align-items:center;overflow:hidden;transition:transform 0.3s;}
  .swiper-slide img {width:100%;height:300px;object-fit:cover;}
  .swiper-slide:hover {transform:scale(1.05);box-shadow:0 0 40px #7289da;}

  /* FOOTER */
  footer {padding:50px 20px;background:#000;text-align:center;color:#888;}
  footer a {color:#7289da;margin:0 10px;transition:0.3s;}
  footer a:hover {color:#fff;}

</style>
</head>
<body>

<!-- HERO -->
<section class="hero">
  <div id="particles-js"></div>
  <div class="hero-content" data-aos="fade-up">
    <h1>Ahh Bot</h1>
    <p id="typed-text"></p>
    <div class="buttons">
      <a href="#">Invite Bot</a>
      <a href="#">Join Server</a>
    </div>
  </div>
</section>

<!-- FEATURES -->
<section class="features">
  <h2 data-aos="fade-up">Features</h2>
  <div class="cards">
    <div class="card" data-aos="fade-up" data-aos-delay="100">
      <h3>Moderation</h3>
      <p>Keep your server safe with advanced moderation commands.</p>
    </div>
    <div class="card" data-aos="fade-up" data-aos-delay="200">
      <h3>Fun Commands</h3>
      <p>Interactive games, memes, and entertainment for your community.</p>
    </div>
    <div class="card" data-aos="fade-up" data-aos-delay="300">
      <h3>Music</h3>
      <p>Play music directly in voice channels with ease.</p>
    </div>
    <div class="card" data-aos="fade-up" data-aos-delay="400">
      <h3>Custom Commands</h3>
      <p>Create your own commands for unique server interactions.</p>
    </div>
  </div>
</section>

<!-- COMMANDS -->
<section class="commands">
  <h2 data-aos="fade-up">Commands</h2>
  <div class="accordion">
    <div class="accordion-item">
      <button>!kick <span>➡</span></button>
      <div class="panel"><p>Kicks a user from the server.</p></div>
    </div>
    <div class="accordion-item">
      <button>!ban <span>➡</span></button>
      <div class="panel"><p>Bans a user from the server.</p></div>
    </div>
    <div class="accordion-item">
      <button>!play <span>➡</span></button>
      <div class="panel"><p>Plays music in your voice channel.</p></div>
    </div>
    <div class="accordion-item">
      <button>!meme <span>➡</span></button>
      <div class="panel"><p>Sends a random meme from the internet.</p></div>
    </div>
    <
