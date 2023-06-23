<template>
    <body>

        <header class="header">
            <div class="container">
                <div class="header__wrapper">

                    <div class="header__logo">
                        <nuxt-link to="/HomePage" class="header__logo-link">
                            <img class="header__logo-img" src="~/assets/images/src/headerlogo.png" alt="logo">
                        </nuxt-link>
                    </div>

                    <nav class="menu">

                        <div class="menu__btn">
                            <span></span>
                        </div>


                        <ul class="menu__list">
                            <li class="menu__list-item">
                                <nuxt-link class="menu__list-link" to="/HomePage">Home</nuxt-link>
                            </li>
                            <li class="menu__list-item">
                                <nuxt-link class="menu__list-link" to="/MenuPage">Menu</nuxt-link>
                            </li>
                            <li class="menu__list-item">
                                <nuxt-link class="menu__list-link" to="/HomePage">Service</nuxt-link>
                            </li>
                            <li class="menu__list-item">
                                <nuxt-link class="menu__list-link" to="/HomePage">Delivery</nuxt-link>
                            </li>
                            <li class="menu__list-item">
                                <nuxt-link class="menu__list-link" to="/HomePage">Contact</nuxt-link>
                            </li>
                        </ul>
                    </nav>

                    <div class="header__buttons">
                        <nuxt-link to="/CartPage" class="header__cart">
                            <img src="~/assets/images/src/cart.png" alt="icon" class="header__cart-img">
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

                        <DishList />

                        <ul class="dishes__pagination">
                            <li class="dishes__pagination-item">
                                <a class="dishes__pagination-link pagination__link--arrow pagination__link--disabled"
                                    aria-label="Предыдущая страница">
                                    <img src="~/assets/images/src/arrowleft.png" alt="" class="dishes__pagination-img">
                                </a>
                            </li>
                            <li class="dishes__pagination-item">
                                <a class="dishes__pagination-link pagination__link--current">
                                    1
                                </a>
                            </li>
                            <li class="dishes__pagination-item">
                                <a class="dishes__pagination-link" href="#">
                                    2
                                </a>
                            </li>
                            <li class="dishes__pagination-item">
                                <a class="dishes__pagination-link" href="#">
                                    3
                                </a>
                            </li>
                            <li class="dishes__pagination-item">
                                <a class="dishes__pagination-link" href="#">
                                    4
                                </a>
                            </li>
                            <li class="dishes__pagination-item">
                                <a class="dishes__pagination-link pagination__link--arrow" href="#"
                                    aria-label="Следующая страница">
                                    <img src="~/assets/images/src/arrowright.png" alt="" class="dishes__pagination-img">
                                </a>
                            </li>
                        </ul>

                    </div>
                </section>
            </main>
        </div>

        <footer class="footer">
            <div class="container">
                <div class="footer__wrapper">
                    <div class="footer__social">
                        <img src="~/assets/images/src/headerlogo.png" alt="logo" class="footer__social-logo">
                        <p class="footer__social-text">The standard chunk of Lorem Ipsum used since the 1500s is reproduced
                            below for those.</p>
                    </div>
                    <div class="footer__menu">
                        <h4 class="footer__title">Our Menu</h4>
                        <div class="footer__menu-links">
                            <ul class="footer__links-list">
                                <li class="footer__link-li"><nuxt-link to="/MenuPage"
                                        class="footer__link">Breakfast</nuxt-link></li>
                                <li class="footer__link-li"><nuxt-link to="/MenuPage" class="footer__link">Lunch</nuxt-link>
                                </li>
                                <li class="footer__link-li"><nuxt-link to="/MenuPage"
                                        class="footer__link">Dinner</nuxt-link></li>
                                <li class="footer__link-li"><nuxt-link to="/MenuPage"
                                        class="footer__link">Snacks</nuxt-link></li>
                            </ul>
                        </div>
                    </div>
                    <div class="footer__links">
                        <h4 class="footer__title">UsefulLinks</h4>
                        <div class="footer__links-links">
                            <ul class="footer__links-list">
                                <li class="footer__link-li"><nuxt-link to="/HomePage" class="footer__link">Terms &
                                        Conditions</nuxt-link></li>
                                <li class="footer__link-li"><nuxt-link to="/HomePage"
                                        class="footer__link">Services</nuxt-link></li>
                                <li class="footer__link-li"><nuxt-link to="/HomePage" class="footer__link">Payment &
                                        Tax</nuxt-link></li>
                                <li class="footer__link-li"><nuxt-link to="/HomePage"
                                        class="footer__link">Support</nuxt-link></li>
                                <li class="footer__link-li"><nuxt-link to="/HomePage" class="footer__link">Return
                                        Policy</nuxt-link></li>
                            </ul>
                        </div>
                    </div>
                    <div class="footer__info">
                        <h4 class="footer__title">Information</h4>
                        <nuxt-link to="/HomePage" class="footer__link footer__link-info">Get Update</nuxt-link>
                        <form action=" " class="footer__form">
                            <input type="email" class="footer__input" placeholder="Email Address...">
                            <input type="submit" value=" " class="footer__button">
                        </form>
                        <nuxt-link to="/HomePage" class="footer__link">Payment Method</nuxt-link>
                        <img src="~/assets/images/src/payment.png" alt="payment" class="footer__payment">
                    </div>
                </div>
        </div>
    </footer>
</body>
</template>

<script>

export default{
    name: 'MenuPage',
}
</script>

<style scoped>
.dishes__pagination {
    display: flex;
    width: 30rem;
    margin: 10rem auto 0;
}
.dishes__pagination-item {
    width: 5rem;
    height: 5rem;
    font-size: 3rem;
    font-weight: 600;
    line-height: 2rem;
    color: #a8a8a8;
}
.dishes__pagination-link {
    color: #a8a8a8;
}
</style>