# Ex.07 Restaurant Website

# Name:Kiruthiga.B

# Reg.no:212224040160

# Date:26.04.2025

# AIM:
To develop a static Restaurant website to display the food items and services provided by them.

# DESIGN STEPS:
## Step 1:
Requirement collection.

## Step 2:
Creating the layout using HTML and CSS.

## Step 3:
Updating the sample content.

## Step 4:
Choose the appropriate style and color scheme.

## Step 5:
Validate the layout in various browsers.

## Step 6:
Validate the HTML code.

## Step 7:
Publish the website in the given URL.

# PROGRAM:
```
restweb.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vintage Foods</title>
    <link rel="stylesheet" href="styler.css">
</head>
<body>
    <header>
        <div class="logo-header">
            <div class="logo-text">
                <h1>VINTAGE FOODS</h1>
            </div>
    	</div>
	<div class='toolbar'>
        <nav>
            <ul>
                <li><a href="home.html">Home</a></li>
                <li><a href="menu.html">Menu</a></li>
                <li><a href="administration.html">Administration</a></li>
                <li><a href="contact.html">Contact Us</a></li>
            </ul>
        </nav>
	</div>
    </header>
    <main>
        <section class="promo">
            <h2>Heavenly Combo</h2>
            <h3>Tradition Foods</h3>
        </section>
        <section class="info">
            <div class="card">
                <img src="new menu.png" alt="New Menu">
                <h4>Our New Menu</h3>
                <p>Enjoy bold coffees and indulge in our treats.</p>
                <a href="menu.html">See our new menu</a>
	
            </div>

            <div class="card">
                <img src="book table.png" alt="Book a Table">
                <h4>Book a table</h4>
                <p>Reserve your seats at vintage foods for wonderful experience.</p>
                <a href="book.html">Book your table now</a>
            </div>
            <div class="card">
                <img src="oh.png" alt="Opening Hours">
                <h4>Opening Hours</h4>
                <p>Mon - Fri: 8am - 10pm<br>Sat: 8am - 11pm<br>Sun: 8am - 12pm</p>
            </div>
        </section>
    </main>
    <div class="footer-content">
        <div class="footer-logo">
            <img src="logo.png" alt="Small Logo">
        </div>
    
    <div class="footer-line"></div>
</div>

    <footer>
        <p>Designed and Developed by <a href="#">Kiruthiga.B</a></p>
    </footer>
</body>
</html>


styler.css


html, body {
    margin: 0;
    padding: 0;
    height: 100%;
    overflow: hidden; /* Prevent scrollbar */
    font-family: Arial, sans-serif;
    background-color: antiquewhite;
    color: #FFFFFF;
}

.logo-header {
    background: url('bg.png') no-repeat center center/cover;
    height: 150px;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: white;
}

.logo-text h1 {
    font-family: 'serif';
    font-size: 5em;
    letter-spacing: 2px;
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.7);
}

.toolbar {
    background-color: #333;
    padding: 10px 0;
    border-radius: 10px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
}

.toolbar ul {
    list-style: none;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
}

.toolbar li {
    margin: 0 15px;
}

.toolbar a {
    text-decoration: none;
    color: #fff;
    font-size: 1.1em;
    font-weight: bold;
}

.toolbar a:hover {
    text-decoration: underline;
}

.promo {
    background: url('logo.png') no-repeat center center/cover;
    color: #fff;
    text-align: center;
    padding: 0px;
    margin: 10px;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}

.promo h2 {
    font-size: 2.0em;
}

.promo h3 {
    font-size: 2.5em; 
}

.info {
    display: flex;
    justify-content: space-around;
    margin: 20px;
    gap: 10px;
}

.info .card {
    background-color: #194274;
    border-radius: 5px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2); 
    overflow: hidden;
    text-align: center;
    padding: 35px;
    flex: 1;
}
.info .card img {
    width: 100%;
    height: 158px;
    object-fit: cover;
    border-radius: 4px;
}

.info .card h4 {
    color: #ffcc00;
    margin: 10px 0;
}

.info .card a {
    color: #FF0000;
    text-decoration: none;
}

.footer-content {
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 20px;
}

.footer-logo img {
    width: 50px;
    height: auto;
    margin-right: 10px;
}

.footer-line {
    flex-grow: 1;
    height: 1px;
    background-color: #333;
    margin-right: 30px;
}

footer {
    text-align: center;
    padding: 0px 0;
    font-size: 0.9em;
    width: 100%;
    z-index: 1000;
}

.footer-border {
    width: 200px;
    height: 0.5px;
    background-color: #333;
    margin: 10px auto 5px auto;
    border-radius: 2px;
}

footer p {
    color: #333;
}

footer a {
    text-decoration: none;
    color: #FF0000;
}


home.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home (Vintage Foods)</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        .hero {
            background-image: url('bg.png');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 80px 20px;
        }
        .hero h1 {
            font-size: 6em;
        }
        .hero p {
            font-size: 1.2em;
            margin: 20px 0;
        }
        .hero button {
            padding: 10px 20px;
            background-color: #ffda79;
            color: #333;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1em;
        }
        .section {
            padding: 40px 20px;
            text-align: center;
        }
        .section h2 {
            font-size: 2em;
            margin-bottom: 20px;
        }
        .cards {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }
        .card {
            background-color: #fff;
            border: 1px solid #ccc;
            border-radius: 10px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            padding: 20px;
	    width: 250px; 
            text-align: center;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .product-image {
            width: 100%;
            height: 150px; 
            object-fit: cover;
            border-radius: 10px;
           margin-bottom: 15px;
       }

       .card h3 {
    		margin: 10px 0 5px;
    		font-size: 1.2em;
	}
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 40px;
        }
    </style>
</head>
<body>
    <header class="hero">
        <h1>Home</h1>
        <p>Enjoy the finest trational foods in town</p>
        <button>Learn More</button>
    </header>

    <section class="section">
        <h2>About Us</h2>
        <p>At Vintage Foods, we bring timeless flavors to the modern table. Inspired by traditional recipes and classic cooking methods, our restaurant is a celebration of heritage, warmth, and unforgettable taste. Every dish is crafted with fresh, locally sourced ingredients and a passion for authenticity. Whether you're craving a comforting meal that reminds you of home or looking to experience a culinary journey through the past, Vintage Foods offers a dining experience that feels both familiar and special.</p>
    </section>
    <footer>
        <p>Designed and Developed by Kiruthiga.B<p>
    </footer>
</body>
</html>

menu.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Menu (Vintage Foods)</title>
  <style>
    html, body {
      margin: 0;
      padding: 0;
      height: 100%;
      overflow: hidden;
      font-family: Arial, sans-serif;
      background-color: #f9f9f9;
      color: #333;
    }

    .page-wrapper {
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
    }

    .hero {
      background-image: url('bg.png');
      background-size: cover;
      background-position: center;
      color: white;
      text-align: center;
      padding: 80px 20px;
      flex: 0 0 auto;
    }

    .hero h1 {
      font-size: 2.5em;
      margin: 0;
    }

    .menu-container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 15px;
      padding: 20px;
      flex: 1 1 auto;
      overflow: hidden;
    }

    .menu-item {
      background: white;
      border: 1px solid #ddd;
      border-radius: 8px;
      width: 220px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
      text-align: center;
      flex-shrink: 1;
    }

    .menu-item img {
      width: 100%;
      height: 130px;
      object-fit: cover;
    }

    .menu-item h3 {
      margin: 10px 0 5px;
      font-size: 16px;
    }

    .menu-item .price {
      font-size: 16px;
      font-weight: bold;
      color: #ff5722;
      margin: 5px 0 10px;
    }

    footer {
      background-color: #333;
      color: white;
      text-align: center;
      padding: 10px;
      font-size: 14px;
      flex: 0 0 auto;
    }

    footer a {
      color: #ffda79;
      text-decoration: none;
    }

    footer .footer-links {
      display: flex;
      justify-content: center;
      gap: 30px;
      margin: 10px 0;
    }

    footer .footer-links div {
      text-align: left;
    }

    footer .footer-links h4 {
      margin-bottom: 5px;
      font-size: 14px;
      color: #ffda79;
    }
  </style>
</head>
<body>
  <div class="page-wrapper">
    <header class="hero">
      <h1>Menu</h1>
    </header>

    <div class="menu-container">
      <div class="menu-item">
        <img src="Screenshot 2025-04-25 133903.png" alt="Dosa">
        <h3>Dosa</h3>
        <div class="price">Rs.40</div>
      </div>
      <div class="menu-item">
        <img src="Screenshot 2025-04-25 133648.png" alt="Puttu">
        <h3>Puttu</h3>
        <div class="price">Rs.50</div>
      </div>
      <div class="menu-item">
        <img src="Screenshot 2025-04-25 133621.png" alt="Kali">
        <h3>Kali</h3>
        <div class="price">Rs.60</div>
      </div>
      <div class="menu-item">
        <img src="Screenshot 2025-04-25 133552.png" alt="Pongal">
        <h3>Pongal</h3>
        <div class="price">Rs.50</div>
      </div>
      <div class="menu-item">
        <img src="Screenshot 2025-04-25 133522.png" alt="Poori">
        <h3>Poori</h3>
        <div class="price">Rs.40</div>
      </div>
      <div class="menu-item">
        <img src="Screenshot 2025-04-25 133504.png" alt="Meals">
        <h3>Meals</h3>
        <div class="price">Rs.120</div>
      </div>
      <div class="menu-item">
        <img src="Screenshot 2025-04-25 133445.png" alt="Idly">
        <h3>Idly</h3>
        <div class="price">Rs.30</div>
      </div>
    </div>

    <footer>
        <div class="footer-links">
            <div>
                <h4>Contact Us</h4>
                <p>123 Little India Road, #07-20, Central, Singapore 890653</p>
                <p>contact@vintagefoods.sg | +65 0865 8643</p>
            </div>
            <div>
                <h4>Our Links</h4>
                <p>About Us | FAQ | Team | Testimonial</p>
            </div>
            <div>
                <h4>Our Services</h4>
                <p>Table Service | Quick Delivery | Fresh Food</p>
            </div>
        </div>
        <p>Designed and Developed by Kiruthiga.B</p>
    </footer>
</body>
</html>

administration.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>ADMINISTRATION (Vintage Foods)</title>
  <style>
    html, body {
      margin: 0;
      padding: 0;
      height: 100%;
      overflow: hidden;
      font-family: Arial, sans-serif;
      background-color:antiquewhite;
      color: #333;
    }

    .container {
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
    }

    .hero {
      background-image: url('bg.png');
      background-size: cover;
      background-position: center;
      color: antiquewhite;
      text-align: center;
      padding: 60px 20px;
      flex: 0 0 auto;
    }

    .hero h1 {
      font-size: 2.5em;
      margin: 0;
    }

    .staff-container {
      display: flex;
      justify-content: center;
      gap: 20px;
      padding: 20px;
      flex-wrap: wrap;
      flex: 1 1 auto;
      overflow: hidden;
    }

    .staff-item {
      background: white;
      border: 1px solid #ddd;
      border-radius: 8px;
      width: 260px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
      text-align: center;
      flex-shrink: 1;
    }

    .staff-item img {
      width: 100%;
      height: 350px;
      object-fit: cover;
    }

    .staff-item h3 {
      margin: 10px 0 5px;
      font-size: 18px;
    }

    .staff-item p {
      font-size: 13px;
      color: #777;
      padding: 0 10px 10px;
    }

    .staff-item .position {
      font-size: 16px;
      font-weight: bold;
      color: #d322ff;
      margin: 5px 0;
    }

    footer {
      background-color: #333;
      color: white;
      text-align: center;
      padding: 10px;
      font-size: 14px;
      flex: 0 0 auto;
    }

    footer a {
      color: #ffda79;
      text-decoration: none;
    }

    footer .footer-links {
      display: flex;
      justify-content: center;
      gap: 30px;
      margin: 10px 0;
    }

    footer .footer-links div {
      text-align: left;
    }

    footer .footer-links h4 {
      margin-bottom: 5px;
      font-size: 14px;
      color: #ffda79;
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="hero">
      <h1>ADMINISTRATION (Vintage Foods)</h1>
    </div>

    <div class="staff-container">
        <div class="staff-item">
            <img src="owner.png" alt="owner">
            <h3>Balu</h3>
            <div class="position">Hotel Owner</div>
        </div>
        <div class="staff-item">
            <img src="Screenshot 2025-04-25 132203.png" alt="Screenshot 2025-04-25 132203">
            <h3>Rani</h3>
        
            <div class="position">Cook</div>
        </div>
        <div class="staff-item">
            <img src="Screenshot 2025-04-25 133053.png" alt="Screenshot 2025-04-25 133053">
            <h3>Latha</h3>
            <div class="position">Chief cook</div>
        </div>
        <div class="staff-item">
            <img src="Screenshot 2025-04-25 133116.png" alt="Mani">
            <h3>Mani</h3>
            <div class="position">Executive Chef</div>
        </div>
        <div class="staff-item">
            <img src="cook.png" alt="cook">
            <h3>Chandru</h3>
            <div class="position">Barista</div>
        </div>
    </div>    
    <footer>
        <div class="footer-links">
            <div>
                <h4>Contact Us</h4>
                <p>123 Little India Road, #07-20, Central, Singapore 890653</p>
                <p>contact@vintagefoods.sg | +65 0865 8643</p>
            </div>
            <div>
                <h4>Our Links</h4>
                <p>About Us | FAQ | Team | Testimonial</p>
            </div>
            <div>
                <h4>Our Services</h4>
                <p>Table Service | Quick Delivery | Fresh Food</p>
            </div>
        </div>
        <p>Designed and Developed by Kiruthiga.B</p>
    </footer>
</body>
</html>

contact.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Contact Us (Vintage Foods)</title>
  <style>
    html, body {
      margin: 0;
      padding: 0;
      height: 100%;
      font-family: Arial, sans-serif;
      overflow: hidden;
    }

    .page-wrapper {
      display: flex;
      flex-direction: column;
      height: 100vh;
    }

    .hero {
      background-image: url('bg.png');
      background-size: cover;
      background-position: center;
      color: antiquewhite;
      text-align: center;
      padding: 60px 20px;
      flex: 0 0 auto;
    }

    .hero h1 {
      font-size: 2.5em;
      margin: 0;
    }

    nav {
      display: flex;
      justify-content: center;
      background-color: #333;
      padding: 8px 0;
      flex: 0 0 auto;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin: 0 12px;
      font-size: 0.95em;
    }

    nav a:hover {
      color: #ffda79;
    }

    .content {
      flex: 1 1 auto;
      display: flex;
      flex-direction: column;
      overflow: hidden;
      padding: 10px 20px;
    }

    .contact-details {
      flex: 0 0 auto;
    }

    .contact-details p {
      font-size: 0.95em;
      margin: 4px 0;
    }

    .contact-form {
      flex: 1 1 auto;
      background-color: antiquewhite;
      padding: 15px;
      border-radius: 5px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
      overflow-y: auto;
    }

    .contact-form h2 {
      font-size: 1.2em;
      margin-top: 0;
    }

    .form-group {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      margin-bottom: 10px;
    }

    .form-group div {
      flex: 1;
      min-width: 100px;
    }

    input, textarea {
      width: 100%;
      padding: 8px;
      margin-top: 5px;
      border: 1px solid #ccc;
      border-radius: 5px;
      font-size: 0.95em;
    }

    textarea {
      resize: vertical;
      height: 80px;
    }

    button {
      background-color: #333;
      color: white;
      border: none;
      padding: 10px;
      font-size: 1em;
      border-radius: 5px;
      cursor: pointer;
      width: 100%;
    }

    button:hover {
      background-color: #555;
    }

    footer {
      background-color: #333;
      color: white;
      text-align: center;
      padding: 10px;
      font-size: 0.9em;
      flex: 0 0 auto;
    }
  </style>
  <script>
    function validateForm(event) {
      event.preventDefault();
      const firstName = document.getElementById("first-name").value;
      const email = document.getElementById("email").value;
      const message = document.getElementById("message").value;

      if (!firstName || !email || !message) {
        alert("Please fill in all required fields.");
        return;
      }
      alert("Your message has been submitted. Thank you!");
    }
  </script>
</head>
<body>
  <div class="page-wrapper">
    <header class="hero">
      <h1>Contact Us</h1>
    </header>

    <nav>
      <a href="#">Home</a>
      <a href="#">About</a>
      <a href="#">Menu</a>
      <a href="#">Contact</a>
    </nav>

    <div class="content">
      <div class="contact-details">
        <h2>Contact Information</h2>
        <p>Email: <a href="mailto:contact@vintagefoods.sg">contact@vintagefoods.sg</a></p>
        <p>Phone: +65 0865 8643</p>
        <p>Address: 123 Little India Road, #07-20, Central, Singapore 890653</p>
      </div>

      <div class="contact-form">
        <h2>Send Us a Message</h2>
        <form onsubmit="validateForm(event)">
          <div class="form-group">
            <div>
              <label for="first-name">First Name</label>
              <input type="text" id="first-name" placeholder="Enter your first name">
            </div>
            <div>
              <label for="last-name">Last Name</label>
              <input type="text" id="last-name" placeholder="Enter your last name">
            </div>
          </div>
          <div class="form-group">
            <div>
              <label for="email">Email</label>
              <input type="email" id="email" placeholder="Enter your email">
            </div>
          </div>
          <div>
            <label for="message">Message</label>
            <textarea id="message" placeholder="Write your message"></textarea>
          </div>
          <button type="submit">Send</button>
        </form>
      </div>
    </div>

    <footer>
        <p>Designed and Developed by Kiruthiga.B</p>
    </footer>

</body>
</html>

book.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Reservation</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            line-height: 1.6;
        }

        .hero {
            background-image: url('bg.png');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 10px 20px;
        }
        .hero h1 {
            font-size: 3em;
        }

        nav {
            display: flex;
            justify-content: center;
            background-color: #333;
            padding: 10px 0;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            font-size: 1em;
        }

        nav a:hover {
            color: #ffda79;
        }

        .container {
            max-width: 1200px;
            margin: auto;
            padding: 20px;
        }

        h1 {
            text-align: center;
            margin-bottom: 20px;
        }

        .reservation-form {
            background-color: #f9f9f9;
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }

        .form-group {
            display: flex;
            justify-content: space-between;
            gap: 20px;
            margin-bottom: 15px;
        }

        .form-group div {
            flex: 1;
        }

        label {
            font-weight: bold;
        }

        input, select, textarea {
            width: 100%;
            padding: 10px;
            margin-top: 5px;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 1em;
        }

        textarea {
            resize: vertical;
            height: 50px;
        }

        button {
            display: block;
            width: 100%;
            background-color: #333;
            color: white;
            border: none;
            padding: 10px;
            font-size: 1.2em;
            border-radius: 5px;
            cursor: pointer;
        }

        button:hover {
            background-color: #555;
        }

        footer {
            text-align: center;
            padding: 1px;
            background-color: #333;
            color: white;
        }
    </style>
    <script>
        
        function validateReservationForm(event) {
            event.preventDefault();
            const name = document.getElementById("name").value;
            const email = document.getElementById("email").value;
            const phone = document.getElementById("phone").value;
            const date = document.getElementById("date").value;
            const time = document.getElementById("time").value;
            const guests = document.getElementById("guests").value;

            if (!name || !email || !phone || !date || !time || !guests) {
                alert("Please fill in all required fields.");
                return;
            }
            alert("Your reservation has been successfully submitted. Thank you!");
        }
    </script>
</head>
<body>

    <header class="hero">
        <h1>Make A Reservation</h1>
    </header>

    <nav>
        <a href="index.html">Home</a>
        <a href="about.html">About</a>
        <a href="menu.html">Menu</a>
        <a href="contact.html">Contact</a>
    </nav>

    <div class="container">
        <div class="reservation-form">
            <h2>Reserve a Table</h2>
            <form onsubmit="validateReservationForm(event)">
                <div class="form-group">
                    <div>
                        <label for="name">Name</label>
                        <input type="text" id="name" placeholder="Enter your name" required>
                    </div>
                    <div>
                        <label for="email">Email</label>
                        <input type="email" id="email" placeholder="Enter your email" required>
                    </div>
                </div>
                <div class="form-group">
                    <div>
                        <label for="phone">Phone Number</label>
                        <input type="tel" id="phone" placeholder="Enter your phone number" required>
                    </div>
                    <div>
                        <label for="date">Date</label>
                        <input type="date" id="date" required>
                    </div>
                </div>
                <div class="form-group">
                    <div>
                        <label for="time">Time</label>
                        <input type="time" id="time" required>
                    </div>
                    <div>
                        <label for="guests">Number of Guests</label>
                        <select id="guests" required>
                            <option value="">Select</option>
                            <option value="1">1</option>
                            <option value="2">2</option>
                            <option value="3">3</option>
                            <option value="4">4</option>
                            <option value="5">5</option>
                            <option value="6+">6+</option>
                        </select>
                    </div>
                </div>
                <div>
                    <label for="special-requests">Special Requests (optional)</label>
                    <textarea id="special-requests" placeholder="Any specific preferences or requests"></textarea>
                </div>
                <button type="submit">Submit Reservation</button>
            </form>
        </div>
    </div>

    <footer>
        <p>Designed and Developed by Kiruthiga.B</p>
    </footer>

</body>
</html>

```
# OUTPUT:

![alt text](<Screenshot 2025-04-26 175132.png>)


![alt text](<Screenshot 2025-04-26 172821.png>)


![alt text](<Screenshot 2025-04-26 172836.png>)


![alt text](<Screenshot 2025-04-26 172905.png>)


![alt text](<Screenshot 2025-04-26 172920.png>)


![alt text](<Screenshot 2025-04-26 172935.png>)


# RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
