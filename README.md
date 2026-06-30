# hanmanth-.D2
I BUILT A NEW WEBSITE THROUGH HTML ,CSS, JAVA SCRIPT 
```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>PhoneHub Store</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}

body{
background:#ffffff;
color:#222;
}

header{
background:linear-gradient(90deg,#ffffff,#ffd9e6,#8b5e3c,#000000);
padding:20px;
display:flex;
justify-content:space-between;
align-items:center;
color:white;
}

.logo{
font-size:30px;
font-weight:bold;
}

nav a{
color:white;
text-decoration:none;
margin:0 15px;
font-weight:bold;
}

.hero{
height:60vh;
display:flex;
justify-content:center;
align-items:center;
text-align:center;
background:linear-gradient(to right,#ffffff,#ffe5ee);
}

.hero-content h1{
font-size:50px;
margin-bottom:15px;
color:#8b5e3c;
}

.hero-content p{
font-size:18px;
margin-bottom:20px;
}

button{
padding:12px 25px;
border:none;
border-radius:25px;
cursor:pointer;
background:black;
color:white;
font-size:16px;
transition:.3s;
}

button:hover{
background:#8b5e3c;
}

.products{
padding:50px;
}

.products h2{
text-align:center;
margin-bottom:30px;
color:#8b5e3c;
}

.product-grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:30px;
}

.card{
background:white;
border-radius:20px;
padding:20px;
box-shadow:0 4px 15px rgba(0,0,0,0.2);
text-align:center;
transition:.3s;
}

.card:hover{
transform:translateY(-10px);
}

.card img{
width:100%;
height:220px;
object-fit:cover;
border-radius:15px;
}

.price{
font-size:22px;
color:#ff4d88;
margin:10px;
font-weight:bold;
}

.cart{
position:fixed;
bottom:20px;
right:20px;
background:black;
padding:15px;
border-radius:50%;
color:white;
font-size:22px;
cursor:pointer;
}

footer{
background:black;
color:white;
padding:25px;
text-align:center;
margin-top:50px;
}
</style>

</head>
<body>

<header>
<div class="logo">PhoneHub</div>

<nav>
<a href="#">Home</a>
<a href="#">Phones</a>
<a href="#">Parts</a>
<a href="#">Accessories</a>
<a href="#">Contact</a>
</nav>

</header>

<section class="hero">
<div class="hero-content">
<h1>Latest Phones & Accessories</h1>
<p>Order phones, spare parts, and accessories online with fast delivery.</p>
<button>Shop Now</button>
</div>
</section>

<section class="products">
<h2>Featured Products</h2>

<div class="product-grid">

<div class="card">
<img src="https://images.unsplash.com/photo-1511707171634-5f897ff02aa9" alt="">
<h3>iPhone 15 Pro</h3>
<p class="price">$999</p>
<button onclick="addCart()">Add To Cart</button>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1598327105666-5b89351aff97" alt="">
<h3>Samsung S25</h3>
<p class="price">$899</p>
<button onclick="addCart()">Add To Cart</button>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1583394838336-acd977736f90" alt="">
<h3>Wireless Earbuds</h3>
<p class="price">$59</p>
<button onclick="addCart()">Add To Cart</button>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1600086827875-a63b01f1335c" alt="">
<h3>Phone Screen</h3>
<p class="price">$99</p>
<button onclick="addCart()">Add To Cart</button>
</div>

</div>
</section>

<div class="cart" id="cart">
🛒 <span id="count">0</span>
</div>

<footer>
<p>© 2026 PhoneHub Store | Fast Delivery | Secure Shopping</p>
</footer>

<script>

let count=0;

function addCart(){
count++;
document.getElementById("count").innerText=count;
alert("Product added to cart");
}

</script>

</body>
</html>
```

