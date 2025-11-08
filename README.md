<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewpoint"content="width=device-width,initial-scale=1.0">
    <Perfume Paradise \ Luxury Fragrances>
        <link rel="stylesheet" href="https://cdnjs.cloudfare.com/ajax/libs/font-awesome/6.4/css/all.min.css">
        <style>
            /* Global Styles */
            *{
                margin:0;
                padding:0;
                box-sizing: border-box;
                font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            }

            :root{
                --primary:#a6d3b;
                --secondary:#d4af37;
                --dark:#1a1a1a;
                --light:#f8f8f8;
                --gray:#e0e0e0;
                --text:#333333         
            }

           body{
            background-color: var(--light);
            color:var(--text);
            line-height: 1.6;
           } 

           .container{
            max-width: 1200px
            margin: 0 auto;
            padding: 0 20px;
           }

           .btn{
            display: inline-block;
            padding: 12px 24px;
            background-color: var(--primary);
            color:white;
            border: none
            border-radius: 4px;
            cursor: pointer;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: all 0.3s ease;
           }

           .btn:hover{
            background-color: var(--secondary);
            tranform:translateY(-2px);
           }

           .btn-outline{
            background-color: transparent;
            border: 2px solid var(--primary);
            color: var(--primary);
           }

           .btn-outline:hover{
            background-color: var(--primary);
            color: white;
           }

           section{
            padding: 80px 0;
           }

           .section-title{
            text-align:center;
            margin-bottom: 50px;
            font-size: 2.5rem;
            color: var(--dark);
            position: relative;
           }

           .section-title::after{
            text-align: center;
            margin-bottom: 50px;
            font-size: 2.5rem;
            color: var(--dark);
            position: relative;
           }

           .section-title::after{
            content: '';
            position: absolute;
            bottom: -15px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 3px;
            background-color: var(--secondary);
           }

           /* Header Styles */
           header {
            background-color: white;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
           }

           .header-container{
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
           }

           .logo{
            font-size: 1.9rem;
            font-weight: 700;
            color: var(--primary);
            text-decoration: none;
           }

           .logo span{
            color: var(--secondary);
           }

           nav ul li a{
            text-decoration: none;
            color: var(--text);
            font-weight: 500;
            transition: color 0.3s ease;
           }

           nav ul li a:hover{
            color: var(--primary);
           }

           .header-icons{
            display: flex;
            align-items: center;
           }

           .header-icons a{
            margin-left: 20px;
            color: var(--text);
            font-size: 1.2rem;
            transition: color 0.3s ease;
           }

           .header-icons a:hover{
            color: var(--primary);
           }

           .cart-count{
            background-color: var(--primary);
            color: white;
            border-radius: 50%;
            width: 18px;
            height: 18px;
            font-size: 0.7rem;
            display: flex;
            justify-content: center;
            align-items: center;
            position: absolute;
            top: -8px;
            right: -8px;
           }

           cart-icon{
            position: relative;
           }

           .mobile-menu{
            display: none;
            font-size: 1.5rem;
            cursor: pointer;
           }

           /* Hero Section */
           .hero{
            background: linear-gradient(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7);url('https://images.unsplash.com/photo-1547887537-6158d64c35b3?)ixlib=rb-4.0.3&auto=format&(fit=crop&w=1950&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 150px 0;
           }

           .hero h1{
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 30px;
           }

           /* Categories Section */
           .categories{
            background-color: white;
           }

           .category-container{
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 30px
           }

           .category-card{
            position: relative;
            height: 400px;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease; 
           }

           .category-card:hover{
            transform: translateY(-10px);
           }

           .category-card img{
            width: 100%;
            height: 100%;
            object-fit: cover;
           }

           .category-content{
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: linear-gradient(transparent, rgba(0, 0, 0, 0.8));
            color: white;
            padding: 30px;
           }

           .category-content h3{
            font-size: 2rem;
            margin-bottom: 10px;
           }

           /*Product Section */
           products{
            background-color: var(--light);
           }

           .product-filters{
            display: flex;
            justify-content: center;
            margin-bottom: 40px;
           }

           .filter-btn{
            padding: 10px 20px;
            margin: 0 10px;
            background: none;
            border: none;
            font-size: 1rem;
            font-weight: 500;
            cursor: pointer;
            transition: color 0.3s ease;
           }

           .filter-btn.active{
            color: var(--primary);
            border-bottom: 2px solid var(--primary);
           }

           .product-grid{
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 30px;
           }

           .product-card{
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
            transition: transform 0.3s ease;
           }

           .product-card:hover{
            transform: translateY(-5px);
           }

           .product-img{
            height: 250px;
            overflow: hidden;
           }

           .product-img img{
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
           }

           .product-card:hover .product-img img{
            transform: scale(1.1);
           }

           .product-info{
            padding: 20px;
           }

           .product-category{
            color: var(--primary);
            font-size: 0.9rem;
            text-transform: uppercase;
            margin-bottom: 5px;
           }

           .product-name{
            font-size: 1.2rem;
            margin-bottom: 10px;
           }

           .product-price{
            font-size: 1.3rem;
            font-weight: 700;
            color: var(--dark);
            margin-bottom: 15px;
           }

           .product-rating{
            color: var(--secondary);
            margin-bottom: 15px;
           }

           /* Testimonials Section */
           .testimonials{
            background-color: white;
           }

           .testimonial-container{
            max-width: 800px;
            margin: 0 auto;
           }

           .testimonial{
            text-align: center;
            padding: 30px;
           }

           .testimonial-text{
            font-size: 1.2rem;
            font-style: italic;
            margin-bottom: 20px;
           }

           .testimonial-author{
            font-weight: 600;
           }

           /*Newsletter Section */
           .newsletter{
            background: linear-gradient(rgba(0, 0, 0, 0.8), rgba(0, 0, 0, 0.8)); url('https://images.unsplash.com/photo-1590736969955-71ac4468e522?ixlib=rb-4.0.3&auto=format&fit=crop&w=1950&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
           }

           .newsletter h2{
            margin-bottom: 20px;
           }

           .newsletter p{
            max-width: 600px;
            margin: 0 auto 30px
           }

           .newsletter-form{
            display: flex;
            max-width: 500px;
            margin: 0 auto;
           }

           .newsletter-form input{
            flex: 1;
            padding: 15px;
            border: none;
            border-radius: 4px 0 0 4px;
        }

        .newsletter-form button{
            padding: 15px 30px;
            border: none;
            background-color: var(--primary);
            color: white;
            border-radius: 0 4px 4px 0;
            cursor: pointer;
        }

        /* Footer */
        footer{
            background-color: var(--dark);
            color: white;
            padding: 60px 0 20px;
           }

            .footer-container{
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 30px;
           }

           .footer-col h3{
            font-size: 1.2rem;
            margin-bottom: 20px;
            position: relative;
            padding-bottom: 10px;
           }

              .footer-col h3::after{
                content: '';
                position: absolute;
                bottom: 0;
                left: 0;
                width: 40px;
                height: 2px;
                background-color: var(--secondary);
              }

              .footer-col ul{
                list-style: none;
              }

              .footer-col ul li{
                margin-bottom: 10px;
              }

              .footer-col ul li a{
                color: #bbb;
                text-decoration: none;
                transition: color 0.3s ease;
              }

                .footer-col ul li a:hover{
                    color: var(--secondary);
                }

                .social-links{
                    display: flex;
                    margin-top: 20px;
                }

                .social-links a{
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    width: 40px;
                    height: 40px;
                    background-color: rgba(255, 255, 255, 0.1);
                    border-radius: 50%;
                    margin-right: 10px;
                    transition: all 0.3s ease;
                }

                .social-links a:hover{
                    background-color: var(--secondary);
                    transform: translateY(-3px);
                }

                .copyright{
                    text-align: center;
                    margin-top: 40px;
                    padding-top: 20px;
                    border-top: 1px solid rgba(255, 255, 255, 0.1);
                    font-size: 0.9rem;
                    color: #bbb;
                }

                /* Responsive Styles */
                @media (max-width: 992px){
                    .footer-container{
                        grid-template-columns: repeat(2, 1fr);
                    }
                }

                @media (max-width: 768px){
                    .header-container{
                        padding: 15px 0;
                    }

                    nav{
                        display: none;
                    }>

                    .mobile-menu{
                        display: block;
                 }

                 .hero h1{
                    font-size: 2.5rem;
                 }

                    .category-container{
                        grid-template-columns: 1fr;
                    }

                    .product-grid{
                        grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
                    }

                    .newsletter-form{
                        flex-direction: column;
                    }

                    .newsletter-form input{
                        border-radius: 4px;
                        margin-bottom: 10px;
                    }

                    .newsletter-form button{
                        border-radius: 4px;
                        padding: 15px;
                    }

                    @media (max-width: 576px){
                        .footer-container{
                            grid-template-columns: 1fr;
                        }

                        .section-title{
                            font-size: 2rem;
                    }
                }

    </style

</head>
<body>
    <!--Header-->
    <header>
        <div class="container header-container">
            <a href="#" class="logo">Perfume <span>Paradise</span></a>

            <nav>
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Shop</a></li>
                    <li><a href="#">For Him</a></li>
                    <li><a href="#">For Her</a></li>
                    <li><a href="#">Collections</a></li>
                    <li><a href="#">About</a></li>
                </ul>
            </nav>

            <div class="header-icons">
                <a href="#"><i class="fas fa-search"></i></a>
                <a href="#"><i class="fas fa-user"></i></a>
                <a href="#" class="cart-icon">
                    <i class="fas fa-shopping-cart"></i>
                    <span class="cart-count">3</span>
                </a>
            </div>

            </div class="mobile-menu">
                <i class="fas fa-bars"></i>
            </div>
        </div>
    <header>
        <!--Hero Section-->
        <section class="hero">
            <div class="container">
                <h1>Discover Your Signature Scent<h1>
                    <p>Explore our exclusive colection of luxury fragrances for both men women. Find the perfect perfume that matches your personality and style.</p>
                    <a href="#" class="btn">Shop Now</a>
                    </div>
            </section>

            <!--Categories Section-->
            <section class="categories
            <div class="container">
                <h2 class="section-title">Shop by Category</h2>
                <div class="category-container">
                    <div class="category-card">
                        <img src="https://images.unsplash.com/photo-1590736969955-71ac4468e522?ixlib=rb-4.0.3&auto=format&fit=crop&w=1950&q=80" alt="Men's Perfumes">
                            <div class="category-content">
                            <h3>For Him</h3>
                            <p>Masculine scents that define confidence</p>
                            <a href="#" class="btn btn-outline">Explore</a>
                        </div>
                    </div>
                    <div class="category-card">
                        <img src="https://images.unsplash.com/photo-1547887537-6158d64c35b3?ixlib=rb-4.0.3&auto=format&fit=crop&w=1950&q=80" alt="Women's Perfumes">
                        <div class="category-content">
                            <h3>For Her</h3>
                            <p>Feminine fragrances that embody elegance</p>
                            <a href="#" class="btn btn-outline">Explore</a>
                        </div>
                    </div>
                    </div>
                    </div>
                    </section>

                    <!--Product Section-->
                    <section class="products">
                        <div class="container">
                            <h2 class="section-title">Featured Products</h2>

                            <div class="product-filters">
                                <button class="filter-btn active">All</button>
                                <button class="filter-btn">For Him</button>
                                <button class="filter-btn">For Her</button>
                                <button class="filter-btn">Best Sellers</button>
                                <button class="filter-btn">New Arrivals</button>
                            </div>

                            <div class="product-grid">
                                <!--Product 1-->
                                <div class="product-card">
                                    <div class="product-img">
                                        <img src="https://images.unsplash.com/photo-1585386959984-a4155224a1ad?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Noir Essence">
                                    </div>
                                    <div class="product-info">
                                        <div class="product category">For Him</div>
                                        <h3 class="product-name">Noir Essence</h3>
                                        <div class="product-rating">
                                            <i class="fas fa-star"></i>
                                            <i class="fas fa-star"></i>
                                            <i class="fas fa-star"></i>
                                            <i class="fas fa-star"></i>
                                            <i class="fas fa-star-half-alt"></i>
                                            </div>
                                            <div class="product-price">R700.00</div>
                                            <a href="#" class="btn">Add to Cart</a>
                                            </div>
                                            </div>

                                            <!--Product 2-->
                                            <div class="product-card">
                                                <div class="product-img">
                                                    <img src="https://images.unsplash.com/photo-1585386959984-a4155224a1ad?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Noir Essence">
                                                </div>
                                                <div class="product-info">
                                                    <div class="product category">For Her</div>
                                                    <h3 class="product-name">Floral Bliss</h3>
                                                    <div class="product-rating">
                                                        <i class="fas fa-star"></i>
                                                        <i class="fas fa-star"></i>
                                                        <i class="fas fa-star"></i>
                                                        <i class="fas fa-star"></i>
                                                        <i class="fas fa-star-half-alt"></i>
                                                        </div>
                                                        <div class="product-price">R650.00</div>
                                                        <a href="#" class="btn">Add to Cart</a>
                                                        </div>
                                                        </div>
                                                        <!--Product-->
                                                        <div class="product-card">
                                                            <div class="product-img">
                                                                <img src="https://images.unsplash.com/photo-1592945403244-b3fbafd7f539?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Ocean Breeze">
                                                            </div>
                                                            <div class="product-info">
                                                                <div class="product category">For Him</div>
                                                                <h3 class="product-name">Ocean Breeze</h3>
                                                                <div class="product-rating">
                                                                    <i class="fas fa-star"></i>
                                                                    <i class="fas fa-star"></i>
                                                                    <i class="fas fa-star"></i>
                                                                    <i class="fas fa-star"></i>
                                                                    <i class="fas fa-star-half-alt"></i>
                                                                    </div>
                                                                    <div class="product-price">R720.00</div>
                                                                    <a href="#" class="btn">Add to Cart</a>
                                                                    </div>
                                                                    </div>
                                                                    <!--Product 4-->
                                                                    <div class="product-card">

                                        <h4 class="product-category">For Him</h4>
                                        <h3 class="product-name">Aventus by Creed</h3>
                                        <p class="product-price">$325.00</p>
                                        <div class="product-rating">
                                            <i class="fas fa-star"></i>
                                            <i class="fas fa-star"></i>
                                            <i class="fas fa-star"></i>
                                            <i class="fas fa-star"></i>
                                            <i class="fas fa-star-half-alt"></i>
                                        </div>
                                        <a href="#" class="btn btn-outline">Add to Cart</a>
                                    </div>
                                </div>

                                <div class="product-card">
                                    <div class="product-img">
                                        <img src="https://images.unsplash.com/photo-1615634260167-85a797113d13?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="<Mystic Rose">
                                    </div>
                                    <div class="product-info">
                                        <div class="product-category">For Her</div>
                                        <h3 class="product-name">Mystic Rose</h3>
                                        <div class="product-rating">
                                            <i class="fas fa-star"></i>
                                            <i class="fas fa-star"></i>
                                            <i class="fas fa-star"></i>
                                            <i class="fas fa-star"></i>
                                            <i class="fas fa-star-half-alt"></i>
                                        </div>
                                        <p class="product-price">R710.00</p>
                                        <a href="#" class="btn">Add to Cart</a>
                                        </div>
                                        </div>
                                    </div>
                                </div>
                    </section>
                    <!--Testimonials Section-->
                    <section class="testimonials">
                        <div class="container">
                            <h2 class="section-title">What Our Customers Say</h2>
                            <div class="testimonial-container">
                                <div class="testimonial">
                                    <p class="testimonial-text">"I absolutely love the selection of perfumes at Perfume Paradise. The quality is top-notch, and the customer service is exceptional!"</p>
                                    <p class="testimonial-text">"I've been searching for the perfect masculine scent for years, and Noir Essence is exactly what I was looking for. It's sophisticated and long-lasting.</p>
                                    <p class="testimonials-author">- B. Plaatjie</p>
                                </div>
                                </div>
                                </div>
                                </section>

                                <!--Newsletter Section-->
                                <section class="newsletter">
                                    <div class="container">
                                        <h2>Subscribe to Our Newsletter</h2>
                                        <p>Be the first to know about new arrivals, exclusive offers, and fragrance tips.</p>
                                        <form class="newsletter-form">
                                            <input type="email" placeholder="Enter your email address" required>
                                            <button type="submit">Subscribe</button>
                                        </form>
                                    </div>
                                </section>
                                
                                <!--Footer-->
                                <footer>
                                    <div class="container footer-container">
                                        <div class="footer-col">
                                            <h3>Perfume Paradise</h3>
                                            <p>Your destination for luxury fragrance that inspire confidence and elegance</p>
                                            <div class="social-links">
                                                <a href="#"><i class="fab fa-facebook-f"></i></a>
                                                <a href="#"><i class="fab fa-twitter"></i></a>
                                                <a href="#"><i class="fab fa-instagram"></i></a>
                                                <a href="#"><i class="fab fa-tiktok"></i></a>
                                                </div>
                                            </div>

                                            <div class="footer-col">
                                                <h3>Shop</h3>
                                                <ul>
                                                    <li><a href="#">For Him</a></li>
                                                    <li><a href="#">For Her</a></li>
                                                    <li><a href="#">Delivery Nationwide</a></li>
                                                    <li><a href="#">Gift sets</a></li>
                                                    <li><a href="#">Travel Sises</a></li>
                                                    <li><a href="#">Limited Editions</a></li>
                                                </ul>
                                            </div>

                                                    <div class="footer-col">
                                                        <h3>Customer Service</h3>
                                                        <ul>
                                                            <li><a href="#">Contact Us</a></li>
                                                            <li><a href="#">Shipping & Returns</a></li>
                                                            <li><a href="#">Order Tracking</a></li>
                                                            <li><a href="#">Privacy Policy</a></li>
                                                            <li><a href="#">Terms of Service</a></li>
                                                            <li><a href="#">FAQs</a></li>
                                                        </ul>
                                                    </div>

                                    </div class="footer-col">
                                    <h3>Contact</h3>
                                    <ul>
                                        <li><i class="fas fa map-marker-alt"></i>323 Nana Sita Street, Pretoria</li>
                                        <li><i class="fas fa-phone"></i>+27 76 884 66177</li>
                                        <li><i class="fas fa-envelope"></i>info@perfumeparadise.co.za</li>
                                    </ul>
                                    </div>
                                    </div>

                                    <div class="copyright">
                                        <p>&copy;2025 Perfume Paradise. All rights reserved.</p>
                                    </div>
                                </div>
                                </footer>

                                <script>
                                    // Simple JavaScript for interactive elements document.addEventListener("DOMContentLoaded", function()) {
                                        // Filter buttons
                                        const filterBtns = <document class="querySelectorAll('filter-btn');

                                        filterBtns.forEach(btn=>{
                                            btn.addEventListener('click', function(){
                                                // Remove active class from all buttons
                                                filterBtns.forEach(b=>b.classList.remove('active'));
                                                //Add active class to clicked button
                                                this.classList.add('active');
                                            })
                                        })

                                        // Mobiile menu toggle
                                        const mobileMenu=document.querySelector('.mobile-menu.');
                                        const nav = document.querySelector('nav');

                                        mobileMenu.addEventListener('click', function(){
                                            nav.style.display = nav.style.display === 'block'? 'none': 'block',
                                        })

                                        // Update cart count (example functionality)
                                        const cartCount = document.querySelector('.cart-count.');
                                        const addToCartBtns = document.querySelectorAll('.product-card .btn.'');

                                        addToCartBtns.forEach(btn =>{
                                            btn.addEventListener('click', function(e){
                                                e.preventDefault();
                                                let count = parseInt(cartCount.textContent);
                                                cartCount.textContent = count + 1;

                                                // Add animation effect
                                                cartCount.parentElement.classList.add('pulse');
                                                setTimeout(() =>{
                                                    cartCount.parentElement.classList.remove('pulse');
                                                }, 300);
                                                })
                                            })
                                        }
                                        </script>
                                    </body>
                                    </html>
