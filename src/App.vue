<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <main>
    <header>
      <div class="content container">
        <div class="logo">
          <RouterLink to="/"
            ><img
              src="https://myteam-multi-page-website-teal.vercel.app/_nuxt/image/085422.svg"
              alt=""
          /></RouterLink>
        </div>
        <i class="fas fa-bars icon"></i>
        <div class="right-side">
          <i class="fas fa-times icon close"></i>
          <ul>
            <li><router-link :class="{ active: $route.path === '/' }" to="/">home</router-link></li>
            <li>
              <router-link :class="{ active: $route.path === '/about' }" to="/about"
                >about</router-link
              >
            </li>
          </ul>
          <RouterLink to="/contact" class="contact-btn">contact us </RouterLink>
        </div>
      </div>
    </header>
    <RouterView></RouterView>
  </main>
</template>

<style scoped>
header {
  background-color: var(--dark-cyan);
  padding: 55px 0;
}
header .icon {
  color: white;
  font-size: 24px;
  display: none;
  cursor: pointer;
}
header .content,
header .right-side,
header ul {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 40px;
}
header .right-side {
  width: 100%;
}
header li a {
  color: white;
  font-size: 20px;
  font-weight: 600;
  transition: 0.3s;
}
header li a:hover,
header li a.active {
  color: var(--salmon);
}
header .contact-btn {
  color: white;
  font-size: 18px;
  font-weight: 600;
  padding: 12px 30px;
  border-radius: 30px;
  border: 2px solid white;
  transition: 0.3s;
  display: block;
  text-align: center;
}
header .contact-btn:hover {
  color: #002529;
  background-color: white;
  transform: scale(1.1);
}
@media (max-width: 767px) {
  header {
    padding: 25px 0;
  }
  header .right-side {
    position: fixed;
    flex-direction: column;
    align-items: self-start;
    width: 50%;
    height: 100%;
    top: 0;
    right: 0;
    background-color: #2c6269;
    z-index: 100;
    padding: 26px;
    padding-top: 50px;
    min-width: 250px;
    justify-content: normal;
    background-image: url(https://myteam-multi-page-website-teal.vercel.app/images/bg-pattern-about-1-mobile-nav-1.svg);
    background-repeat: no-repeat;
    background-position: right -100px bottom;
    transition: 0.3s;
    transform: scaleX(0);
    transform-origin: right;
  }
  header .right-side.shown {
    transform: scaleX(1);
  }
  header .right-side ul {
    flex-direction: column;
  }
  header .contact-btn {
    width: 100%;
  }
  header .icon {
    display: block;
  }
  header .icon.close {
    text-align: right;
    width: 100%;
  }
}
</style>

<script>
export default {
  mounted() {
    const icons = document.querySelectorAll('.icon')
    const rightSide = document.querySelector('header .right-side')

    icons.forEach((icon) => {
      icon.addEventListener('click', () => {
        console.log('here')
        rightSide.classList.toggle('shown')
      })
    })
  }
}
</script>
