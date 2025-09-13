# DP
?
<!doctype html>
<html lang="id">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Menu Minuman — Weeb Premium</title>
  <style>
    :root{
      --g1: #F4AC05;
      --g2: #112424;
      --g3: #277C8C;
      --gradient: linear-gradient(135deg,var(--g1),var(--g2),var(--g3));
      --bg: #0f1113;
      --card-bg: rgba(255,255,255,0.04);
      --glass: rgba(255,255,255,0.06);
      --muted: rgba(255,255,255,0.65);
      --accent: var(--g1);
      --radius: 14px;
      --shadow: 0 8px 24px rgba(2,6,23,0.6);
      font-family: Inter, ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    *{box-sizing:border-box}
    body{
      margin:0;min-height:100vh;background:#06131a;color:#fff;padding:40px;display:flex;align-items:flex-start;justify-content:center;font-smoothing:antialiased}
    .container{width:100%;max-width:1200px}
    header{display:flex;gap:20px;align-items:center;margin-bottom:28px}
    .logo{width:96px;height:96px;border-radius:20px;background:var(--gradient);display:grid;place-items:center;box-shadow: var(--shadow)}
    .logo h1{margin:0;font-size:20px;color:#071011}
    .title-block h2{margin:0;font-size:20px}
    .title-block p{margin:6px 0 0;color:var(--muted);font-size:13px}
    .menu{background:linear-gradient(180deg,rgba(255,255,255,0.02),rgba(255,255,255,0.01));border-radius:20px;padding:22px;box-shadow: var(--shadow)}
    .section{margin-bottom:20px;padding:12px 6px}
    .section-header{display:flex;align-items:center;gap:12px;margin-bottom:12px}
    .section-header .badge{width:44px;height:44px;border-radius:10px;display:grid;place-items:center;background:var(--glass);backdrop-filter: blur(6px)}
    .section-header h3{margin:0;font-size:18px}
    .section-header p{margin:0;color:var(--muted);font-size:13px}
    .drink-row{display:grid;grid-template-columns: repeat(auto-fit,minmax(220px,1fr));gap:14px}
    .card{background:linear-gradient(180deg,rgba(255,255,255,0.02),rgba(255,255,255,0.01));border-radius:12px;padding:14px;display:flex;gap:12px;align-items:center;border:1px solid rgba(255,255,255,0.03);transition: transform .2s ease, box-shadow .2s ease}
    .card:hover{transform:translateY(-6px);box-shadow:0 20px 40px rgba(2,6,23,0.7)}
    .illustration{width:84px;height:84px;border-radius:10px;overflow:hidden;display:grid;place-items:center;background:rgba(255,255,255,0.02)}
    .illustration img{width:100%;height:100%;object-fit:cover;border-radius:10px}
    .meta{flex:1}
    .meta h4{margin:0 0 6px 0;font-size:16px}
    .meta p{margin:0;color:var(--muted);font-size:13px}
    .price{white-space:nowrap;font-weight:700;color:var(--g1)}
    .tags{margin-top:8px;display:flex;gap:8px;flex-wrap:wrap}
    .tag{font-size:11px;padding:6px 8px;border-radius:999px;background:rgba(255,255,255,0.03);color:var(--muted)}
    .accent-ribbon{height:6px;border-radius:6px;background:var(--gradient);margin-top:14px;box-shadow:0 6px 30px rgba(39,124,140,0.12)}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="logo"><h1>Weeb</h1></div>
      <div class="title-block">
        <h2>Weeb Premium — Menu Minuman</h2>
        <p>Kopi · Smoothies · Juice · Soda · Teh</p>
      </div>
    </header>
    <main class="menu">

      <!-- Kopi Section -->
      <section class="section" id="kopi">
        <div class="section-header">
          <div class="badge">☕</div>
          <div>
            <h3>Kopi</h3>
            <p>Espresso, Latte, Cappuccino</p>
          </div>
        </div>
        <div class="drink-row">
          <article class="card">
            <div class="illustration"><img src="https://images.unsplash.com/photo-1509042239860-f550ce710b93?auto=format&fit=crop&w=200&q=80" alt="Latte Hazelnut with foam art"></div>
            <div class="meta"><h4>Latte Hazelnut</h4><p>Espresso + susu uap + hazelnut</p></div>
            <div class="price">Rp28.000</div>
          </article>
          <article class="card">
            <div class="illustration"><img src="https://images.unsplash.com/photo-1511920170033-f8396924c348?auto=format&fit=crop&w=200&q=80" alt="Single espresso shot"></div>
            <div class="meta"><h4>Espresso Single</h4><p>Shot kopi intens</p></div>
            <div class="price">Rp18.000</div>
          </article>
          <article class="card">
            <div class="illustration"><img src="https://images.unsplash.com/photo-1527168027773-0cc890c4f42e?auto=format&fit=crop&w=200&q=80" alt="Cappuccino with milk foam"></div>
            <div class="meta"><h4>Cappuccino</h4><p>Espresso + steamed milk + foam</p></div>
            <div class="price">Rp25.000</div>
          </article>
        </div>
      </section>

      <!-- Smoothies Section -->
      <section class="section" id="smoothies">
        <div class="section-header"><div class="badge">🥤</div><div><h3>Smoothies</h3><p>Buah segar & yoghurt</p></div></div>
        <div class="drink-row">
          <article class="card"><div class="illustration"><img src="https://images.unsplash.com/photo-1572441710534-6801be2d4e8b?auto=format&fit=crop&w=200&q=80" alt="Berry Bliss Smoothie"></div><div class="meta"><h4>Berry Bliss</h4><p>Strawberry, blueberry, pisang</p></div><div class="price">Rp30.000</div></article>
          <article class="card"><div class="illustration"><img src="https://images.unsplash.com/photo-1551024709-8f23befc6f87?auto=format&fit=crop&w=200&q=80" alt="Mango Mania Smoothie"></div><div class="meta"><h4>Mango Mania</h4><p>Mangga segar, susu almond</p></div><div class="price">Rp32.000</div></article>
          <article class="card"><div class="illustration"><img src="https://images.unsplash.com/photo-1585238341986-9d94b4a55dfd?auto=format&fit=crop&w=200&q=80" alt="Banana Choco Smoothie"></div><div class="meta"><h4>Banana Choco</h4><p>Pisang, cokelat, oats</p></div><div class="price">Rp28.000</div></article>
        </div>
      </section>

      <!-- Juice Section -->
      <section class="section" id="juice">
        <div class="section-header"><div class="badge">🧃</div><div><h3>Juice</h3><p>Peras segar</p></div></div>
        <div class="drink-row">
          <article class="card"><div class="illustration"><img src="https://images.unsplash.com/photo-1580910051074-7c9b4e4f6e2f?auto=format&fit=crop&w=200&q=80" alt="Orange Fresh Juice"></div><div class="meta"><h4>Orange Fresh</h4><p>Jeruk peras tanpa gula</p></div><div class="price">Rp22.000</div></article>
          <article class="card"><div class="illustration"><img src="https://images.unsplash.com/photo-1617196039897-36ad0f5bd8c1?auto=format&fit=crop&w=200&q=80" alt="Apple Juice"></div><div class="meta"><h4>Apple Juice</h4><p>Apel segar murni</p></div><div class="price">Rp24.000</div></article>
          <article class="card"><div class="illustration"><img src="https://images.unsplash.com/photo-1626178803222-eca6e8ff9e4e?auto=format&fit=crop&w=200&q=80" alt="Carrot Boost Juice"></div><div class="meta"><h4>Carrot Boost</h4><p>Wortel, jahe, lemon</p></div><div class="price">Rp26.000</div></article>
          <article class="card"><div class="illustration"><img src="https://images.unsplash.com/photo-1587202372775-98951b85b9d6?auto=format&fit=crop&w=200&q=80" alt="Pineapple Zest Juice"></div><div class="meta"><h4>Pineapple Zest</h4><p>Nanas segar tropical</p></div><div class="price">Rp25.000</div></article>
        </div>
      </section>

      <!-- Soda Section -->
      <section class="section" id="soda">
        <div class="section-header"><div class="badge">🥤</div><div><h3>Soda</h3><p>Mocktail & sparkling</p></div></div>
        <div class="drink-row">
          <article class="card"><div class="illustration"><img src="https://images.unsplash.com/photo-1621263764180-fdd7cba4e7d5?auto=format&fit=crop&w=200&q=80" alt="Lime Spark Soda"></div><div class="meta"><h4>Lime Spark</h4><p>Soda lime, mint, sirup</p></div><div class="price">Rp20.000</div></article>
          <article class="card"><div class="illustration"><img src="https://images.unsplash.com/photo-1621072156002-5ef7d56c7cc8?auto=format&fit=crop&w=200&q=80" alt="Strawberry Fizz Soda"></div><div class="meta"><h4>Strawberry Fizz</h4><p>Soda strawberry manis</p></div><div class="price">Rp22.000</div></article>
          <article class="card"><div class="illustration"><img src="https://images.unsplash.com/photo-1621072155571-83a25d816f1d?auto=format&fit=crop&w=200&q=80" alt="Peach Soda"></div><div class="meta"><h4>Peach Soda</h4><p>Soda rasa peach</p></div><div class="price">Rp23.000</div></article>
        </div>
      </section>

      <!-- Teh Section -->
      <section class="section" id="teh">
        <div class="section-header"><div class="badge">🍵</div><div><h3>Teh</h3><p>Teh hijau, hitam, milk tea</p></div></div>
        <div class="drink-row">
          <article class="card"><div class="illustration"><img src="https://images.unsplash.com/photo-1590080875833-35e7aef30c11?auto=format&fit=crop&w=200&q=80" alt="Jasmine Tea"></div><div class="meta"><h4>Jasmine Tea</h4><p>Teh melati harum</p></div><div class="price">Rp18.000</div></article>
          <article class="card"><div class="illustration"><img src="https://images.unsplash.com/photo-1573878731277-705f3b5f2d89?auto=format&fit=crop&w=200&q=80" alt="Milk Tea"></div><div class="meta"><h4>Milk Tea</h4><p>Teh hitam + susu</p></div><div class="price">Rp20.000</div></article>
          <article class="card"><div class="illustration"><img src="https://images.unsplash.com/photo-1567055656781-1b3a3aaecf3e?auto=format&fit=crop&w=200&q=80" alt="Peach Iced Tea"></div><div class="meta"><h4>Peach Iced Tea</h4><p>Teh dingin rasa peach</p></div><div class="price">Rp22.000</div></article>
        </div>
      </section>

    </main>
  </div>
</body>
</html>
