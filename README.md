<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Local Restaurant</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Header Section -->
    <header>
        <div class="logo">
            <h1>Local Restaurant</h1>
        </div>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#menu">Menu</a></li>
                <li><a href="#reservation">Reservation</a></li>
                <li><a href="#location">Location</a></li>
                <li><a href="#reviews">Reviews</a></li>
            </ul>
        </nav>
    </header>

    <!-- Home Section -->
    <section id="home">
        <div class="hero">
            <h2>Welcome to Local Restaurant</h2>
            <p>Great food, cozy ambiance, and the best service in town!</p>
        </div>
    </section>

    <!-- Menu Section -->
    <section id="menu">
        <div class="container">
            <h2>Our Menu</h2>
            <div class="menu-item">
                <img src="https://via.placeholder.com/250x150" alt="Dish 1">
                <h3>Dish 1</h3>
                <p>A delicious dish made with fresh ingredients.</p>
                <p class="price">$12.99</p>
            </div>
            <div class="menu-item">
                <img src="https://via.placeholder.com/250x150" alt="Dish 2">
                <h3>Dish 2</h3>
                <p>A special dish served with a side of love.</p>
                <p class="price">$15.99</p>
            </div>
            <div class="menu-item">
                <img src="https://via.placeholder.com/250x150" alt="Dish 3">
                <h3>Dish 3</h3>
                <p>A healthy and flavorful choice for your meal.</p>
                <p class="price">$10.99</p>
            </div>
        </div>
    </section>

    <!-- Reservation Section -->
    <section id="reservation">
        <div class="container">
            <h2>Make a Reservation</h2>
            <form action="#">
                <label for="name">Full Name</label>
                <input type="text" id="name" name="name" required>

                <label for="email">Email</label>
                <input type="email" id="email" name="email" required>

                <label for="phone">Phone</label>
                <input type="tel" id="phone" name="phone" required>

                <label for="date">Reservation Date</label>
                <input type="date" id="date" name="date" required>

                <label for="time">Reservation Time</label>
                <input type="time" id="time" name="time" required>

                <button type="submit">Reserve Table</button>
            </form>
        </div>
    </section>

    <!-- Location Section with Google Maps Embed -->
    <section id="location">
        <div class="container">
            <h2>Our Location</h2>
            <div class="map">
                <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3153.014174460059!2d-122.41941838468124!3d37.77492927975987!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x8085809cc6601b2b%3A0x526750e698ce5e58!2sSan%20Francisco%2C%20CA!5e0!3m2!1sen!2sus!4v1676184285401!5m2!1sen!2sus" width="100%" height="450" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
            </div>
        </div>
    </section>

    <!-- Customer Reviews Section -->
    <section id="reviews">
        <div class="container">
            <h2>What Our Customers Say</h2>
            <div class="review">
                <p>"The food was amazing and the service was excellent. Highly recommend this place!" - John D.</p>
            </div>
            <div class="review">
                <p>"Great atmosphere and delicious dishes. Will definitely come back!" - Emily S.</p>
            </div>
            <div class="review">
                <p>"A hidden gem in the city. Loved every bite!" - Mark T.</p>
            </div>
        </div>
    </section>

    <!-- Footer Section -->
    <footer>
        <p>&copy; 2025 Local Restaurant | All Rights Reserved</p>
    </footer>
</body>
</html>
css code
/* Reset some default styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    color: #333;
}

/* Header Styles */
header {
    background-color: #333;
    color: white;
    padding: 1rem 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

header .logo h1 {
    margin-left: 20px;
}

header nav ul {
    list-style: none;
    display: flex;
}

header nav ul li {
    margin: 0 15px;
}

header nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 1.1rem;
}

/* Hero Section */
#home {
    background: url('https://via.placeholder.com/1200x600') no-repeat center center/cover;
    text-align: center;
    padding: 100px 0;
    color: white;
}

#home h2 {
    font-size: 3rem;
}

#home p {
    font-size: 1.5rem;
    margin-top: 10px;
}

/* Menu Section */
#menu {
    background-color: #fff;
    padding: 50px 0;
}

#menu .container {
    width: 80%;
    margin: 0 auto;
}

#menu h2 {
    text-align: center;
    font-size: 2.5rem;
    margin-bottom: 30px;
}

.menu-item {
    margin-bottom: 30px;
    text-align: center;
}

.menu-item img {
    width: 250px;
    height: 150px;
    object-fit: cover;
    border-radius: 10px;
}

.menu-item h3 {
    font-size: 2rem;
    margin-top: 10px;
}

.menu-item p {
    font-size: 1.2rem;
    color: #777;
}

.price {
    font-size: 1.3rem;
    font-weight: bold;
    margin-top: 5px;
}

/* Reservation Section */
#reservation {
    background-color: #f9f9f9;
    padding: 50px 0;
}

#reservation .container {
    width: 60%;
    margin: 0 auto;
    text-align: center;
}

#reservation form {
    display: flex;
    flex-direction: column;
    align-items: center;
}

#reservation label {
    margin: 10px 0;
    font-size: 1.1rem;
}

#reservation input, #reservation button {
    width: 80%;
    max-width: 500px;
    padding: 10px;
    margin-bottom: 15px;
    font-size: 1rem;
}

#reservation button {
    background-color: #333;
    color: white;
    border: none;
    cursor: pointer;
}

#reservation button:hover {
    background-color: #555;
}

/* Location Section */
#location {
    padding: 50px 0;
    background-color: #fff;
}

.map iframe {
    border: 0;
    width: 100%;
    height: 450px;
}

/* Customer Reviews Section */
#reviews {
    background-color: #f9f9f9;
    padding: 50px 0;
}

#reviews .container {
    width: 80%;
    margin: 0 auto;
    text-align: center;
}

#reviews .review {
    margin-bottom: 20px;
    font-size: 1.2rem;
}

/* Footer */
footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px 0;
}
