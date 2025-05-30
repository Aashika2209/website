# Ex.07 Restaurant Website
# Date:12-05-2025
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
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Chini Chaataka Kitchen | Restaurant</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', sans-serif;
    }

    body {
      line-height: 1.6;
      color: #6431dc;
      background-color: #fdfdfd;
    }

    header {
      background: url("sss.jpg") no-repeat center center/cover;
      height: 100vh;
      color: rgb(239, 249, 249);
      text-align: center;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 0 20px;
    }

    header h1 {
      font-size: 4rem;
      margin-bottom: 10px;
    }

    header p {
      font-size: 1.5rem;
    }

    nav {
      background-color: #141313;
      display: flex;
      justify-content: center;
      padding: 15px 0;
      position: sticky;
      top: 0;
      z-index: 100;
    }

    nav a {
      color: white;
      margin: 0 20px;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s ease;
    }

    nav a:hover {
      color: #f4b400;
    }

    section {
      
      background: url("bbb.jpg") no-repeat center center/cover;
      height: 100vh;
      color:rgb(237, 224, 224);
      text-align: center;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 0 20px;
    }
    .menu {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }

    .menu-item {
      background:rgb(29, 29, 28);
      border: 1px solid #111111;
      border-radius: 10px;
      padding: 20px;
      text-align: center;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }

    .menu-item img {
      max-width: 100%;
      border-radius: 8px;
    }

    .chef-name {
      font-style: italic;
      font-size: 0.9rem;
      color: #121212;
      margin-top: 5px;
    }

    .chefs {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 40px;
      margin-top: 40px;
    }

    .chef-card {
      background: rgb(211, 39, 39);
      border: 1px solid #ddd;
      border-radius: 10px;
      text-align: center;
      padding: 20px;
      width: 250px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }

    .chef-card img {

      width: 150px;
      height: 150px;
      object-fit: cover;
      border-radius: 50%;
      margin-bottom: 15px;
    }

    .about, .contact, .book {
      background-color: #0f0202;
      border-radius: 10px;
      padding: 30px;
    }

    .book form {
      display: flex;
      flex-direction: column;
      gap: 15px;
    }

    .book input, .book textarea {
      padding: 10px;
      border: 1px solid #041017;
      border-radius: 5px;
    }

    .book button {
      background-color: #222;
      color: rgb(9, 2, 2);
      padding: 10px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      font-weight: bold;
    }

    .book button:hover {
      background-color: #f4b400;
      color: #000;
    }

    footer {
      text-align: center;
      padding: 20px;
      background-color: #222;
      color: rgb(179, 173, 173);
    }

    @media (max-width: 600px) {
      header h1 {
        font-size: 2.5rem;
      }

      nav {
        flex-direction: column;
      }

      nav a {
        margin: 10px 0;
      }

      .chefs {
        flex-direction: column;
        align-items: center;
      }
    }
  </style>

  Chini Chaataka Kitchen

  </head>
<body>

  <header>
    <h1>Chini Chaataka Kitchen</h1>
    <p>"Where every meal is a masterpiece, and every bite tells a story"</p>
  </header>

  <nav>
    <a href="#menu">Menu</a>
    <a href="#chefs">Chefs</a>
    <a href="#book">Book</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
  </nav>

  Our Menu

   <section id="menu">
    <h2>Our Menu</h2>
    <div class="menu">
      <div class="menu-item">
        <img src="cheese balls.jpg" alt="CHEESE BALL">
        <h3>CHEESE BALL</h3>
        
      </div>
      <div class="menu-item">
        <img src="chilli panner.jpg" alt="CHILLI PANNER">
        <h3>CHILLI PANNER</h3>
        
      </div>
      <div class="menu-item">
        <img src="GGG.jpg" alt="GARLIC BREADr"> 
        <h3>GARLIC BREAD</h3>
        
      </div>
      <div class="menu-item">
        <img src="MMMM.jpg" alt="MANCHUARIAN">
        <h3>MANCHUARIAN</h3>

      </div>
      <div class="menu-item">
        <img src="MOMO.jpg" alt="MOMOS">
        <h3>MOMO</h3>
        
      </div>
      <div class="menu-item">
        <img src="noondles.jpg" alt="NOODLES">
        <h3>NOODLES</h3>
       </div>
      <div class="menu-item">
        <img src="pasta.webp" alt="PASTA">
        <h3>PASTA</h3>
       
      </div>
      <div class="menu-item">
        <img src="pizza.jpg" alt="PIZZA">
        <h3>PIZZA</h3>
       
      </div>
      <div class="menu-item">
        <img src="SchezwanFriedRice.webp" alt="SCHEZWAN RICE">
        <h3>SCHEZWAN RICE</h3>
       
      </div>
      <div class="menu-item">
        <img src="spring roll.jpg" alt="SPRING ROLL">
        <h3>SPRING ROLL</h3>
      </div>
       
      </div>
    </div>
  </section>
  </section>

   <section id="chefs">
        <h2>Meet Our Chefs</h2>
        <div class="chefs">
          <div class="chef-card">
            <img src="CHE 1.jpg" alt="Chef Damu">
            <h3>Chef Damu</h3>
            <p>Chef Damu, born Dr. K. Damodaran, is a celebrated Indian chef and television personality renowned for his expertise in South Indian cuisine</p>
          </div>
          <div class="chef-card">
            <img src="CHE 2.jpeg" alt="Chef Vijaya Kumar">
            <h3>Chef Vijaya Kumar</h3>
            <p>Chef Vijay Kumar is a Michelin-starred Tamil Nadu native known for bringing bold, authentic South Indian village cuisine to New York’s acclaimed restaurant Semma.</p>
          </div>
          <div class="chef-card">
              <img src="CHE 3.jpg" alt="Chef Vikas Khanna">
              <h3>Chef Vikas Khanna</h3>
              <p>Chef Vikas Khanna is a Michelin-starred Indian chef renowned for his mastery of traditional Indian cuisine, culinary innovation, and global advocacy of Indian culinary heritage.</p>
        </div>
        </div>
        </section>
    
  </section>



  <section id="book" class="book">
    <h2>Book a Table</h2>
    <form>
      <input type="text" placeholder="Full Name" required>
      <input type="email" placeholder="Email Address" required>
      <input type="tel" placeholder="Phone Number" required>
      <input type="date" required>
      <input type="time" required>
      <input type="number" placeholder="Number of Guests" required>
      <textarea placeholder="Special Requests"></textarea>
      <button type="submit">Reserve Now</button>
    </form>
  </section>



  <section id="about" class="about">
    <h2>About Us</h2>
    <p>At Chini Chaataka Kitchen, we believe in the timeless tradition of cooking with care and serving with love. Our name reflects our commitment to delivering hearty, flavorful meals that bring people together. Each dish is crafted with the finest ingredients and a touch of culinary artistry, ensuring a memorable dining experience.</p>
  </section>



  
  <section id="contact" class="contact">
    <h2>Contact</h2>
    <p><strong>Address:</strong> Food Town,Jaipur</p>
    <p><strong>Phone:</strong> 91-10987-65432</p>
    <p><strong>Email:</strong> chinichatakakitchen@gmail.com</p>
  </section>

  <footer>
    <p>&copy; 2025 Chini Chaataka Kitchen. All rights reserved.</p>
  </footer>

</body>
</html>
```

# OUTPUT:
![alt text](<holtelapp/static/Screenshot (78).png>)
![alt text](<holtelapp/static/Screenshot (79).png>)
![alt text](<holtelapp/static/Screenshot (80).png>)
![alt text](<holtelapp/static/Screenshot (81).png>)
![alt text](<holtelapp/static/Screenshot (82).png>)
![alt text](<holtelapp/static/Screenshot (83).png>)

![alt text](<holtelapp/static/Screenshot (84).png>)


# RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
