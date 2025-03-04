# Diamond-Perfume
Diamond Perfume is your perfect destination for luxurious and distinctive fragrances. The store offers a selection of luxury fragrances that combine elegance and luxury, with elegant diamond-inspired packaging.
/* General Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  
  body {
    font-family: "Montserrat", sans-serif;
    line-height: 1.6;
    color: #333;
  }
  
  /* Container */
  .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
  }
  
  /* Header */
  .header {
    background: #111;
    color: #fff;
    padding: 15px 0;
    position: sticky;
    top: 0;
    z-index: 1000;
  }
  
  .header-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  .header .logo {
    font-size: 2rem;
    font-weight: bold;
  }
  
  .nav {
    display: flex;
    align-items: center;
  }
  
  .nav-list {
    list-style: none;
    display: flex;
    gap: 20px;
  }
  
  .nav-list a {
    color: #fff;
    text-decoration: none;
    font-weight: 700;
    transition: color 0.3s ease-in-out;
  }
  
  .nav-list a:hover {
    color: #ff8c00;
  }
  
  .mobile-menu {
    display: none;
    cursor: pointer;
    flex-direction: column;
    gap: 5px;
  }
  
  .menu-bar {
    width: 30px;
    height: 3px;
    background: #fff;
    border-radius: 5px;
  }
  
  /* Hero Section */
  .hero {
    height: 100vh;
    background: url("candles.jpg") no-repeat left center/cover;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #fff;
    text-align: left;
  }
  
  .hero-content {
    animation: fadeIn 2s ease-in-out;
  }
  
  @keyframes fadeIn {
    from {
      opacity: 0;
      transform: translateY(30px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }
  
  .hero-content h2 {
    font-size: 3rem;
    margin-bottom: 15px;
  }
  
  .hero-content p {
    font-size: 1.3rem;
    margin-bottom: 25px;
  }
  
  .btn {
    display: inline-block;
    background: #ff8c00;
    color: #fff;
    padding: 12px 25px;
    border: none;
    border-radius: 25px;
    text-decoration: none;
    font-size: 1rem;
    cursor: pointer;
    transition: background 0.3s ease-in-out, transform 0.2s ease-in-out;
  }
  
  .btn:hover {
    background: #e07a00;
    transform: translateY(-3px);
  }
  
  /* Products Section */
  .products {
    padding: 60px 20px;
    text-align: center;
    background: #f9f9f9;
  }
  
  .section-title {
    font-size: 2.5rem;
    margin-bottom: 30px;
  }
  
  .product-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(270px, 1fr));
    gap: 30px;
  }
  
  .product {
    background: #fff;
    border-radius: 15px;
    padding: 20px;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;
  }
  
  .product:hover {
    transform: scale(1.05);
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15);
  }
  
  .product img {
    width: 100%;
    height: auto;
    border-radius: 10px;
  }
  
  .product-info {
    text-align: left;
    margin-top: 15px;
  }
  
  .product h3 {
    font-size: 1.5rem;
    margin-bottom: 5px;
  }
  
  .price {
    color: #ff8c00;
    font-weight: bold;
  }
  
  .description {
    margin: 10px 0;
    font-size: 0.9rem;
  }
  /* About Section */
  .about {
    padding: 50px 20px;
    background: #fff;
    text-align: center;
  }
  
  .about-container {
    max-width: 800px;
    margin: 0 auto;
  }
  
  /* Contact Section */
  .contact {
    padding: 50px 20px;
    background: #f9f9f9;
    text-align: center;
  }
  
  .contact-form {
    max-width: 500px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    gap: 15px;
  }
  
  .contact-form input,
  .contact-form textarea {
    width: 100%;
    padding: 10px;
    border: 1px solid #ddd;
    border-radius: 5px;
  }
  /* Footer */
  .footer {
    background: #111;
    color: #fff;
    padding: 25px 0;
  }
  
  .footer-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
  }
  
  .footer-content p {
    margin-bottom: 10px;
  }
  
  /* Responsive Design */
  @media (max-width: 768px) {
    .mobile-menu {
      display: flex;
    }
  
    .nav-list {
      display: none;
      flex-direction: column;
      gap: 10px;
      background: #222;
      position: absolute;
      top: 100%;
      right: 20px;
      padding: 15px;
      border-radius: 5px;
    }
  
    .nav-list.show {
      display: flex;
    }
  
    .hero-content h2 {
      font-size: 2.5rem;
    }
  
    .hero-content p {
      font-size: 1.1rem;
    }
  }
