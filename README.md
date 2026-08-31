```html
<!DOCTYPE html>
<html lang="en">

<head>

    <meta charset="UTF-8">

    <meta name="viewport"
          content="width=device-width, initial-scale=1.0">

    <title>Little Blossom Works</title>


    <style>

        /* =========================================
           BASIC SETTINGS
        ========================================== */

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {

            font-family: Georgia, "Times New Roman", serif;

            /* BABY PINK BACKGROUND */

            background: #FFDDE8;

            /* DARK PINK FONT */

            color: #8B1746;

            line-height: 1.6;

        }


        /* =========================================
           NAVIGATION BAR
        ========================================== */

        header {

            position: sticky;

            top: 0;

            z-index: 1000;

            background: #FFEAF1;

            border-bottom:
                2px solid #F2A9BF;

        }


        nav {

            max-width: 1200px;

            margin: auto;

            padding: 20px 30px;

            display: flex;

            justify-content: space-between;

            align-items: center;

        }


        .logo {

            font-size: 26px;

            font-weight: bold;

            color: #8B1746;

        }


        .nav-links {

            display: flex;

            gap: 30px;

            list-style: none;

        }


        .nav-links a {

            text-decoration: none;

            color: #8B1746;

            font-weight: bold;

        }


        .nav-links a:hover {

            color: #C2185B;

        }



        /* =========================================
           HOME SECTION
        ========================================== */

        .hero {

            min-height: 90vh;

            max-width: 1200px;

            margin: auto;

            padding: 80px 30px;

            display: flex;

            align-items: center;

            justify-content: space-between;

            gap: 50px;

        }


        .hero-text {

            max-width: 650px;

        }


        .hero-small {

            letter-spacing: 4px;

            font-size: 13px;

            font-weight: bold;

            margin-bottom: 20px;

        }


        .hero h1 {

            font-size: 65px;

            line-height: 1.1;

            margin-bottom: 25px;

        }


        .hero h1 span {

            color: #C2185B;

        }


        .hero p {

            font-size: 19px;

            max-width: 600px;

        }


        .button {

            display: inline-block;

            margin-top: 30px;

            padding: 14px 30px;

            background: #C2185B;

            color: white;

            text-decoration: none;

            border-radius: 30px;

            font-weight: bold;

            border: none;

            cursor: pointer;

        }


        .button:hover {

            background: #8B1746;

        }


        /* Decorative circle */

        .hero-art {

            width: 380px;

            height: 380px;

            border-radius: 50%;

            background: #F4B4C8;

            display: flex;

            justify-content: center;

            align-items: center;

            flex-direction: column;

            font-size: 90px;

            box-shadow:
                0 15px 35px
                rgba(139, 23, 70, 0.15);

        }


        .hero-art p {

            font-size: 18px;

            text-align: center;

        }



        /* =========================================
           BRAND HIGHLIGHTS
        ========================================== */

        .highlights {

            background: #FFEAF1;

            padding: 50px 8%;

            display: grid;

            grid-template-columns:
                repeat(3, 1fr);

            gap: 25px;

            text-align: center;

        }


        .highlight {

            padding: 25px;

        }


        .highlight-icon {

            font-size: 40px;

            margin-bottom: 10px;

        }


        .highlight h3 {

            margin-bottom: 8px;

        }



        /* =========================================
           SHOP SECTION
        ========================================== */

        .shop {

            max-width: 1200px;

            margin: auto;

            padding: 100px 30px;

            text-align: center;

        }


        .section-label {

            font-size: 13px;

            letter-spacing: 4px;

            font-weight: bold;

            margin-bottom: 15px;

        }


        .section-title {

            font-size: 45px;

            margin-bottom: 15px;

        }


        .section-text {

            max-width: 650px;

            margin: auto auto 50px;

        }



        /* =========================================
           EMPTY PRODUCT SPACE

           YOU CAN ADD YOUR PRODUCTS HERE.

           Each card has:
           - Picture
           - Product name
           - Description
           - Price
        ========================================== */

        .products {

            display: grid;

            grid-template-columns:
                repeat(3, 1fr);

            gap: 30px;

            text-align: left;

        }


        .product-card {

            background: #FFEAF1;

            border:
                2px dashed #D9799A;

            border-radius: 20px;

            overflow: hidden;

            min-height: 450px;

        }


        /* PRODUCT IMAGE SPACE */

        .product-image {

            height: 280px;

            background: #F8C9D8;

            display: flex;

            justify-content: center;

            align-items: center;

            text-align: center;

            padding: 20px;

            color: #A93A63;

            font-size: 15px;

        }


        /*
        WHEN YOU HAVE A PRODUCT IMAGE,
        YOU CAN PUT:

        <img src="your-image.jpg">

        INSIDE .product-image
        */


        .product-image img {

            width: 100%;

            height: 100%;

            object-fit: cover;

        }


        .product-info {

            padding: 25px;

        }


        .product-name {

            font-size: 22px;

            margin-bottom: 8px;

        }


        .product-description {

            font-size: 14px;

            margin-bottom: 15px;

        }


        .product-price {

            font-size: 20px;

            font-weight: bold;

            color: #C2185B;

        }



        /* =========================================
           ABOUT SECTION
        ========================================== */

        .about {

            background: #FFEAF1;

            padding: 100px 8%;

            display: flex;

            align-items: center;

            justify-content: center;

            gap: 80px;

        }


        .about-art {

            width: 400px;

            height: 400px;

            border-radius: 25px;

            background: #F4B4C8;

            display: flex;

            align-items: center;

            justify-content: center;

            font-size: 100px;

        }


        .about-text {

            max-width: 600px;

        }


        .about-text h2 {

            font-size: 45px;

            margin-bottom: 20px;

        }


        .about-text p {

            margin-bottom: 15px;

        }


        .founder {

            margin-top: 25px;

            font-size: 20px;

            font-weight: bold;

        }



        /* =========================================
           CUSTOM ORDERS
        ========================================== */

        .custom {

            padding: 100px 30px;

            text-align: center;

        }


        .custom h2 {

            font-size: 45px;

            margin-bottom: 20px;

        }


        .custom p {

            max-width: 650px;

            margin: auto;

        }



        /* =========================================
           CONTACT
        ========================================== */

        .contact {

            background: #FFEAF1;

            padding: 100px 30px;

            text-align: center;

        }


        .contact h2 {

            font-size: 45px;

            margin-bottom: 20px;

        }


        .contact-info {

            margin: 30px 0;

        }


        .contact-info p {

            margin: 10px;

            font-weight: bold;

        }



        /* =========================================
           FOOTER
        ========================================== */

        footer {

            background: #8B1746;

            color: white;

            text-align: center;

            padding: 40px 20px;

        }


        footer h3 {

            font-size: 24px;

            margin-bottom: 10px;

        }


        footer p {

            opacity: 0.9;

        }



        /* =========================================
           MOBILE RESPONSIVE DESIGN
        ========================================== */

        @media (max-width: 900px) {

            .hero {

                flex-direction: column;

                text-align: center;

            }


            .hero h1 {

                font-size: 50px;

            }


            .products {

                grid-template-columns:
                    repeat(2, 1fr);

            }


            .about {

                flex-direction: column;

                text-align: center;

            }


            .highlights {

                grid-template-columns:
                    repeat(2, 1fr);

            }

        }


        @media (max-width: 600px) {

            .nav-links {

                display: none;

            }


            .logo {

                font-size: 20px;

            }


            .hero {

                padding-top: 60px;

            }


            .hero h1 {

                font-size: 40px;

            }


            .hero-art {

                width: 280px;

                height: 280px;

                font-size: 70px;

            }


            .products {

                grid-template-columns: 1fr;

            }


            .highlights {

                grid-template-columns: 1fr;

            }


            .about-art {

                width: 100%;

                height: 280px;

            }


            .section-title,
            .about-text h2,
            .custom h2,
            .contact h2 {

                font-size: 34px;

            }

        }

    </style>

</head>



<body>


    <!-- =========================================
         NAVIGATION
    ========================================== -->

    <header>

        <nav>

            <div class="logo">

                🌸 Little Blossom Works

            </div>


            <ul class="nav-links">

                <li>
                    <a href="#home">
                        Home
                    </a>
                </li>

                <li>
                    <a href="#shop">
                        Shop
                    </a>
                </li>

                <li>
                    <a href="#about">
                        About
                    </a>
                </li>

                <li>
                    <a href="#contact">
                        Contact
                    </a>
                </li>

            </ul>

        </nav>

    </header>



    <!-- =========================================
         HOME
    ========================================== -->

    <section
        class="hero"
        id="home">


        <div class="hero-text">


            <p class="hero-small">

                HANDMADE • UNIQUE • MADE WITH LOVE

            </p>


            <h1>

                Welcome to

                <span>
                    Little Blossom Works
                </span>

            </h1>


            <p>

                A little corner where creativity
                blossoms into beautiful handmade
                crochet creations.

            </p>


            <a
                href="#shop"
                class="button">

                Explore Collection

            </a>


        </div>



        <div class="hero-art">

            🧶

            <p>

                Handmade<br>
                with love ♡

            </p>

        </div>


    </section>



    <!-- =========================================
         HIGHLIGHTS
    ========================================== -->

    <section class="highlights">


        <div class="highlight">

            <div class="highlight-icon">
                🧶
            </div>

            <h3>
                Handmade
            </h3>

            <p>
                Every creation is made by hand
                with care and attention.
            </p>

        </div>


        <div class="highlight">

            <div class="highlight-icon">
                💕
            </div>

            <h3>
                Made With Love
            </h3>

            <p>
                Crafted with creativity,
                patience and lots of love.
            </p>

        </div>


        <div class="highlight">

            <div class="highlight-icon">
                ✨
            </div>

            <h3>
                Unique Creations
            </h3>

            <p>
                Little handmade pieces
                made to feel special.
            </p>

        </div>


    </section>



    <!-- =========================================
         SHOP

         EMPTY PRODUCT TEMPLATE

         DO NOT ADD PRODUCTS HERE YET.

         ADD YOUR OWN PRODUCT DETAILS
         WHEN YOU ARE READY.
    ========================================== -->

    <section
        class="shop"
        id="shop">


        <p class="section-label">

            OUR COLLECTION

        </p>


        <h2 class="section-title">

            Crochet Creations

        </h2>


        <p class="section-text">

            Explore our handmade collection.
            Our products will be displayed here.

        </p>



        <div class="products">



            <!-- =================================
                 PRODUCT SPACE 1
            ================================== -->

            <div class="product-card">


                <div class="product-image">

                    <!--
                    ADD PRODUCT IMAGE HERE

                    Example:

                    <img src="images/product1.jpg">

                    -->

                    <span>
                        YOUR PRODUCT IMAGE
                    </span>

                </div>


                <div class="product-info">

                    <!-- ADD PRODUCT NAME -->

                    <h3 class="product-name">

                        Product Name

                    </h3>


                    <!-- ADD DESCRIPTION -->

                    <p class="product-description">

                        Product description goes here.

                    </p>


                    <!-- ADD PRICE -->

                    <p class="product-price">

                        ₹___

                    </p>

                </div>


            </div>



            <!-- =================================
                 PRODUCT SPACE 2
            ================================== -->

            <div class="product-card">


                <div class="product-image">

                    <span>
                        YOUR PRODUCT IMAGE
                    </span>

                </div>


                <div class="product-info">

                    <h3 class="product-name">

                        Product Name

                    </h3>


                    <p class="product-description">

                        Product description goes here.

                    </p>


                    <p class="product-price">

                        ₹___

                    </p>

                </div>


            </div>



            <!-- =================================
                 PRODUCT SPACE 3
            ================================== -->

            <div class="product-card">


                <div class="product-image">

                    <span>
                        YOUR PRODUCT IMAGE
                    </span>

                </div>


                <div class="product-info">

                    <h3 class="product-name">

                        Product Name

                    </h3>


                    <p class="product-description">

                        Product description goes here.

                    </p>


                    <p class="product-price">

                        ₹___

                    </p>

                </div>


            </div>



            <!-- =================================
                 PRODUCT SPACE 4
            ================================== -->

            <div class="product-card">


                <div class="product-image">

                    <span>
                        YOUR PRODUCT IMAGE
                    </span>

                </div>


                <div class="product-info">

                    <h3 class="product-name">

                        Product Name

                    </h3>


                    <p class="product-description">

                        Product description goes here.

                    </p>


                    <p class="product-price">

                        ₹___

                    </p>

                </div>


            </div>



            <!-- =================================
                 PRODUCT SPACE 5
            ================================== -->

            <div class="product-card">


                <div class="product-image">

                    <span>
                        YOUR PRODUCT IMAGE
                    </span>

                </div>


                <div class="product-info">

                    <h3 class="product-name">

                        Product Name

                    </h3>


                    <p class="product-description">

                        Product description goes here.

                    </p>


                    <p class="product-price">

                        ₹___

                    </p>

                </div>


            </div>



            <!-- =================================
                 PRODUCT SPACE 6
            ================================== -->

            <div class="product-card">


                <div class="product-image">

                    <span>
                        YOUR PRODUCT IMAGE
                    </span>

                </div>


                <div class="product-info">

                    <h3 class="product-name">

                        Product Name

                    </h3>


                    <p class="product-description">

                        Product description goes here.

                    </p>


                    <p class="product-price">

                        ₹___

                    </p>

                </div>


            </div>


        </div>

    </section>



    <!-- =========================================
         ABOUT
    ========================================== -->

    <section
        class="about"
        id="about">


        <div class="about-art">

            🌸🧶

        </div>


        <div class="about-text">


            <p class="section-label">

                ABOUT THE BRAND

            </p>


            <h2>

                Where creativity
                blossoms.

            </h2>


            <p>

                Little Blossom Works is a handmade
                crochet brand created with a love
                for creativity, colours and
                beautiful little details.

            </p>


            <p>

                Every creation is thoughtfully
                handcrafted, making each piece
                unique and special.

            </p>


            <p>

                Our goal is simple — to turn
                ordinary yarn into little pieces
                of happiness.

            </p>


            <div class="founder">

                Founder: Ishita Rai 🌸

            </div>


        </div>


    </section>



    <!-- =========================================
         CUSTOM ORDERS
    ========================================== -->

    <section class="custom">


        <p class="section-label">

            CUSTOM CREATIONS

        </p>


        <h2>

            Have an idea in mind?

        </h2>


        <p>

            Create something that is uniquely yours.
            Custom crochet requests can be added
            here in the future.

        </p>


        <a
            href="#contact"
            class="button">

            Get In Touch

        </a>


    </section>



    <!-- =========================================
         CONTACT
    ========================================== -->

    <section
        class="contact"
        id="contact">


        <p class="section-label">

            CONTACT

        </p>


        <h2>

            Let's Connect 🌸

        </h2>


        <p>

            Have a question or want to know
            more about our creations?

        </p>


        <div class="contact-info">


            <!--
            REPLACE THESE WITH YOUR
            ACTUAL BUSINESS DETAILS.
            -->


            <p>

                📧 Your Email Here

            </p>


            <p>

                📱 Your Instagram Here

            </p>


            <p>

                👩‍🎨 Founder: Ishita Rai

            </p>


        </div>


        <a
            href="#"
            class="button">

            Contact Us

        </a>


    </section>



    <!-- =========================================
         FOOTER
    ========================================== -->

    <footer>


        <h3>

            🌸 Little Blossom Works

        </h3>


        <p>

            Handmade with love by Ishita Rai

        </p>


        <p>

            © 2026 Little Blossom Works.
            All Rights Reserved.

        </p>


    </footer>


</body>

</html>
```
