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

        <div class="wrapper">
            <main class="main">
                <section class="dishes">
                    <div class="container">
                        <h2 class="dishes__title">Our Most Popular Dishes</h2>
                        <div class="dishes__list">
                            <ul class="dishes__list-items">
                                <li class="dishes__list-item">Breakfast</li>
                                <li class="dishes__list-item">Lunch</li>
                                <li class="dishes__list-item">Dinner</li>
                                <li class="dishes__list-item">Fastfood</li>
                                <li class="dishes__list-item">Drinks</li>
                                <li class="dishes__list-item">Others</li>
                            </ul>
                        </div>

                        <div class="dishes__list">
                            <ul class="dishes__list-items dishes__list-filter">
                                <li class="dishes__list-item">New</li>
                                <li class="dishes__list-item">Hot</li>
                                <li class="dishes__list-item">Vegan</li>
                            </ul>
                        </div>

                        <div class="dishes__filter-price">
                            <h3 class="dishes__filter-price-title">Price</h3>
                            <label class="dishes__filter-price-label">
                                <input class="dishes__filter-price-input" type="text" name="min-price" placeholder="From">
                            </label>
                            <label class="dishes__filter-price-label">
                                <input class="dishes__filter-price-input" type="text" name="max-price" placeholder="To">
                            </label>
                        </div>

                        <div class="dishes__items">
                            <div class="dishes__item">
                                <nuxt-link to="/item" class="dishes__item-link">
                                    <div class="dishes__price"><b>$14.53</b></div>
                                    <img src="../images/src/dish1.png" alt="image" class="dishes__item-img">

                                    <div class="dishes__item-content">
                                        <div class="dishes__item-content-top">
                                            <h3 class="dishes__item-content-title">Italian Fusilli Pasta</h3>

                                            <div class="dishes__form-counter">
                                                <button class="dishes__minus-btn" type="button"
                                                    aria-label="Убрать один товар">-</button>

                                                <input class="dishes__input" type="text" value="+2" name="count">

                                                <button class="dishes__plus-btn" type="button"
                                                    aria-label="Добавить один товар">+</button>
                                            </div>
                                        </div>

                                        <div class="dishes__item-content-down">
                                            <div class="dishes__content-time">25 Min Away</div>
                                        </div>
                                    </div>
                                </nuxt-link>
                            </div>
                            <div class="dishes__item">
                                <nuxt-link to="/item" class="dishes__item-link">
                                    <div class="dishes__price"><b>$13.20</b></div>
                                    <img src="../images/src/dish2.png" alt="image" class="dishes__item-img">

                                    <div class="dishes__item-content">
                                        <div class="dishes__item-content-top">
                                            <h3 class="dishes__item-content-title">Braised belly caramelised </h3>

                                            <div class="dishes__form-counter">
                                                <button class="dishes__minus-btn" type="button"
                                                    aria-label="Убрать один товар">-</button>

                                                <input class="dishes__input" type="text" value="+1" name="count">

                                                <button class="dishes__plus-btn" type="button"
                                                    aria-label="Добавить один товар">+</button>
                                            </div>
                                        </div>

                                        <div class="dishes__item-content-down">
                                            <div class="dishes__content-time">45 Min Away</div>
                                        </div>
                                    </div>
                                </nuxt-link>
                            </div>
                            <div class="dishes__item">
                                <nuxt-link to="/item" class="dishes__item-link">
                                    <div class="dishes__price"><b>$6.50</b></div>
                                    <img src="../images/src/dish3.png" alt="image" class="dishes__item-img">

                                    <div class="dishes__item-content">
                                        <div class="dishes__item-content-top">
                                            <h3 class="dishes__item-content-title">Fried Crap Bow Rice</h3>

                                            <div class="dishes__form-counter">
                                                <button class="dishes__minus-btn" type="button"
                                                    aria-label="Убрать один товар">-</button>

                                                <input class="dishes__input" type="text" value="+1" name="count">

                                                <button class="dishes__plus-btn" type="button"
                                                    aria-label="Добавить один товар">+</button>
                                            </div>
                                        </div>

                                        <div class="dishes__item-content-down">
                                            <div class="dishes__content-time">1 Hour Away</div>
                                        </div>
                                    </div>
                                </nuxt-link>
                            </div>
                        </div>
                    </div>
                </section>
            </main>
        </div>

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