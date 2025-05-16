# Ex.07 Restaurant Website
## Date:15-05-2025

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
home.html

<!DOCTYPE html>
<html lang="en"> 
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">  
  <meta name="viewport" content="width=device-width, initial-scale=1.0">  
  <title>Home - Moonlit Saphore</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body, html { width: 100%; height: 100%; font-family: Arial, sans-serif; }

    .container {
      height: 100%;
      width: 100%;  
      background-color: rgb(12, 12, 12);  
      background-size: cover;  
      background-position: center;   
    }

    .nav-bar {  
      display: flex;  
      align-items: center;  
      justify-content: space-between;  
      padding: 30px 80px;
    }

    .nav-bar .title {
      color: #fff;
      font-size: 67px;
    }

    .nav-bar p {
      position: absolute;
      margin-top: 120px;
      margin-left: 50px;
      color: #fff;
      font-size: 20px;
      font-weight: 500;
    }

    .menu li {
      list-style: none;
      display: inline-block;
    }

    .menu li a {
      text-decoration: none;
      color: #fff;
      font-size: 27px;
      font-weight: 600;
      margin-left: 25px;
      transition: .4s ease;
    }

    .menu li a:hover {
      color: crimson;
      padding: 10px 20px;
      border: 2px solid #fff;
    }

    .home {
      padding: 70px;
      text-align: center;
    }

    .title-1 {
      font-size: 56px;
      color: #fff;
      font-weight: 600;
    }

    .home p {
      color: yellow;
      font-size: 25px;
      padding-top: 10px;
    }

    .image-row {
      display: flex;
      justify-content: center;
      gap: 30px;
      margin-top: 40px;
      flex-wrap: wrap;
    }

    .image-row img {
      width: 1400px;
      height: 700px;
      object-fit: cover;
      border-radius: 10px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.4);
      transition: transform 0.3s ease;
    }

    .image-row img:hover {
      transform: scale(1.05);
    }
  </style>
</head>  
<body>  
  <div class="container"> 
    <div class="nav-bar">  
      <h1 class="title">Moonlit Saphore</h1> 
      <p>Elegant. Enchanting. Exquisite.</p>  
      <ul class="menu"> 
        <li><a href="home.html">HOME</a></li>  
        <li><a href="menu.html">MENU</a></li> 
        <li><a href="administration.html">ADMIN</a></li>  
        <li><a href="contact.html">CONTACT</a></li> 
      </ul>  
    </div>
    <div class="home">
      <h1 class="title-1">"Taste the magic that shines beyond the stars."</h1>
      <p>Moonlit Saphore invites you to indulge in culinary delights inspired by the mystery <br>
      and beauty of the night sky. Every dish is a celebration of flavor and ambiance, designed to enchant<br>your senses and elevate your dining experience.</p>
      
      <div class="image-row">
        <img src="Screenshot 2025-05-16 010004.png" alt="Restaurant interior">
      </div>
    </div>
  </div>
</body>
</html>


menu.html

<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menu - Moonlit Saphore</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background-color: #080808;
            color: #f5f2f2;
        }

        header {
            background-color: #9b1b1b;
            color: #fff;
            padding: 20px 0;
            text-align: center;
        }

        header h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }

        nav ul {
            list-style-type: none;
            display: flex;
            justify-content: center;
            gap: 20px;
        }

        nav a {
            color: #fff;
            text-decoration: none;
            font-size: 1.2rem;
            transition: color 0.3s ease;
        }

        nav a:hover {
            color: #f4a261; /* Light orange on hover */
        }

        main {
            padding: 40px 20px;
            text-align: center;
        }

        h2 {
            font-size: 2rem;
            margin-bottom: 20px;
            color: #ffffff;
        }

        .menu-list {
            list-style-type: none;
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
            justify-items: center;
        }

        .menu-list li {
            width: 300px;
            background-color: #1d0404;
            padding: 15px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(225, 224, 224, 0.1);
            text-align: center;
        }

        .menu-list img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            border-radius: 10px;
            margin-bottom: 15px;
        }

        .menu-list li p {
            font-size: 1.1rem;
            color: #fffdfd;
            font-weight: bold;
        }

        .menu-list li:hover {
            transform: translateY(-5px);
            box-shadow: 0 6px 12px rgba(255, 255, 255, 0.15);
        }

        footer {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>
    <header>
        <h1>Our Menu</h1>
        <nav>
            <ul>
                <li><a href="home.html">Home</a></li>
                <li><a href="menu.html">Menu</a></li>
                <li><a href="administration.html">Administration</a></li>
                <li><a href="contact.html">Contact Us</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <h2>Food Items</h2>
        <ul class="menu-list">
            <li><img src="Biryani.jpeg" alt="Food Item 1">Pizza - $10</li>
            <li><img src="Chocolate Shrikhand-video recipe.jpeg" alt="Food Item 2">Burger - $8</li>
            <li><img src="Classic Cheeseburger with Melted Cheese Drip😋.jpeg" alt="Food Item 3">Pasta - $12</li>
            <li><img src="Fish fry.jpeg" alt="Food Item 4">Salad - $7</li>
            <li><img src="Masala Noodles _ Video - NISH KITCHEN.jpeg" alt="Food Item 5">Nuggets - $15</li>
            <li><img src="mutton chukka.jpeg" alt="Food Item 6">Ice Cream - $5</li>
            <li><img src="paratha.jpeg" alt="Food Item 7">Sandwich - $6</li>
            <li><img src="pizza.jpeg" alt="Food Item 8">French Fries - $4</li>
            <li><img src="Pork Meal.jpeg" alt="Food Item 9">Soup - $5</li>
            <li><img src="Prawn Balti.jpeg" alt="Food Item 10">Chocolate Cake - $6</li>
            <li><img src="tandoori.jpeg" alt="Food Item 11">Smiley Fries - $6</li>
        </ul>
    </main>
    <footer>
        <p>&copy; 2025 Nabithra</p>
    </footer>
</body>
</html>


administration.html

<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Administration - Moonlit Saphore</title>
    <style>
     *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
      }

body {
    font-family: Arial, sans-serif;
    background-color: #3a3636;
    color: #fffefe;
}

header {
    background-color: #643030;
    color: #fff;
    padding: 20px 0;
    text-align: center;
}

header h1 {
    font-size: 2.5rem;
    margin-bottom: 10px;
}

nav ul {
    list-style-type: none;
    display: flex;
    justify-content: center;
    gap: 20px;
}

nav a {
    color: #fff;
    text-decoration: none;
    font-size: 1.2rem;
    transition: color 0.3s ease;
}

nav a:hover {
    color: #f4a261; 
}

main {
    padding: 40px 20px;
    text-align: center;
}

h2 {
    font-size: 2rem;
    margin-bottom: 20px;
    color: #333;
}


.team {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 30px;
    justify-items: center;
    margin-top: 30px;
}

.member {
    background-color: #090606;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    text-align: center;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.member img {
    width: 100%;
    height: auto;
    border-radius: 50%;
    margin-bottom: 15px;
    border: 4px solid #f4a261; 
}

.member h3 {
    font-size: 1.5rem;
    margin-bottom: 10px;
    color: #f2f2f2;
}

.member p {
    font-size: 1.1rem;
    color: #ffffff;
}

.member:hover {
    transform: translateY(-5px);
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
}

h3 {
    margin-bottom: 10px;
    font-size: 1.5rem;
    color: #eae9e9;
}

footer {
    background-color: #333;
    color: #5b4f4f;
    text-align: center;
    padding: 10px;
    position: fixed;
    bottom: 0;
    width: 100%;
}
</style>
</head>
<body>
    <header>
        <h1>Administration Team</h1>
        <nav>
            <ul>
                <li><a href="home.html">Home</a></li>
                <li><a href="menu.html">Menu</a></li>
                <li><a href="administration.html">Administration</a></li>
                <li><a href="contact.html">Contact Us</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <h2>Meet Our Team</h2>
        <div class="team">
            <div class="member">
                <img src="ceo.jpeg" alt="Member 1">
                <h3>Ananya Venkat</h3>
                <p>CEO</p>
            </div>
            <div class="member">
                <img src="market.jpeg" alt="Member 2">
                <h3>Kimson<h3>
                <p>Marketing Manager</p>
            </div>
            <div class="member">
                <img src="oper.jpeg" alt="Member 3">
                <h3>Seong<h3>
                <p>Operations Manager</p>
            </div>
            <div class="member">
                <img src="hr.jpeg" alt="Member 4">
                <h3>Grace<h3>
                <p>HR Manager</p>
            </div>
            <div class="member">
                <img src="chef.jpeg" alt="Member 5">
                <h3>Faizal<h3>
                <p>Executive Chef</p>
            </div>
            <div class="member">
                <img src="customer.jpeg" alt="Member 6">
                <h3>Aria<h3>
                <p>Customer Service Manger</p>
            </div>
        </div>
    </main>
</body>
</html>

contact.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Contact - Moonlit Saphore</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-image: url('https://media.istockphoto.com/id/2196880285/photo/spices-and-herbs-on-graphite-board.jpg?s=2048x2048&w=is&k=20&c=92O_RN6uOchDpzMeNaaWDPfULGoGWhhadBFyN1Wl0yI=');
      background-size: cover;
      background-position: center;
      color: #333;
    }

    #contact {
      background-color: #d1ba85;
      padding: 80px 20px;
      margin: 400px auto;
      max-width: 800px;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
      text-align: center;
    }

    #contact h2 {
      font-size: 5rem;
      margin-bottom: 30px;
      color: #333;
    }

    #contact p, address {
      font-size: 3rem;
      margin-bottom: 20px;
      color: #555;
    }

    address {
      font-style: normal;
    }
  </style>
</head>
<body>
  <section id="contact">
    <h2>Contact Us</h2>
    <p>Visit us at:</p>
    <address>
      156 Cresta Street, Alpha area, India<br>
      Phone: (123) 456-7890<br>
      Email: moonlit@gmail.com
    </address>
  </section>
</body>
</html>


```
## OUTPUT:
![alt text](<Screenshot 2025-05-17 010754.png>)
![alt text](<Screenshot 2025-05-17 010818.png>)
![alt text](<Screenshot 2025-05-17 010838.png>)
![alt text](<Screenshot 2025-05-17 010900.png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
