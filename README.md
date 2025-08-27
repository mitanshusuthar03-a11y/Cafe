# Cafe
This is my first github Repository
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>FastBite Cafe</title>
  <style>
    * {margin:0; padding:0; box-sizing:border-box; font-family:'Poppins', sans-serif;}
    body {background:#fafafa; color:#333;}

    /* Navbar */
    nav {position:fixed;top:0;left:0;width:100%;background:rgba(0,0,0,0.7);
      padding:15px 50px;display:flex;justify-content:space-between;align-items:center;
      color:white;z-index:1000;}
    nav h2 {font-size:26px;font-weight:bold;color:#ffcc00;}
    nav ul {list-style:none;display:flex;gap:20px;}
    nav ul li a {text-decoration:none;color:white;font-weight:500;}
    nav ul li a:hover {color:#ffcc00;}

    /* Hero */
    header {height:100vh;background:url('https://images.unsplash.com/photo-1607013251379-e6eecfffe234?auto=format&fit=crop&w=1600&q=80') no-repeat center/cover;
      display:flex;align-items:center;justify-content:center;text-align:center;color:white;}
    header h1 {font-size:4rem;color:#ffcc00;text-shadow:2px 2px 15px rgba(0,0,0,0.7);}
    header p {font-size:1.5rem;margin-top:15px;text-shadow:2px 2px 10px rgba(0,0,0,0.6);}

    section {padding:80px 10%;}
    .menu h2,.about h2,.contact h2 {text-align:center;font-size:2.5rem;margin-bottom:40px;color:#e63946;}

    /* Menu Cards */
    .menu-items {display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:30px;}
    .card {background:white;padding:20px;border-radius:15px;
      box-shadow:0 5px 15px rgba(0,0,0,0.15);text-align:center;transition:transform 0.3s;}
    .card:hover {transform:translateY(-10px);}
    .card img {width:100%;height:200px;object-fit:cover;border-radius:12px;margin-bottom:15px;}
    .card h3 {margin-bottom:10px;color:#e63946;}
    .card a {display:inline-block;margin-top:10px;padding:10px 20px;background:#e63946;
      color:white;text-decoration:none;border-radius:8px;transition:0.3s;}
    .card a:hover {background:#ff3b3b;}

    /* About */
    .about {background:#fbeae7;text-align:center;}
    .about p {max-width:700px;margin:auto;font-size:1.2rem;line-height:1.8;}

    /* Contact */
    .contact {background:#e63946;color:white;text-align:center;}
    .contact p {font-size:1.2rem;}
    footer {background:#1c1c1c;color:#ccc;text-align:center;padding:15px;}

    /* Popup Modal */
    .modal {position:fixed;top:0;left:0;width:100%;height:100%;
      background:rgba(0,0,0,0.8);display:none;align-items:center;justify-content:center;z-index:2000;}
    .modal:target {display:flex;}
    .modal-content {background:white;padding:30px;border-radius:15px;
      max-width:400px;width:90%;text-align:center;position:relative;}
    .modal-content h3 {color:#e63946;margin-bottom:10px;}
    .modal-content p {margin-bottom:20px;font-size:1.2rem;}
    .modal-content a.close {position:absolute;top:10px;right:15px;
      text-decoration:none;font-size:22px;color:#333;}
    .order-btn {display:inline-block;padding:12px 25px;background:#e63946;
      color:white;text-decoration:none;border-radius:8px;}
    .order-btn:hover {background:#ff3b3b;}
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav>
    <h2>FastBite Cafe</h2>
    <ul>
      <li><a href="#menu">Menu</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <!-- Hero -->
  <header>
    <div>
      <h1>FastBite Cafe</h1>
      <p>Pizza • Burgers • Shakes – Fresh & Delicious</p>
    </div>
  </header>

  <!-- Menu -->
  <section id="menu" class="menu">
    <h2>Our Menu</h2>
    <div class="menu-items">
      <div class="card">
        <img src="https://images.unsplash.com/photo-1594007654729-407eedc4be65?auto=format&fit=crop&w=800&q=80" alt="Pizza">
        <h3>Cheesy Pizza</h3>
        <p>Loaded with mozzarella & toppings.</p>
        <a href="#pizza">Order Now</a>
      </div>
      <div class="card">
        <img src="https://images.unsplash.com/photo-1550547660-d9450f859349?auto=format&fit=crop&w=800&q=80" alt="Burger">
        <h3>Juicy Burger</h3>
        <p>Grilled patty with cheese & sauces.</p>
        <a href="#burger">Order Now</a>
      </div>
      <div class="card">
        <img src="chocolate-milkshake.png"alt="Shake">
        <h3>Choco Shake</h3>
        <p>Creamy & rich milkshake.</p>
        <a href="#shake">Order Now</a>
      </div>
    </div>
  </section>

  <!-- About -->
  <section id="about" class="about">
    <h2>About Us</h2>
    <p>
      At FastBite Cafe, we serve handcrafted pizzas, juicy burgers, and irresistible shakes made with love.  
      Fresh, quick, and always delicious – your favorite fast food, reimagined!
    </p>
  </section>

  <!-- Contact -->
  <section id="contact" class="contact">
    <h2>Contact Us</h2>
    <p>Email: order@fastbitecafe.com</p>
    <p>Phone: +91 9876543210</p>
    <p>Address: 77 Food Street, Delhi, India</p>
  </section>

  <!-- Footer -->
  <footer>
    <p>© 2025 FastBite Cafe. All Rights Reserved.</p>
  </footer>

  <!-- Modals -->
  <div id="pizza" class="modal">
    <div class="modal-content">
      <a href="#" class="close">✖</a>
      <h3>Cheesy Pizza</h3>
      <p>₹299 – Large | ₹199 – Medium | ₹129 – Small</p>
      <a href="#contact" class="order-btn">Order Now</a>
    </div>
  </div>

  <div id="burger" class="modal">
    <div class="modal-content">
      <a href="#" class="close">✖</a>
      <h3>Juicy Burger</h3>
      <p>₹149 – Classic | ₹199 – Double Cheese</p>
      <a href="#contact" class="order-btn">Order Now</a>
    </div>
  </div>

  <div id="shake" class="modal">
    <div class="modal-content">
      <a href="#" class="close">✖</a>
      <h3>Choco Shake</h3>
      <p>₹99 – Regular | ₹149 – Large</p>
      <a href="#contact" class="order-btn">Order Now</a>
    </div>
  </div>

</body>
</html>

