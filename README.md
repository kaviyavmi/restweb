# Ex.07 Restaurant Website
## Date:12-05-2025

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```
index.html
<!-- index.html -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>RASAM & RAMEN- Home</title>
  <link rel="stylesheet" href="style.css">
  <style>
    body, html {
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', sans-serif;
      overflow-x: hidden;
    }
    .hero {
      position: relative;
      height: 100vh;
      background: url('background.png') no-repeat center center/cover;

      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      color: white;
      animation: fadeIn 2s ease-in-out;
    }
    .hero h1{
      font-size: 4em;
      background: rgba(0, 0, 0, 0.5);
      padding: 20px;
      border-radius: 10px;
      animation: slideInDown 1.5s ease-out;
    }
    .nav {
      display: flex;
      justify-content: center;
      background-color: #f4a261;
      padding: 10px 0;
      position: sticky;
      top: 0;
      z-index: 1000;
    }
    .nav a {
      color: white;
      text-decoration: none;
      margin: 0 15px;
      padding: 8px 12px;
      border-radius: 4px;
      transition: background 0.3s ease;
    }
    .nav a:hover {
      background-color: #e76f51;
    }
    .highlights {
      display: flex;
      flex-wrap: wrap;
      padding: 40px;
      justify-content: space-around;
      background: #fff3e6;
    }
    .highlight-card {
      width: 300px;
      margin: 20px;
      background: #fff;
      border-radius: 10px;
      box-shadow: 0 8px 16px rgba(0,0,0,0.1);
      overflow: hidden;
      transition: transform 0.3s ease;
    }
    .highlight-card:hover {
      transform: translateY(-10px);
    }
    .highlight-card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }
    .highlight-card h3 {
      margin: 10px;
      color: #264653;
    }
    .highlight-card p {
      padding: 0 10px 10px;
      color: #555;
    }
    footer {
      text-align: center;
      background-color: #f4a261;
      color: white;
      padding: 20px;
    }

    @keyframes slideInDown {
      from {
        transform: translateY(-100px);
        opacity: 0;
      }
      to {
        transform: translateY(0);
        opacity: 1;
      }
    }
    @keyframes fadeIn {
      from {
        opacity: 0;
      }
      to {
        opacity: 1;
      }
    }
  </style>
</head>
<body>
  <div class="nav">
    <a href="index.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="admin.html">Administration</a>
    <a href="contact.html">Contact</a>
  </div>

  <section class="hero">
    <h1>Welcome to RASAM & RAMEN 👩‍🍳A Multicuisine Restaurant</h1>
    
  </section>

  <section class="highlights">
    <div class="highlight-card">
      <img src="rasam ramen.jpg" alt="Dish 1">
      <h3>Signature fusion dish </h3>
      <p>Rasam Ramen Bowl (Fusion of South Indian rasam base with ramen noodles, soft egg, and veggies/meat).</p>
    </div>
    <div class="highlight-card">
      <img src="fried rice.webp" alt="Sandwich">
      <h3>Indo-Asian Fried Rice</h3>
      <p>Spicy rice with gunpowder prawns.</p>
    </div>
    <div class="highlight-card">
      <img src="dosa quesadilla.avif" alt="Choco Lava Cake">
      <h3>Dosa Quesadilla</h3>
      <p>Layer of melted cheese and other fillings like vegetables with two dosa.</p>
    </div>
  </section>

  <footer>
    <p>&copy; 2025 RASAM & RAMEN . Created by KAVIYA V M.</p>
  </footer>
</body>
</html>

menu.html

<!-- menu.html -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Menu - RASAM & RAMEN</title>
  <link rel="stylesheet" href="style.css">
  <style>
    .menu-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      padding: 40px;
    }
    .card {
      background-color: #fff;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      padding: 15px;
      text-align: center;
    }
    .card img {
      width: 100%;
      height: 180px;
      object-fit: cover;
      border-radius: 8px;
    }
    .card h3 {
      margin-top: 15px;
      color: #f4a261;
    }
  </style>
</head>
<body>
     <div class="nav">
    <a href="index.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="admin.html">Administration</a>
    <a href="contact.html">Contact</a>
  </div>
  <h2 class="title">Our Signature Dishes</h2>
  <div class="menu-grid">
    <div class="card">
      <img src="panner tikka.jpg" alt="Paneer Tikka Skewers">
      <h3>Paneer Tikka Skewers</h3>
      <p>Assorted maki rolls with wasabi and soy dip</p>
      <p>₹950</p>
    </div>
    <div class="card">
      <img src="Chicken Kebab Wrap.jpg" alt="Chicken kebab wrap">
      <h3>Chicken kebab wrap</h3>
      <p>Rich creamy North Indian curry with tandoori naan</p>
      <p>₹480</p>
    </div>
    <div class="card">
      <img src="shrimp tempura.jpg" alt="Crispy Tempura Prawns">
      <h3>Crispy Tempura Prawns</h3>
      <p>Classic pizza topped with mozzarella and basil</p>
      <p>₹550</p>
    </div>
    <div class="card">
      <img src="chickenwings.jpg" alt="Korean Gochujang Wings">
      <h3>Korean Gochujang Wings</h3>
      <p>Grilled cottage cheese with mint chutney</p>
      <p>₹360</p>
    </div>
    <div class="card">
      <img src="pepper rasam.jpg" alt="Pepper Rasam with Garlic Croutons">
      <h3>Pepper Rasam with Garlic Croutons</h3>
      <p>Served with fries and coleslaw</p>
      <p>₹250</p>
    </div>
    <div class="card">
      <img src="koream soup.jpg" alt="Spicy Korean Kimchi Soup">
      <h3>Spicy Korean Kimchi Soup</h3>
      <p>Flaky French-style croissant</p>
      <p>₹120</p>
    </div>
    <div class="card">
      <img src="paratto.webp" alt="Chicken Chettinad with Parotta">
      <h3>Chicken Chettinad with Parotta</h3>
      <p>Mixed grilled chicken, fish, and prawns</p>
      <p>₹850</p>
    </div>
    <div class="card">
      <img src="mutton briyani.jpg" alt="Mutton Biryani with Raita & Salna">
      <h3>Mutton Biryani with Raita & Salna</h3>
      <p>Molten chocolate dessert with vanilla scoop</p>
      <p>₹180</p>
    </div>
    <div class="card">
      <img src="pad thai.jpg" alt="Pad Thai Noodles">
      <h3>Pad Thai Noodles</h3>
      <p>Italian creamy rice with mushrooms and herbs</p>
      <p>₹470</p>
    </div>
    <div class="card">
      <img src="pasta.jpg" alt="Pasta Alfredo / Arrabbiata">
      <h3>Pasta Alfredo / Arrabbiata</h3>
      <p>New York-style cheesecake with berry topping</p>
      <p>₹230</p>
    </div>
    <div class="card">
      <img src="mango basil.webp" alt="Mango Basil Lemonade">
      <h3>Mango Basil Lemonade</h3>
      <p>Soft-baked cookie with melted chocolate chips</p>
      <p>₹50</p>
    </div>
    <div class="card">
      <img src="thai iced.jpg" alt="Thai Iced Tea">
      <h3>Thai Iced Tea</h3>
      <p>Stacked layers with fresh veggies and cheese</p>
      <p>₹200</p>
    </div>
    <div class="card">
      <img src="gulab cheesecake.jpg" alt="Gulab Jamun Cheesecake">
      <h3>Gulab Jamun Cheesecake</h3>
      <p>Traditional biryani with raita and salan</p>
      <p>₹480</p>
    </div>
    <div class="card">
      <img src="mochi.webp" alt="Mochi Ice Cream">
      <h3>Mochi Ice Cream</h3>
      <p>Crispy tart filled with cream and fresh fruits</p>
      <p>₹210</p>
    </div>
  </div>

  <footer>
    <p>&copy; 2025 RASAM & RAMEN. Created by KAVIYA V M.</p>
  </footer>
</body>
</html>


admin.html

<!-- admin.html -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Administration - RASAM & RAMEN</title>
  <link rel="stylesheet" href="style.css">
  <style>
    .admin-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      padding: 40px;
      text-align: center;
    }
    .admin-card {
      background-color: #fff;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      padding: 20px;
    }
    .admin-card img {
      width: 120px;
      height: 120px;
      object-fit: cover;
      border-radius: 50%;
      margin-bottom: 15px;
    }
    .admin-card h3 {
      margin: 0;
      color: #f4a261;
    }
    .admin-card p {
      margin-top: 5px;
      font-size: 0.95rem;
    }
  </style>
</head>
 <div class="nav">
    <a href="index.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="admin.html">Administration</a>
    <a href="contact.html">Contact</a>
  </div>
<body>
  <h2 class="title">Meet Our Culinary & Management Experts</h2>
  <div class="admin-grid">
    <div class="admin-card">
      <img src="stafff1.jpg" alt="Executive Chef">
      <h3>Chef Rohan kumar</h3>
      <p>Executive Chef</p>
    </div>
    <div class="admin-card">
      <img src="staff2 baker.jpg" alt="Head Baker">
      <h3>Aisha sharma</h3>
      <p>Head Baker</p>
    </div>
    <div class="admin-card">
      <img src="staff3 manager.jpg" alt="Hotel manager">
      <h3>Shraddha kapoor</h3>
      <p>Hotel manager</p>
    </div>
    <div class="admin-card">
      <img src="staff4 assisstant manger.jpg" alt="Assistant Manager">
      <h3>Arjun</h3>
      <p>Assistant Manager</p>
    </div>
    <div class="admin-card">
      <img src="staff5 chef.jpg" alt="chef">
      <h3>krupa rakesh</h3>
      <p>chef</p>
    </div>
    
  </div>
  <footer>
    <p>&copy; 2025 RASAM & RAMEN. Created by KAVIYA V M.</p>
  </footer>
</body>
</html>

contact.html

<!-- contact.html -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Contact Us - Fun With Bun</title>
  <link rel="stylesheet" href="style.css">
  <style>
    .contact-form {
      max-width: 500px;
      margin: 0 auto;
      background-color:#c16a1e;
      padding: 20px;
      border-radius: 3px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }
    .contact-form label {
      display: block;
      margin-top: 15px;
      font-weight: bold;
    }
    .contact-form input, .contact-form textarea {
      width: 100%;
      padding: 10px;
      margin-top: 5px;
      border: 1px solid black;
      border-radius: 5px;
    }
    .contact-form button {
      margin-top: 20px;
      padding: 10px 20px;
      background-color: #b0a03e;
      color: rgb(37, 61, 117);
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    .contact-form button:hover {
      background-color: #b05c48;
    }
  </style>
</head>
<body>
     <div class="nav">
    <a href="index.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="admin.html">Administration</a>
    <a href="contact.html">Contact</a>
  </div>
  <h2 class="title">Get in Touch & Book a Table</h2>
  <div style="text-align: center; padding: 20px;">
    <p><strong>Address:</strong> 123 Gourmet Street, Sweet City, India - 560001</p>
    <p><strong>Phone:</strong> +91 98765 43210</p>
    <p><strong>Email:</strong> contact@funwithbun.in</p>
  </div>

  <div class="contact-form">
    <form action="#" method="post">
      <label for="name">Full Name</label>
      <input type="text" id="name" name="name" required>

      <label for="email">Email</label>
      <input type="email" id="email" name="email" required>

      <label for="phone">Phone</label>
      <input type="tel" id="phone" name="phone" required>

      <label for="date">Booking Date</label>
      <input type="date" id="date" name="date" required>

      <label for="time">Booking Time</label>
      <input type="time" id="time" name="time" required>

      <label for="people">Number of People</label>
      <input type="number" id="people" name="people" min="1" max="20" required>

      <label for="message">Additional Message</label>
      <textarea id="message" name="message" rows="4"></textarea>

      <button type="submit">Book Now</button>
    </form>
  </div>

  <footer>
    <p>&copy; 2025 RASAM & RAMEN. Created by KAVIYA V M.</p>
  </footer>
</body>
</html>

style.css

/* Global Styles */
body, html {
  margin: 0;
  padding: 0;
  font-family: 'Segoe UI', sans-serif;
  background-color: #f4f4f9;
  color: #333;
}

h2.title {
  font-size: 2.5em;
  color: #264653;
  margin-top: 40px;
  text-align: center;
}

footer {
  background-color: #f4a261;
  color: white;
  padding: 20px;
  text-align: center;
}

a {
  text-decoration: none;
  color: inherit;
}

/* Navigation Bar */
.nav {
  display: flex;
  justify-content: center;
  background-color: #f4a261;
  padding: 10px 0;
  position: sticky;
  top: 0;
  z-index: 1000;
}

.nav a {
  color: white;
  text-decoration: none;
  margin: 0 15px;
  padding: 8px 12px;
  border-radius: 4px;
  transition: background 0.3s ease;
}

.nav a:hover {
  background-color: #e76f51;
}

/* Hero Section */
.hero {
  position: relative;
  height: 100vh;
  background: url('images/banner.jpg') no-repeat center center/cover;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  color: white;
  animation: fadeIn 2s ease-in-out;
}

.hero h1 {
  font-size: 4em;
  background: rgba(0, 0, 0, 0.5);
  padding: 20px;
  border-radius: 10px;
  animation: slideInDown 1.5s ease-out;
}

@keyframes slideInDown {
  from {
    transform: translateY(-100px);
    opacity: 0;
  }
  to {
    transform: translateY(0);
    opacity: 1;
  }
}

@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

/* Menu Page Styles */
.menu-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 20px;
  padding: 40px;
}

.card {
  background-color: #fff;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  padding: 15px;
  text-align: center;
}

.card img {
  width: 100%;
  height: 180px;
  object-fit: cover;
  border-radius: 8px;
}

.card h3 {
  margin-top: 15px;
  color: #f4a261;
}

.card p {
  color: #777;
  margin: 10px 0;
}

/* Contact Form Styles */
.contact-form {
  max-width: 500px;
  margin: 40px auto;
  background-color: #fff;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.contact-form label {
  display: block;
  margin-top: 15px;
  font-weight: bold;
}

.contact-form input,
.contact-form textarea {
  width: 100%;
  padding: 10px;
  margin-top: 5px;
  border: 1px solid #ccc;
  border-radius: 5px;
}

.contact-form button {
  margin-top: 20px;
  padding: 10px 20px;
  background-color: #f4a261;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.contact-form button:hover {
  background-color: #e76f51;
}

/* Admin Page Styles */
.admin-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 20px;
  padding: 40px;
  text-align: center;
}

.admin-card {
  background-color: #fff;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  padding: 20px;
}

.admin-card img {
  width: 120px;
  height: 120px;
  object-fit: cover;
  border-radius: 50%;
  margin-bottom: 15px;
}

.admin-card h3 {
  margin: 0;
  color: #f4a261;
}

.admin-card p {
  margin-top: 5px;
  font-size: 0.95rem;
}

/* Highlights Section */
.highlights {
  display: flex;
  flex-wrap: wrap;
  padding: 40px;
  justify-content: space-around;
  background: #fff3e6;
}

.highlight-card {
  width: 300px;
  margin: 20px;
  background: #fff;
  border-radius: 10px;
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.1);
  overflow: hidden;
  transition: transform 0.3s ease;
}

.highlight-card:hover {
  transform: translateY(-10px);
}

.highlight-card img {
  width: 100%;
  height: 200px;
  object-fit: cover;
}

.highlight-card h3 {
  margin: 10px;
  color: #264653;
}

.highlight-card p {
  padding: 0 10px 10px;
  color: #555;
}
```


## OUTPUT:

![alt text](1.png)
![alt text](2.png)
![alt text](3.png)
![alt text](4.png)
![alt text](5.png)



## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
