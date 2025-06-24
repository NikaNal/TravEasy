<!DOCTYPE HTML>
<html>
<head>
    <title>Your Brand | Modern Business Solutions</title>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no" />
    <!-- Enhanced Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&family=Playfair+Display:wght@400;700&display=swap" rel="stylesheet">
    <!-- Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Animate.css -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css">
    <!-- Custom CSS -->
    <style>
        :root {
            --primary-color: #3a86ff;
            --secondary-color: #8338ec;
            --accent-color: #ff006e;
            --dark-color: #1a1a2e;
            --light-color: #f8f9fa;
            --gradient: linear-gradient(135deg, var(--primary-color) 0%, var(--secondary-color) 100%);
        }
        
        body {
            font-family: 'Montserrat', sans-serif;
            background-color: #ffffff;
            color: #333;
            line-height: 1.6;
            overflow-x: hidden;
        }
        
        h1, h2, h3, h4, h5, h6 {
            font-family: 'Playfair Display', serif;
            font-weight: 700;
            color: var(--dark-color);
        }
        
        /* Header Styles */
        #header {
            background: rgba(255, 255, 255, 0.95);
            box-shadow: 0 2px 15px rgba(0, 0, 0, 0.1);
            position: fixed;
            width: 100%;
            z-index: 1000;
            transition: all 0.3s ease;
        }
        
        #header.scrolled {
            background: rgba(255, 255, 255, 0.98);
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.15);
        }
        
        /* Hero Section */
        #hero {
            background: var(--gradient);
            color: white;
            padding: 180px 0 120px;
            position: relative;
            overflow: hidden;
        }
        
        #hero video {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            z-index: 0;
            opacity: 0.15;
        }
        
        #hero .content {
            position: relative;
            z-index: 1;
        }
        
        #hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.2);
        }
        
        /* Feature Cards */
        .features {
            padding: 100px 0;
        }
        
        .feature-card {
            background: white;
            border-radius: 10px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.05);
            padding: 30px;
            margin-bottom: 30px;
            transition: all 0.3s ease;
            height: 100%;
        }
        
        .feature-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.1);
        }
        
        .feature-icon {
            font-size: 2.5rem;
            margin-bottom: 20px;
            color: var(--primary-color);
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        /* Testimonials */
        #testimonials {
            background-color: var(--light-color);
            padding: 100px 0;
        }
        
        .testimonial-card {
            background: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            margin: 15px;
            position: relative;
        }
        
        .testimonial-card:before {
            content: '"';
            font-family: 'Playfair Display', serif;
            font-size: 5rem;
            color: rgba(0, 0, 0, 0.05);
            position: absolute;
            top: 10px;
            left: 20px;
            line-height: 1;
        }
        
        .client-img {
            width: 70px;
            height: 70px;
            border-radius: 50%;
            object-fit: cover;
            border: 3px solid var(--primary-color);
        }
        
        /* CTA Section */
        #cta {
            background: var(--gradient);
            color: white;
            padding: 80px 0;
            text-align: center;
        }
        
        .btn-brand {
            background: white;
            color: var(--primary-color);
            border: none;
            padding: 12px 30px;
            font-weight: 600;
            border-radius: 50px;
            transition: all 0.3s ease;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .btn-brand:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.2);
            color: var(--primary-color);
        }
        
        /* Footer */
        #footer {
            background: var(--dark-color);
            color: white;
            padding: 60px 0 30px;
        }
        
        .social-icons a {
            color: white;
            font-size: 1.2rem;
            margin-right: 15px;
            transition: all 0.3s ease;
        }
        
        .social-icons a:hover {
            color: var(--primary-color);
            transform: translateY(-3px);
        }
        
        /* Animations */
        .animate-on-scroll {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.6s ease;
        }
        
        .animate-on-scroll.animated {
            opacity: 1;
            transform: translateY(0);
        }
        
        /* Responsive Adjustments */
        @media (max-width: 768px) {
            #hero h1 {
                font-size: 2.5rem;
            }
            
            .feature-card {
                margin-bottom: 20px;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header id="header">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-md-6">
                    <h1 class="logo">Your<span style="color: var(--primary-color);">Brand</span></h1>
                </div>
                <div class="col-md-6 text-right">
                    <nav>
                        <ul class="list-inline">
                            <li class="list-inline-item"><a href="#hero">Home</a></li>
                            <li class="list-inline-item"><a href="#features">Features</a></li>
                            <li class="list-inline-item"><a href="#about">About</a></li>
                            <li class="list-inline-item"><a href="#testimonials">Testimonials</a></li>
                            <li class="list-inline-item"><a href="#contact">Contact</a></li>
                        </ul>
                    </nav>
                </div>
            </div>
        </div>
    </header>

    <!-- Hero Section with Video Background -->
    <section id="hero" class="text-center">
        <video autoplay muted loop>
            <source src="https://assets.mixkit.co/videos/preview/mixkit-woman-holding-a-light-bulb-while-seated-12303-large.mp4" type="video/mp4">
        </video>
        <div class="container">
            <div class="content animate__animated animate__fadeIn">
                <h1 class="mb-4">Transform Your Business With Our Solutions</h1>
                <p class="lead mb-5">We help innovative companies scale their business with our cutting-edge technology and strategic expertise.</p>
                <a href="#contact" class="btn btn-brand btn-lg">Get Started Today</a>
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section id="features" class="features">
        <div class="container">
            <div class="section-title text-center mb-5">
                <h2>Our Core Services</h2>
                <p class="lead">Everything you need to grow your business</p>
            </div>
            <div class="row">
                <div class="col-md-4 animate-on-scroll">
                    <div class="feature-card">
                        <div class="feature-icon">
                            <i class="fas fa-chart-line"></i>
                        </div>
                        <h3>Business Growth</h3>
                        <p>We provide strategic planning and execution to help your business expand into new markets and increase revenue.</p>
                        <a href="#" class="btn btn-outline-primary">Learn More</a>
                    </div>
                </div>
                <div class="col-md-4 animate-on-scroll">
                    <div class="feature-card">
                        <div class="feature-icon">
                            <i class="fas fa-laptop-code"></i>
                        </div>
                        <h3>Technology Solutions</h3>
                        <p>Custom software development and IT solutions tailored to your specific business needs and challenges.</p>
                        <a href="#" class="btn btn-outline-primary">Learn More</a>
                    </div>
                </div>
                <div class="col-md-4 animate-on-scroll">
                    <div class="feature-card">
                        <div class="feature-icon">
                            <i class="fas fa-bullseye"></i>
                        </div>
                        <h3>Marketing Strategy</h3>
                        <p>Data-driven marketing campaigns that deliver measurable results and increase your brand awareness.</p>
                        <a href="#" class="btn btn-outline-primary">Learn More</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section with Stats -->
    <section id="about" class="py-5 bg-light">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-lg-6 mb-5 mb-lg-0 animate-on-scroll">
                    <h2 class="mb-4">Why Choose Our Company</h2>
                    <p class="lead">We combine industry expertise with innovative technology to deliver exceptional results.</p>
                    <p>Founded in 2010, we've helped over 500 clients achieve their business goals through our comprehensive suite of services. Our team of experts brings decades of combined experience across multiple industries.</p>
                    <div class="row mt-4">
                        <div class="col-6">
                            <div class="counter">
                                <h3 class="count" data-count="500">0</h3>
                                <p>Happy Clients</p>
                            </div>
                        </div>
                        <div class="col-6">
                            <div class="counter">
                                <h3 class="count" data-count="150">0</h3>
                                <p>Projects Completed</p>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-lg-6 animate-on-scroll">
                    <img src="https://images.unsplash.com/photo-1552664730-d307ca884978?ixlib=rb-1.2.1&auto=format&fit=crop&w=1000&q=80" alt="Team meeting" class="img-fluid rounded shadow">
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section id="testimonials">
        <div class="container">
            <div class="section-title text-center mb-5">
                <h2>What Our Clients Say</h2>
                <p class="lead">Don't just take our word for it</p>
            </div>
            <div class="row">
                <div class="col-md-4 animate-on-scroll">
                    <div class="testimonial-card">
                        <p>"Working with YourBrand has transformed our business. Their strategic insights helped us increase revenue by 150% in just 6 months."</p>
                        <div class="client-info mt-4 d-flex align-items-center">
                            <img src="https://randomuser.me/api/portraits/women/44.jpg" alt="Client" class="client-img mr-3">
                            <div>
                                <h5 class="mb-0">Sarah Johnson</h5>
                                <small>CEO, TechSolutions Inc.</small>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 animate-on-scroll">
                    <div class="testimonial-card">
                        <p>"The technology solutions provided were exactly what we needed to streamline our operations. Highly recommend their services!"</p>
                        <div class="client-info mt-4 d-flex align-items-center">
                            <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="Client" class="client-img mr-3">
                            <div>
                                <h5 class="mb-0">Michael Chen</h5>
                                <small>CTO, Global Enterprises</small>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 animate-on-scroll">
                    <div class="testimonial-card">
                        <p>"Exceptional service from start to finish. Their team went above and beyond to ensure our project was a success."</p>
                        <div class="client-info mt-4 d-flex align-items-center">
                            <img src="https://randomuser.me/api/portraits/women/68.jpg" alt="Client" class="client-img mr-3">
                            <div>
                                <h5 class="mb-0">Emily Rodriguez</h5>
                                <small>Marketing Director, BrightStar</small>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section id="cta" class="animate-on-scroll">
        <div class="container">
            <h2 class="mb-4">Ready to Transform Your Business?</h2>
            <p class="lead mb-5">Get in touch with our team today to discuss how we can help you achieve your goals.</p>
            <a href="#contact" class="btn btn-brand btn-lg">Schedule a Consultation</a>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-5">
        <div class="container">
            <div class="section-title text-center mb-5">
                <h2>Get In Touch</h2>
                <p class="lead">We'd love to hear from you</p>
            </div>
            <div class="row">
                <div class="col-lg-6 mb-5 mb-lg-0 animate-on-scroll">
                    <form id="contactForm" action="https://formspree.io/f/yourformid" method="POST">
                        <div class="form-group">
                            <input type="text" class="form-control" placeholder="Your Name" required>
                        </div>
                        <div class="form-group">
                            <input type="email" class="form-control" placeholder="Your Email" required>
                        </div>
                        <div class="form-group">
                            <input type="text" class="form-control" placeholder="Subject">
                        </div>
                        <div class="form-group">
                            <textarea class="form-control" rows="5" placeholder="Your Message" required></textarea>
                        </div>
                        <button type="submit" class="btn btn-primary">Send Message</button>
                    </form>
                </div>
                <div class="col-lg-6 animate-on-scroll">
                    <div class="contact-info">
                        <div class="contact-item d-flex mb-4">
                            <div class="icon mr-4">
                                <i class="fas fa-map-marker-alt fa-2x text-primary"></i>
                            </div>
                            <div>
                                <h5>Location</h5>
                                <p>123 Business Ave, Suite 500<br>San Francisco, CA 94107</p>
                            </div>
                        </div>
                        <div class="contact-item d-flex mb-4">
                            <div class="icon mr-4">
                                <i class="fas fa-phone-alt fa-2x text-primary"></i>
                            </div>
                            <div>
                                <h5>Phone</h5>
                                <p>(123) 456-7890</p>
                            </div>
                        </div>
                        <div class="contact-item d-flex mb-4">
                            <div class="icon mr-4">
                                <i class="fas fa-envelope fa-2x text-primary"></i>
                            </div>
                            <div>
                                <h5>Email</h5>
                                <p>info@yourbrand.com</p>
                            </div>
                        </div>
                    </div>
                    <div class="social-icons mt-5">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-linkedin-in"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer id="footer">
        <div class="container">
            <div class="row">
                <div class="col-md-4 mb-4 mb-md-0">
                    <h4>About YourBrand</h4>
                    <p>We are a leading business solutions provider helping companies of all sizes achieve their growth objectives through innovative strategies and technology.</p>
                </div>
                <div class="col-md-2 mb-4 mb-md-0">
                    <h4>Quick Links</h4>
                    <ul class="list-unstyled">
                        <li><a href="#hero">Home</a></li>
                        <li><a href="#features">Services</a></li>
                        <li><a href="#about">About</a></li>
                        <li><a href="#contact">Contact</a></li>
                    </ul>
                </div>
                <div class="col-md-3 mb-4 mb-md-0">
                    <h4>Services</h4>
                    <ul class="list-unstyled">
                        <li><a href="#">Business Consulting</a></li>
                        <li><a href="#">Digital Marketing</a></li>
                        <li><a href="#">Web Development</a></li>
                        <li><a href="#">Data Analytics</a></li>
                    </ul>
                </div>
                <div class="col-md-3">
                    <h4>Subscribe</h4>
                    <p>Stay updated with our latest news and offers.</p>
                    <form class="subscribe-form">
                        <div class="input-group">
                            <input type="email" class="form-control" placeholder="Your Email">
                            <div class="input-group-append">
                                <button class="btn btn-primary" type="submit"><i class="fas fa-paper-plane"></i></button>
                            </div>
                        </div>
                    </form>
                </div>
            </div>
            <hr class="mt-5 mb-4" style="border-color: rgba(255,255,255,0.1);">
            <div class="row">
                <div class="col-md-6 text-center text-md-left">
                    <p class="mb-0">&copy; 2023 YourBrand. All rights reserved.</p>
                </div>
                <div class="col-md-6 text-center text-md-right">
                    <ul class="list-inline mb-0">
                        <li class="list-inline-item"><a href="#">Privacy Policy</a></li>
                        <li class="list-inline-item"><a href="#">Terms of Service</a></li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>

    <!-- JavaScript Libraries -->
    <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/waypoints/4.0.1/jquery.waypoints.min.js"></script>
    <script>
        // Header scroll effect
        $(window).scroll(function() {
            if ($(this).scrollTop() > 100) {
                $('#header').addClass('scrolled');
            } else {
                $('#header').removeClass('scrolled');
            }
        });
        
        // Animation on scroll
        $(document).ready(function() {
            $('.animate-on-scroll').each(function() {
                var element = $(this);
                var animationTrigger = element.offset().top - $(window).height() + 100;
                
                $(window).scroll(function() {
                    var scrollPosition = $(window).scrollTop();
                    if (scrollPosition > animationTrigger) {
                        element.addClass('animated');
                    }
                });
                
                // Trigger once on page load if already in view
                if ($(window).scrollTop() > animationTrigger) {
                    element.addClass('animated');
                }
            });
            
            // Counter animation
            $('.count').each(function() {
                $(this).prop('Counter', 0).animate({
                    Counter: $(this).data('count')
                }, {
                    duration: 2000,
                    easing: 'swing',
                    step: function(now) {
                        $(this).text(Math.ceil(now));
                    }
                });
            });
            
            // Smooth scrolling for anchor links
            $('a[href*="#"]').on('click', function(e) {
                e.preventDefault();
                
                $('html, body').animate(
                    {
                        scrollTop: $($(this).attr('href')).offset().top - 80,
                    },
                    500,
                    'linear'
                );
            });
        });
    </script>
</body>
</html>
