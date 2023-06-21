<template>
    <body>

        <header class="header">
            <div class="container">
                <div class="header__wrapper">

                    <div class="header__logo">
                        <nuxt-link to="/" class="header__logo-link">
                            <img class="header__logo-img" src="../images/src/headerlogo.png" alt="logo">
                        </nuxt-link>
                    </div>

                    <nav class="menu">

                        <div class="menu__btn">
                            <span></span>
                        </div>


                        <ul class="menu__list">
                            <li class="menu__list-item">
                                <nuxt-link class="menu__list-link" to="/">Home</nuxt-link>
                            </li>
                            <li class="menu__list-item">
                                <nuxt-link class="menu__list-link" to="/menu">Menu</nuxt-link>
                            </li>
                            <li class="menu__list-item">
                                <nuxt-link class="menu__list-link" to="/">Service</nuxt-link>
                            </li>
                            <li class="menu__list-item">
                                <nuxt-link class="menu__list-link" to="/">Delivery</nuxt-link>
                            </li>
                            <li class="menu__list-item">
                                <nuxt-link class="menu__list-link" to="/">Contact</nuxt-link>
                            </li>
                        </ul>
                    </nav>

                    <div class="header__buttons">
                        <nuxt-link to="/cart" class="header__cart">
                            <img src="../images/src/cart.png" alt="icon" class="header__cart-img">
                            <span class="header__count" aria-label="Количество товаров">3</span>
                        </nuxt-link>
                    </div>

                </div>

            </div>
        </header>


    <main class="main">
        <section class="item">
            <div class="item__top">
                <ul class="item__top-breadcrumbs">
                    <li class="item__top-breadcrumbs-item">
                        <nuxt-link class="item__top-breadcrumbs-link" to="/menu">
                            Menu -
                        </nuxt-link>
                    </li>
                    <li class="item__top-breadcrumbs-item">
                        <nuxt-link class="item__top-breadcrumbs-link" to="/menu">
                            Breakfast -
                        </nuxt-link>
                    </li>
                    <li class="item__top-breadcrumbs-item">
                        <a class="item__top-breadcrumbs-link">
                            Italian Fusilli Pasta
                        </a>
                    </li>
                </ul>
            </div>
    
            <div class="item__wrapper">
                <div class="item__image">
                    <img src="../images/src/dish1.png" alt="image" class="item__img">
                </div>
    
                <div class="item__item-content">
                    <h3 class="item__item-content-title">Italian Fusilli Pasta</h3>

                    <p class="item__info">New -</p>
                    <p class="item__info">Hot +</p>
                    <p class="item__info">Vegan +</p>
                
                    <div class="item__content-time">Delivery: 25 Min Away</div>

                    <div class="item__form-counter">
                        <div class="item__count">
                            <button class="item__minus-btn" type="button" aria-label="Убрать один товар">-</button>
                            <input class="item__input" type="text" value="+2" name="count">
                            <button class="item__plus-btn" type="button" aria-label="Добавить один товар">+</button>
                        </div>

                        <button class="item__cart">add to cart</button>
                    </div>
                </div>
            </div>

            <div class="item__down">
                <h2 class="item__down-title">Description</h2>
                <p class="item__down-text">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Non laborum obcaecati sequi facilis quis qui velit consequuntur, officiis, quo recusandae libero a dignissimos facere saepe nostrum voluptate! Aliquam, accusantium totam.
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit. Doloremque harum nam, quas corporis iure expedita commodi. Consequuntur aut consequatur sed voluptas numquam sapiente porro, culpa autem ut repellat, perferendis quos!
                    Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quam earum dicta temporibus error saepe omnis ducimus aspernatur corporis itaque libero tenetur dolore explicabo consectetur repellat odit eos obcaecati, nisi blanditiis.
                </p>
            </div>
        </section>
    </main>


    <footer class="footer">
            <div class="container">
                <div class="footer__wrapper">
                    <div class="footer__social">
                        <img src="../images/src/headerlogo.png" alt="logo" class="footer__social-logo">
                        <p class="footer__social-text">The standard chunk of Lorem Ipsum used since the 1500s is reproduced
                            below for those.</p>
                    </div>
                    <div class="footer__menu">
                        <h4 class="footer__title">Our Menu</h4>
                        <div class="footer__menu-links">
                            <ul class="footer__links-list">
                                <li class="footer__link-li"><nuxt-link to="/menu" class="footer__link">Breakfast</nuxt-link></li>
                                <li class="footer__link-li"><nuxt-link to="/menu" class="footer__link">Lunch</nuxt-link></li>
                                <li class="footer__link-li"><nuxt-link to="/menu" class="footer__link">Dinner</nuxt-link></li>
                                <li class="footer__link-li"><nuxt-link to="/menu" class="footer__link">Snacks</nuxt-link></li>
                            </ul>
                        </div>
                    </div>
                    <div class="footer__links">
                        <h4 class="footer__title">UsefulLinks</h4>
                        <div class="footer__links-links">
                            <ul class="footer__links-list">
                                <li class="footer__link-li"><nuxt-link to="/" class="footer__link">Terms & Conditions</nuxt-link></li>
                                <li class="footer__link-li"><nuxt-link to="/" class="footer__link">Services</nuxt-link></li>
                                <li class="footer__link-li"><nuxt-link to="/" class="footer__link">Payment & Tax</nuxt-link></li>
                                <li class="footer__link-li"><nuxt-link to="/" class="footer__link">Support</nuxt-link></li>
                                <li class="footer__link-li"><nuxt-link to="/" class="footer__link">Return Policy</nuxt-link></li>
                            </ul>
                        </div>
                    </div>
                    <div class="footer__info">
                        <h4 class="footer__title">Information</h4>
                        <nuxt-link to="/" class="footer__link footer__link-info">Get Update</nuxt-link>
                        <form action=" " class="footer__form">
                            <input type="email" class="footer__input" placeholder="Email Address...">
                            <input type="submit" value=" " class="footer__button">
                        </form>
                        <nuxt-link to="/" class="footer__link">Payment Method</nuxt-link>
                        <img src="../images/src/payment.png" alt="payment" class="footer__payment">
                    </div>
                </div>
            </div>
    </footer>
</body>
</template>