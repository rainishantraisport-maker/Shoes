# Shoes
Bzhzbs6

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Shoe Store</title>
<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, sans-serif;
}

body {
  background: #f5f5f5;
  color: #222;
}

header {
  background: #111;
  color: white;
  padding: 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

header h2 { color: orange; }

nav a {
  color: white;
  text-decoration: none;
  margin-left: 15px;
}

.hero {
  text-align: center;
  padding: 60px 20px;
  background: #222;
  color: white;
}

.hero h1 {
  font-size: 35px;
  margin-bottom: 15px;
}

.hero button {
  background: orange;
  border: none;
  padding: 12px 25px;
  margin-top: 20px;
  border-radius: 5px;
  cursor: pointer;
}

.products {
  padding: 35px 20px;
  text-align: center;
}

.container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 20px;
  margin-top: 25px;
}

.card {
  background: white;
  width: 230px;
  padding: 15px;
  border-radius: 12px;
  box-shadow: 0 3px 10px #ddd;
}

.card img {
  width: 100%;
  height: 150px;
  object-fit: contain;
}

.card h3 { margin: 10px; }

.price {
  color: #e87500;
  font-weight: bold;
  margin: 10px;
}

.card button {
  background: #111;
  color: white;
  border: none;
  padding: 10px 20px;
  border-radius: 5px;
  cursor: pointer;
}

.card button:hover {
  background: orange;
}

footer {
  background: #111;
  color: white;
  text-align: center;
  padding: 20px;
  margin-top: 30px;
}
</style>
</head>

<body>

<header>
  <h2>SHOEZONE</h2>
  <nav>
    <a href="#">Home</a>
    <a href="#products">Shoes</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<section class="hero">
  <h1>Step Into Style</h1>
  <p>Discover Premium Shoes At Amazing Prices.</p>
  <button onclick="document.getElementById('products').scrollIntoView()">
    Shop Now
  </button>
</section>

<section class="products" id="products">
  <h2>Our Latest Collection</h2>

  <div class="container">

    <div class="card">
      <img src="https://placehold.co/300x200?text=Running+Shoes">
      <h3>Running Shoes</h3>
      <p class="price">₹1,499</p>
      <button onclick="buy('Running Shoes')">Buy Now</button>
    </div>

    <div class="card">
      <img src="https://placehold.co/300x200?text=Sneakers">
      <h3>Casual Sneakers</h3>
      <p class="price">₹1,999</p>
      <button onclick="buy('Casual Sneakers')">Buy Now</button>
    </div>

    <div class="card">
      <img src="https://placehold.co/300x200?text=Sports+Shoes">
      <h3>Sports Shoes</h3>
      <p class="price">₹1,799</p>
      <button onclick="buy('Sports Shoes')">Buy Now</button>
    </div>

  </div>
</section>

<footer id="contact">
  <p>© 2026 SHOEZONE | All Rights Reserved</p>
</footer>

<script>
function buy(product) {
  alert("You selected: " + product);
}
</script>

</body>
</html>
