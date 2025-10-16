<!DOCTYPE html>
<html lang="en">
<head>
  <link rel="stylesheet" href="style.css">
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Waffle House</title>
  <style>
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background-image: url('https://images.unsplash.com/photo-1586985289907-7c7e2abf4c74?auto=format&fit=crop&w=1600&q=80');
      background-size: cover;
      background-attachment: fixed;
      background-position: center;
      color: #333;
    }

    .frameset-container {
      display: flex;
      flex-direction: column;
      height: 100vh;
      border: 5px solid #e67e22;
      margin: 20px;
      border-radius: 15px;
      background-image: url('https://images.unsplash.com/photo-1532634993-15f421e42ec0?auto=format&fit=crop&w=1600&q=80');
      background-size: cover;
      background-position: center;
      background-repeat: no-repeat;
      backdrop-filter: blur(2px);
      overflow: hidden;
      box-shadow: 0 4px 10px rgba(0,0,0,0.3);
    }

    .frame-top {
      background-color: rgba(211, 84, 0, 0.95);
      text-align: center;
      padding: 25px 20px;
      border-bottom: 4px solid #f1c40f;
      color: white;
      font-size: 2.3em;
      letter-spacing: 3px;
      font-weight: bold;
      text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
    }

    .nav-buttons {
      margin-top: 10px;
    }

    .nav-buttons a {
      display: inline-block;
      margin: 5px;
      padding: 8px 16px;
      font-size: 16px;
      color: #fff;
      background-color: #e67e22;
      border-radius: 5px;
      text-decoration: none;
      border: 1px solid white;
      text-shadow: 1px 1px 3px rgba(0,0,0,0.3);
    }

    .frame-bottom {
      flex: 1;
      overflow-y: auto;
      background-color: rgba(255, 255, 255, 0.88);
      padding: 40px;
    }

    h2 {
      text-align: center;
      font-size: 2em;
      text-transform: uppercase;
      color: #d35400;
      margin-bottom: 20px;
      border-bottom: 3px solid #f39c12;
      display: inline-block;
      padding-bottom: 5px;
      text-shadow: 1px 1px 4px rgba(243, 156, 18, 0.7);
    }

    section {
      border: 2px solid #f1c40f;
      border-radius: 10px;
      padding: 25px;
      margin-bottom: 30px;
      background-color: #fffef8;
      box-shadow: 0px 3px 6px rgba(0, 0, 0, 0.1);
    }

    p {
      font-size: 1.1em;
      line-height: 1.8;
      color: #444;
      text-align: center;
      max-width: 900px;
      margin: 0 auto 20px auto;
      text-shadow: 0.5px 0.5px 2px rgba(0,0,0,0.1);
    }

    .about-container {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 30px;
    }

    .about-text {
      flex: 1;
      font-size: 1.1em;
      line-height: 1.7;
      color: #333;
      text-shadow: 0.5px 0.5px 2px rgba(0,0,0,0.1);
    }

    .about-image {
      flex: 1;
      text-align: center;
    }

    .about-image img {
      width: 100%;
      max-width: 420px;
      border-radius: 15px;
      border: 3px solid #f1c40f;
      box-shadow: 0px 3px 8px rgba(0,0,0,0.2);
    }

    .services {
      display: flex;
      justify-content: center;
      gap: 20px;
    }

    .service-card {
      flex: 1 1 30%;
      border: 2px solid #f39c12;
      border-radius: 10px;
      background-color: #fffaf0;
      padding: 20px;
      text-align: center;
      box-shadow: 0px 2px 6px rgba(0, 0, 0, 0.1);
    }

    .service-card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 10px;
      border: 2px solid #f1c40f;
      margin-bottom: 15px;
      box-shadow: 0px 3px 6px rgba(0,0,0,0.2);
    }

    .service-card h3 {
      color: #e67e22;
      text-transform: uppercase;
      font-size: 1.3em;
      margin-bottom: 10px;
      text-shadow: 1px 1px 3px rgba(0,0,0,0.3);
    }

    .service-card p {
      color: #555;
      font-size: 1em;
      text-shadow: 0.5px 0.5px 2px rgba(0,0,0,0.1);
    }

    .contact-info {
      text-align: center;
      font-size: 1.1em;
      line-height: 1.6;
      color: #333;
      padding: 20px;
      border: 2px dashed #f39c12;
      background-color: #fffbea;
      border-radius: 10px;
      text-shadow: 0.5px 0.5px 2px rgba(0,0,0,0.1);
    }

    .thank-you {
      text-align: center;
      margin-top: 40px;
      font-size: 1.3em;
      font-weight: bold;
      color: #d35400;
      background-color: rgba(255, 243, 224, 0.9);
      border-radius: 10px;
      padding: 15px;
      border: 2px solid #f1c40f;
      box-shadow: 0px 3px 5px rgba(0,0,0,0.1);
      text-shadow: 1px 1px 3px rgba(243, 156, 18, 0.6);
    }
  </style>
</head>
<body>
  <div class="frameset-container">
    <div class="frame-top">
      Waffle House
      <div class="nav-buttons">
        <a href="#about">Home</a>
        <a href="#menu">Menu</a>
        <a href="#contact">Contacts</a>
      </div>
    </div>

    <div class="frame-bottom">
      <section id="about">
        <h2>About Us</h2>
        <div class="about-container">
          <div class="about-text">
            <p><strong>Welcome to Waffle House!</strong> We’re all about serving tasty homemade waffles made from local, fresh ingredients and innovative toppings that bring smiles and warmth in every serving.</p>
            <p>From classics to new flavor profiles, our menu satisfies all cravings — perfect for breakfast, brunch, or an indulgent afternoon treat.</p>
          </div>
          <div class="about-image">
            <img src="https://images.unsplash.com/photo-1509482560494-4126f8225994?auto=format&fit=crop&w=800&q=80" alt="Delicious Waffles">
          </div>
        </div>
      </section>

      <section id="menu">
        <h2>Our Menu</h2>
        <div class="services">
          <div class="service-card">
            <img src="https://images.unsplash.com/photo-1551024601-bec78aea704b?auto=format&fit=crop&w=800&q=80" alt="Belgian Waffles" />
            <h3>Belgian Waffles</h3>
            <p>Fluffy golden waffles topped with berries, syrup, and whipped cream — crisp on the outside, soft and buttery inside!</p>
          </div>

          <div class="service-card">
            <img src="https://images.unsplash.com/photo-1509440159596-0249088772ff?auto=format&fit=crop&w=800&q=80" alt="Chocolate Dream">
            <h3>Chocolate Dream</h3>
            <p>Rich cocoa waffles drizzled with warm chocolate syrup and topped with vanilla ice cream — an irresistible treat!</p>
          </div>

          <div class="service-card">
            <img src="https://images.unsplash.com/photo-1511920170033-f8396924c348?auto=format&fit=crop&w=800&q=80" alt="Mocha Delight" />
            <h3>Mocha Delight</h3>
            <p>Freshly baked mocha waffles infused with espresso and dark chocolate, topped with whipped cream and cocoa dust — pure indulgence!</p>
          </div>
        </div>
      </section>

      <section id="contact">
        <h2>Contact Us</h2>
        <div class="contact-info">
          <p><strong>Location:</strong> 143, Carl Justine Street, Magboo City</p>
          <p><strong>Phone:</strong> (143) 0993-344-456</p>
          <p><strong>Email:</strong> contact@wafflehousecafe.com</p>
        </div>
      </section>

      <div class="thank-you">
        🍽️ Thank you for visiting my shop! 🍯  
        <br>We hope to see you again soon!
      </div>
    </div>
  </div>
</body>
</html>
