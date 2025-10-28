<!--
Atithi Multi Cuisine Restaurant - Single-file HTML/CSS website
Instructions:
1) Open this file in any browser to preview the website locally.
2) Replace placeholder images (src="images/..." or the placeholder URLs) with your real image URLs or local image paths.
3) To host: upload this file to GitHub Pages, Netlify, or any static host. For GitHub Pages, create a repo and push this file as index.html.
4) For menu updates, edit the <section id="menu"> part where items are organized by category.

Made for: Atithi Multi Cuisine Restaurant
Contact: 01-5914639 / 9851346924 (WhatsApp: 9851346924)
-->

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Atithi Multi Cuisine Restaurant</title>
  <meta name="description" content="Atithi Multi Cuisine Restaurant - Greenland Chowk, Tokha Road. Order via WhatsApp or Call." />
  <style>
    :root{--accent:#d9534f;--dark:#222;--muted:#666}
    *{box-sizing:border-box}
    body{font-family:Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial; margin:0;color:var(--dark);line-height:1.4}
    header{background:linear-gradient(90deg, #ffecd2, #fcb69f);padding:18px 20px;display:flex;align-items:center;justify-content:space-between}
    .brand{display:flex;gap:12px;align-items:center}
    .brand img{width:64px;height:64px;object-fit:cover;border-radius:8px}
    .brand h1{font-size:20px;margin:0}
    nav{display:flex;gap:12px}
    nav a{color:var(--dark);text-decoration:none;padding:8px 10px;border-radius:8px}
    nav a:hover{background:rgba(0,0,0,0.06)}

    .hero{display:grid;grid-template-columns:1fr;gap:18px;padding:28px 20px;align-items:center}
    .hero-content{max-width:740px}
    .hero h2{margin:0 0 8px;font-size:28px}
    .hero p{margin:0 0 16px;color:var(--muted)}
    .cta{display:flex;gap:10px}
    .btn{background:var(--accent);color:#fff;padding:10px 14px;border-radius:10px;text-decoration:none;font-weight:600}
    .btn.call{background:#2d9cdb}

    .container{padding:18px 20px}
    .grid{display:grid;grid-template-columns:1fr 360px;gap:20px}
    @media (max-width:920px){.grid{grid-template-columns:1fr} header{flex-direction:column;align-items:flex-start} .hero{padding:18px} }

    /* Menu styles */
    .menu-category{margin-bottom:22px}
    .menu-category h3{margin:0 0 10px;background:#f7f7f7;padding:8px;border-radius:8px}
    .item{display:flex;gap:12px;padding:10px 8px;border-bottom:1px solid #eee;align-items:center}
    .item:last-child{border-bottom:none}
    .item .thumb{width:84px;height:64px;flex-shrink:0;border-radius:6px;background:#f2f2f2;display:flex;align-items:center;justify-content:center;overflow:hidden}
    .item .thumb img{width:100%;height:100%;object-fit:cover}
    .item .meta{flex:1}
    .item .meta h4{margin:0;font-size:16px}
    .item .meta p{margin:6px 0 0;color:var(--muted);font-size:14px}
    .price{font-weight:700}
    .order-actions{display:flex;flex-direction:column;gap:6px}
    .order-actions a{display:inline-block;padding:8px 10px;border-radius:8px;text-decoration:none;color:#fff;font-weight:600}
    .order-actions a.wh{background:#25D366}
    .order-actions a.call{background:#2d9cdb}

    /* Sidebar */
    .card{background:#fff;padding:14px;border-radius:10px;box-shadow:0 6px 18px rgba(0,0,0,0.06)}
    .contact-list{list-style:none;padding:0;margin:0}
    .contact-list li{padding:8px 0;border-bottom:1px dashed #eee}

    footer{padding:18px 20px;text-align:center;color:var(--muted);font-size:14px}
  </style>
</head>
<body>
  <header>
    <div class="brand">
      <img src="https://via.placeholder.com/160x160?text=Atithi+Logo" alt="Atithi Logo">
      <div>
        <h1>Atithi Multi Cuisine Restaurant</h1>
        <div style="color:var(--muted);font-size:13px">Greenland Chowk, Tokha Road</div>
      </div>
    </div>
    <nav>
      <a href="#menu">Menu</a>
      <a href="#offers">Offers</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section class="hero">
    <div class="hero-content">
      <h2>Welcome to Atithi — Taste the best of multi-cuisine delights</h2>
      <p>Fresh food, friendly service. Order by WhatsApp or call us directly for delivery and pickup. Specials every week.</p>
      <div class="cta">
        <a class="btn" href="https://wa.me/9851346924?text=Hello%20Atithi%20-%20I%20want%20to%20place%20an%20order" target="_blank">Order on WhatsApp</a>
        <a class="btn call" href="tel:+9779851346924">Call Now</a>
      </div>
    </div>
    <div style="display:flex;justify-content:center;">
      <img src="https://via.placeholder.com/420x260?text=Delicious+Food" alt="hero" style="width:100%;max-width:420px;border-radius:12px;object-fit:cover">
    </div>
  </section>

  <div class="container">
    <div class="grid">
      <main>
        <section id="menu">
          <h2 style="margin-top:0">Our Menu</h2>

          <!-- FRIDAY SPECIAL -->
          <div class="menu-category">
            <h3>FRIDAY SPECIAL</h3>
            <div class="item">
              <div class="thumb"><img src="https://via.placeholder.com/200x150?text=Fried+Chicken" alt="Crunchy Fried Chicken"></div>
              <div class="meta">
                <h4>CRUNCHY FRIED CHICKEN 8PCS BUCKET</h4>
                <p>Special price and crispy delight</p>
              </div>
              <div style="text-align:right">
                <div class="price">Rs. 999</div>
                <div class="order-actions">
                  <a class="wh" href="https://wa.me/9851346924?text=I%20want%20to%20order%20CRUNCHY%20FRIED%20CHICKEN%208PCS%20BUCKET" target="_blank">WhatsApp</a>
                  <a class="call" href="tel:+9779851346924">Call</a>
                </div>
              </div>
            </div>
          </div>

          <!-- WEDNESDAY -->
          <div class="menu-category">
            <h3>WEDNESDAY SPECIAL</h3>
            <div class="item">
              <div class="thumb"><img src="https://via.placeholder.com/200x150?text=Wings" alt="Crispy Wings"></div>
              <div class="meta">
                <h4>CRISPY WINGS 20 PCS BUCKET</h4>
                <p>Perfect for sharing</p>
              </div>
              <div style="text-align:right">
                <div class="price">Rs. 999</div>
                <div class="order-actions">
                  <a class="wh" href="https://wa.me/9851346924?text=I%20want%20to%20order%20CRISPY%20WINGS%2020%20PCS%20BUCKET" target="_blank">WhatsApp</a>
                  <a class="call" href="tel:+9779851346924">Call</a>
                </div>
              </div>
            </div>
          </div>

          <!-- VEG GRAVY (short sample) -->
          <div class="menu-category">
            <h3>VEG GRAVY</h3>
            <div class="item">
              <div class="thumb"><img src="https://via.placeholder.com/200x150?text=Dal+Tadka" alt="Dal Tadka"></div>
              <div class="meta"><h4>DAL TADKA</h4><p>Served with steamed rice or roti</p></div>
              <div style="text-align:right"><div class="price">Rs. 270</div><div class="order-actions"><a class="wh" href="https://wa.me/9851346924?text=I%20want%20to%20order%20DAL%20TADKA" target="_blank">WhatsApp</a><a class="call" href="tel:+9779851346924">Call</a></div></div>
            </div>

            <div class="item">
              <div class="thumb"><img src="https://via.placeholder.com/200x150?text=Dal+Makhani" alt="Dal Makhani"></div>
              <div class="meta"><h4>DAL MAKHANI</h4><p>Creamy and rich</p></div>
              <div style="text-align:right"><div class="price">Rs. 400</div><div class="order-actions"><a class="wh" href="https://wa.me/9851346924?text=I%20want%20to%20order%20DAL%20MAKHANI" target="_blank">WhatsApp</a><a class="call" href="tel:+9779851346924">Call</a></div></div>
            </div>

          </div>

          <!-- CHICKEN GRAVY (short sample) -->
          <div class="menu-category">
            <h3>CHICKEN GRAVY</h3>
            <div class="item">
              <div class="thumb"><img src="https://via.placeholder.com/200x150?text=Chicken+Curry" alt="Chicken Curry"></div>
              <div class="meta"><h4>CHICKEN CURRY</h4><p>Classic home-style curry</p></div>
              <div style="text-align:right"><div class="price">Rs. 340</div><div class="order-actions"><a class="wh" href="https://wa.me/9851346924?text=I%20want%20to%20order%20CHICKEN%20CURRY" target="_blank">WhatsApp</a><a class="call" href="tel:+9779851346924">Call</a></div></div>
            </div>

            <div class="item">
              <div class="thumb"><img src="https://via.placeholder.com/200x150?text=Butter+Chicken" alt="Butter Chicken"></div>
              <div class="meta"><h4>BUTTER CHICKEN</h4><p>Rich, buttery and creamy</p></div>
              <div style="text-align:right"><div class="price">Rs. 470</div><div class="order-actions"><a class="wh" href="https://wa.me/9851346924?text=I%20want%20to%20order%20BUTTER%20CHICKEN" target="_blank">WhatsApp</a><a class="call" href="tel:+9779851346924">Call</a></div></div>
            </div>

          </div>

          <!-- MOMO (sample) -->
          <div class="menu-category">
            <h3>MOMO</h3>
            <div class="item">
              <div class="thumb"><img src="https://via.placeholder.com/200x150?text=Steam+Momo" alt="Steam Momo"></div>
              <div class="meta"><h4>STEAM MOMO</h4><p>Raj / Mushroom / Buff / Chicken options available</p></div>
              <div style="text-align:right"><div class="price">Rs. 200 - 280</div><div class="order-actions"><a class="wh" href="https://wa.me/9851346924?text=I%20want%20to%20order%20STEAM%20MOMO" target="_blank">WhatsApp</a><a class="call" href="tel:+9779851346924">Call</a></div></div>
            </div>
          </div>

          <!-- FRIED CHICKEN quick sample -->
          <div class="menu-category">
            <h3>FRIED CHICKEN</h3>
            <div class="item">
              <div class="thumb"><img src="https://via.placeholder.com/200x150?text=Fried+Chicken" alt="Fried Chicken"></div>
              <div class="meta"><h4>FRIED CHICKEN (2/4/6/8 pcs)</h4><p>2pc Rs.450 | 4pc Rs.799 | 6pc Rs.1099 | 8pc Rs.1400</p></div>
              <div style="text-align:right"><div class="price">See sizes</div><div class="order-actions"><a class="wh" href="https://wa.me/9851346924?text=I%20want%20to%20order%20FRIED%20CHICKEN" target="_blank">WhatsApp</a><a class="call" href="tel:+9779851346924">Call</a></div></div>
            </div>
          </div>

          <!-- More categories can be copied here from the full menu as needed -->

        </section>

        <section id="offers" style="margin-top:24px">
          <h2>Offers & Specials</h2>
          <div style="display:grid;gap:10px;margin-top:10px">
            <div class="card">Friday Offer: Crispy Fried Chicken 8pcs bucket at Rs.1099</div>
            <div class="card">Tuesday Offer: Crispy Chicken Wings 20pcs at Rs.999</div>
            <div class="card">Monsoon Special: Check in-store for seasonal combo deals</div>
          </div>
        </section>

      </main>

      <aside>
        <div class="card">
          <h3>Contact & Order</h3>
          <ul class="contact-list">
            <li><strong>Phone:</strong> 01-5914639</li>
            <li><strong>Mobile / WhatsApp:</strong> 9851346924</li>
            <li><strong>Address:</strong> Greenland Chowk, Tokha Road</li>
            <li><strong>Hours:</strong> 11:00 AM - 11:00 PM</li>
          </ul>
          <div style="margin-top:12px;display:flex;gap:8px">
            <a class="btn" href="https://wa.me/9851346924?text=Hi%20Atithi%20-%20I%20want%20to%20order" target="_blank">Order on WhatsApp</a>
            <a class="btn call" href="tel:+9779851346924">Call Now</a>
          </div>
        </div>

        <div style="height:16px"></div>

        <div class="card">
          <h3>Location</h3>
          <!-- Replace the src below with your Google Maps embed URL or an image of the map -->
          <iframe
            src="https://www.google.com/maps?q=Greenland+Chowk+Tokha+Road&output=embed"
            width="100%" height="200" style="border:0;border-radius:8px" allowfullscreen loading="lazy"></iframe>
        </div>

        <div style="height:16px"></div>

        <div class="card">
          <h3>Follow Us</h3>
          <p style="margin:6px 0">Add your social links below:</p>
          <p style="margin:6px 0"><a href="#">Facebook</a> · <a href="#">Instagram</a></p>
        </div>

      </aside>
    </div>
  </div>

  <footer>
    © <span id="year"></span> Atithi Multi Cuisine Restaurant • All rights reserved • Terms & Conditions apply
  </footer>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
