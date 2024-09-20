<template>
  <footer>
    <div class="content container">
      <div class="left-side">
        <div class="logo">
          <RouterLink to="/"
            ><img
              src="https://myteam-multi-page-website-teal.vercel.app/_nuxt/image/085422.svg"
              alt=""
          /></RouterLink>
        </div>
        <ul>
          <li><router-link :class="{ active: $route.path === '/' }" to="/">home</router-link></li>
          <li>
            <router-link :class="{ active: $route.path === '/about' }" to="/about"
              >about</router-link
            >
          </li>
        </ul>
      </div>
      <div class="right-side">
        <ul class="detials">
          <li>987 Hillcrest Lane</li>
          <li>Irvine, CA</li>
          <li>California 92714</li>
          <li>Call Us : 949-833-7432</li>
        </ul>
        <ul class="socials">
          <li>
            <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
          </li>
          <li>
            <a href="#"><i class="fa-brands fa-twitter"></i></a>
          </li>
          <li>
            <a href="#"><i class="fa-brands fa-instagram"></i></a>
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<style scoped>
footer {
  background-color: var(--midnight-blue);
  padding: 20px 0;
}
footer .content {
  display: flex;
  gap: 60px;
  align-items: center;
}
footer .left-side ul {
  display: flex;
  gap: 20px;
  align-content: center;
  justify-content: space-between;
}
footer .left-side li a {
  color: white;
  font-size: 20px;
  font-weight: 600;
  transition: 0.3s;
}
footer .left-side li a:hover,
footer .left-side li a.active {
  color: var(--salmon);
}
footer .right-side {
  gap: 20px;
  width: 100%;
  display: flex;
  justify-content: space-between;
}
footer .detials li {
  color: #99a8a9;
  font-weight: 600;
}
footer .socials {
  display: flex;
  align-items: center;
  gap: 20px;
}
footer .socials a {
  color: white;
  font-size: 22px;
}
@media (max-width: 768px) {
  footer .content {
    gap: 20px;
    flex-direction: column;
  }
  footer .right-side {
    flex-direction: column;
    align-items: center;
  }
  footer .detials {
    text-align: center;
  }
}
</style>
