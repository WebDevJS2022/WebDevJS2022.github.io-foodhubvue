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
              <span>.</span>
            </div>

            <ul class="menu__list">
              <li class="menu__list-item">
                <nuxt-link class="menu__list-link" to="/HomePage">
                  Home
                </nuxt-link>
              </li>
              <li class="menu__list-item">
                <nuxt-link class="menu__list-link" to="/MenuPage">
                  Menu
                </nuxt-link>
              </li>
              <li class="menu__list-item">
                <a class="menu__list-link" href="#service">
                  Service
                </a>
              </li>
              <li class="menu__list-item">
                <a class="menu__list-link" href="#delivery">
                  Delivery
                </a>
              </li>
              <li class="menu__list-item">
                <a class="menu__list-link" href="#contact">
                  Contact
                </a>
              </li>
            </ul>
          </nav>
          <div class="header__buttons">
            <nuxt-link to="/CartPage" class="header__cart">
              <img src="~/assets/images/src/cart.png" alt="icon" class="header__cart-img">
              <span class="header__count" aria-label="Количество товаров">
                3
              </span>
            </nuxt-link>
          </div>
        </div>
      </div>
    </header>

    <div class="wrapper">
      <main class="main">
        <section class="top">
          <div class="container">
            <div class="top__wrapper">
              <div class="top__content">
                <p class="top__content-subtitle">
                  Welcome to Foodhub
                </p>
                <h1 class="top__content-title">
                  Enjoy Healthy & Tasty Food
                </h1>
                <p class="top__content-text">
                  Food is usually of plant, animal or fungal origin, and contains essential nutrients, such as carbohydrates, fats, proteins, vitamins, or minerals.
                </p>

                <nuxt-link to="/menu">
                  <button class="top__content-btn">
                    Explore Menu
                  </button>
                </nuxt-link>
              </div>
              <div class="top__images">
                <img src="~/assets/images/src/top1.png" alt="image" class="top__images-1">
                <img src="~/assets/images/src/top2.png" alt="image" class="top__images-2">
                <img src="~/assets/images/src/top3.png" alt="image" class="top__images-3">
                <img src="~/assets/images/src/top4.png" alt="image" class="top__images-4">
                <img src="~/assets/images/src/top5.png" alt="image" class="top__images-5">
              </div>
            </div>
          </div>
        </section>

        <section class="dishes">
          <div class="container">
            <h2 class="dishes__title">
              Our Most Popular Dishes
            </h2>
            <div class="dishes__list">
              <ul class="dishes__list-items">
                <li class="dishes__list-item">
                  Breakfast
                </li>
                <li class="dishes__list-item">
                  Lunch
                </li>
                <li class="dishes__list-item">
                  Dinner
                </li>
                <li class="dishes__list-item">
                  Fastfood
                </li>
                <li class="dishes__list-item">
                  Drinks
                </li>
                <li class="dishes__list-item">
                  Others
                </li>
              </ul>
            </div>
            <DishList />
          </div>
        </section>

        <section class="about">
          <div class="container">
            <div class="about__wrapper">
              <div class="about__image">
                <img src="~/assets/images/src/about.png" alt="image" class="about__img">
              </div>

              <div class="about__content">
                <h2 class="about__title">
                  Serving Best Food is Our First Priority
                </h2>
                <p class="about__text">
                  nutrients used in the body of an organism to sustain growth and vital processes and to furnish energy. The absorption and utilization of food by the body is fundamental to nutrition and is facilitated by digestion
                </p>
                <button class="about__btn">
                  Learn About Us
                </button>
              </div>
            </div>
          </div>
        </section>

        <section id="delivery" class="offer">
          <div class="container">
            <h2 class="offer__title">
              We Offer People Many Type of Food
            </h2>
            <div class="offer__items">
              <div class="offer__item">
                <div class="offer__item-top">
                  <div class="offer__image">
                    <img src="~/assets/images/src/offer1.png" alt="image" class="offer__img">
                  </div>
                  <div class="offer__item-stars">
                    <img src="~/assets/images/src/stars.png" alt="icon" class="offer__stars">
                    <p class="offer__item-avaible">
                      300+ Items Availble
                    </p>
                  </div>
                </div>

                <div class="offer__item-down">
                  <h3 class="offer__item-title">
                    Local/Traditional Food
                  </h3>
                  <p class="offer__item-text">
                    It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout.
                  </p>
                </div>
              </div>
              <div class="offer__item">
                <div class="offer__item-top">
                  <div class="offer__image">
                    <img src="~/assets/images/src/offer2.png" alt="image" class="offer__img">
                  </div>
                  <div class="offer__item-stars">
                    <img src="~/assets/images/src/stars.png" alt="icon" class="offer__stars">
                    <p class="offer__item-avaible">
                      140+ Items Availble
                    </p>
                  </div>
                </div>

                <div class="offer__item-down">
                  <h3 class="offer__item-title">
                    Inter/Continental Food
                  </h3>
                  <p class="offer__item-text">
                    It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout.
                  </p>
                </div>
              </div>
              <div class="offer__item">
                <div class="offer__item-top">
                  <div class="offer__image">
                    <img src="~/assets/images/src/offer3.png" alt="image" class="offer__img">
                  </div>
                  <div class="offer__item-stars">
                    <img src="~/assets/images/src/stars.png" alt="icon" class="offer__stars">
                    <p class="offer__item-avaible">
                      200+ Items Availble
                    </p>
                  </div>
                </div>

                <div class="offer__item-down">
                  <h3 class="offer__item-title">
                    Fastfood
                  </h3>
                  <p class="offer__item-text">
                    It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout.
                  </p>
                </div>
              </div>
            </div>
          </div>
        </section>

        <section class="discount">
          <div class="container">
            <h2 class="discount__title">
              Up to
              <span>
                50%
              </span>
              Discount on Selected Items
            </h2>
            <p class="discount__text">
              Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s
            </p>
            <div class="discount__buttons">
              <a href="#" class="discount__items-btn">
                All Discount Item
              </a>
              <a href="#" class="discount__menu-btn">
                View All Menu
              </a>
            </div>
          </div>
        </section>

        <section id="service" class="service">
          <div class="container">
            <div class="service__wrapper">
              <div class="service__item">
                <div class="service__image">
                  <img src="~/assets/images/src/service1.png" alt="icon" class="service__img service__img-1">
                </div>
                <h3 class="service__title">
                  Online Food Sell
                </h3>
              </div>
              <div class="service__item">
                <div class="service__image">
                  <img src="~/assets/images/src/service2.png" alt="icon" class="service__img service__img-2">
                </div>
                <h3 class="service__title">
                  Delivery Service
                </h3>
              </div>
              <div class="service__item">
                <div class="service__image">
                  <img src="~/assets/images/src/service3.png" alt="icon" class="service__img service__img-3">
                </div>
                <h3 class="service__title">
                  Catering Service
                </h3>
              </div>
            </div>
          </div>
        </section>

        <section class="app">
          <div class="container">
            <div class="app__wrapper">
              <div class="app__content">
                <h3 class="app__content-title">
                  Easiest way to get your food by our app
                </h3>
                <button class="app__content-btn">
                  Download now
                </button>
              </div>

              <img src="~/assets/images/src/app.png" alt="image" class="app__image">
            </div>
          </div>
        </section>
      </main>
    </div>

    <footer id="contact" class="footer">
      <div class="container">
        <div class="footer__wrapper">
          <div class="footer__social">
            <img src="~/assets/images/src/headerlogo.png" alt="logo" class="footer__social-logo">
            <p class="footer__social-text">
              The standard chunk of Lorem Ipsum used since the 1500s is reproduced below for those.
            </p>
          </div>
          <div class="footer__menu">
            <nuxt-link to="/MenuPage" class="footer__menu-link">
              <h4 class="footer__title">
                Our Menu
              </h4>
            </nuxt-link>
            <div class="footer__menu-links">
              <ul class="footer__links-list">
                <li class="footer__link-li">
                  <nuxt-link to="/MenuPage" class="footer__link">
                    Breakfast
                  </nuxt-link>
                </li>
                <li class="footer__link-li">
                  <nuxt-link to="/MenuPage" class="footer__link">
                    Lunch
                  </nuxt-link>
                </li>
                <li class="footer__link-li">
                  <nuxt-link to="/MenuPage" class="footer__link">
                    Dinner
                  </nuxt-link>
                </li>
                <li class="footer__link-li">
                  <nuxt-link to="/MenuPage" class="footer__link">
                    Snacks
                  </nuxt-link>
                </li>
              </ul>
            </div>
          </div>
          <div class="footer__links">
            <h4 class="footer__title">
              UsefulLinks
            </h4>
            <div class="footer__links-links">
              <ul class="footer__links-list">
                <li class="footer__link-li">
                  <nuxt-link to="/HomePage" class="footer__link">
                    Terms & Conditions
                  </nuxt-link>
                </li>
                <li class="footer__link-li">
                  <nuxt-link to="/HomePage" class="footer__link">
                    Services
                  </nuxt-link>
                </li>
                <li class="footer__link-li">
                  <nuxt-link to="/HomePage" class="footer__link">
                    Payment & Tax
                  </nuxt-link>
                </li>
                <li class="footer__link-li">
                  <nuxt-link to="/HomePage" class="footer__link">
                    Support
                  </nuxt-link>
                </li>
                <li class="footer__link-li">
                  <nuxt-link to="/HomePage" class="footer__link">
                    Return Policy
                  </nuxt-link>
                </li>
              </ul>
            </div>
          </div>
          <div class="footer__info">
            <h4 class="footer__title">
              Information
            </h4>
            <nuxt-link to="/HomePage" class="footer__link footer__link-info">
              Get Update
            </nuxt-link>
            <form action=" " class="footer__form">
              <input type="email" class="footer__input" placeholder="Email Address...">
              <input type="submit" value=" " class="footer__button">
            </form>
            <nuxt-link to="/HomePage" class="footer__link">
              Payment Method
            </nuxt-link>
            <img src="~/assets/images/src/payment.png" alt="payment" class="footer__payment">
          </div>
        </div>
      </div>
    </footer>
  </body>
</template>

<script>
export default {
  name: 'HomePage'
}
</script>
