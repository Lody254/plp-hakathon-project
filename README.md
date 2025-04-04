!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Kenya Real Estate</title>
  <style>
    /* General Styles */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }

    header {
      padding: 20px;
      background-color: #333;
      color: white;
      text-align: center;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin: 0 15px;
      font-weight: bold;
    }

    footer {
      padding: 10px;
      background-color: #333;
      color: white;
      text-align: center;
    }

    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 20px;
    }

    /* Listings Section */
    .listings {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 20px;
      padding: 20px;
    }

    .card {
      border: 1px solid #ccc;
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }

    .card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }

    .card-body {
      padding: 15px;
    }

    .tag {
      display: inline-block;
      background-color: #007bff;
      color: #fff;
      padding: 5px 10px;
      border-radius: 5px;
      font-size: 0.9em;
      margin-bottom: 10px;
    }

    .view-btn {
      display: inline-block;
      margin-top: 10px;
      background: #28a745;
      color: #fff;
      padding: 8px 12px;
      text-decoration: none;
      border-radius: 5px;
    }

    /* Filter Section */
    .filter-section {
      display: flex;
      gap: 10px;
      margin-bottom: 20px;
    }

    select,
    input {
      padding: 8px;
      font-size: 1em;
      width: 200px;
    }

    /* Map Section */
    .map-section {
      margin-top: 40px;
      background-color: #f8f9fa;
      padding: 20px;
      border-radius: 10px;
    }

    /* Contact Us Section */
    .contact-form h2 {
      font-weight: bold;
      color: #FFA500; /* Orange color */
      font-size: 1.8em;
      margin-bottom: 20px;
    }

    .contact-form input,
    .contact-form textarea {
      padding: 10px;
      font-size: 1em;
      width: 100%;
      border: 2px solid #ccc;
      border-radius: 5px;
      margin-bottom: 10px;
    }

    .contact-form button {
      background-color: #FFA500; /* Orange color */
      color: white;
      padding: 10px;
      font-size: 1em;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      font-weight: bold;
    }

    .contact-form button:hover {
      background-color: #e68900; /* Slightly darker orange for hover effect */
    }

    .whatsapp-btn {
      display: inline-block;
      margin-top: 20px;
      background-color: #25d366;
      color: white;
      padding: 10px 15px;
      text-decoration: none;
      border-radius: 5px;
    }

    /* Map iframe visibility */
    iframe {
      width: 100%;
      height: 480px;
      border: none;
    }
  </style>
</head>

<body>
  <header>
    <h1>Kenya Real Estate</h1>
    <nav>
      <a href="#">Home</a>
      <a href="#listings">Listings</a>
      <a href="#map">Map</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <div class="container">
    <section class="filter-section">
      <select>
        <option>Location</option>
        <option>Nairobi</option>
        <option>Mombasa</option>
        <option>Kisumu</option>
        <option>Nakuru</option>
      </select>
      <select>
        <option>Type</option>
        <option>Apartment</option>
        <option>House</option>
        <option>Land</option>
        <option>Commercial</option>
      </select>
      <input type="text" placeholder="Max Price (KES)">
    </section>

    <section id="listings" class="listings">
      <!-- Property Listings -->
      <div class="card">
        <img src="4.jpg" alt="House in Nairobi">
        <div class="card-body">
          <h3>Modern House - Nairobi</h3>
          <span class="tag">KES 12M</span>
          <p>4 Bedroom House in Kilimani, gated community with ample parking.</p>
          <a class="view-btn" href="#">View More</a>
        </div>
      </div>
      <div class="card">
        <img src="5.jpg" alt="Villa in Mombasa">
        <div class="card-body">
          <h3>Beach Villa - Mombasa</h3>
          <span class="tag">KES 45M</span>
          <p>5 Bedroom beachfront villa with private pool and garden.</p>
          <a class="view-btn" href="#">View More</a>
        </div>
      </div>
      <div class="card">
        <img src="1.jpg" alt="Apartment">
        <div class="card-body">
          <h3>2BR Apartment - Westlands</h3>
          <span class="tag">KES 8.5M</span>
          <p>Luxury apartment near Sarit Centre, with balcony and gym access.</p>
          <a class="view-btn" href="#">View More</a>
        </div>
      </div>
      <div class="card">
        <img src="3.jpg" alt="Land in Kiambu">
        <div class="card-body">
          <h3>1 Acre Land - Kiambu</h3>
          <span class="tag">KES 6M</span>
          <p>Prime land for residential development near Tatu City.</p>
          <a class="view-btn" href="#">View More</a>
        </div>
      </div>
      <div class="card">
        <img src="2.jpg" alt="Mansion">
        <div class="card-body">
          <h3>Luxury Mansion - Runda</h3>
          <span class="tag">KES 90M</span>
          <p>Spacious 6 Bedroom mansion with garden, pool, and high security.</p>
          <a class="view-btn" href="#">View More</a>
        </div>
      </div>
    </section>

    <section id="map" class="map-section">
      <h2>Property Map</h2>
      <iframe src="https://maps.google.com/maps?q=Kenya&t=&z=6&ie=UTF8&iwloc=&output=embed" allowfullscreen></iframe>
    </section>

    <section id="contact" class="contact-form">
      <h2>Contact Us</h2>
      <form>
        <input type="text" placeholder="Your Name" required>
        <input type="email" placeholder="Your Email" required>
        <textarea rows="4" placeholder="Message"></textarea>
        <button type="submit">Send Message</button>
      </form>
      <a class="whatsapp-btn" href="https://wa.me/254703476522" target="_blank">Chat on WhatsApp</a>
    </section>
  </div>

  <footer>
    <p>Kenya Real Estate &copy; 2025 | Built by Carlos Ndeda for PLP Hackathon</p>
  </footer>
</body>

</html># plp-hakathon-project
