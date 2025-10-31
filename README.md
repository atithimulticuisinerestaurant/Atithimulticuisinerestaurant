Atithi Multi Cuisine Restaurant - Full Menu Classic Single-file HTML/CSS website
Instructions:
1) Open this file in any browser to preview the website locally.
2) Replace placeholder images (src="images/..." or the placeholder URLs) with your real image URLs or local image paths.
3) To host: upload this file to GitHub Pages, Netlify, or any static host. For GitHub Pages, create a repo and push this file as index.html.
4) For quick edits, open the file in a text editor and update the menu inside the <section id="menu"> block.

Made for: Atithi Multi Cuisine Restaurant
Contact: 01-5914639 / 9851346924 (WhatsApp: 9851346924)
Style: Classic restaurant look (warm colors, food background, elegant fonts)
-->

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Atithi Multi Cuisine Restaurant • Greenland Chowk, Tokha Road</title>
  <meta name="description" content="Atithi Multi Cuisine Restaurant — Nepali, Indian & Continental cuisine in Tokha. Order via WhatsApp or call 9851346924. Free delivery within 6 km." />
  <style>
    :root{--accent:#c43b31;--accent-dark:#942825;--bg:#fff6f4;--card:#fff;--muted:#6b6b6b}
    *{box-sizing:border-box}
    body{font-family:'Playfair Display', Georgia, serif;margin:0;color:#222;background:var(--bg);line-height:1.45}

    header{background:linear-gradient(90deg, rgba(196,59,49,0.12), rgba(255,230,220,0.08));padding:18px 24px;display:flex;align-items:center;justify-content:space-between}
    .brand{display:flex;gap:14px;align-items:center}
    .brand img{width:72px;height:72px;object-fit:cover;border-radius:10px;border:3px solid rgba(255,255,255,0.6)}
    .brand h1{font-size:20px;margin:0;font-weight:700}
    .brand p{margin:0;color:var(--muted);font-size:13px}
    nav{display:flex;gap:12px}
    nav a{color:var(--accent-dark);text-decoration:none;padding:8px 10px;border-radius:8px;font-weight:600}
    nav a:hover{background:rgba(0,0,0,0.04)}

    .hero{display:flex;gap:20px;align-items:center;padding:28px 24px;background-image:url('https://images.unsplash.com/photo-1544025162-d76694265947?auto=format&fit=crop&w=1500&q=60');background-size:cover;background-position:center;color:white}
    .hero-overlay{background:linear-gradient(180deg, rgba(0,0,0,0.35), rgba(0,0,0,0.45));padding:36px;border-radius:12px;max-width:820px}
    .hero h2{margin:0 0 8px;font-size:34px;font-family:'Playfair Display', serif}
    .hero p{margin:0 0 14px;color:rgba(255,255,255,0.95)}
    .cta{display:flex;gap:12px}
    .btn{background:var(--accent);color:#fff;padding:10px 16px;border-radius:10px;text-decoration:none;font-weight:700}
    .btn.ghost{background:transparent;border:2px solid rgba(255,255,255,0.25)}

    .container{padding:24px}
    .grid{display:grid;grid-template-columns:1fr 360px;gap:24px}
    @media (max-width:980px){.grid{grid-template-columns:1fr} .hero{flex-direction:column;align-items:flex-start}}

    /* Menu */
    .menu-wrap{background:transparent}
    .menu-category{margin-bottom:18px}
    .menu-category h3{margin:0 0 10px;padding:10px 12px;background:var(--card);border-radius:8px;font-family:inherit;color:var(--accent-dark);box-shadow:0 6px 18px rgba(0,0,0,0.04)}
    .item{display:flex;gap:12px;padding:10px 8px;border-bottom:1px dashed #eee;align-items:center;background:var(--card);border-radius:8px;margin-bottom:10px}
    .item .thumb{width:96px;height:76px;flex-shrink:0;border-radius:8px;background:#f4f4f4;overflow:hidden}
    .item .thumb img{width:100%;height:100%;object-fit:cover}
    .item .meta{flex:1}
    .item .meta h4{margin:0;font-size:16px;font-weight:700}
    .item .meta p{margin:6px 0 0;color:var(--muted);font-size:14px}
    .price{font-weight:800;color:var(--accent-dark)}
    .order-actions{display:flex;flex-direction:column;gap:8px}
    .order-actions a{display:inline-block;padding:8px 10px;border-radius:8px;text-decoration:none;color:#fff;font-weight:700}
    .order-actions a.wh{background:#25D366}
    .order-actions a.call{background:#2d9cdb}

    /* Sidebar */
    .card{background:var(--card);padding:14px;border-radius:12px;box-shadow:0 8px 24px rgba(0,0,0,0.06)}
    .contact-list{list-style:none;padding:0;margin:0}
    .contact-list li{padding:10px 0;border-bottom:1px dashed #f0f0f0}

    footer{padding:18px 20px;text-align:center;color:var(--muted);font-size:14px}
  </style>
</head>
<body>
  <header>
    <div class="brand">
      <img src="https://via.placeholder.com/240x240?text=Atithi+Logo" alt="Atithi Logo">
      <div>
        <h1>Atithi Multi Cuisine Restaurant</h1>
        <p>Greenland Chowk, Tokha Road • Call: 01-5914639 / 9851346924</p>
      </div>
    </div>
    <nav>
      <a href="#menu">Menu</a>
      <a href="#offers">Offers</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section class="hero">
    <div class="hero-overlay">
      <h2>Atithi — Where every meal is a warm welcome</h2>
      <p>Experience authentic flavors across Nepali, Indian and Continental cuisines. Fresh ingredients, generous portions, and special weekly offers.</p>
      <div class="cta">
        <a class="btn" href="https://wa.me/9851346924?text=Hello%20Atithi%20-%20I%20want%20to%20place%20an%20order" target="_blank">Order on WhatsApp</a>
        <a class="btn ghost" href="tel:+9779851346924">Call Now</a>
      </div>
    </div>
  </section>

  <div class="container">
    <div class="grid">
      <main>
        <section id="menu" class="menu-wrap">
          <h2 style="margin-top:0;font-family:'Playfair Display', serif">Full Menu</h2>

          <!-- FRIDAY SPECIAL -->
          <div class="menu-category">
            <h3>FRIDAY SPECIAL</h3>
            <div class="item">
              <div class="thumb"><img src="https://via.placeholder.com/320x240?text=Fried+Chicken" alt="Crunchy Fried Chicken"></div>
              <div class="meta"><h4>CRUNCHY FRIED CHICKEN 8PCS BUCKET</h4><p>Special crispy bucket for sharing</p></div>
              <div style="text-align:right"><div class="price">Rs. 999</div><div class="order-actions"><a class="wh" href="https://wa.me/9851346924?text=I%20want%20to%20order%20CRUNCHY%20FRIED%20CHICKEN%208PCS%20BUCKET" target="_blank">WhatsApp</a><a class="call" href="tel:+9779851346924">Call</a></div></div>
            </div>
          </div>

          <!-- WEDNESDAY SPECIAL -->
          <div class="menu-category">
            <h3>WEDNESDAY SPECIAL</h3>
            <div class="item">
              <div class="thumb"><img src="https://via.placeholder.com/320x240?text=Wings" alt="Crispy Wings"></div>
              <div class="meta"><h4>CRISPY WINGS 20 PCS BUCKET</h4><p>Perfect for groups</p></div>
              <div style="text-align:right"><div class="price">Rs. 999</div><div class="order-actions"><a class="wh" href="https://wa.me/9851346924?text=I%20want%20to%20order%20CRISPY%20WINGS%2020%20PCS%20BUCKET" target="_blank">WhatsApp</a><a class="call" href="tel:+9779851346924">Call</a></div></div>
            </div>
          </div>

          <!-- VEG GRAVY -->
          <div class="menu-category">
            <h3>VEG GRAVY</h3>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Dal+Tadka"></div><div class="meta"><h4>DAL TADKA</h4><p>Served hot with rice or roti</p></div><div style="text-align:right"><div class="price">Rs. 270</div><div class="order-actions"><a class="wh" href="https://wa.me/9851346924?text=I%20want%20to%20order%20DAL%20TADKA" target="_blank">WhatsApp</a><a class="call" href="tel:+9779851346924">Call</a></div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Dal+Makhani"></div><div class="meta"><h4>DAL MAKHANI</h4><p>Creamy and richly spiced</p></div><div style="text-align:right"><div class="price">Rs. 400</div><div class="order-actions"><a class="wh" href="https://wa.me/9851346924?text=I%20want%20to%20order%20DAL%20MAKHANI" target="_blank">WhatsApp</a><a class="call" href="tel:+9779851346924">Call</a></div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Rajma"></div><div class="meta"><h4>RAJMA</h4><p>Homestyle rajma with aromatic spices</p></div><div style="text-align:right"><div class="price">Rs. 270</div><div class="order-actions"><a class="wh" href="https://wa.me/9851346924?text=I%20want%20to%20order%20RAJMA" target="_blank">WhatsApp</a><a class="call" href="tel:+9779851346924">Call</a></div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Mixed+Veg"></div><div class="meta"><h4>MIXED VEG</h4><p>Seasonal vegetables cooked with light spices</p></div><div style="text-align:right"><div class="price">Rs. 340</div><div class="order-actions"><a class="wh" href="https://wa.me/9851346924?text=I%20want%20to%20order%20MIXED%20VEG" target="_blank">WhatsApp</a><a class="call" href="tel:+9779851346924">Call</a></div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Matar+Paneer"></div><div class="meta"><h4>MATAR PANEER</h4><p>Classic matar-paneer curry</p></div><div style="text-align:right"><div class="price">Rs. 340</div><div class="order-actions"><a class="wh" href="https://wa.me/9851346924?text=I%20want%20to%20order%20MATAR%20PANEER" target="_blank">WhatsApp</a><a class="call" href="tel:+9779851346924">Call</a></div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Paneer+Butter+Masala"></div><div class="meta"><h4>PANEER BUTTER MASALA</h4><p>Rich tomato & butter-based curry</p></div><div style="text-align:right"><div class="price">Rs. 470</div><div class="order-actions"><a class="wh" href="https://wa.me/9851346924?text=I%20want%20to%20order%20PANEER%20BUTTER%20MASALA" target="_blank">WhatsApp</a><a class="call" href="tel:+9779851346924">Call</a></div></div></div>
          </div>

          <!-- CHICKEN GRAVY -->
          <div class="menu-category">
            <h3>CHICKEN & MUTTON GRAVY</h3>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Chicken+Curry"></div><div class="meta"><h4>CHICKEN CURRY</h4><p>Classic home-style curry</p></div><div style="text-align:right"><div class="price">Rs. 340</div><div class="order-actions"><a class="wh" href="https://wa.me/9851346924?text=I%20want%20to%20order%20CHICKEN%20CURRY" target="_blank">WhatsApp</a><a class="call" href="tel:+9779851346924">Call</a></div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Mutton+Curry"></div><div class="meta"><h4>MUTTON CURRY</h4><p>Slow-cooked for deep flavor</p></div><div style="text-align:right"><div class="price">Rs. 470</div><div class="order-actions"><a class="wh" href="https://wa.me/9851346924?text=I%20want%20to%20order%20MUTTON%20CURRY" target="_blank">WhatsApp</a><a class="call" href="tel:+9779851346924">Call</a></div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Butter+Chicken"></div><div class="meta"><h4>BUTTER CHICKEN</h4><p>Rich buttery tomato gravy</p></div><div style="text-align:right"><div class="price">Rs. 470</div><div class="order-actions"><a class="wh" href="https://wa.me/9851346924?text=I%20want%20to%20order%20BUTTER%20CHICKEN" target="_blank">WhatsApp</a><a class="call" href="tel:+9779851346924">Call</a></div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Chicken+Rara"></div><div class="meta"><h4>CHICKEN RARA</h4><p>Chef's special spicy preparation</p></div><div style="text-align:right"><div class="price">Rs. 530</div><div class="order-actions"><a class="wh" href="https://wa.me/9851346924?text=I%20want%20to%20order%20CHICKEN%20RARA" target="_blank">WhatsApp</a><a class="call" href="tel:+9779851346924">Call</a></div></div></div>
          </div>

          <!-- ROTI / NAAN -->
          <div class="menu-category">
            <h3>ROTI • NAAN</h3>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Tandoori+Roti"></div><div class="meta"><h4>TANDOORI ROTI</h4></div><div style="text-align:right"><div class="price">Rs. 50</div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Butter+Naan"></div><div class="meta"><h4>BUTTER NAAN</h4></div><div style="text-align:right"><div class="price">Rs. 90</div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Garlic+Naan"></div><div class="meta"><h4>GARLIC NAAN</h4></div><div style="text-align:right"><div class="price">Rs. 140</div></div></div>
          </div>

          <!-- VEG SNACKS -->
          <div class="menu-category">
            <h3>VEG SNACKS</h3>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=French+Fries"></div><div class="meta"><h4>FRENCH FRIES</h4><p>Lightly salted</p></div><div style="text-align:right"><div class="price">Rs. 299</div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Masala+Fries"></div><div class="meta"><h4>MASALA FRIES</h4></div><div style="text-align:right"><div class="price">Rs. 349</div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Paneer+Tikka"></div><div class="meta"><h4>PANEER TIKKA</h4><p>Char-grilled paneer</p></div><div style="text-align:right"><div class="price">Rs. 549</div></div></div>
          </div>

          <!-- CHICKEN SNACKS -->
          <div class="menu-category">
            <h3>CHICKEN SNACKS</h3>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Chilly+Chicken"></div><div class="meta"><h4>CHILLY CHICKEN</h4></div><div style="text-align:right"><div class="price">Rs. 399</div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Lollypop"></div><div class="meta"><h4>CHICKEN LOLLYPOP</h4></div><div style="text-align:right"><div class="price">Rs. 399</div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Chicken+Tikka"></div><div class="meta"><h4>CHICKEN TIKKA</h4><p>Boneless skewers</p></div><div style="text-align:right"><div class="price">Rs. 599</div></div></div>
          </div>

          <!-- ATITHI SPECIAL -->
          <div class="menu-category">
            <h3>ATITHI SPECIAL</h3>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Pork+Ribs"></div><div class="meta"><h4>PORK RIBS</h4></div><div style="text-align:right"><div class="price">Rs. 499</div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Mutton+Bhutan"></div><div class="meta"><h4>MUTTON BHUTAN</h4></div><div style="text-align:right"><div class="price">Rs. 399</div></div></div>
          </div>

          <!-- BIRYANI -->
          <div class="menu-category">
            <h3>BIRYANI</h3>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Veg+Biryani"></div><div class="meta"><h4>VEG DUM BIRYANI</h4></div><div style="text-align:right"><div class="price">Rs. 500</div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Chicken+Biryani"></div><div class="meta"><h4>CHICKEN DUM BIRYANI</h4></div><div style="text-align:right"><div class="price">Rs. 600</div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Mutton+Biryani"></div><div class="meta"><h4>MUTTON DUM BIRYANI</h4></div><div style="text-align:right"><div class="price">Rs. 750</div></div></div>
          </div>

          <!-- SALAD -->
          <div class="menu-category">
            <h3>SALAD</h3>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Chicken+Salad"></div><div class="meta"><h4>SPICY CHICKEN SALAD</h4></div><div style="text-align:right"><div class="price">Rs. 300</div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Fruit+Salad"></div><div class="meta"><h4>FRUIT SALAD</h4></div><div style="text-align:right"><div class="price">Rs. 450</div></div></div>
          </div>

          <!-- MOMO -->
          <div class="menu-category">
            <h3>MOMO</h3>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Steam+Momo"></div><div class="meta"><h4>STEAM MOMO</h4><p>Raj / Mushroom / Buff / Chicken available</p></div><div style="text-align:right"><div class="price">Rs. 200 - 280</div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Kothey"></div><div class="meta"><h4>KOTHEY MOMO</h4></div><div style="text-align:right"><div class="price">Rs. 250 - 299</div></div></div>
          </div>

          <!-- SEKUWA -->
          <div class="menu-category">
            <h3>SEKUWA</h3>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Chicken+Sekuwa"></div><div class="meta"><h4>CHICKEN SEKUWA</h4><p>Plate / Half Kg / Full Kg available</p></div><div style="text-align:right"><div class="price">Rs. 399 / 799 / 1499</div></div></div>
          </div>

          <!-- CHINESE -->
          <div class="menu-category">
            <h3>CHINESE</h3>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Hakka+Noodles"></div><div class="meta"><h4>HAKKA NOODLES</h4><p>Veg / Egg / Chicken / Mix</p></div><div style="text-align:right"><div class="price">Rs. 249 - 325</div></div></div>
          </div>

          <!-- FISH & SEAFOOD -->
          <div class="menu-category">
            <h3>FISH & SEAFOOD</h3>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Fish+Amritsari"></div><div class="meta"><h4>FISH AMRITSARI</h4></div><div style="text-align:right"><div class="price">Rs. 399</div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Golden+Prawns"></div><div class="meta"><h4>GOLDEN FRIED PRAWNS</h4></div><div style="text-align:right"><div class="price">Rs. 699</div></div></div>
          </div>

          <!-- FRIED CHICKEN -->
          <div class="menu-category">
            <h3>FRIED CHICKEN</h3>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Fried+Chicken+2pc"></div><div class="meta"><h4>FRIED CHICKEN — 2 / 4 / 6 / 8 PCS</h4><p>2pc Rs.450 | 4pc Rs.799 | 6pc Rs.1099 | 8pc Rs.1400</p></div><div style="text-align:right"><div class="price">See sizes</div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Chicken+Popcorn"></div><div class="meta"><h4>CHICKEN POPCORN</h4></div><div style="text-align:right"><div class="price">Rs. 299</div></div></div>
          </div>

          <!-- PASTA & FASTFOOD -->
          <div class="menu-category">
            <h3>PASTA • SANDWICH • BURGER • WRAP</h3>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Pasta"></div><div class="meta"><h4>CARBONARA / ARRABBIATA / AGLIO E OLIO</h4><p>Veg Rs.349 | Chicken Rs.399</p></div><div style="text-align:right"><div class="price">Rs. 349 - 399</div></div></div>
            <div class="item"><div class="thumb"><img src="https://via.placeholder.com/320x240?text=Burger"></div><div class="meta"><h4>BURGER / SANDWICH / WRAP</h4><p>Veg Rs.299 | Chicken Rs.349</p></div><div style="text-align:right"><div class="price">Rs. 299 - 349</div></div></div>
          </div>

          <!-- OFFERS SUMMARY -->
          <div id="offers" class="menu-category">
            <h3>OFFERS & SPECIALS</h3>
            <div class="item" style="background:linear-gradient(90deg,#fff7f6,#fffefa);"><div class="meta"><h4>Friday Offer</h4><p>Crispy Fried Chicken 8pcs bucket at Rs.1099</p></div></div>
            <div class="item" style="background:linear-gradient(90deg,#fff7f6,#fffefa);"><div class="meta"><h4>Tuesday Offer</h4><p>Crispy Chicken Wings 20pcs at Rs.999</p></div></div>
          </div>

        </section>

      </main>

      <aside>
        <div class="card">
          <h3>Contact & Order</h3>
          <ul class="contact-list">
            <li><strong>Phone:</strong> 01-5914639</li>
            <li><strong>Mobile / WhatsApp:</strong> <a href="https://wa.me/9851346924">9851346924</a></li>
            <li><strong>Address:</strong> Greenland Chowk, Tokha Road, Kathmandu, Nepal</li>
            <li><strong>Hours:</strong> 11:00 AM - 11:00 PM</li>
            <li><strong>Delivery:</strong> Free within 6 km; partners: Foodmandu, Hello Service Nepal</li>
          </ul>
          <div style="margin-top:12px;display:flex;gap:8px">
            <a class="btn" href="https://wa.me/9851346924?text=Hi%20Atithi%20-%20I%20want%20to%20order" target="_blank">Order on WhatsApp</a>
            <a class="btn ghost" href="tel:+9779851346924">Call Now</a>
          </div>
        </div>

        <div style="height:16px"></div>

        <div class="card">
          <h3>Location</h3>
          <iframe src="https://www.google.com/maps?q=Greenland+Chowk+Tokha+Road+Kathmandu&output=embed" width="100%" height="200" style="border:0;border-radius:8px" allowfullscreen loading="lazy"></iframe>
        </div>

        <div style="height:16px"></div>

        <div class="card">
          <h3>Policies</h3>
          <p style="margin:6px 0;color:var(--muted)">Orders accepted via WhatsApp or Call. Cancellation within 10 minutes for full refund (if pre-paid). Delivery times may vary. For full Terms & Conditions, contact us.</p>
        </div>
      </aside>
    </div>
  </div>

  <footer>
    © <span id="year"></span> Atithi Multi Cuisine Restaurant • All rights reserved • <a href="#contact">Contact us</a>
  </footer>

  <script>document.getElementById('year').textContent = new Date().getFullYear();</script>
</body>
</html>
