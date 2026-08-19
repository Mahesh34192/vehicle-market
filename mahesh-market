<!DOCTYPE html>
<html lang="si">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Mahesh Market</title>

<style>
*{
  box-sizing:border-box;
  margin:0;
  padding:0;
  font-family:Arial,sans-serif;
}

body{
  background:#f4f6f8;
  color:#222;
}

header{
  background:#111827;
  color:white;
  padding:20px;
  text-align:center;
}

header h1{
  font-size:30px;
}

header p{
  margin-top:8px;
  font-size:15px;
}

.search{
  padding:18px;
  background:white;
}

.search input{
  width:100%;
  padding:14px;
  border:1px solid #ddd;
  border-radius:10px;
  font-size:16px;
}

.categories{
  display:flex;
  gap:10px;
  overflow-x:auto;
  padding:15px;
  background:white;
}

.categories button{
  border:0;
  background:#e5e7eb;
  padding:11px 16px;
  border-radius:20px;
  white-space:nowrap;
  cursor:pointer;
}

.categories button:hover{
  background:#111827;
  color:white;
}

.products{
  padding:18px;
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
  gap:18px;
}

.card{
  background:white;
  border-radius:14px;
  overflow:hidden;
  box-shadow:0 3px 12px rgba(0,0,0,.10);
}

.card img{
  width:100%;
  height:210px;
  object-fit:cover;
}

.info{
  padding:15px;
}

.info h3{
  font-size:19px;
  margin-bottom:8px;
}

.category{
  color:#666;
  font-size:14px;
}

.price{
  font-size:21px;
  font-weight:bold;
  margin:10px 0;
}

.stock{
  color:green;
  margin-bottom:12px;
}

.order{
  width:100%;
  border:0;
  padding:12px;
  border-radius:8px;
  background:#16a34a;
  color:white;
  font-size:16px;
  cursor:pointer;
}

footer{
  margin-top:30px;
  padding:25px;
  background:#111827;
  color:white;
  text-align:center;
}

@media(max-width:500px){
  header h1{
    font-size:24px;
  }

  .products{
    grid-template-columns:repeat(2,1fr);
    padding:10px;
    gap:10px;
  }

  .card img{
    height:150px;
  }

  .info{
    padding:10px;
  }

  .info h3{
    font-size:16px;
  }

  .price{
    font-size:17px;
  }
}
</style>
</head>

<body>

<header>
  <h1>🛒 Mahesh Market</h1>
  <p>විදුලි උපකරණ • Electronics • Home & Furniture</p>
</header>

<div class="search">
  <input
    type="text"
    id="searchBox"
    placeholder="🔎 භාණ්ඩයක් සොයන්න..."
    onkeyup="searchProducts()">
</div>

<div class="categories">
  <button onclick="filterProducts('all')">සියල්ල</button>
  <button onclick="filterProducts('tv')">📺 TV</button>
  <button onclick="filterProducts('fridge')">🧊 Fridge</button>
  <button onclick="filterProducts('laptop')">💻 Laptop</button>
  <button onclick="filterProducts('computer')">🖥️ Computer</button>
  <button onclick="filterProducts('phone')">📱 Phone</button>
  <button onclick="filterProducts('oven')">🍳 Oven</button>
  <button onclick="filterProducts('washing')">🧺 Washing Machine</button>
  <button onclick="filterProducts('furniture')">🛋️ Furniture</button>
  <button onclick="filterProducts('electrical')">⚡ Electrical</button>
  <button onclick="filterProducts('aluminium')">🔩 Aluminium</button>
</div>

<div class="products" id="products">

  <div class="card" data-category="tv" data-name="Samsung Smart TV">
    <img src="https://images.unsplash.com/photo-1593359677879-a4bb92f829d1" alt="TV">
    <div class="info">
      <h3>Samsung Smart TV</h3>
      <p class="category">📺 TV</p>
      <p class="price">රු. 125,000</p>
      <p class="stock">✓ Stock Available</p>
      <button class="order" onclick="order('Samsung Smart TV')">
        Order Now
      </button>
    </div>
  </div>

  <div class="card" data-category="fridge" data-name="LG Refrigerator">
    <img src="https://images.unsplash.com/photo-1571175443880-49e1d25b2bc5" alt="Fridge">
    <div class="info">
      <h3>LG Refrigerator</h3>
      <p class="category">🧊 Fridge</p>
      <p class="price">රු. 185,000</p>
      <p class="stock">✓ Stock Available</p>
      <button class="order" onclick="order('LG Refrigerator')">
        Order Now
      </button>
    </div>
  </div>

  <div class="card" data-category="laptop" data-name="HP Laptop">
    <img src="https://images.unsplash.com/photo-1496181133206-80ce9b88a853" alt="Laptop">
    <div class="info">
      <h3>HP Laptop</h3>
      <p class="category">💻 Laptop</p>
      <p class="price">රු. 165,000</p>
      <p class="stock">✓ Stock Available</p>
      <button class="order" onclick="order('HP Laptop')">
        Order Now
      </button>
    </div>
  </div>

  <div class="card" data-category="computer" data-name="Desktop Computer">
    <img src="https://images.unsplash.com/photo-1593640408182-31c70c8268f5" alt="Computer">
    <div class="info">
      <h3>Desktop Computer</h3>
      <p class="category">🖥️ Computer</p>
      <p class="price">රු. 145,000</p>
      <p class="stock">✓ Stock Available</p>
      <button class="order" onclick="order('Desktop Computer')">
        Order Now
      </button>
    </div>
  </div>

  <div class="card" data-category="phone" data-name="Samsung Galaxy Phone">
    <img src="https://images.unsplash.com/photo-1511707171634-5f897ff02aa9" alt="Phone">
    <div class="info">
      <h3>Samsung Galaxy Phone</h3>
      <p class="category">📱 Phone</p>
      <p class="price">රු. 95,000</p>
      <p class="stock">✓ Stock Available</p>
      <button class="order" onclick="order('Samsung Galaxy Phone')">
        Order Now
      </button>
    </div>
  </div>

  <div class="card" data-category="oven" data-name="Electric Oven">
    <img src="https://images.unsplash.com/photo-1585659722983-3a675dabf23d" alt="Oven">
    <div class="info">
      <h3>Electric Oven</h3>
      <p class="category">🍳 Oven</p>
      <p class="price">රු. 75,000</p>
      <p class="stock">✓ Stock Available</p>
      <button class="order" onclick="order('Electric Oven')">
        Order Now
      </button>
    </div>
  </div>

  <div class="card" data-category="washing" data-name="Washing Machine">
    <img src="https://images.unsplash.com/photo-1626806787461-102c1bfaaea1" alt="Washing Machine">
    <div class="info">
      <h3>Washing Machine</h3>
      <p class="category">🧺 Washing Machine</p>
      <p class="price">රු. 135,000</p>
      <p class="stock">✓ Stock Available</p>
      <button class="order" onclick="order('Washing Machine')">
        Order Now
      </button>
    </div>
  </div>

  <div class="card" data-category="furniture" data-name="Modern Sofa">
    <img src="https://images.unsplash.com/photo-1555041469-a586c61ea9bc" alt="Furniture">
    <div class="info">
      <h3>Modern Sofa</h3>
      <p class="category">🛋️ Furniture</p>
      <p class="price">රු. 120,000</p>
      <p class="stock">✓ Stock Available</p>
      <button class="order" onclick="order('Modern Sofa')">
        Order Now
      </button>
    </div>
  </div>

</div>

<footer>
  <h3>Mahesh Market</h3>
  <p>Quality Products • Best Prices</p>
  <p>📞 WhatsApp / Phone Orders Available</p>
</footer>

<script>

function filterProducts(category){

  let products = document.querySelectorAll('.card');

  products.forEach(function(product){

    if(category === 'all'){
      product.style.display = 'block';
    }
    else if(product.dataset.category === category){
      product.style.display = 'block';
    }
    else{
      product.style.display = 'none';
    }

  });
}

function searchProducts(){

  let search = document
    .getElementById('searchBox')
    .value
    .toLowerCase();

  let products = document.querySelectorAll('.card');

  products.forEach(function(product){

    let name = product.dataset.name.toLowerCase();

    if(name.includes(search)){
      product.style.display = 'block';
    }
    else{
      product.style.display = 'none';
    }

  });
}

function order(product){

  let message =
    "මට මේ භාණ්ඩය Order කිරීමට අවශ්‍යයි:%0A%0A" +
    "භාණ්ඩය: " + product;

  let phone = "94751551758";

  window.open(
    "https://wa.me/" + phone + "?text=" + message,
    "_blank"
  );
}

</script>

</body>
</html>
