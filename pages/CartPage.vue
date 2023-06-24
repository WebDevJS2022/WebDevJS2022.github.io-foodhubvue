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
                <nuxt-link class="menu__list-link" to="/HomePage">
                  Service
                </nuxt-link>
              </li>
              <li class="menu__list-item">
                <nuxt-link class="menu__list-link" to="/HomePage">
                  Delivery
                </nuxt-link>
              </li>
              <li class="menu__list-item">
                <nuxt-link class="menu__list-link" to="/HomePage">
                  Contact
                </nuxt-link>
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

    <main class="main">
      <section class="cart">
        <div class="container">
          <div class="item__top">
            <ul class="item__top-breadcrumbs">
              <li class="item__top-breadcrumbs-item">
                <nuxt-link to="/MenuPage" class="item__top-breadcrumbs-link" href="menu.html">
                  Menu -
                </nuxt-link>
              </li>
              <li class="item__top-breadcrumbs-item">
                <nuxt-link to="/CartPage" class="item__top-breadcrumbs-link" href="#">
                  Cart
                </nuxt-link>
              </li>
            </ul>
          </div>

          <h2 class="cart__title">
            CART
          </h2>
          <p class="cart__amount">
            3 goods
          </p>

          <div class="cart__wrapper">
            <div class="cart__items">
              <div class="cart__item">
                <div class="item__image cart__image">
                  <img src="~/assets/images/src/dish1.png" alt="image" class="item__img">
                </div>

                <div class="item__item-content cart__content">
                  <img src="~/assets/images/src/del.png" alt="icon" class="cart__content-del">
                  <h3 class="item__item-content-title">
                    Italian Fusilli Pasta
                  </h3>

                  <div class="cart__price">
                    Price: $14.53
                  </div>

                  <div class="item__form-counter">
                    <div class="item__count">
                      <button class="item__minus-btn" type="button" aria-label="Убрать один товар">
                        -
                      </button>
                      <input class="item__input" type="text" value="+2" name="count">
                      <button class="item__plus-btn" type="button" aria-label="Добавить один товар">
                        +
                      </button>
                    </div>

                    <button class="item__cart">
                      add to cart
                    </button>
                  </div>
                </div>
              </div>
              <div class="cart__item">
                <div class="item__image cart__image">
                  <img src="~/assets/images/src/dish1.png" alt="image" class="item__img">
                </div>

                <div class="item__item-content cart__content">
                  <img src="~/assets/images/src/del.png" alt="icon" class="cart__content-del">
                  <h3 class="item__item-content-title">
                    Italian Fusilli Pasta
                  </h3>

                  <div class="cart__price">
                    Price: $14.53
                  </div>

                  <div class="item__form-counter">
                    <div class="item__count">
                      <button class="item__minus-btn" type="button" aria-label="Убрать один товар">
                        -
                      </button>
                      <input class="item__input" type="text" value="+2" name="count">
                      <button class="item__plus-btn" type="button" aria-label="Добавить один товар">
                        +
                      </button>
                    </div>

                    <button class="item__cart">
                      add to cart
                    </button>
                  </div>
                </div>
              </div>
              <div class="cart__item">
                <div class="item__image cart__image">
                  <img src="~/assets/images/src/dish1.png" alt="image" class="item__img">
                </div>

                <div class="item__item-content cart__content">
                  <img src="~/assets/images/src/del.png" alt="icon" class="cart__content-del">
                  <h3 class="item__item-content-title">
                    Italian Fusilli Pasta
                  </h3>

                  <div class="cart__price">
                    Price: $14.53
                  </div>

                  <div class="item__form-counter">
                    <div class="item__count">
                      <button class="item__minus-btn" type="button" aria-label="Убрать один товар">
                        -
                      </button>
                      <input class="item__input" type="text" value="+2" name="count">
                      <button class="item__plus-btn" type="button" aria-label="Добавить один товар">
                        +
                      </button>
                    </div>

                    <button class="item__cart">
                      add to cart
                    </button>
                  </div>
                </div>
              </div>
            </div>

            <div class="cart__offer">
              <p class="cart__offer-text">
                We will calculate the cost of delivery in the next step
              </p>
              <p class="cart__offer-price">
                Total: $23.54
              </p>
              <button class="cart__offer-btn">
                place an order
              </button>
            </div>
          </div>
        </div>
      </section>
    </main>

    <footer class="footer">
      <div class="container">
        <div class="footer__wrapper">
          <div class="footer__social">
            <img src="~/assets/images/src/headerlogo.png" alt="logo" class="footer__social-logo">
            <p class="footer__social-text">
              The standard chunk of Lorem Ipsum used since the 1500s is reproduced below for those.
            </p>
          </div>
          <div class="footer__menu">
            <h4 class="footer__title">
              Our Menu
            </h4>
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
                  <nuxt-link to="/" class="footer__link">
                    Terms & Conditions
                  </nuxt-link>
                </li>
                <li class="footer__link-li">
                  <nuxt-link to="/" class="footer__link">
                    Services
                  </nuxt-link>
                </li>
                <li class="footer__link-li">
                  <nuxt-link to="/" class="footer__link">
                    Payment & Tax
                  </nuxt-link>
                </li>
                <li class="footer__link-li">
                  <nuxt-link to="/" class="footer__link">
                    Support
                  </nuxt-link>
                </li>
                <li class="footer__link-li">
                  <nuxt-link to="/" class="footer__link">
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
  name: 'CartPage'
}
</script>
