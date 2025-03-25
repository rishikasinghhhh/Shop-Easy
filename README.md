<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ShopEasy - Your Online Store</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
<body>
    <header>
        <div class="container">
            <div class="logo">
                <h1>ShopEasy</h1>
            </div>
            <nav>
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#products">Products</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
            <div class="cart-icon">
                <i class="fas fa-shopping-cart"></i>
                <span class="cart-count">0</span>
            </div>
        </div>
    </header>

    <main>
        <section class="hero">
            <div class="container">
                <h2>Welcome to ShopEasy</h2>
                <p>Discover amazing products at unbeatable prices</p>
                <a href="#products" class="btn">Shop Now</a>
            </div>
        </section>

        <section id="products" class="products">
            <div class="container">
                <h2>Our Products</h2>
                <div class="product-filters">
                    <button class="filter-btn active" data-filter="all">All</button>
                    <button class="filter-btn" data-filter="electronics">Electronics</button>
                    <button class="filter-btn" data-filter="clothing">Clothing</button>
                    <button class="filter-btn" data-filter="home">Home</button>
                </div>
                <div class="product-grid" id="product-grid">
                    <!-- Products will be loaded here via JavaScript -->
                </div>
            </div>
        </section>

        <section id="about" class="about">
            <div class="container">
                <h2>About Us</h2>
                <p>ShopEasy is your one-stop online shop for all your needs. We offer high-quality products at competitive prices with excellent customer service.</p>
            </div>
        </section>

        <section id="contact" class="contact">
            <div class="container">
                <h2>Contact Us</h2>
                <form id="contact-form">
                    <input type="text" placeholder="Your Name" required>
                    <input type="email" placeholder="Your Email" required>
                    <textarea placeholder="Your Message" required></textarea>
                    <button type="submit" class="btn">Send Message</button>
                </form>
            </div>
        </section>
    </main>

    <!-- Shopping Cart Sidebar -->
    <div class="cart-sidebar">
        <div class="cart-header">
            <h3>Your Cart</h3>
            <button class="close-cart">&times;</button>
        </div>
        <div class="cart-items">
            <!-- Cart items will be loaded here -->
        </div>
        <div class="cart-footer">
            <div class="cart-total">
                <span>Total:</span>
                <span class="total-price">$0.00</span>
            </div>
            <button class="btn checkout-btn">Checkout</button>
        </div>
    </div>
    <div class="overlay"></div>

    <footer>
        <div class="container">
            <p>&copy; 2023 ShopEasy. All rights reserved.</p>
        </div>
    </footer>

    <script src="script.js"></script>
</body>
</html>
