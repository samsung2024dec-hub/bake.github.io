<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Good Morning Bakery</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            background-color: #fff8f0;
            color: #5a342e;
            line-height: 1.6;
        }
        header {
            background-color: #f9a03f;
            color: white;
            padding: 20px 0;
            text-align: center;
            box-shadow: 0 4px 6px -1px rgba(0,0,0,0.1);
        }
        header h1 {
            margin: 0;
            font-size: 2.8rem;
            font-weight: 900;
            letter-spacing: 3px;
        }
        nav {
            background-color: #fbcc80;
            display: flex;
            justify-content: center;
            padding: 12px 0;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        nav a {
            color: #5a342e;
            text-decoration: none;
            margin: 0 20px;
            font-size: 1.1rem;
            font-weight: 600;
            transition: color 0.3s ease;
        }
        nav a:hover {
            color: #d46a07;
        }
        .hero {
            background-image: url('https://images.unsplash.com/photo-1565958011703-44f9829ba187?auto=format&fit=crop&w=1200&q=80');
            background-size: cover;
            background-position: center center;
            height: 300px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            text-shadow: 0 2px 6px rgba(0,0,0,0.55);
            font-size: 2.5rem;
            font-weight: 700;
            letter-spacing: 2px;
        }
        main {
            max-width: 1000px;
            margin: 30px auto;
            padding: 0 20px;
        }
        section {
            margin-bottom: 40px;
        }
        section h2 {
            font-size: 2rem;
            border-bottom: 3px solid #f9a03f;
            padding-bottom: 8px;
            margin-bottom: 15px;
            font-weight: 700;
        }
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit,minmax(250px,1fr));
            gap: 20px;
        }
        .product-card {
            background: white;
            border-radius: 8px;
            box-shadow: 0 2px 6px rgba(0,0,0,0.1);
            overflow: hidden;
            transition: transform 0.3s ease;
        }
        .product-card:hover {
            transform: translateY(-6px);
        }
        .product-card img {
            width: 100%;
            height: 180px;
            object-fit: cover;
        }
        .product-details {
            padding: 15px 18px;
        }
        .product-title {
            font-weight: 700;
            font-size: 1.1rem;
            margin: 0 0 6px 0;
        }
        .product-desc {
            font-size: 0.95rem;
            color: #7d574a;
            margin-bottom: 10px;
        }
        .product-price {
            font-weight: 700;
            color: #d46a07;
            font-size: 1.05rem;
        }
        footer {
            text-align: center;
            background-color: #fbcc80;
            color: #5a342e;
            font-size: 0.9rem;
            padding: 15px 0;
            margin-top: 50px;
            box-shadow: 0 -2px 4px rgba(0,0,0,0.1);
        }
        /* Responsive text */
        @media (max-width: 600px) {
            header h1 {
                font-size: 2rem;
            }
            nav a {
                margin: 0 12px;
                font-size: 1rem;
            }
            .hero {
                font-size: 1.8rem;
                height: 220px;
                padding: 0 10px;
                text-align: center;
            }
        }
    </style>
</head>
<body>

<header>
    <h1>Good Morning Bakery</h1>
</header>

<nav>
    <a href="#products">Products</a>
    <a href="#about">About Us</a>
    <a href="#contact">Contact</a>
</nav>

<div class="hero">
    Freshly Baked Delights Every Morning
</div>

<main>

<section id="products">
    <h2>Our Best Sellers</h2>
    <div class="product-grid">

        <div class="product-card">
          <img src="https://images.unsplash.com/photo-1558021212-51b6cb8a9e54?auto=format&fit=crop&w=600&q=80" alt="Soft Bread Loaf" />
          <div class="product-details">
              <h3 class="product-title">Soft Wheat Bread</h3>
              <p class="product-desc">Freshly baked, soft and fluffy whole wheat bread loaf perfect for your breakfast.</p>
              <p class="product-price">₹70 / loaf</p>
          </div>
        </div>

        <div class="product-card">
          <img src="https://images.unsplash.com/photo-1542831371-29b0f74f9713?auto=format&fit=crop&w=600&q=80" alt="Butter Croissant" />
          <div class="product-details">
              <h3 class="product-title">Butter Croissant</h3>
              <p class="product-desc">Golden, flaky croissants with rich buttery flavor to start your day right.</p>
              <p class="product-price">₹50 / piece</p>
          </div>
        </div>

        <div class="product-card">
          <img src="https://images.unsplash.com/photo-1562440499-459d2e548a34?auto=format&fit=crop&w=600&q=80" alt="Sweet Cookies" />
          <div class="product-details">
              <h3 class="product-title">Chocolate Chip Cookies</h3>
              <p class="product-desc">Chewy and delicious cookies loaded with chocolate chips. Perfect with a cup of tea.</p>
              <p class="product-price">₹120 / pack</p>
          </div>
        </div>

        <div class="product-card">
          <img src="https://images.unsplash.com/photo-1511689983235-0f8581befc09?auto=format&fit=crop&w=600&q=80" alt="Fresh Rusks" />
          <div class="product-details">
              <h3 class="product-title">Crispy Rusks</h3>
              <p class="product-desc">Crispy and light, ideal for dipping into your morning coffee.</p>
              <p class="product-price">₹80 / pack</p>
          </div>
        </div>

    </div>
</section>

<section id="about">
    <h2>About Us</h2>
    <p>Good Morning Bakery is dedicated to bringing you the freshest and most delicious baked goods each morning. Our products are made with premium ingredients and baked fresh daily to ensure quality and taste that brighten your day.</p>
</section>

<section id="contact">
    <h2>Contact Us</h2>
    <p>Phone: +91 12345 67890</p>
    <p>Email: contact@goodmorningbakery.com</p>
    <p>Visit us at: 123 Bakery Street, Your City</p>
</section>

</main>

<footer>
    <p>© 2025 Good Morning Bakery. All rights reserved.</p>
</footer>

</body>
</html>
